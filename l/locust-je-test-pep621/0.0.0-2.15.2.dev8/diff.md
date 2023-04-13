# Comparing `tmp/locust_je_test_pep621-0.0.0.tar.gz` & `tmp/locust_je_test_pep621-2.15.2.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locust_je_test_pep621-0.0.0.tar", last modified: Thu Apr 13 13:58:09 2023, max compression
+gzip compressed data, was "locust_je_test_pep621-2.15.2.dev8.tar", last modified: Thu Apr 13 14:08:42 2023, max compression
```

## Comparing `locust_je_test_pep621-0.0.0.tar` & `locust_je_test_pep621-2.15.2.dev8.tar`

### file list

```diff
@@ -1,116 +1,250 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:09.021237 locust_je_test_pep621-0.0.0/
--rw-rw-rw-   0        0        0     1115 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      115 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     8457 2023-04-13 13:58:09.022235 locust_je_test_pep621-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/README
--rw-rw-rw-   0        0        0     5760 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.919509 locust_je_test_pep621-0.0.0/locust/
--rw-rw-rw-   0        0        0     1385 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/__init__.py
--rw-rw-rw-   0        0        0       34 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/__main__.py
--rw-rw-rw-   0        0        0    25259 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/argument_parser.py
--rw-rw-rw-   0        0        0    15095 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/clients.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.921505 locust_je_test_pep621-0.0.0/locust/contrib/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/contrib/__init__.py
--rw-rw-rw-   0        0        0    26952 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/contrib/fasthttp.py
--rw-rw-rw-   0        0        0     4858 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/debug.py
--rw-rw-rw-   0        0        0    19147 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/dispatch.py
--rw-rw-rw-   0        0        0    11617 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/env.py
--rw-rw-rw-   0        0        0     6121 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/event.py
--rw-rw-rw-   0        0        0     2029 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/exception.py
--rw-rw-rw-   0        0        0     3677 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/html.py
--rw-rw-rw-   0        0        0     3161 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/input_events.py
--rw-rw-rw-   0        0        0     2859 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/log.py
--rw-rw-rw-   0        0        0    20295 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/main.py
--rw-rw-rw-   0        0        0       66 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.927488 locust_je_test_pep621-0.0.0/locust/rpc/
--rw-rw-rw-   0        0        0       60 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/rpc/__init__.py
--rw-rw-rw-   0        0        0      508 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/rpc/protocol.py
--rw-rw-rw-   0        0        0     2667 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/rpc/zmqrpc.py
--rw-rw-rw-   0        0        0    65383 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/runners.py
--rw-rw-rw-   0        0        0     1482 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/shape.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.939456 locust_je_test_pep621-0.0.0/locust/static/
--rw-rw-rw-   0        0        0     4929 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/chart.js
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.943445 locust_je_test_pep621-0.0.0/locust/static/css/
--rw-rw-rw-   0        0        0     9617 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/css/application.css
--rw-rw-rw-   0        0        0     2089 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/css/application.css.map
--rw-rw-rw-   0        0        0     1477 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/css/tables.css
--rw-rw-rw-   0        0        0      411 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/css/tables.css.map
--rw-rw-rw-   0        0        0   620479 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/echarts.common.min.js
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.950427 locust_je_test_pep621-0.0.0/locust/static/img/
--rw-rw-rw-   0        0        0     8348 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/img/favicon.ico
--rw-rw-rw-   0        0        0    24553 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/img/logo.png
--rw-rw-rw-   0        0        0    79701 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-charts.png
--rw-rw-rw-   0        0        0    64670 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-start-test.png
--rw-rw-rw-   0        0        0    95837 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-stats.png
--rw-rw-rw-   0        0        0   151806 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-workers.png
--rw-rw-rw-   0        0        0    95962 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/jquery-1.11.3.min.js
--rw-rw-rw-   0        0        0     3395 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/jquery.jqote2.min.js
--rw-rw-rw-   0        0        0     2998 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/jquery.tools.min.js
--rw-rw-rw-   0        0        0    10588 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/locust.js
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.956412 locust_je_test_pep621-0.0.0/locust/static/sass/
--rw-rw-rw-   0        0        0      485 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/sass/_base.sass
--rw-rw-rw-   0        0        0       72 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/sass/_mixins.sass
--rw-rw-rw-   0        0        0     8832 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/sass/application.sass
--rw-rw-rw-   0        0        0     1422 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/sass/tables.sass
--rw-rw-rw-   0        0        0     1418 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/tasks.js
--rw-rw-rw-   0        0        0     1171 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/static/vintage.js
--rw-rw-rw-   0        0        0    45246 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/stats.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.959403 locust_je_test_pep621-0.0.0/locust/templates/
--rw-rw-rw-   0        0        0    22248 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/templates/index.html
--rw-rw-rw-   0        0        0    10932 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/templates/report.html
--rw-rw-rw-   0        0        0     1274 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/templates/stats_data.html
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.990320 locust_je_test_pep621-0.0.0/locust/test/
--rw-rw-rw-   0        0        0      411 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/__init__.py
--rw-rw-rw-   0        0        0      171 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/fake_module1_for_env_test.py
--rw-rw-rw-   0        0        0      171 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/fake_module2_for_env_test.py
--rw-rw-rw-   0        0        0     1331 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/mock_locustfile.py
--rw-rw-rw-   0        0        0      810 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/mock_logging.py
--rw-rw-rw-   0        0        0   168977 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_dispatch.py
--rw-rw-rw-   0        0        0     6327 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_env.py
--rw-rw-rw-   0        0        0    30195 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_fasthttp.py
--rw-rw-rw-   0        0        0    12065 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_http.py
--rw-rw-rw-   0        0        0     5520 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_load_locustfile.py
--rw-rw-rw-   0        0        0    26371 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_locust_class.py
--rw-rw-rw-   0        0        0     6943 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_log.py
--rw-rw-rw-   0        0        0    61009 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_main.py
--rw-rw-rw-   0        0        0        0 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_old_wait_api.py
--rw-rw-rw-   0        0        0    16559 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_parser.py
--rw-rw-rw-   0        0        0   157889 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_runners.py
--rw-rw-rw-   0        0        0     3533 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_sequential_taskset.py
--rw-rw-rw-   0        0        0    34710 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_stats.py
--rw-rw-rw-   0        0        0    13576 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_tags.py
--rw-rw-rw-   0        0        0     2836 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_taskratio.py
--rw-rw-rw-   0        0        0     2204 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_users.py
--rw-rw-rw-   0        0        0     1260 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_util.py
--rw-rw-rw-   0        0        0     2432 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_wait_time.py
--rw-rw-rw-   0        0        0    42011 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_web.py
--rw-rw-rw-   0        0        0     2119 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/test_zmqrpc.py
--rw-rw-rw-   0        0        0     6573 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/testcases.py
--rw-rw-rw-   0        0        0     2753 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/test/util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:08.996303 locust_je_test_pep621-0.0.0/locust/user/
--rw-rw-rw-   0        0        0       73 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/user/__init__.py
--rw-rw-rw-   0        0        0     2721 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/user/inspectuser.py
--rw-rw-rw-   0        0        0     2604 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/user/sequential_taskset.py
--rw-rw-rw-   0        0        0    17070 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/user/task.py
--rw-rw-rw-   0        0        0     9438 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/user/users.py
--rw-rw-rw-   0        0        0     2861 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/user/wait_time.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:09.003285 locust_je_test_pep621-0.0.0/locust/util/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/util/__init__.py
--rw-rw-rw-   0        0        0     1097 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/util/cache.py
--rw-rw-rw-   0        0        0     2086 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/util/deprecation.py
--rw-rw-rw-   0        0        0      823 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/util/exception_handler.py
--rw-rw-rw-   0        0        0     2712 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/util/load_locustfile.py
--rw-rw-rw-   0        0        0       94 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/util/rounding.py
--rw-rw-rw-   0        0        0     1022 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/util/timespan.py
--rw-rw-rw-   0        0        0    25689 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/locust/web.py
-drwxrwxrwx   0        0        0        0 2023-04-13 13:58:09.020239 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/
--rw-rw-rw-   0        0        0     8457 2023-04-13 13:58:08.000000 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2752 2023-04-13 13:58:08.000000 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 13:58:08.000000 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-13 13:58:08.000000 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 13:57:10.000000 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      286 2023-04-13 13:58:08.000000 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 13:58:08.000000 locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2766 2023-04-13 13:57:59.000000 locust_je_test_pep621-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     2203 2023-04-13 13:58:09.028218 locust_je_test_pep621-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      174 2023-04-13 12:45:27.000000 locust_je_test_pep621-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.424521 locust_je_test_pep621-2.15.2.dev8/
+-rw-rw-rw-   0        0        0      319 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.coveragerc
+-rw-rw-rw-   0        0        0      211 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.dockerignore
+-rw-rw-rw-   0        0        0      295 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.git-blame-ignore-revs
+-rw-rw-rw-   0        0        0      490 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.gitattributes
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.203842 locust_je_test_pep621-2.15.2.dev8/.github/
+-rw-rw-rw-   0        0        0      485 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.github/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.206834 locust_je_test_pep621-2.15.2.dev8/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0     1422 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      397 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      949 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.209827 locust_je_test_pep621-2.15.2.dev8/.github/workflows/
+-rw-rw-rw-   0        0        0     1231 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.github/workflows/stale.yml
+-rw-rw-rw-   0        0        0     6701 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.github/workflows/tests.yml
+-rw-rw-rw-   0        0        0      373 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.gitignore
+-rw-rw-rw-   0        0        0      197 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.readthedocs.yml
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.212826 locust_je_test_pep621-2.15.2.dev8/.vscode/
+-rw-rw-rw-   0        0        0      302 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.vscode/launch.json
+-rw-rw-rw-   0        0        0      531 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.vscode/launch_locust.json
+-rw-rw-rw-   0        0        0     1120 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/.vscode/settings.json
+-rw-rw-rw-   0        0        0    81934 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/CHANGELOG.md
+-rw-rw-rw-   0        0        0      756 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/Dockerfile
+-rw-rw-rw-   0        0        0     1115 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/LICENSE
+-rw-rw-rw-   0        0        0      115 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/MANIFEST.in
+-rw-rw-rw-   0        0        0      459 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/Makefile
+-rw-rw-rw-   0        0        0     8463 2023-04-13 14:08:42.424521 locust_je_test_pep621-2.15.2.dev8/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/README
+-rw-rw-rw-   0        0        0     5760 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/README.md
+-rw-rw-rw-   0        0        0      210 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/Vagrantfile
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.214813 locust_je_test_pep621-2.15.2.dev8/benchmarks/
+-rw-rw-rw-   0        0        0    11166 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/benchmarks/dispatch.py
+-rw-rw-rw-   0        0        0      122 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/codecov.yml
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.242739 locust_je_test_pep621-2.15.2.dev8/docs/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.243735 locust_je_test_pep621-2.15.2.dev8/docs/_static/
+-rw-rw-rw-   0        0        0      277 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/_static/theme-overrides.css
+-rw-rw-rw-   0        0        0     3858 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/api.rst
+-rw-rw-rw-   0        0        0    48404 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/changelog.rst
+-rw-rw-rw-   0        0        0     5764 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/conf.py
+-rw-rw-rw-   0        0        0     7109 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/configuration.rst
+-rw-rw-rw-   0        0        0     4084 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/custom-load-shape.rst
+-rw-rw-rw-   0        0        0     4494 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/developing-locust.rst
+-rw-rw-rw-   0        0        0     8072 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/extending-locust.rst
+-rw-rw-rw-   0        0        0     1769 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/further-reading.rst
+-rw-rw-rw-   0        0        0     1746 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/history.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.250762 locust_je_test_pep621-2.15.2.dev8/docs/images/
+-rw-rw-rw-   0        0        0    33267 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/images/number_of_users.png
+-rw-rw-rw-   0        0        0    39252 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/images/response_times.png
+-rw-rw-rw-   0        0        0    37701 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/images/total_requests_per_second.png
+-rw-rw-rw-   0        0        0   162727 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/images/userclass_picker_example.png
+-rw-rw-rw-   0        0        0   196117 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/images/webui-running-statistics.png
+-rw-rw-rw-   0        0        0   163847 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/images/webui-splash-screenshot.png
+-rw-rw-rw-   0        0        0     4959 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/increase-performance.rst
+-rw-rw-rw-   0        0        0     1641 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/index.rst
+-rw-rw-rw-   0        0        0     1053 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/installation.rst
+-rw-rw-rw-   0        0        0     2609 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/logging.rst
+-rw-rw-rw-   0        0        0     4759 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/quickstart.rst
+-rw-rw-rw-   0        0        0      119 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/requirements.txt
+-rw-rw-rw-   0        0        0     1710 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/retrieving-stats.rst
+-rw-rw-rw-   0        0        0      851 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/running-cloud-integration.rst
+-rw-rw-rw-   0        0        0     5654 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/running-distributed.rst
+-rw-rw-rw-   0        0        0     4009 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/running-in-debugger.rst
+-rw-rw-rw-   0        0        0     2160 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/running-in-docker.rst
+-rw-rw-rw-   0        0        0     4610 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/running-without-web-ui.rst
+-rw-rw-rw-   0        0        0     6346 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/tasksets.rst
+-rw-rw-rw-   0        0        0     3328 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/testing-other-systems.rst
+-rw-rw-rw-   0        0        0     2420 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/use-as-lib.rst
+-rw-rw-rw-   0        0        0     4432 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/what-is-locust.rst
+-rw-rw-rw-   0        0        0    26100 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/docs/writing-a-locustfile.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.274653 locust_je_test_pep621-2.15.2.dev8/examples/
+-rw-rw-rw-   0        0        0      991 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/add_command_line_argument.py
+-rw-rw-rw-   0        0        0      618 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/basic.py
+-rw-rw-rw-   0        0        0     1566 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/browse_docs_sequence_test.py
+-rw-rw-rw-   0        0        0     1420 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/browse_docs_test.py
+-rw-rw-rw-   0        0        0     2055 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_messages.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.280878 locust_je_test_pep621-2.15.2.dev8/examples/custom_shape/
+-rw-rw-rw-   0        0        0     1404 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_shape/double_wave.py
+-rw-rw-rw-   0        0        0     1540 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_shape/stages.py
+-rw-rw-rw-   0        0        0     1971 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_shape/staging_user_classes.py
+-rw-rw-rw-   0        0        0      960 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_shape/step_load.py
+-rw-rw-rw-   0        0        0     2342 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_shape/wait_user_count.py
+-rw-rw-rw-   0        0        0     1423 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_wait_function.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.282873 locust_je_test_pep621-2.15.2.dev8/examples/custom_xmlrpc_client/
+-rw-rw-rw-   0        0        0      490 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_xmlrpc_client/server.py
+-rw-rw-rw-   0        0        0     2308 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/custom_xmlrpc_client/xmlrpc_locustfile.py
+-rw-rw-rw-   0        0        0      460 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/debugging.py
+-rw-rw-rw-   0        0        0      685 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/debugging_advanced.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.283871 locust_je_test_pep621-2.15.2.dev8/examples/docker-compose/
+-rw-rw-rw-   0        0        0      364 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/docker-compose/docker-compose.yml
+-rw-rw-rw-   0        0        0      665 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/dynamic_user_credentials.py
+-rw-rw-rw-   0        0        0     2404 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/events.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.284869 locust_je_test_pep621-2.15.2.dev8/examples/extend_web_ui/
+-rw-rw-rw-   0        0        0     4663 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/extend_web_ui/extend.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.286862 locust_je_test_pep621-2.15.2.dev8/examples/extend_web_ui/static/
+-rw-rw-rw-   0        0        0      809 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/extend_web_ui/static/custom-stats-table.css
+-rw-rw-rw-   0        0        0     2485 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/extend_web_ui/static/extend.js
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.287860 locust_je_test_pep621-2.15.2.dev8/examples/extend_web_ui/templates/
+-rw-rw-rw-   0        0        0     2056 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/extend_web_ui/templates/extend.html
+-rw-rw-rw-   0        0        0      578 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/fast_http_locust.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.294841 locust_je_test_pep621-2.15.2.dev8/examples/grpc/
+-rw-rw-rw-   0        0        0     1952 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/grpc/grpc_user.py
+-rw-rw-rw-   0        0        0      234 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/grpc/hello.proto
+-rw-rw-rw-   0        0        0     4829 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/grpc/hello_pb2.py
+-rw-rw-rw-   0        0        0     2493 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/grpc/hello_pb2_grpc.py
+-rw-rw-rw-   0        0        0      777 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/grpc/hello_server.py
+-rw-rw-rw-   0        0        0      562 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/grpc/locustfile.py
+-rw-rw-rw-   0        0        0      514 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/locustfile.py
+-rw-rw-rw-   0        0        0     2223 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/manual_stats_reporting.py
+-rw-rw-rw-   0        0        0      897 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/multiple_hosts.py
+-rw-rw-rw-   0        0        0      607 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/nested_inline_tasksets.py
+-rw-rw-rw-   0        0        0     4501 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/rest.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.295838 locust_je_test_pep621-2.15.2.dev8/examples/sdk_session_patching/
+-rw-rw-rw-   0        0        0      783 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/sdk_session_patching/session_patch_locustfile.py
+-rw-rw-rw-   0        0        0      652 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/semaphore_wait.py
+-rw-rw-rw-   0        0        0     1072 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/stop_on_threshold.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.166942 locust_je_test_pep621-2.15.2.dev8/examples/terraform/
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.301822 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/
+-rw-rw-rw-   0        0        0     1794 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/README.md
+-rw-rw-rw-   0        0        0      120 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/data_subnet.tf
+-rw-rw-rw-   0        0        0      954 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/main.tf
+-rw-rw-rw-   0        0        0      783 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/output.tf
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.302819 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/plan/
+-rw-rw-rw-   0        0        0      523 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/plan/basic.py
+-rw-rw-rw-   0        0        0       47 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/provisioner.tf
+-rw-rw-rw-   0        0        0      307 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/terraform/aws/variables.tf
+-rw-rw-rw-   0        0        0     4154 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/test_data_management.py
+-rw-rw-rw-   0        0        0     1147 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/use_as_lib.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.305811 locust_je_test_pep621-2.15.2.dev8/examples/vagrant/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/vagrant/README.md
+-rw-rw-rw-   0        0        0     1604 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/vagrant/supervisord.conf
+-rw-rw-rw-   0        0        0      504 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/vagrant/vagrant.sh
+-rw-rw-rw-   0        0        0      662 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/examples/worker_index.py
+-rw-rw-rw-   0        0        0      975 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/generate_changelog.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.326756 locust_je_test_pep621-2.15.2.dev8/locust/
+-rw-rw-rw-   0        0        0     1385 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/__init__.py
+-rw-rw-rw-   0        0        0       34 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/__main__.py
+-rw-rw-rw-   0        0        0      179 2023-04-13 14:08:41.000000 locust_je_test_pep621-2.15.2.dev8/locust/_version.py
+-rw-rw-rw-   0        0        0    25259 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/argument_parser.py
+-rw-rw-rw-   0        0        0    15095 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/clients.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.327752 locust_je_test_pep621-2.15.2.dev8/locust/contrib/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/contrib/__init__.py
+-rw-rw-rw-   0        0        0    26952 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/contrib/fasthttp.py
+-rw-rw-rw-   0        0        0     4858 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/debug.py
+-rw-rw-rw-   0        0        0    19147 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/dispatch.py
+-rw-rw-rw-   0        0        0    11617 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/env.py
+-rw-rw-rw-   0        0        0     6121 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/event.py
+-rw-rw-rw-   0        0        0     2029 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/exception.py
+-rw-rw-rw-   0        0        0     3677 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/html.py
+-rw-rw-rw-   0        0        0     3161 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/input_events.py
+-rw-rw-rw-   0        0        0     2859 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/log.py
+-rw-rw-rw-   0        0        0    20295 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/main.py
+-rw-rw-rw-   0        0        0       66 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.330744 locust_je_test_pep621-2.15.2.dev8/locust/rpc/
+-rw-rw-rw-   0        0        0       60 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/rpc/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/rpc/protocol.py
+-rw-rw-rw-   0        0        0     2667 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/rpc/zmqrpc.py
+-rw-rw-rw-   0        0        0    65383 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/runners.py
+-rw-rw-rw-   0        0        0     1482 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/shape.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.340719 locust_je_test_pep621-2.15.2.dev8/locust/static/
+-rw-rw-rw-   0        0        0     4929 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/chart.js
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.345706 locust_je_test_pep621-2.15.2.dev8/locust/static/css/
+-rw-rw-rw-   0        0        0     9617 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/css/application.css
+-rw-rw-rw-   0        0        0     2089 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/css/application.css.map
+-rw-rw-rw-   0        0        0     1477 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/css/tables.css
+-rw-rw-rw-   0        0        0      411 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/css/tables.css.map
+-rw-rw-rw-   0        0        0   620479 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/echarts.common.min.js
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.352686 locust_je_test_pep621-2.15.2.dev8/locust/static/img/
+-rw-rw-rw-   0        0        0     8348 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/img/favicon.ico
+-rw-rw-rw-   0        0        0    24553 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/img/logo.png
+-rw-rw-rw-   0        0        0    79701 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-charts.png
+-rw-rw-rw-   0        0        0    64670 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-start-test.png
+-rw-rw-rw-   0        0        0    95837 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-stats.png
+-rw-rw-rw-   0        0        0   151806 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-workers.png
+-rw-rw-rw-   0        0        0    95962 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/jquery-1.11.3.min.js
+-rw-rw-rw-   0        0        0     3395 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/jquery.jqote2.min.js
+-rw-rw-rw-   0        0        0     2998 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/jquery.tools.min.js
+-rw-rw-rw-   0        0        0    10588 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/locust.js
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.356675 locust_je_test_pep621-2.15.2.dev8/locust/static/sass/
+-rw-rw-rw-   0        0        0      485 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/sass/_base.sass
+-rw-rw-rw-   0        0        0       72 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/sass/_mixins.sass
+-rw-rw-rw-   0        0        0     8832 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/sass/application.sass
+-rw-rw-rw-   0        0        0     1422 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/sass/tables.sass
+-rw-rw-rw-   0        0        0     1418 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/tasks.js
+-rw-rw-rw-   0        0        0     1171 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/static/vintage.js
+-rw-rw-rw-   0        0        0    45246 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/stats.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.360959 locust_je_test_pep621-2.15.2.dev8/locust/templates/
+-rw-rw-rw-   0        0        0    22248 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/templates/index.html
+-rw-rw-rw-   0        0        0    10932 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/templates/report.html
+-rw-rw-rw-   0        0        0     1274 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/templates/stats_data.html
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.389070 locust_je_test_pep621-2.15.2.dev8/locust/test/
+-rw-rw-rw-   0        0        0      411 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/__init__.py
+-rw-rw-rw-   0        0        0      171 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/fake_module1_for_env_test.py
+-rw-rw-rw-   0        0        0      171 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/fake_module2_for_env_test.py
+-rw-rw-rw-   0        0        0     1331 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/mock_locustfile.py
+-rw-rw-rw-   0        0        0      810 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/mock_logging.py
+-rw-rw-rw-   0        0        0   168977 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_dispatch.py
+-rw-rw-rw-   0        0        0     6327 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_env.py
+-rw-rw-rw-   0        0        0    30195 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_fasthttp.py
+-rw-rw-rw-   0        0        0    12065 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_http.py
+-rw-rw-rw-   0        0        0     5520 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_load_locustfile.py
+-rw-rw-rw-   0        0        0    26371 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_locust_class.py
+-rw-rw-rw-   0        0        0     6943 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_log.py
+-rw-rw-rw-   0        0        0    61009 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_main.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_old_wait_api.py
+-rw-rw-rw-   0        0        0    16559 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_parser.py
+-rw-rw-rw-   0        0        0   157889 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_runners.py
+-rw-rw-rw-   0        0        0     3533 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_sequential_taskset.py
+-rw-rw-rw-   0        0        0    34710 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_stats.py
+-rw-rw-rw-   0        0        0    13576 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_tags.py
+-rw-rw-rw-   0        0        0     2836 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_taskratio.py
+-rw-rw-rw-   0        0        0     2204 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_users.py
+-rw-rw-rw-   0        0        0     1260 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_util.py
+-rw-rw-rw-   0        0        0     2432 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_wait_time.py
+-rw-rw-rw-   0        0        0    42011 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_web.py
+-rw-rw-rw-   0        0        0     2119 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/test_zmqrpc.py
+-rw-rw-rw-   0        0        0     6573 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/testcases.py
+-rw-rw-rw-   0        0        0     2753 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/test/util.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.395054 locust_je_test_pep621-2.15.2.dev8/locust/user/
+-rw-rw-rw-   0        0        0       73 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/user/__init__.py
+-rw-rw-rw-   0        0        0     2721 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/user/inspectuser.py
+-rw-rw-rw-   0        0        0     2604 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/user/sequential_taskset.py
+-rw-rw-rw-   0        0        0    17070 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/user/task.py
+-rw-rw-rw-   0        0        0     9438 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/user/users.py
+-rw-rw-rw-   0        0        0     2861 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/user/wait_time.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.402035 locust_je_test_pep621-2.15.2.dev8/locust/util/
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/util/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/util/cache.py
+-rw-rw-rw-   0        0        0     2086 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/util/deprecation.py
+-rw-rw-rw-   0        0        0      823 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/util/exception_handler.py
+-rw-rw-rw-   0        0        0     2712 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/util/load_locustfile.py
+-rw-rw-rw-   0        0        0       94 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/util/rounding.py
+-rw-rw-rw-   0        0        0     1022 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/util/timespan.py
+-rw-rw-rw-   0        0        0    25689 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/locust/web.py
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.418537 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/
+-rw-rw-rw-   0        0        0     8463 2023-04-13 14:08:41.000000 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5910 2023-04-13 14:08:42.000000 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 14:08:41.000000 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-13 14:08:41.000000 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-13 14:06:54.000000 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      286 2023-04-13 14:08:41.000000 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-13 14:08:41.000000 locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2814 2023-04-13 14:08:26.000000 locust_je_test_pep621-2.15.2.dev8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-13 14:08:42.423523 locust_je_test_pep621-2.15.2.dev8/scripts/
+-rw-rw-rw-   0        0        0     2209 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/scripts/locustfile.py
+-rw-rw-rw-   0        0        0     1340 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/scripts/run-disributed-headless.sh
+-rw-rw-rw-   0        0        0     1325 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/scripts/run-disributed-web.sh
+-rw-rw-rw-   0        0        0      478 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/scripts/run-local-headless.sh
+-rw-rw-rw-   0        0        0      463 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/scripts/run-local-web.sh
+-rw-rw-rw-   0        0        0     2203 2023-04-13 14:08:42.430505 locust_je_test_pep621-2.15.2.dev8/setup.cfg
+-rw-rw-rw-   0        0        0      174 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/setup.py
+-rw-rw-rw-   0        0        0     1390 2023-04-13 12:45:27.000000 locust_je_test_pep621-2.15.2.dev8/tox.ini
```

### Comparing `locust_je_test_pep621-0.0.0/LICENSE` & `locust_je_test_pep621-2.15.2.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/PKG-INFO` & `locust_je_test_pep621-2.15.2.dev8/locust_je_test_pep621.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: locust_je_test_pep621
-Version: 0.0.0
+Name: locust-je-test-pep621
+Version: 2.15.2.dev8
 Summary: Developer friendly load testing framework
 Home-page: https://locust.io/
 License: The MIT License
         
         Copyright (c) 2009-2010, Carl Byström, Jonatan Heyman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `locust_je_test_pep621-0.0.0/README.md` & `locust_je_test_pep621-2.15.2.dev8/README.md`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/__init__.py` & `locust_je_test_pep621-2.15.2.dev8/locust/__init__.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/argument_parser.py` & `locust_je_test_pep621-2.15.2.dev8/locust/argument_parser.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/clients.py` & `locust_je_test_pep621-2.15.2.dev8/locust/clients.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/contrib/fasthttp.py` & `locust_je_test_pep621-2.15.2.dev8/locust/contrib/fasthttp.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/debug.py` & `locust_je_test_pep621-2.15.2.dev8/locust/debug.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/dispatch.py` & `locust_je_test_pep621-2.15.2.dev8/locust/dispatch.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/env.py` & `locust_je_test_pep621-2.15.2.dev8/locust/env.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/event.py` & `locust_je_test_pep621-2.15.2.dev8/locust/event.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/exception.py` & `locust_je_test_pep621-2.15.2.dev8/locust/exception.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/html.py` & `locust_je_test_pep621-2.15.2.dev8/locust/html.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/input_events.py` & `locust_je_test_pep621-2.15.2.dev8/locust/input_events.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/log.py` & `locust_je_test_pep621-2.15.2.dev8/locust/log.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/main.py` & `locust_je_test_pep621-2.15.2.dev8/locust/main.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/rpc/zmqrpc.py` & `locust_je_test_pep621-2.15.2.dev8/locust/rpc/zmqrpc.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/runners.py` & `locust_je_test_pep621-2.15.2.dev8/locust/runners.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/shape.py` & `locust_je_test_pep621-2.15.2.dev8/locust/shape.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/chart.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/chart.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/css/application.css` & `locust_je_test_pep621-2.15.2.dev8/locust/static/css/application.css`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/css/application.css.map` & `locust_je_test_pep621-2.15.2.dev8/locust/static/css/application.css.map`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/css/tables.css` & `locust_je_test_pep621-2.15.2.dev8/locust/static/css/tables.css`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/echarts.common.min.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/echarts.common.min.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/img/favicon.ico` & `locust_je_test_pep621-2.15.2.dev8/locust/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/img/logo.png` & `locust_je_test_pep621-2.15.2.dev8/locust/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-charts.png` & `locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-charts.png`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-start-test.png` & `locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-start-test.png`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-stats.png` & `locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-stats.png`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/img/ui-screenshot-workers.png` & `locust_je_test_pep621-2.15.2.dev8/locust/static/img/ui-screenshot-workers.png`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/jquery-1.11.3.min.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/jquery-1.11.3.min.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/jquery.jqote2.min.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/jquery.jqote2.min.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/jquery.tools.min.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/locust.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/locust.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/sass/application.sass` & `locust_je_test_pep621-2.15.2.dev8/locust/static/sass/application.sass`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/sass/tables.sass` & `locust_je_test_pep621-2.15.2.dev8/locust/static/sass/tables.sass`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/tasks.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/tasks.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/static/vintage.js` & `locust_je_test_pep621-2.15.2.dev8/locust/static/vintage.js`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/stats.py` & `locust_je_test_pep621-2.15.2.dev8/locust/stats.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/templates/index.html` & `locust_je_test_pep621-2.15.2.dev8/locust/templates/index.html`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/templates/report.html` & `locust_je_test_pep621-2.15.2.dev8/locust/templates/report.html`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/templates/stats_data.html` & `locust_je_test_pep621-2.15.2.dev8/locust/templates/stats_data.html`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/mock_locustfile.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/mock_locustfile.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/mock_logging.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/mock_logging.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_dispatch.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_env.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_env.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_fasthttp.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_fasthttp.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_http.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_http.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_load_locustfile.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_load_locustfile.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_locust_class.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_locust_class.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_log.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_log.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_main.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_main.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_parser.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_runners.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_runners.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_sequential_taskset.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_sequential_taskset.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_stats.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_tags.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_tags.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_taskratio.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_taskratio.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_users.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_users.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_util.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_util.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_wait_time.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_wait_time.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_web.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_web.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/test_zmqrpc.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/test_zmqrpc.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/testcases.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/testcases.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/test/util.py` & `locust_je_test_pep621-2.15.2.dev8/locust/test/util.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/user/inspectuser.py` & `locust_je_test_pep621-2.15.2.dev8/locust/user/inspectuser.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/user/sequential_taskset.py` & `locust_je_test_pep621-2.15.2.dev8/locust/user/sequential_taskset.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/user/task.py` & `locust_je_test_pep621-2.15.2.dev8/locust/user/task.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/user/users.py` & `locust_je_test_pep621-2.15.2.dev8/locust/user/users.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/user/wait_time.py` & `locust_je_test_pep621-2.15.2.dev8/locust/user/wait_time.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/util/cache.py` & `locust_je_test_pep621-2.15.2.dev8/locust/util/cache.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/util/deprecation.py` & `locust_je_test_pep621-2.15.2.dev8/locust/util/deprecation.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/util/exception_handler.py` & `locust_je_test_pep621-2.15.2.dev8/locust/util/exception_handler.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/util/load_locustfile.py` & `locust_je_test_pep621-2.15.2.dev8/locust/util/load_locustfile.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/util/timespan.py` & `locust_je_test_pep621-2.15.2.dev8/locust/util/timespan.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust/web.py` & `locust_je_test_pep621-2.15.2.dev8/locust/web.py`

 * *Files identical despite different names*

### Comparing `locust_je_test_pep621-0.0.0/locust_je_test_pep621.egg-info/PKG-INFO` & `locust_je_test_pep621-2.15.2.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: locust-je-test-pep621
-Version: 0.0.0
+Name: locust_je_test_pep621
+Version: 2.15.2.dev8
 Summary: Developer friendly load testing framework
 Home-page: https://locust.io/
 License: The MIT License
         
         Copyright (c) 2009-2010, Carl Byström, Jonatan Heyman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `locust_je_test_pep621-0.0.0/pyproject.toml` & `locust_je_test_pep621-2.15.2.dev8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["setuptools>=61"]
+requires = ["setuptools>=61", "setuptools_scm", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "locust_je_test_pep621"
 license = { file = "LICENSE"}
 description = "Developer friendly load testing framework"
 dynamic = ["version"]
-
+requires-python = ">=3.7"
 dependencies = [
     "gevent >=20.12.1",
     "flask >=2.0.0",
     "Werkzeug >=2.0.0",
     "requests >=2.23.0",
     "msgpack >=0.6.2",
     "pyzmq >=22.2.1, !=23.0.0",
@@ -65,15 +65,14 @@
 
 [tool.setuptools_scm]
 write_to = "locust/_version.py"
 local_scheme = "no-local-version"
 
 [options]
 zip_safe = false
-requires-python = ">=3.7"
 
 [options.packages.find]
 namespace = true
 include = ["locust*"]
 exclude = [
     "examples",
     "tests",
```

### Comparing `locust_je_test_pep621-0.0.0/setup.cfg` & `locust_je_test_pep621-2.15.2.dev8/setup.cfg`

 * *Files identical despite different names*

