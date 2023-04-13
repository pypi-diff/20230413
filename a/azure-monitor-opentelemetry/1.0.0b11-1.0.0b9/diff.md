# Comparing `tmp/azure-monitor-opentelemetry-1.0.0b11.tar.gz` & `tmp/azure-monitor-opentelemetry-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ApplicationInsights-Python/ApplicationInsights-Python/dist/azure-monitor-opentelemetry-1.0.0b11.tar", last modified: Thu Apr 13 18:21:58 2023, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-1.0.0b9.tar", last modified: Wed Feb 22 22:31:32 2023, max compression
```

## Comparing `azure-monitor-opentelemetry-1.0.0b11.tar` & `azure-monitor-opentelemetry-1.0.0b9.tar`

### file list

```diff
@@ -1,96 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/autoinstrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/autoinstrumentation/_distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/diagnostics/_diagnostic_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/diagnostics/_status_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/util/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/util/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/logging/correlated_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/logging/custom_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/logging/exception_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/logging/logs_with_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/logging/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/metrics/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/metrics/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/metrics/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/db_psycopg2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/example/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/sample/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/sample/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/sample/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/sample/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/django/sample/sample/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/http_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/http_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/http_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/http_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/http_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/samples/tracing/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/tests/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/autoinstrumentation/test_distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    22056 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/configuration/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/configuration/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/tests/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/diagnostics/test_diagnostic_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/diagnostics/test_status_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/tests/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/exporter/test_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:21:58.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/test_django.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/test_psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/instrumentation/test_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-13 18:21:52.000000 azure-monitor-opentelemetry-1.0.0b11/tests/test_constants.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.179282 azure-monitor-opentelemetry-1.0.0b9/
+-rw-rw-rw-   0        0        0     9608 2023-02-22 22:31:32.180284 azure-monitor-opentelemetry-1.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     8745 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.049037 azure-monitor-opentelemetry-1.0.0b9/azure/
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.050037 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.080216 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/
+-rw-rw-rw-   0        0        0      494 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/__init__.py
+-rw-rw-rw-   0        0        0     9163 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_configure.py
+-rw-rw-rw-   0        0        0     2299 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_constants.py
+-rw-rw-rw-   0        0        0      734 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_types.py
+-rw-rw-rw-   0        0        0      334 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_version.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.094215 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/
+-rw-rw-rw-   0        0        0      310 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/__init__.py
+-rw-rw-rw-   0        0        0     1125 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py
+-rw-rw-rw-   0        0        0     2984 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_distro.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.107694 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/
+-rw-rw-rw-   0        0        0        0 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_diagnostic_logging.py
+-rw-rw-rw-   0        0        0     1987 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_status_logger.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.112712 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/util/
+-rw-rw-rw-   0        0        0      647 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.175279 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      295 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-22 21:49:02.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      320 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-02-22 22:31:32.195109 azure-monitor-opentelemetry-1.0.0b9/setup.cfg
+-rw-rw-rw-   0        0        0     3587 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.178279 azure-monitor-opentelemetry-1.0.0b9/tests/
+-rw-rw-rw-   0        0        0     5452 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/tests/test_constants.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/PKG-INFO` & `azure-monitor-opentelemetry-1.0.0b9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,142 @@
-Metadata-Version: 2.1
-Name: azure-monitor-opentelemetry
-Version: 1.0.0b11
-Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
-Home-page: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry
-Author: Microsoft Corporation
-Author-email: ascl@microsoft.com
-License: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Azure Monitor Opentelemetry Distro
-
-The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] provides multiple installable components available for an Opentelemetry Azure Monitor monitoring solution. It allows you to instrument your Python applications to capture and report telemetry to Azure Monitor via the Azure monitor exporters.
-
-This distro automatically installs the following libraries:
-
-* [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters]
-* A subset of OpenTelemetry [instrumentations][ot_instrumentations] that are officially supported as listed below.
-
-## Officially supported instrumentations
-
-OpenTelemetry instrumentations allow automatic collection of requests sent from underlying instrumented libraries. The following is a list of OpenTelemetry instrumentations that come bundled in with the Azure monitor distro. If you would like to add support for another OpenTelemetry instrumentation, please submit a feature [request][distro_feature_request]. In the meantime, you can use the OpenTelemetry instrumentation manually via it's own APIs (i.e. `instrument()`) in your code. See [this][samples_manual] for an example.
-
-| Instrumentation | Supported library | Supported versions |
-| ------------------------------------- | ----------------- | ------------------ |
-| [OpenTelemetry Django Instrumentation][ot_instrumentation_django] | [django][pypi_django] | [link][ot_instrumentation_django_version]
-| [OpenTelemetry FastApi Instrumentation][ot_instrumentation_fastapi] | [fastapi][pypi_fastapi] | [link][ot_instrumentation_fastapi_version]
-| [OpenTelemetry Flask Instrumentation][ot_instrumentation_flask] | [flask][pypi_flask] | [link][ot_instrumentation_flask_version]
-| [OpenTelemetry Psycopg2 Instrumentation][ot_instrumentation_psycopg2] | [psycopg2][pypi_psycopg2] | [link][ot_instrumentation_psycopg2_version]
-| [OpenTelemetry Requests Instrumentation][ot_instrumentation_requests] | [requests][pypi_requests] | [link][ot_instrumentation_requests_version]
-| [OpenTelemetry UrlLib Instrumentation][ot_instrumentation_urllib] | [urllib][pypi_urllib] | All
-| [OpenTelemetry UrlLib3 Instrumentation][ot_instrumentation_urllib3] | [urllib3][pypi_urllib3] | [link][ot_instrumentation_urllib3_version]
-
-## Getting started
-
-### Key Concepts
-
-This package bundles a series of OpenTelemetry and Azure Monitor components to enable the collection and sending of telemetry to Azure Monitor. For MANUAL instrumentation, use the `configure_azure_monitor` function. AUTOMATIC instrumentation is not yet supported.
-
-The [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters] are the main components in accomplishing this. You will be able to use the exporters and their APIs directly through this package. Please go the exporter documentation to understand how OpenTelemetry and Azure Monitor components work in enabling telemetry collection and exporting.
-
-Currently, all instrumentations available in OpenTelemetry are in a beta state, meaning they are not stable and may have breaking changes in the future. Efforts are being made in pushing these to a more stable state.
-
-### Prerequisites
-
-To use this package, you must have:
-
-* Azure subscription - [Create a free account][azure_sub]
-* Azure Monitor - [How to use application insights][application_insights_namespace]
-* Opentelemetry SDK - [Opentelemetry SDK for Python][ot_sdk_python]
-* Python 3.7 or later - [Install Python][python]
-
-### Install the package
-
-Install the Azure Monitor Opentelemetry Distro with [pip][pip]:
-
-```Bash
-pip install azure-monitor-opentelemetry --pre
-```
-
-### Usage
-
-You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments:
-
-| Parameter | Description | Environment Variable |
-|-------------------|----------------------------------------------------|----------------------|
-| `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
-| `exclude_instrumentations` | By default, all supported [instrumentations](#officially-supported-instrumentations) are enabled to collect telemetry. Specify instrumentations you do not want to enable to collect telemetry by passing in a comma separated list of instrumented library names. e.g. `["requests", "flask"]` | |
-| `resource` | Specifies the OpenTelemetry [resource][opentelemetry_spec_resource] associated with your application. See [this][ot_sdk_python_resource] for default behavior. | [OTEL_SERVICE_NAME][opentelemetry_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][opentelemetry_spec_resource_attributes] |
-| `disable_logging` | If set to `True`, disables collection and export of logging telemetry. Defaults to `False`. | |
-| `disable_metrics` | If set to `True`, disables collection and export of metric telemetry. Defaults to `False`. | |
-| `disable_tracing` | If set to `True`, disables collection and export of distributed tracing telemetry. Defaults to `False`. | |
-| `logging_level` | Specifies the [logging level][logging_level] of the logs you would like to collect for your logging pipeline. Defaults to 0 which is `logging.NOTSET`. | |
-| `logger_name` | Specifies the [logger name][logger_name_hierarchy_doc] under which logging will be instrumented. Defaults to "" which corresponds to the root logger. | |
-| `logging_export_interval_ms`| Specifies the logging export interval in milliseconds. Defaults to 5000. | `OTEL_BLRP_SCHEDULE_DELAY` |
-| `metric_readers` | Specifies the [metric readers][ot_metric_reader] that you would like to use for your metric pipeline. Accepts a list of [metric readers][ot_sdk_python_metric_reader]. | |
-| `views` | Specifies the list of [views][opentelemetry_spec_view] to configure for the metric pipeline. See [here][ot_sdk_python_view_examples] for example usage. | |
-| `sampling_ratio` | Specifies the ratio of distributed tracing telemetry to be [sampled][application_insights_sampling]. Accepted values are in the range [0,1]. Defaults to 1.0, meaning no telemetry is sampled out. | `OTEL_TRACES_SAMPLER_ARG` |
-| `tracing_export_interval_ms`| Specifies the distributed tracing export interval in milliseconds. Defaults to 5000. | `OTEL_BSP_SCHEDULE_DELAY` |
-| `instrumentation_config` | Specifies a dictionary of kwargs that will be applied to instrumentation configuration. You can specify which instrumentation you want to configure by name in the key field and value as a dictionary representing `kwargs` for the corresponding instrumentation. Refer to the `Supported Library` section [above](#officially-supported-instrumentations) for the list of supported library names. | |
-
-Example for use of `instrumentation_config`:
-```python
-...
-configure_azure_monitor(
-    connection_string="<your-connection-string>",
-    instrumentation_config={
-        "flask": {
-            "excluded_urls": "http://localhost:8080/ignore",
-        },
-        "requests": {
-            "excluded_urls": "http://example.com"
-        }
-    }
-)
-...
-```
-
-Take a look at the specific [instrumenation][ot_instrumentations] documentation for available configurations.
-
-#### Azure monitor OpenTelemetry Exporter configurations
-
-You can pass Azure monitor OpenTelemetry exporter configuration parameters directly into `configure_azure_monitor`. See additional [configuration related to exporting here][exporter_configuration_docs].
-
-```python
-...
-configure_azure_monitor(
-   connection_string="<your-connection-string>",
-   disable_offline_storage=True, 
-)
-...
-```
-
-### Samples
-
-Samples are available [here][samples] to demonstrate how to utilize the above configuration options.
-
-### Additional documentation
-
-* [Azure Portal][azure_portal]
-* [Official Azure monitor docs][azure_monitor_opentelemetry]
-* [OpenTelemetry Python Official Docs][ot_python_docs]
-
-<!-- LINKS -->
-[azure_monitor_opentelemetry]: https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-enable?tabs=python
-[azure_monitor_opentelemetry_exporters]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#microsoft-opentelemetry-exporter-for-azure-monitor
-[azure_portal]: https://portal.azure.com
-[azure_sub]: https://azure.microsoft.com/free/
-[application_insights_namespace]: https://learn.microsoft.com/azure/azure-monitor/app/app-insights-overview
-[application_insights_sampling]: https://learn.microsoft.com/azure/azure-monitor/app/sampling
-[connection_string_doc]: https://learn.microsoft.com/azure/azure-monitor/app/sdk-connection-string
-[distro_feature_request]: https://github.com/microsoft/ApplicationInsights-Python/issues/new
-[exporter_configuration_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#configuration
-[logging_level]: https://docs.python.org/3/library/logging.html#levels
-[logger_name_hierarchy_doc]: https://docs.python.org/3/library/logging.html#logger-objects
-[ot_instrumentations]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
-[ot_metric_reader]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#metricreader
-[ot_python_docs]: https://opentelemetry.io/docs/instrumentation/python/
-[ot_sdk_python]: https://github.com/open-telemetry/opentelemetry-python
-[ot_sdk_python_metric_reader]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/metrics.export.html#opentelemetry.sdk.metrics.export.MetricReader
-[ot_sdk_python_resource]: https://github.com/open-telemetry/opentelemetry-python/blob/main/opentelemetry-sdk/src/opentelemetry/sdk/resources/__init__.py#L153
-[ot_sdk_python_view_examples]: https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples/metrics/views
-[ot_instrumentation_django]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django
-[ot_instrumentation_django_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-django/src/opentelemetry/instrumentation/django/package.py#L16
-[ot_instrumentation_fastapi]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-fastapi
-[ot_instrumentation_fastapi_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-fastapi/src/opentelemetry/instrumentation/fastapi/package.py#L16
-[ot_instrumentation_flask]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask
-[ot_instrumentation_flask_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-flask/src/opentelemetry/instrumentation/flask/package.py#L16
-[ot_instrumentation_psycopg2]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-psycopg2
-[ot_instrumentation_psycopg2_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-psycopg2/src/opentelemetry/instrumentation/psycopg2/package.py#L16
-[ot_instrumentation_requests]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
-[ot_instrumentation_requests_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-requests/src/opentelemetry/instrumentation/requests/package.py#L16
-[ot_instrumentation_urllib]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3
-[ot_instrumentation_urllib3]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3
-[ot_instrumentation_urllib3_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-urllib3/src/opentelemetry/instrumentation/urllib3/package.py#L16
-[opentelemetry_spec_resource]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/resource/sdk.md#resource-sdk
-[opentelemetry_spec_resource_attributes]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/resource/sdk.md#specifying-resource-information-via-an-environment-variable
-[opentelemetry_spec_service_name]: https://github.com/open-telemetry/opentelemetry-specification/tree/main/specification/resource/semantic_conventions#semantic-attributes-with-sdk-provided-default-value
-[opentelemetry_spec_view]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#view
-[pip]: https://pypi.org/project/pip/
-[pypi_django]: https://pypi.org/project/Django/
-[pypi_fastapi]: https://pypi.org/project/fastapi/
-[pypi_flask]: https://pypi.org/project/Flask/
-[pypi_psycopg2]: https://pypi.org/project/psycopg2/
-[pypi_requests]: https://pypi.org/project/requests/
-[pypi_urllib]: https://docs.python.org/3/library/urllib.html
-[pypi_urllib3]: https://pypi.org/project/urllib3/
-[python]: https://www.python.org/downloads/
-[samples]: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry/samples
-[samples_manual]: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry/samples/tracing/manual.py
+Metadata-Version: 2.1
+Name: azure-monitor-opentelemetry
+Version: 1.0.0b9
+Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
+Home-page: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry
+Author: Microsoft Corporation
+Author-email: ascl@microsoft.com
+License: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# Azure Monitor Opentelemetry Distro
+
+The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] provides multiple installable components available for an Opentelemetry Azure Monitor monitoring solution. It allows you to instrument your Python applications to capture and report telemetry to Azure Monitor via the Azure monitor exporters.
+
+This distro automatically installs the following libraries:
+
+* [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters]
+* [OpenTelemetry Requests Instrumentation][opentelemetry_instrumentation_requests]
+* [OpenTelemetry Django Instrumentation][opentelemetry_instrumentation_django]
+* [OpenTelemetry Flask Instrumentation][opentelemetry_instrumentation_flask]
+* [OpenTelemetry Psycopg2 Instrumentation][opentelemetry_instrumentation_psycopg2]
+
+## Getting started
+
+### Key Concepts
+
+This package bundles a series of OpenTelemetry and Azure Monitor components to enable the collection and sending of telemetry to Azure Monitor. For MANUAL instrumentation, use the `configure_azure_monitor` function. AUTOMATIC instrumentation is not yet supported.
+
+The [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters] are the main components in accomplishing this. You will be able to use the exporters and their APIs directly through this package. Please go the exporter documentation to understand how OpenTelemetry and Azure Monitor components work in enabling telemetry collection and exporting.
+
+Currently, all instrumentations available in OpenTelemetry are in a beta state, meaning they are not stable and may have breaking changes in the future. Efforts are being made in pushing these to a more stable state.
+
+### Prerequisites
+
+To use this package, you must have:
+
+* Azure subscription - [Create a free account][azure_sub]
+* Azure Monitor - [How to use application insights][application_insights_namespace]
+* Opentelemetry SDK - [Opentelemetry SDK for Python][ot_sdk_python]
+* Python 3.7 or later - [Install Python][python]
+
+### Install the package
+
+Install the Azure Monitor Opentelemetry Distro with [pip][pip]:
+
+```Bash
+pip install azure-monitor-opentelemetry --pre
+```
+
+### Usage
+
+You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments:
+
+* connection_string - The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in.
+* instrumentations - Specifies the libraries with [instrumentations][ot_instrumentations] that you would like to use. Accepts a comma separated list. e.g. `["requests", "flask"]`
+* disable_logging - If set to `True`, disables collection and export of logging telemetry. Defaults to `False`.
+* disable_metrics - If set to `True`, disables collection and export of metric telemetry. Defaults to `False`.
+* disable_tracing - If set to `True`, disables collection and export of distributed tracing telemetry. Defaults to `False`.
+* resource - Specified the OpenTelemetry [resource][opentelemetry_spec_resource] associated with your application. See [this][ot_sdk_python_resource] for default behavior.
+* logging_level - Specifies the [logging level][logging_level] of the logs you would like to collect for your logging pipeline. Defaults to logging.NOTSET.
+* logger_name = Specifies the [logger name][logger_name_hierarchy_doc] under which logging will be instrumented. Defaults to "" which corresponds to the root logger.
+* logging_export_interval_millis - Specifies the logging export interval in milliseconds. Defaults to 5000.
+* metric_readers - Specifies the [metric readers][ot_metric_reader] that you would like to use for your metric pipeline. Accepts a list of [metric readers][ot_sdk_python_metric_reader].
+* views - Specifies the list of [views][opentelemetry_spec_view] to configure for the metric pipeline. See [here][ot_sdk_python_view_examples] for example usage.
+* sampling_ratio - Specifies the ratio of distributed tracing telemetry to be [sampled][application_insights_sampling]. Accepted values are in the range [0,1]. Defaults to 1.0, meaning no telemetry is sampled out.
+* tracing_export_interval_millis - Specifies the distributed tracing export interval in milliseconds. Defaults to 5000.
+
+#### Exporter configurations
+
+You can pass exporter configuration parameters directly into `configure_azure_monitor`. See additional [configuration related to exporting here][exporter_configuration_docs].
+
+```python
+...
+configure_azure_monitor(
+   connection_string="<your-connection-string>",
+   disable_offline_storage=True, 
+)
+...
+```
+
+#### Instrumentation configurations
+
+You can pass in instrumentation specific configuration into `configure_azure_monitor` with the key `<instrumented-library-name>_config` and value as a dictionary representing `kwargs` for the corresponding instrumentation. Note the instrumented library must also be enabled through the `instrumentations` configuration.
+
+```python
+...
+configure_azure_monitor(
+    connection_string="<your-connection-string>",
+    instrumentations=["flask", "requests"],
+    flask_config={"excluded_urls": "http://localhost:8080/ignore"},
+    requests_config={"excluded_urls": "http://example.com"},
+)
+...
+```
+
+Take a look at the specific [instrumenation][ot_instrumentations] documentation for available configurations.
+
+### Samples
+
+Samples are available [here][samples] to demonstrate how to utilize the above configuration options.
+
+### Additional documentation
+
+[Azure Portal][azure_portal]
+[OpenTelemetry Python Official Docs][ot_python_docs]
+
+<!-- LINKS -->
+[azure_monitor_opentelemetry_exporters]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#microsoft-opentelemetry-exporter-for-azure-monitor
+[azure_portal]: https://portal.azure.com
+[azure_sub]: https://azure.microsoft.com/free/
+[application_insights_namespace]: https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview
+[application_insights_sampling]: https://learn.microsoft.com/en-us/azure/azure-monitor/app/sampling
+[connection_string_doc]: https://learn.microsoft.com/en-us/azure/azure-monitor/app/sdk-connection-string
+[exporter_configuration_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#configuration
+[logging_level]: https://docs.python.org/3/library/logging.html#levels
+[logger_name_hierarchy_doc]: https://docs.python.org/3/library/logging.html#logger-objects
+[ot_instrumentations]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
+[ot_metric_reader]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#metricreader
+[ot_python_docs]: https://opentelemetry.io/docs/instrumentation/python/
+[ot_sdk_python]: https://github.com/open-telemetry/opentelemetry-python
+[ot_sdk_python_metric_reader]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/metrics.export.html#opentelemetry.sdk.metrics.export.MetricReader
+[ot_sdk_python_resource]: https://github.com/open-telemetry/opentelemetry-python/blob/main/opentelemetry-sdk/src/opentelemetry/sdk/resources/__init__.py#L153
+[ot_sdk_python_view_examples]: https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples/metrics/views
+[opentelemetry_instrumentation_requests]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
+[opentelemetry_instrumentation_django]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django
+[opentelemetry_instrumentation_flask]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask
+[opentelemetry_instrumentation_psycopg2]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-psycopg2
+[opentelemetry_spec_resource]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/resource/sdk.md#resource-sdk
+[opentelemetry_spec_view]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#view
+[python]: https://www.python.org/downloads/
+[pip]: https://pypi.org/project/pip/
+[samples]: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry/samples
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/_configure.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_configure.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,210 +1,198 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-from logging import getLogger
-from typing import Any, Dict
-
-from azure.monitor.opentelemetry._constants import (
-    DISABLE_LOGGING_ARG,
-    DISABLE_METRICS_ARG,
-    DISABLE_TRACING_ARG,
-    EXCLUDE_INSTRUMENTATIONS_ARG,
-    INSTRUMENTATION_CONFIG_ARG,
-    LOGGER_NAME_ARG,
-    LOGGING_EXPORT_INTERVAL_MS_ARG,
-    LOGGING_LEVEL_ARG,
-    METRIC_READERS_ARG,
-    RESOURCE_ARG,
-    SAMPLING_RATIO_ARG,
-    TRACING_EXPORT_INTERVAL_MS_ARG,
-    VIEWS_ARG,
-)
-from azure.monitor.opentelemetry._types import ConfigurationValue
-from azure.monitor.opentelemetry.exporter import (
-    ApplicationInsightsSampler,
-    AzureMonitorLogExporter,
-    AzureMonitorMetricExporter,
-    AzureMonitorTraceExporter,
-)
-from azure.monitor.opentelemetry.util.configurations import _get_configurations
-from opentelemetry._logs import get_logger_provider, set_logger_provider
-from opentelemetry.instrumentation.dependencies import (
-    get_dist_dependency_conflicts,
-)
-from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
-from opentelemetry.metrics import set_meter_provider
-from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
-from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
-from opentelemetry.sdk.metrics import MeterProvider
-from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
-from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.trace import TracerProvider
-from opentelemetry.sdk.trace.export import BatchSpanProcessor
-from opentelemetry.trace import get_tracer_provider, set_tracer_provider
-from pkg_resources import iter_entry_points
-
-_logger = getLogger(__name__)
-
-
-_SUPPORTED_INSTRUMENTED_LIBRARIES = (
-    "django",
-    "fastapi",
-    "flask",
-    "psycopg2",
-    "requests",
-    "urllib",
-    "urllib3",
-)
-
-
-InstrumentationConfig = Dict[str, Dict[str, Any]]
-
-
-def configure_azure_monitor(**kwargs) -> None:
-    """
-    This function works as a configuration layer that allows the
-    end user to configure OpenTelemetry and Azure monitor components. The
-    configuration can be done via arguments passed to this function.
-    :keyword str connection_string: Connection string for your Application Insights resource.
-    :keyword Sequence[str] exclude_instrumentations: Specifies instrumentations you want to disable.
-    :keyword Resource resource: Specified the OpenTelemetry [resource][opentelemetry_spec_resource] associated with your application.
-    :keyword bool disable_logging: If set to `True`, disables collection and export of logging telemetry. Defaults to `False`.
-    :keyword bool disable_metrics: If set to `True`, disables collection and export of metric telemetry. Defaults to `False`.
-    :keyword bool disable_tracing: If set to `True`, disables collection and export of distributed tracing telemetry. Defaults to `False`.
-    :keyword int logging_level: Specifies the logging of the logs you would like to collect for your logging pipeline.
-    :keyword str logger_name: Specifies the logger name under which logging will be instrumented. Defaults to "" which corresponds to the root logger.
-    :keyword int logging_export_interval_ms: Specifies the logging export interval in milliseconds. Defaults to 5000.
-    :keyword Sequence[MetricReader] metric_readers: Specifies the metric readers that you would like to use for your metric pipeline.
-    :keyword Sequence[View] views: Specifies the list of views to configure for the metric pipeline.
-    :keyword float sampling_ratio: Specifies the ratio of distributed tracing telemetry to be sampled. Accepted values are in the range [0,1]. Defaults to 1.0, meaning no telemetry is sampled out.
-    :keyword int tracing_export_interval_ms: Specifies the distributed tracing export interval in milliseconds. Defaults to 5000.
-    :keyword InstrumentationConfig instrumentation_config: Specifies a dictionary of kwargs that will be applied to instrumentation configuration. You can specify which instrumentation you want to
-        configure by name in the key field and value as a dictionary representing `kwargs` for the corresponding instrumentation.
-        Refer to the `Supported Library` section of https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry#officially-supported-instrumentations for the list of suppoprted library names.
-    :keyword bool disable_offline_storage: Boolean value to determine whether to disable storing failed telemetry records for retry. Defaults to `False`.
-    :keyword str storage_directory: Storage directory in which to store retry files. Defaults to `<tempfile.gettempdir()>/Microsoft/AzureMonitor/opentelemetry-python-<your-instrumentation-key>`.
-    :rtype: None
-    """
-
-    configurations = _get_configurations(**kwargs)
-
-    disable_tracing = configurations[DISABLE_TRACING_ARG]
-    disable_logging = configurations[DISABLE_LOGGING_ARG]
-    disable_metrics = configurations[DISABLE_METRICS_ARG]
-
-    resource = None
-    if not disable_logging or not disable_tracing or not disable_metrics:
-        resource = _get_resource(configurations)
-
-    # Setup tracing pipeline
-    if not disable_tracing:
-        _setup_tracing(resource, configurations)
-
-    # Setup logging pipeline
-    if not disable_logging:
-        _setup_logging(resource, configurations)
-
-    # Setup metrics pipeline
-    if not disable_metrics:
-        _setup_metrics(resource, configurations)
-
-    # Setup instrumentations
-    # Instrumentations need to be setup last so to use the global providers
-    # instanstiated in the other setup steps
-    _setup_instrumentations(configurations)
-
-
-def _get_resource(configurations: Dict[str, ConfigurationValue]) -> Resource:
-    return configurations.get(RESOURCE_ARG, Resource.create())
-
-
-def _setup_tracing(
-    resource: Resource, configurations: Dict[str, ConfigurationValue]
-):
-    sampling_ratio = configurations[SAMPLING_RATIO_ARG]
-    tracing_export_interval_ms = configurations[TRACING_EXPORT_INTERVAL_MS_ARG]
-    tracer_provider = TracerProvider(
-        sampler=ApplicationInsightsSampler(sampling_ratio=sampling_ratio),
-        resource=resource,
-    )
-    set_tracer_provider(tracer_provider)
-    trace_exporter = AzureMonitorTraceExporter(**configurations)
-    span_processor = BatchSpanProcessor(
-        trace_exporter,
-        schedule_delay_millis=tracing_export_interval_ms,
-    )
-    get_tracer_provider().add_span_processor(span_processor)
-
-
-def _setup_logging(
-    resource: Resource, configurations: Dict[str, ConfigurationValue]
-):
-    logger_name = configurations[LOGGER_NAME_ARG]
-    logging_level = configurations[LOGGING_LEVEL_ARG]
-    logging_export_interval_ms = configurations[LOGGING_EXPORT_INTERVAL_MS_ARG]
-    logger_provider = LoggerProvider(resource=resource)
-    set_logger_provider(logger_provider)
-    log_exporter = AzureMonitorLogExporter(**configurations)
-    log_record_processor = BatchLogRecordProcessor(
-        log_exporter,
-        schedule_delay_millis=logging_export_interval_ms,
-    )
-    get_logger_provider().add_log_record_processor(log_record_processor)
-    handler = LoggingHandler(
-        level=logging_level, logger_provider=get_logger_provider()
-    )
-    getLogger(logger_name).addHandler(handler)
-
-
-def _setup_metrics(
-    resource: Resource, configurations: Dict[str, ConfigurationValue]
-):
-    views = configurations[VIEWS_ARG]
-    metric_readers = configurations[METRIC_READERS_ARG]
-    metric_exporter = AzureMonitorMetricExporter(**configurations)
-    reader = PeriodicExportingMetricReader(metric_exporter)
-    meter_provider = MeterProvider(
-        metric_readers=[reader] + metric_readers,
-        resource=resource,
-        views=views,
-    )
-    set_meter_provider(meter_provider)
-
-
-def _setup_instrumentations(configurations: Dict[str, ConfigurationValue]):
-    exclude_instrumentations = configurations[EXCLUDE_INSTRUMENTATIONS_ARG]
-    instrumentation_configs = configurations[INSTRUMENTATION_CONFIG_ARG]
-
-    # use pkg_resources for now until https://github.com/open-telemetry/opentelemetry-python/pull/3168 is merged
-    for entry_point in iter_entry_points("opentelemetry_instrumentor"):
-        lib_name = entry_point.name
-        if lib_name not in _SUPPORTED_INSTRUMENTED_LIBRARIES:
-            continue
-        if lib_name in exclude_instrumentations:
-            _logger.debug("Instrumentation excluded for library %s", lib_name)
-            continue
-        try:
-            # Check if dependent libraries/version are installed
-            conflict = get_dist_dependency_conflicts(entry_point.dist)
-            if conflict:
-                _logger.debug(
-                    "Skipping instrumentation %s: %s",
-                    entry_point.name,
-                    conflict,
-                )
-                continue
-            # Load the instrumentor via entrypoint
-            instrumentor: BaseInstrumentor = entry_point.load()
-            # Call instrument() with configuration
-            config = instrumentation_configs.get(lib_name, {})
-            # tell instrumentation to not run dep checks again as we already did it above
-            config["skip_dep_check"] = True
-            instrumentor().instrument(**config)
-        except Exception as ex:
-            _logger.warning(
-                "Exception occured when instrumenting: %s.",
-                lib_name,
-                exc_info=ex,
-            )
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+import importlib
+from logging import NOTSET, getLogger
+from typing import Dict
+
+from azure.monitor.opentelemetry._types import ConfigurationValue
+from azure.monitor.opentelemetry.exporter import (
+    ApplicationInsightsSampler,
+    AzureMonitorLogExporter,
+    AzureMonitorMetricExporter,
+    AzureMonitorTraceExporter,
+)
+from azure.monitor.opentelemetry.util import _get_configurations
+from opentelemetry._logs import get_logger_provider, set_logger_provider
+from opentelemetry.metrics import set_meter_provider
+from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
+from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
+from opentelemetry.sdk.metrics import MeterProvider
+from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
+from opentelemetry.sdk.resources import Resource
+from opentelemetry.sdk.trace import TracerProvider
+from opentelemetry.sdk.trace.export import BatchSpanProcessor
+from opentelemetry.trace import get_tracer_provider, set_tracer_provider
+
+_logger = getLogger(__name__)
+
+
+_INSTRUMENTATION_CONFIG_SUFFIX = "_config"
+_SUPPORTED_INSTRUMENTED_LIBRARIES = (
+    "django",
+    "flask",
+    "psycopg2",
+    "requests",
+)
+
+
+def configure_azure_monitor(**kwargs) -> None:
+    """
+    This function works as a configuration layer that allows the
+    end user to configure OpenTelemetry and Azure monitor components. The
+    configuration can be done via arguments passed to this function.
+    :keyword str connection_string: Connection string for your Application Insights resource.
+    :keyword Sequence[str] connection_string: Specifies the libraries with instrumentations to be enabled.
+    :keyword Resource resource: Specified the OpenTelemetry [resource][opentelemetry_spec_resource] associated with your application.
+    :keyword bool disable_logging: If set to `True`, disables collection and export of logging telemetry. Defaults to `False`.
+    :keyword bool disable_metrics: If set to `True`, disables collection and export of metric telemetry. Defaults to `False`.
+    :keyword bool disable_tracing: If set to `True`, disables collection and export of distributed tracing telemetry. Defaults to `False`.
+    :keyword int logging_level: Specifies the logging of the logs you would like to collect for your logging pipeline.
+    :keyword str logger_name: Specifies the logger name under which logging will be instrumented. Defaults to "" which corresponds to the root logger.
+    :keyword int logging_export_interval_millis: Specifies the logging export interval in milliseconds. Defaults to 5000.
+    :keyword Sequence[MetricReader] metric_readers: Specifies the metric readers that you would like to use for your metric pipeline.
+    :keyword Sequence[View] views: Specifies the list of views to configure for the metric pipeline.
+    :keyword float sampling_ratio: Specifies the ratio of distributed tracing telemetry to be sampled. Accepted values are in the range [0,1]. Defaults to 1.0, meaning no telemetry is sampled out.
+    :keyword int tracing_export_interval_millis: Specifies the distributed tracing export interval in milliseconds. Defaults to 5000.
+    :keyword Dict[str, Any] <instrumentation>_config: Specifies a dictionary of kwargs that will be applied to configuration for instrumentation <instrumentation>.
+    :keyword bool disable_offline_storage: Boolean value to determine whether to disable storing failed telemetry records for retry. Defaults to `False`.
+    :keyword str storage_directory: Storage directory in which to store retry files. Defaults to `<tempfile.gettempdir()>/Microsoft/AzureMonitor/opentelemetry-python-<your-instrumentation-key>`.
+    :rtype: None
+    """
+
+    configurations = _get_configurations(**kwargs)
+
+    disable_tracing = configurations.get("disable_tracing", False)
+    disable_logging = configurations.get("disable_logging", False)
+    disable_metrics = configurations.get("disable_metrics", False)
+
+    resource = None
+    if not disable_logging or not disable_tracing or not disable_metrics:
+        resource = _get_resource(configurations)
+
+    # Setup tracing pipeline
+    if not disable_tracing:
+        _setup_tracing(resource, configurations)
+
+    # Setup logging pipeline
+    if not disable_logging:
+        _setup_logging(resource, configurations)
+
+    # Setup metrics pipeline
+    if not disable_metrics:
+        _setup_metrics(resource, configurations)
+
+    # Setup instrumentations
+    # Instrumentations need to be setup last so to use the global providers
+    # instanstiated in the other setup steps
+    _setup_instrumentations(configurations)
+
+
+def _get_resource(configurations: Dict[str, ConfigurationValue]) -> Resource:
+    return configurations.get("resource", Resource.create())
+
+
+def _setup_tracing(
+    resource: Resource, configurations: Dict[str, ConfigurationValue]
+):
+    sampling_ratio = configurations.get("sampling_ratio", 1.0)
+    tracing_export_interval_millis = configurations.get(
+        "tracing_export_interval_millis", 5000
+    )
+    tracer_provider = TracerProvider(
+        sampler=ApplicationInsightsSampler(sampling_ratio=sampling_ratio),
+        resource=resource,
+    )
+    set_tracer_provider(tracer_provider)
+    trace_exporter = AzureMonitorTraceExporter(**configurations)
+    span_processor = BatchSpanProcessor(
+        trace_exporter,
+        schedule_delay_millis=tracing_export_interval_millis,
+    )
+    get_tracer_provider().add_span_processor(span_processor)
+
+
+def _setup_logging(
+    resource: Resource, configurations: Dict[str, ConfigurationValue]
+):
+    logger_name = configurations.get("logger_name", "")
+    logging_level = configurations.get("logging_level", NOTSET)
+    logging_export_interval_millis = configurations.get(
+        "logging_export_interval_millis", 5000
+    )
+    logger_provider = LoggerProvider(resource=resource)
+    set_logger_provider(logger_provider)
+    log_exporter = AzureMonitorLogExporter(**configurations)
+    log_record_processor = BatchLogRecordProcessor(
+        log_exporter,
+        schedule_delay_millis=logging_export_interval_millis,
+    )
+    get_logger_provider().add_log_record_processor(log_record_processor)
+    handler = LoggingHandler(
+        level=logging_level, logger_provider=get_logger_provider()
+    )
+    getLogger(logger_name).addHandler(handler)
+
+
+def _setup_metrics(
+    resource: Resource, configurations: Dict[str, ConfigurationValue]
+):
+    views = configurations.get("views", ())
+    metric_readers = configurations.get("metric_readers", [])
+    metric_exporter = AzureMonitorMetricExporter(**configurations)
+    reader = PeriodicExportingMetricReader(metric_exporter)
+    meter_provider = MeterProvider(
+        metric_readers=[reader] + metric_readers,
+        resource=resource,
+        views=views,
+    )
+    set_meter_provider(meter_provider)
+
+
+def _setup_instrumentations(configurations: Dict[str, ConfigurationValue]):
+    instrumentations = configurations.get("instrumentations", [])
+    instrumentation_configs = {}
+
+    # Instrumentation specific configs
+    # Format is {"<library_name>": {"<config>":<value>}}
+    for k, v in configurations.items():
+        if k.endswith(_INSTRUMENTATION_CONFIG_SUFFIX):
+            lib_name = k.partition(_INSTRUMENTATION_CONFIG_SUFFIX)[0]
+            instrumentation_configs[lib_name] = v
+
+    for lib_name in instrumentations:
+        if lib_name in _SUPPORTED_INSTRUMENTED_LIBRARIES:
+            try:
+                importlib.import_module(lib_name)
+            except ImportError:
+                _logger.warning(
+                    "Unable to import %s. Please make sure it is installed.",
+                    lib_name,
+                )
+                continue
+            instr_lib_name = "opentelemetry.instrumentation." + lib_name
+            try:
+                module = importlib.import_module(instr_lib_name)
+                instrumentor_name = "{}Instrumentor".format(
+                    lib_name.capitalize()
+                )
+                class_ = getattr(module, instrumentor_name)
+                config = instrumentation_configs.get(lib_name, {})
+                class_().instrument(**config)
+            except ImportError:
+                _logger.warning(
+                    "Unable to import %s. Please make sure it is installed.",
+                    instr_lib_name,
+                )
+            except Exception as ex:
+                _logger.warning(
+                    "Exception occured when instrumenting: %s.",
+                    lib_name,
+                    exc_info=ex,
+                )
+        else:
+            _logger.warning(
+                "Instrumentation not supported for library: %s.", lib_name
+            )
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/_types.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_types.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from typing import Sequence, Union
-
-from opentelemetry.sdk.metrics.export import MetricReader
-from opentelemetry.sdk.metrics.view import View
-from opentelemetry.sdk.resources import Resource
-
-ConfigurationValue = Union[
-    str,
-    bool,
-    int,
-    float,
-    Resource,
-    Sequence[str],
-    Sequence[bool],
-    Sequence[int],
-    Sequence[float],
-    Sequence[MetricReader],
-    Sequence[View],
-]
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from typing import Sequence, Union
+
+from opentelemetry.sdk.metrics.export import MetricReader
+from opentelemetry.sdk.metrics.view import View
+from opentelemetry.sdk.resources import Resource
+
+ConfigurationValue = Union[
+    str,
+    bool,
+    int,
+    float,
+    Resource,
+    Sequence[str],
+    Sequence[bool],
+    Sequence[int],
+    Sequence[float],
+    Sequence[MetricReader],
+    Sequence[View],
+]
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-
-import logging
-
-from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
-    AzureDiagnosticLogging,
-)
-from opentelemetry.sdk._configuration import _OTelSDKConfigurator
-
-_logger = logging.getLogger(__name__)
-
-
-class AzureMonitorConfigurator(_OTelSDKConfigurator):
-    def _configure(self, **kwargs):
-        try:
-            AzureDiagnosticLogging.enable(_logger)
-            super()._configure(**kwargs)
-        except ValueError as e:
-            _logger.error(
-                f"Azure Monitor Configurator failed during configuration due to a ValueError: {e}"
-            )
-            raise e
-        except Exception as e:
-            _logger.error(
-                f"Azure Monitor Configurator failed during configuration: {e}"
-            )
-            raise e
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+
+import logging
+
+from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
+    AzureDiagnosticLogging,
+)
+from opentelemetry.sdk._configuration import _OTelSDKConfigurator
+
+_logger = logging.getLogger(__name__)
+
+
+class AzureMonitorConfigurator(_OTelSDKConfigurator):
+    def _configure(self, **kwargs):
+        try:
+            AzureDiagnosticLogging.enable(_logger)
+            super()._configure(**kwargs)
+        except ValueError as e:
+            _logger.error(
+                f"Azure Monitor Configurator failed during configuration due to a ValueError: {e}"
+            )
+            raise e
+        except Exception as e:
+            _logger.error(
+                f"Azure Monitor Configurator failed during configuration: {e}"
+            )
+            raise e
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/autoinstrumentation/_distro.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_distro.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-import logging
-from os import environ
-
-from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
-    AzureDiagnosticLogging,
-)
-from azure.monitor.opentelemetry.diagnostics._status_logger import (
-    AzureStatusLogger,
-)
-from opentelemetry.environment_variables import (
-    OTEL_LOGS_EXPORTER,
-    OTEL_METRICS_EXPORTER,
-    OTEL_TRACES_EXPORTER,
-)
-from opentelemetry.instrumentation.distro import BaseDistro
-from opentelemetry.sdk.environment_variables import (
-    _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
-)
-
-_logger = logging.getLogger(__name__)
-_opentelemetry_logger = logging.getLogger("opentelemetry")
-# TODO: Enabled when duplicate logging issue is solved
-# _exporter_logger = logging.getLogger("azure.monitor.opentelemetry.exporter")
-
-
-class AzureMonitorDistro(BaseDistro):
-    def _configure(self, **kwargs) -> None:
-        try:
-            _configure_auto_instrumentation()
-        except Exception as ex:
-            _logger.exception(
-                ("Error occured auto-instrumenting AzureMonitorDistro")
-            )
-            raise ex
-
-
-def _configure_auto_instrumentation() -> None:
-    try:
-        AzureStatusLogger.log_status(False, "Distro being configured.")
-        AzureDiagnosticLogging.enable(_logger)
-        AzureDiagnosticLogging.enable(_opentelemetry_logger)
-        # TODO: Enabled when duplicate logging issue is solved
-        # if _EXPORTER_DIAGNOSTICS_ENABLED:
-        #     exporter_logger = logging.getLogger(
-        #         "azure.monitor.opentelemetry.exporter"
-        #     )
-        #     AzureDiagnosticLogging.enable(_exporter_logger)
-        environ.setdefault(
-            OTEL_METRICS_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            OTEL_TRACES_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            OTEL_LOGS_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED, "true"
-        )
-        AzureStatusLogger.log_status(True)
-        _logger.info(
-            "Azure Monitor OpenTelemetry Distro configured successfully."
-        )
-    except Exception as exc:
-        AzureStatusLogger.log_status(False, reason=exc)
-        _logger.error(
-            "Azure Monitor OpenTelemetry Distro failed during "
-            + f"configuration: {exc}"
-        )
-        raise exc
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+import logging
+from os import environ
+
+from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
+    AzureDiagnosticLogging,
+)
+from azure.monitor.opentelemetry.diagnostics._status_logger import (
+    AzureStatusLogger,
+)
+from opentelemetry.environment_variables import (
+    OTEL_LOGS_EXPORTER,
+    OTEL_METRICS_EXPORTER,
+    OTEL_TRACES_EXPORTER,
+)
+from opentelemetry.instrumentation.distro import BaseDistro
+from opentelemetry.sdk.environment_variables import (
+    _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
+)
+
+_logger = logging.getLogger(__name__)
+_opentelemetry_logger = logging.getLogger("opentelemetry")
+# TODO: Enabled when duplicate logging issue is solved
+# _exporter_logger = logging.getLogger("azure.monitor.opentelemetry.exporter")
+
+
+class AzureMonitorDistro(BaseDistro):
+    def _configure(self, **kwargs) -> None:
+        try:
+            _configure_auto_instrumentation()
+        except Exception as ex:
+            _logger.exception(
+                ("Error occured auto-instrumenting AzureMonitorDistro")
+            )
+            raise ex
+
+
+def _configure_auto_instrumentation() -> None:
+    try:
+        AzureStatusLogger.log_status(False, "Distro being configured.")
+        AzureDiagnosticLogging.enable(_logger)
+        AzureDiagnosticLogging.enable(_opentelemetry_logger)
+        # TODO: Enabled when duplicate logging issue is solved
+        # if _EXPORTER_DIAGNOSTICS_ENABLED:
+        #     exporter_logger = logging.getLogger(
+        #         "azure.monitor.opentelemetry.exporter"
+        #     )
+        #     AzureDiagnosticLogging.enable(_exporter_logger)
+        # TODO: Uncomment when logging is out of preview
+        # environ.setdefault(OTEL_LOGS_EXPORTER,
+        #     "azure_monitor_opentelemetry_exporter")
+        environ.setdefault(
+            OTEL_METRICS_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            OTEL_TRACES_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            OTEL_LOGS_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED, "true"
+        )
+        AzureStatusLogger.log_status(True)
+        _logger.info(
+            "Azure Monitor OpenTelemetry Distro configured successfully."
+        )
+    except Exception as exc:
+        AzureStatusLogger.log_status(False, reason=exc)
+        _logger.error(
+            "Azure Monitor OpenTelemetry Distro failed during "
+            + f"configuration: {exc}"
+        )
+        raise exc
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/azure/monitor/opentelemetry/diagnostics/_status_logger.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_status_logger.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from json import dumps
-from os import getpid, makedirs
-from os.path import exists, join
-from platform import node
-
-from azure.monitor.opentelemetry._constants import (
-    _CUSTOMER_IKEY,
-    _EXTENSION_VERSION,
-    _IS_DIAGNOSTICS_ENABLED,
-    _get_log_path,
-)
-from azure.monitor.opentelemetry._version import VERSION
-
-_MACHINE_NAME = node()
-_STATUS_LOG_PATH = _get_log_path(status_log_path=True)
-
-
-class AzureStatusLogger:
-    def _get_status_json(agent_initialized_successfully, pid, reason=None):
-        status_json = {
-            "AgentInitializedSuccessfully": agent_initialized_successfully,
-            "AppType": "python",
-            "MachineName": _MACHINE_NAME,
-            "PID": pid,
-            "SdkVersion": VERSION,
-            "Ikey": _CUSTOMER_IKEY,
-            "ExtensionVersion": _EXTENSION_VERSION,
-        }
-        if reason:
-            status_json["Reason"] = reason
-        return status_json
-
-    def log_status(agent_initialized_successfully, reason=None):
-        if _IS_DIAGNOSTICS_ENABLED and _STATUS_LOG_PATH:
-            pid = getpid()
-            status_json = AzureStatusLogger._get_status_json(
-                agent_initialized_successfully, pid, reason
-            )
-            if not exists(_STATUS_LOG_PATH):
-                makedirs(_STATUS_LOG_PATH)
-            # Change to be hostname and pid
-            status_logger_file_name = f"status_{_MACHINE_NAME}_{pid}.json"
-            with open(
-                join(_STATUS_LOG_PATH, status_logger_file_name), "w"
-            ) as f:
-                f.seek(0)
-                f.write(dumps(status_json))
-                f.truncate()
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from json import dumps
+from os import getpid, makedirs
+from os.path import exists, join
+from platform import node
+
+from azure.monitor.opentelemetry._constants import (
+    _CUSTOMER_IKEY,
+    _EXTENSION_VERSION,
+    _IS_DIAGNOSTICS_ENABLED,
+    _get_log_path,
+)
+from azure.monitor.opentelemetry._version import VERSION
+
+_MACHINE_NAME = node()
+_STATUS_LOG_PATH = _get_log_path(status_log_path=True)
+
+
+class AzureStatusLogger:
+    def _get_status_json(agent_initialized_successfully, pid, reason=None):
+        status_json = {
+            "AgentInitializedSuccessfully": agent_initialized_successfully,
+            "AppType": "python",
+            "MachineName": _MACHINE_NAME,
+            "PID": pid,
+            "SdkVersion": VERSION,
+            "Ikey": _CUSTOMER_IKEY,
+            "ExtensionVersion": _EXTENSION_VERSION,
+        }
+        if reason:
+            status_json["Reason"] = reason
+        return status_json
+
+    def log_status(agent_initialized_successfully, reason=None):
+        if _IS_DIAGNOSTICS_ENABLED and _STATUS_LOG_PATH:
+            pid = getpid()
+            status_json = AzureStatusLogger._get_status_json(
+                agent_initialized_successfully, pid, reason
+            )
+            if not exists(_STATUS_LOG_PATH):
+                makedirs(_STATUS_LOG_PATH)
+            # Change to be hostname and pid
+            status_logger_file_name = f"status_{_MACHINE_NAME}_{pid}.json"
+            with open(
+                join(_STATUS_LOG_PATH, status_logger_file_name), "w"
+            ) as f:
+                f.seek(0)
+                f.write(dumps(status_json))
+                f.truncate()
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/azure_monitor_opentelemetry.egg-info/PKG-INFO` & `azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,181 +1,142 @@
-Metadata-Version: 2.1
-Name: azure-monitor-opentelemetry
-Version: 1.0.0b11
-Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
-Home-page: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry
-Author: Microsoft Corporation
-Author-email: ascl@microsoft.com
-License: MIT License
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Azure Monitor Opentelemetry Distro
-
-The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] provides multiple installable components available for an Opentelemetry Azure Monitor monitoring solution. It allows you to instrument your Python applications to capture and report telemetry to Azure Monitor via the Azure monitor exporters.
-
-This distro automatically installs the following libraries:
-
-* [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters]
-* A subset of OpenTelemetry [instrumentations][ot_instrumentations] that are officially supported as listed below.
-
-## Officially supported instrumentations
-
-OpenTelemetry instrumentations allow automatic collection of requests sent from underlying instrumented libraries. The following is a list of OpenTelemetry instrumentations that come bundled in with the Azure monitor distro. If you would like to add support for another OpenTelemetry instrumentation, please submit a feature [request][distro_feature_request]. In the meantime, you can use the OpenTelemetry instrumentation manually via it's own APIs (i.e. `instrument()`) in your code. See [this][samples_manual] for an example.
-
-| Instrumentation | Supported library | Supported versions |
-| ------------------------------------- | ----------------- | ------------------ |
-| [OpenTelemetry Django Instrumentation][ot_instrumentation_django] | [django][pypi_django] | [link][ot_instrumentation_django_version]
-| [OpenTelemetry FastApi Instrumentation][ot_instrumentation_fastapi] | [fastapi][pypi_fastapi] | [link][ot_instrumentation_fastapi_version]
-| [OpenTelemetry Flask Instrumentation][ot_instrumentation_flask] | [flask][pypi_flask] | [link][ot_instrumentation_flask_version]
-| [OpenTelemetry Psycopg2 Instrumentation][ot_instrumentation_psycopg2] | [psycopg2][pypi_psycopg2] | [link][ot_instrumentation_psycopg2_version]
-| [OpenTelemetry Requests Instrumentation][ot_instrumentation_requests] | [requests][pypi_requests] | [link][ot_instrumentation_requests_version]
-| [OpenTelemetry UrlLib Instrumentation][ot_instrumentation_urllib] | [urllib][pypi_urllib] | All
-| [OpenTelemetry UrlLib3 Instrumentation][ot_instrumentation_urllib3] | [urllib3][pypi_urllib3] | [link][ot_instrumentation_urllib3_version]
-
-## Getting started
-
-### Key Concepts
-
-This package bundles a series of OpenTelemetry and Azure Monitor components to enable the collection and sending of telemetry to Azure Monitor. For MANUAL instrumentation, use the `configure_azure_monitor` function. AUTOMATIC instrumentation is not yet supported.
-
-The [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters] are the main components in accomplishing this. You will be able to use the exporters and their APIs directly through this package. Please go the exporter documentation to understand how OpenTelemetry and Azure Monitor components work in enabling telemetry collection and exporting.
-
-Currently, all instrumentations available in OpenTelemetry are in a beta state, meaning they are not stable and may have breaking changes in the future. Efforts are being made in pushing these to a more stable state.
-
-### Prerequisites
-
-To use this package, you must have:
-
-* Azure subscription - [Create a free account][azure_sub]
-* Azure Monitor - [How to use application insights][application_insights_namespace]
-* Opentelemetry SDK - [Opentelemetry SDK for Python][ot_sdk_python]
-* Python 3.7 or later - [Install Python][python]
-
-### Install the package
-
-Install the Azure Monitor Opentelemetry Distro with [pip][pip]:
-
-```Bash
-pip install azure-monitor-opentelemetry --pre
-```
-
-### Usage
-
-You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments:
-
-| Parameter | Description | Environment Variable |
-|-------------------|----------------------------------------------------|----------------------|
-| `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
-| `exclude_instrumentations` | By default, all supported [instrumentations](#officially-supported-instrumentations) are enabled to collect telemetry. Specify instrumentations you do not want to enable to collect telemetry by passing in a comma separated list of instrumented library names. e.g. `["requests", "flask"]` | |
-| `resource` | Specifies the OpenTelemetry [resource][opentelemetry_spec_resource] associated with your application. See [this][ot_sdk_python_resource] for default behavior. | [OTEL_SERVICE_NAME][opentelemetry_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][opentelemetry_spec_resource_attributes] |
-| `disable_logging` | If set to `True`, disables collection and export of logging telemetry. Defaults to `False`. | |
-| `disable_metrics` | If set to `True`, disables collection and export of metric telemetry. Defaults to `False`. | |
-| `disable_tracing` | If set to `True`, disables collection and export of distributed tracing telemetry. Defaults to `False`. | |
-| `logging_level` | Specifies the [logging level][logging_level] of the logs you would like to collect for your logging pipeline. Defaults to 0 which is `logging.NOTSET`. | |
-| `logger_name` | Specifies the [logger name][logger_name_hierarchy_doc] under which logging will be instrumented. Defaults to "" which corresponds to the root logger. | |
-| `logging_export_interval_ms`| Specifies the logging export interval in milliseconds. Defaults to 5000. | `OTEL_BLRP_SCHEDULE_DELAY` |
-| `metric_readers` | Specifies the [metric readers][ot_metric_reader] that you would like to use for your metric pipeline. Accepts a list of [metric readers][ot_sdk_python_metric_reader]. | |
-| `views` | Specifies the list of [views][opentelemetry_spec_view] to configure for the metric pipeline. See [here][ot_sdk_python_view_examples] for example usage. | |
-| `sampling_ratio` | Specifies the ratio of distributed tracing telemetry to be [sampled][application_insights_sampling]. Accepted values are in the range [0,1]. Defaults to 1.0, meaning no telemetry is sampled out. | `OTEL_TRACES_SAMPLER_ARG` |
-| `tracing_export_interval_ms`| Specifies the distributed tracing export interval in milliseconds. Defaults to 5000. | `OTEL_BSP_SCHEDULE_DELAY` |
-| `instrumentation_config` | Specifies a dictionary of kwargs that will be applied to instrumentation configuration. You can specify which instrumentation you want to configure by name in the key field and value as a dictionary representing `kwargs` for the corresponding instrumentation. Refer to the `Supported Library` section [above](#officially-supported-instrumentations) for the list of supported library names. | |
-
-Example for use of `instrumentation_config`:
-```python
-...
-configure_azure_monitor(
-    connection_string="<your-connection-string>",
-    instrumentation_config={
-        "flask": {
-            "excluded_urls": "http://localhost:8080/ignore",
-        },
-        "requests": {
-            "excluded_urls": "http://example.com"
-        }
-    }
-)
-...
-```
-
-Take a look at the specific [instrumenation][ot_instrumentations] documentation for available configurations.
-
-#### Azure monitor OpenTelemetry Exporter configurations
-
-You can pass Azure monitor OpenTelemetry exporter configuration parameters directly into `configure_azure_monitor`. See additional [configuration related to exporting here][exporter_configuration_docs].
-
-```python
-...
-configure_azure_monitor(
-   connection_string="<your-connection-string>",
-   disable_offline_storage=True, 
-)
-...
-```
-
-### Samples
-
-Samples are available [here][samples] to demonstrate how to utilize the above configuration options.
-
-### Additional documentation
-
-* [Azure Portal][azure_portal]
-* [Official Azure monitor docs][azure_monitor_opentelemetry]
-* [OpenTelemetry Python Official Docs][ot_python_docs]
-
-<!-- LINKS -->
-[azure_monitor_opentelemetry]: https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-enable?tabs=python
-[azure_monitor_opentelemetry_exporters]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#microsoft-opentelemetry-exporter-for-azure-monitor
-[azure_portal]: https://portal.azure.com
-[azure_sub]: https://azure.microsoft.com/free/
-[application_insights_namespace]: https://learn.microsoft.com/azure/azure-monitor/app/app-insights-overview
-[application_insights_sampling]: https://learn.microsoft.com/azure/azure-monitor/app/sampling
-[connection_string_doc]: https://learn.microsoft.com/azure/azure-monitor/app/sdk-connection-string
-[distro_feature_request]: https://github.com/microsoft/ApplicationInsights-Python/issues/new
-[exporter_configuration_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#configuration
-[logging_level]: https://docs.python.org/3/library/logging.html#levels
-[logger_name_hierarchy_doc]: https://docs.python.org/3/library/logging.html#logger-objects
-[ot_instrumentations]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
-[ot_metric_reader]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#metricreader
-[ot_python_docs]: https://opentelemetry.io/docs/instrumentation/python/
-[ot_sdk_python]: https://github.com/open-telemetry/opentelemetry-python
-[ot_sdk_python_metric_reader]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/metrics.export.html#opentelemetry.sdk.metrics.export.MetricReader
-[ot_sdk_python_resource]: https://github.com/open-telemetry/opentelemetry-python/blob/main/opentelemetry-sdk/src/opentelemetry/sdk/resources/__init__.py#L153
-[ot_sdk_python_view_examples]: https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples/metrics/views
-[ot_instrumentation_django]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django
-[ot_instrumentation_django_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-django/src/opentelemetry/instrumentation/django/package.py#L16
-[ot_instrumentation_fastapi]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-fastapi
-[ot_instrumentation_fastapi_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-fastapi/src/opentelemetry/instrumentation/fastapi/package.py#L16
-[ot_instrumentation_flask]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask
-[ot_instrumentation_flask_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-flask/src/opentelemetry/instrumentation/flask/package.py#L16
-[ot_instrumentation_psycopg2]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-psycopg2
-[ot_instrumentation_psycopg2_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-psycopg2/src/opentelemetry/instrumentation/psycopg2/package.py#L16
-[ot_instrumentation_requests]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
-[ot_instrumentation_requests_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-requests/src/opentelemetry/instrumentation/requests/package.py#L16
-[ot_instrumentation_urllib]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3
-[ot_instrumentation_urllib3]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-urllib3
-[ot_instrumentation_urllib3_version]: https://github.com/open-telemetry/opentelemetry-python-contrib/blob/main/instrumentation/opentelemetry-instrumentation-urllib3/src/opentelemetry/instrumentation/urllib3/package.py#L16
-[opentelemetry_spec_resource]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/resource/sdk.md#resource-sdk
-[opentelemetry_spec_resource_attributes]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/resource/sdk.md#specifying-resource-information-via-an-environment-variable
-[opentelemetry_spec_service_name]: https://github.com/open-telemetry/opentelemetry-specification/tree/main/specification/resource/semantic_conventions#semantic-attributes-with-sdk-provided-default-value
-[opentelemetry_spec_view]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#view
-[pip]: https://pypi.org/project/pip/
-[pypi_django]: https://pypi.org/project/Django/
-[pypi_fastapi]: https://pypi.org/project/fastapi/
-[pypi_flask]: https://pypi.org/project/Flask/
-[pypi_psycopg2]: https://pypi.org/project/psycopg2/
-[pypi_requests]: https://pypi.org/project/requests/
-[pypi_urllib]: https://docs.python.org/3/library/urllib.html
-[pypi_urllib3]: https://pypi.org/project/urllib3/
-[python]: https://www.python.org/downloads/
-[samples]: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry/samples
-[samples_manual]: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry/samples/tracing/manual.py
+Metadata-Version: 2.1
+Name: azure-monitor-opentelemetry
+Version: 1.0.0b9
+Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
+Home-page: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry
+Author: Microsoft Corporation
+Author-email: ascl@microsoft.com
+License: MIT License
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# Azure Monitor Opentelemetry Distro
+
+The Azure Monitor Distro of [Opentelemetry Python][ot_sdk_python] provides multiple installable components available for an Opentelemetry Azure Monitor monitoring solution. It allows you to instrument your Python applications to capture and report telemetry to Azure Monitor via the Azure monitor exporters.
+
+This distro automatically installs the following libraries:
+
+* [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters]
+* [OpenTelemetry Requests Instrumentation][opentelemetry_instrumentation_requests]
+* [OpenTelemetry Django Instrumentation][opentelemetry_instrumentation_django]
+* [OpenTelemetry Flask Instrumentation][opentelemetry_instrumentation_flask]
+* [OpenTelemetry Psycopg2 Instrumentation][opentelemetry_instrumentation_psycopg2]
+
+## Getting started
+
+### Key Concepts
+
+This package bundles a series of OpenTelemetry and Azure Monitor components to enable the collection and sending of telemetry to Azure Monitor. For MANUAL instrumentation, use the `configure_azure_monitor` function. AUTOMATIC instrumentation is not yet supported.
+
+The [Azure Monitor OpenTelemetry exporters][azure_monitor_opentelemetry_exporters] are the main components in accomplishing this. You will be able to use the exporters and their APIs directly through this package. Please go the exporter documentation to understand how OpenTelemetry and Azure Monitor components work in enabling telemetry collection and exporting.
+
+Currently, all instrumentations available in OpenTelemetry are in a beta state, meaning they are not stable and may have breaking changes in the future. Efforts are being made in pushing these to a more stable state.
+
+### Prerequisites
+
+To use this package, you must have:
+
+* Azure subscription - [Create a free account][azure_sub]
+* Azure Monitor - [How to use application insights][application_insights_namespace]
+* Opentelemetry SDK - [Opentelemetry SDK for Python][ot_sdk_python]
+* Python 3.7 or later - [Install Python][python]
+
+### Install the package
+
+Install the Azure Monitor Opentelemetry Distro with [pip][pip]:
+
+```Bash
+pip install azure-monitor-opentelemetry --pre
+```
+
+### Usage
+
+You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments:
+
+* connection_string - The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in.
+* instrumentations - Specifies the libraries with [instrumentations][ot_instrumentations] that you would like to use. Accepts a comma separated list. e.g. `["requests", "flask"]`
+* disable_logging - If set to `True`, disables collection and export of logging telemetry. Defaults to `False`.
+* disable_metrics - If set to `True`, disables collection and export of metric telemetry. Defaults to `False`.
+* disable_tracing - If set to `True`, disables collection and export of distributed tracing telemetry. Defaults to `False`.
+* resource - Specified the OpenTelemetry [resource][opentelemetry_spec_resource] associated with your application. See [this][ot_sdk_python_resource] for default behavior.
+* logging_level - Specifies the [logging level][logging_level] of the logs you would like to collect for your logging pipeline. Defaults to logging.NOTSET.
+* logger_name = Specifies the [logger name][logger_name_hierarchy_doc] under which logging will be instrumented. Defaults to "" which corresponds to the root logger.
+* logging_export_interval_millis - Specifies the logging export interval in milliseconds. Defaults to 5000.
+* metric_readers - Specifies the [metric readers][ot_metric_reader] that you would like to use for your metric pipeline. Accepts a list of [metric readers][ot_sdk_python_metric_reader].
+* views - Specifies the list of [views][opentelemetry_spec_view] to configure for the metric pipeline. See [here][ot_sdk_python_view_examples] for example usage.
+* sampling_ratio - Specifies the ratio of distributed tracing telemetry to be [sampled][application_insights_sampling]. Accepted values are in the range [0,1]. Defaults to 1.0, meaning no telemetry is sampled out.
+* tracing_export_interval_millis - Specifies the distributed tracing export interval in milliseconds. Defaults to 5000.
+
+#### Exporter configurations
+
+You can pass exporter configuration parameters directly into `configure_azure_monitor`. See additional [configuration related to exporting here][exporter_configuration_docs].
+
+```python
+...
+configure_azure_monitor(
+   connection_string="<your-connection-string>",
+   disable_offline_storage=True, 
+)
+...
+```
+
+#### Instrumentation configurations
+
+You can pass in instrumentation specific configuration into `configure_azure_monitor` with the key `<instrumented-library-name>_config` and value as a dictionary representing `kwargs` for the corresponding instrumentation. Note the instrumented library must also be enabled through the `instrumentations` configuration.
+
+```python
+...
+configure_azure_monitor(
+    connection_string="<your-connection-string>",
+    instrumentations=["flask", "requests"],
+    flask_config={"excluded_urls": "http://localhost:8080/ignore"},
+    requests_config={"excluded_urls": "http://example.com"},
+)
+...
+```
+
+Take a look at the specific [instrumenation][ot_instrumentations] documentation for available configurations.
+
+### Samples
+
+Samples are available [here][samples] to demonstrate how to utilize the above configuration options.
+
+### Additional documentation
+
+[Azure Portal][azure_portal]
+[OpenTelemetry Python Official Docs][ot_python_docs]
+
+<!-- LINKS -->
+[azure_monitor_opentelemetry_exporters]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#microsoft-opentelemetry-exporter-for-azure-monitor
+[azure_portal]: https://portal.azure.com
+[azure_sub]: https://azure.microsoft.com/free/
+[application_insights_namespace]: https://learn.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview
+[application_insights_sampling]: https://learn.microsoft.com/en-us/azure/azure-monitor/app/sampling
+[connection_string_doc]: https://learn.microsoft.com/en-us/azure/azure-monitor/app/sdk-connection-string
+[exporter_configuration_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#configuration
+[logging_level]: https://docs.python.org/3/library/logging.html#levels
+[logger_name_hierarchy_doc]: https://docs.python.org/3/library/logging.html#logger-objects
+[ot_instrumentations]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
+[ot_metric_reader]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#metricreader
+[ot_python_docs]: https://opentelemetry.io/docs/instrumentation/python/
+[ot_sdk_python]: https://github.com/open-telemetry/opentelemetry-python
+[ot_sdk_python_metric_reader]: https://opentelemetry-python.readthedocs.io/en/stable/sdk/metrics.export.html#opentelemetry.sdk.metrics.export.MetricReader
+[ot_sdk_python_resource]: https://github.com/open-telemetry/opentelemetry-python/blob/main/opentelemetry-sdk/src/opentelemetry/sdk/resources/__init__.py#L153
+[ot_sdk_python_view_examples]: https://github.com/open-telemetry/opentelemetry-python/tree/main/docs/examples/metrics/views
+[opentelemetry_instrumentation_requests]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-requests
+[opentelemetry_instrumentation_django]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-django
+[opentelemetry_instrumentation_flask]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-flask
+[opentelemetry_instrumentation_psycopg2]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation/opentelemetry-instrumentation-psycopg2
+[opentelemetry_spec_resource]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/resource/sdk.md#resource-sdk
+[opentelemetry_spec_view]: https://github.com/open-telemetry/opentelemetry-specification/blob/main/specification/metrics/sdk.md#view
+[python]: https://www.python.org/downloads/
+[pip]: https://pypi.org/project/pip/
+[samples]: https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry/samples
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/setup.py` & `azure-monitor-opentelemetry-1.0.0b9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,104 @@
-#!/usr/bin/env python
-
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-
-import os
-import re
-
-from setuptools import find_packages, setup
-
-# Change the PACKAGE_NAME only to change folder and different name
-PACKAGE_NAME = "azure-monitor-opentelemetry"
-PACKAGE_PPRINT_NAME = "Azure Monitor Opentelemetry Distro"
-
-# a-b-c => a/b/c
-package_folder_path = PACKAGE_NAME.replace("-", "/")
-
-
-# azure v0.x is not compatible with this package
-# azure v0.x used to have a __version__ attribute (newer versions don't)
-try:
-    import azure
-
-    try:
-        ver = azure.__version__
-        raise Exception(
-            "This package is incompatible with azure=={}. ".format(ver)
-            + 'Uninstall it with "pip uninstall azure".'
-        )
-    except AttributeError:
-        pass
-except ImportError:
-    pass
-
-# Version extraction inspired from 'requests'
-with open(os.path.join(package_folder_path, "_version.py"), "r") as fd:
-    version = re.search(
-        r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
-    ).group(1)
-
-if not version:
-    raise RuntimeError("Cannot find version information")
-
-setup(
-    name=PACKAGE_NAME,
-    version=version,
-    description="Microsoft {} Client Library for Python".format(
-        PACKAGE_PPRINT_NAME
-    ),
-    long_description=open("README.md", "r").read(),
-    long_description_content_type="text/markdown",
-    license="MIT License",
-    author="Microsoft Corporation",
-    author_email="ascl@microsoft.com",
-    url="https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-    ],
-    zip_safe=False,
-    packages=find_packages(
-        exclude=[
-            "tests",
-            "samples",
-            # Exclude packages that will be covered by PEP420 or nspkg
-            "azure",
-            "azure.monitor",
-        ]
-    ),
-    include_package_data=True,
-    package_data={
-        "pytyped": ["py.typed"],
-    },
-    python_requires=">=3.7",
-    install_requires=[
-        "azure-monitor-opentelemetry-exporter>=1.0.0b13",
-        "opentelemetry-instrumentation~=0.38b0",
-        "opentelemetry-instrumentation-django~=0.38b0",
-        "opentelemetry-instrumentation-fastapi~=0.38b0",
-        "opentelemetry-instrumentation-flask~=0.38b0",
-        "opentelemetry-instrumentation-psycopg2~=0.38b0",
-        "opentelemetry-instrumentation-requests~=0.38b0",
-        "opentelemetry-instrumentation-urllib~=0.38b0",
-        "opentelemetry-instrumentation-urllib3~=0.38b0",
-        "opentelemetry-api==1.17.0",
-        "opentelemetry-sdk==1.17.0",
-    ],
-    entry_points={
-        "opentelemetry_distro": [
-            "azure_monitor_opentelemetry_distro = azure.monitor.opentelemetry.autoinstrumentation._distro:AzureMonitorDistro"
-        ],
-        "opentelemetry_configurator": [
-            "azure_monitor_opentelemetry_configurator = azure.monitor.opentelemetry.autoinstrumentation._configurator:AzureMonitorConfigurator"
-        ],
-    },
-)
+#!/usr/bin/env python
+
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+
+import os
+import re
+
+from setuptools import find_packages, setup
+
+# Change the PACKAGE_NAME only to change folder and different name
+PACKAGE_NAME = "azure-monitor-opentelemetry"
+PACKAGE_PPRINT_NAME = "Azure Monitor Opentelemetry Distro"
+
+# a-b-c => a/b/c
+package_folder_path = PACKAGE_NAME.replace("-", "/")
+
+
+# azure v0.x is not compatible with this package
+# azure v0.x used to have a __version__ attribute (newer versions don't)
+try:
+    import azure
+
+    try:
+        ver = azure.__version__
+        raise Exception(
+            "This package is incompatible with azure=={}. ".format(ver)
+            + 'Uninstall it with "pip uninstall azure".'
+        )
+    except AttributeError:
+        pass
+except ImportError:
+    pass
+
+# Version extraction inspired from 'requests'
+with open(os.path.join(package_folder_path, "_version.py"), "r") as fd:
+    version = re.search(
+        r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
+    ).group(1)
+
+if not version:
+    raise RuntimeError("Cannot find version information")
+
+setup(
+    name=PACKAGE_NAME,
+    version=version,
+    description="Microsoft {} Client Library for Python".format(
+        PACKAGE_PPRINT_NAME
+    ),
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
+    license="MIT License",
+    author="Microsoft Corporation",
+    author_email="ascl@microsoft.com",
+    url="https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry",
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+    ],
+    zip_safe=False,
+    packages=find_packages(
+        exclude=[
+            "tests",
+            "samples",
+            # Exclude packages that will be covered by PEP420 or nspkg
+            "azure",
+            "azure.monitor",
+        ]
+    ),
+    include_package_data=True,
+    package_data={
+        "pytyped": ["py.typed"],
+    },
+    python_requires=">=3.7",
+    install_requires=[
+        "azure-monitor-opentelemetry-exporter>=1.0.0b12",
+        "opentelemetry-instrumentation~=0.36b0",
+        "opentelemetry-instrumentation-django~=0.36b0",
+        "opentelemetry-instrumentation-requests~=0.36b0",
+        "opentelemetry-instrumentation-flask~=0.36b0",
+        "opentelemetry-instrumentation-psycopg2~=0.36b0",
+        "opentelemetry-api==1.15.0",
+        "opentelemetry-sdk==1.15.0",
+    ],
+    entry_points={
+        "opentelemetry_distro": [
+            "azure_monitor_opentelemetry_distro = azure.monitor.opentelemetry.autoinstrumentation._distro:AzureMonitorDistro"
+        ],
+        "opentelemetry_configurator": [
+            "azure_monitor_opentelemetry_configurator = azure.monitor.opentelemetry.autoinstrumentation._configurator:AzureMonitorConfigurator"
+        ],
+    },
+)
```

### Comparing `azure-monitor-opentelemetry-1.0.0b11/tests/test_constants.py` & `azure-monitor-opentelemetry-1.0.0b9/tests/test_constants.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from importlib import reload
-from os import environ
-from unittest import TestCase
-from unittest.mock import patch
-
-from azure.monitor.opentelemetry import _constants
-
-TEST_VALUE = "TEST_VALUE"
-TEST_IKEY = "1234abcd-ab12-34cd-ab12-a23456abcdef"
-TEST_CONN_STR = f"InstrumentationKey={TEST_IKEY};IngestionEndpoint=https://centralus-2.in.applicationinsights.azure.com/;LiveEndpoint=https://centralus.livediagnostics.monitor.azure.com/"
-
-
-def clear_env_var(env_var):
-    if env_var in environ:
-        del environ[env_var]
-
-
-class TestConstants(TestCase):
-    @patch.dict(
-        "os.environ",
-        {"ApplicationInsightsAgent_EXTENSION_VERSION": TEST_VALUE},
-    )
-    def test_extension_version(self):
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, TEST_VALUE)
-
-    def test_extension_version_default(self):
-        clear_env_var("ApplicationInsightsAgent_EXTENSION_VERSION")
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, "disabled")
-
-    @patch.dict(
-        "os.environ", {"APPLICATIONINSIGHTS_CONNECTION_STRING": TEST_CONN_STR}
-    )
-    def test_ikey(self):
-        reload(_constants)
-        self.assertEqual(_constants._CUSTOMER_IKEY, TEST_IKEY)
-
-    def test_ikey_defaults(self):
-        clear_env_var("APPLICATIONINSIGHTS_CONNECTION_STRING")
-        reload(_constants)
-        self.assertEqual(_constants._CUSTOMER_IKEY, "unknown")
-
-    # TODO: Enabled when duplciate logging issue is solved
-    # @patch.dict(
-    #     "os.environ",
-    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "True"},
-    # )
-    # def test_exporter_diagnostics_enabled(self):
-    #     reload(_constants)
-    #     self.assertTrue(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    # def test_exporter_diagnostics_disabled(self):
-    #     clear_env_var("AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS")
-    #     reload(_constants)
-    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    # @patch.dict(
-    #     "os.environ",
-    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "foobar"},
-    # )
-    # def test_exporter_diagnostics_other(self):
-    #     reload(_constants)
-    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    @patch.dict("os.environ", {"WEBSITE_SITE_NAME": TEST_VALUE})
-    def test_diagnostics_enabled(self):
-        reload(_constants)
-        self.assertTrue(_constants._IS_DIAGNOSTICS_ENABLED)
-
-    def test_diagnostics_disabled(self):
-        clear_env_var("WEBSITE_SITE_NAME")
-        reload(_constants)
-        self.assertFalse(_constants._IS_DIAGNOSTICS_ENABLED)
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Linux",
-    )
-    def test_log_path_linux(self, mock_system):
-        self.assertEqual(
-            _constants._get_log_path(), "/var/log/applicationinsights"
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Linux",
-    )
-    def test_status_log_path_linux(self, mock_system):
-        self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
-            "/var/log/applicationinsights",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Windows",
-    )
-    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
-    def test_log_path_windows(self, mock_system, mock_home):
-        self.assertEqual(
-            _constants._get_log_path(),
-            "\\HOME\\DIR\\LogFiles\\ApplicationInsights",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Windows",
-    )
-    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
-    def test_status_log_path_windows(self, mock_system, mock_home):
-        self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
-            "\\HOME\\DIR\\LogFiles\\ApplicationInsights\\status",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Window",
-    )
-    def test_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path())
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="linux",
-    )
-    def test_status_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path(status_log_path=True))
-
-    @patch.dict("os.environ", {"key": "value"})
-    def test_env_var_or_default(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "value")
-
-    @patch.dict("os.environ", {})
-    def test_env_var_or_default_empty(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "")
-
-    @patch.dict("os.environ", {})
-    def test_env_var_or_default_empty_with_defaults(self):
-        self.assertEqual(
-            _constants._env_var_or_default("key", default_val="value"), "value"
-        )
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from importlib import reload
+from os import environ
+from unittest import TestCase
+from unittest.mock import patch
+
+from azure.monitor.opentelemetry import _constants
+
+TEST_VALUE = "TEST_VALUE"
+TEST_IKEY = "1234abcd-ab12-34cd-ab12-a23456abcdef"
+TEST_CONN_STR = f"InstrumentationKey={TEST_IKEY};IngestionEndpoint=https://centralus-2.in.applicationinsights.azure.com/;LiveEndpoint=https://centralus.livediagnostics.monitor.azure.com/"
+
+
+def clear_env_var(env_var):
+    if env_var in environ:
+        del environ[env_var]
+
+
+class TestConstants(TestCase):
+    @patch.dict(
+        "os.environ",
+        {"ApplicationInsightsAgent_EXTENSION_VERSION": TEST_VALUE},
+    )
+    def test_extension_version(self):
+        reload(_constants)
+        self.assertEqual(_constants._EXTENSION_VERSION, TEST_VALUE)
+
+    def test_extension_version_default(self):
+        clear_env_var("ApplicationInsightsAgent_EXTENSION_VERSION")
+        reload(_constants)
+        self.assertEqual(_constants._EXTENSION_VERSION, "disabled")
+
+    @patch.dict(
+        "os.environ", {"APPLICATIONINSIGHTS_CONNECTION_STRING": TEST_CONN_STR}
+    )
+    def test_ikey(self):
+        reload(_constants)
+        self.assertEqual(_constants._CUSTOMER_IKEY, TEST_IKEY)
+
+    def test_ikey_defaults(self):
+        clear_env_var("APPLICATIONINSIGHTS_CONNECTION_STRING")
+        reload(_constants)
+        self.assertEqual(_constants._CUSTOMER_IKEY, "unknown")
+
+    # TODO: Enabled when duplciate logging issue is solved
+    # @patch.dict(
+    #     "os.environ",
+    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "True"},
+    # )
+    # def test_exporter_diagnostics_enabled(self):
+    #     reload(_constants)
+    #     self.assertTrue(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    # def test_exporter_diagnostics_disabled(self):
+    #     clear_env_var("AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS")
+    #     reload(_constants)
+    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    # @patch.dict(
+    #     "os.environ",
+    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "foobar"},
+    # )
+    # def test_exporter_diagnostics_other(self):
+    #     reload(_constants)
+    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    @patch.dict("os.environ", {"WEBSITE_SITE_NAME": TEST_VALUE})
+    def test_diagnostics_enabled(self):
+        reload(_constants)
+        self.assertTrue(_constants._IS_DIAGNOSTICS_ENABLED)
+
+    def test_diagnostics_disabled(self):
+        clear_env_var("WEBSITE_SITE_NAME")
+        reload(_constants)
+        self.assertFalse(_constants._IS_DIAGNOSTICS_ENABLED)
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Linux",
+    )
+    def test_log_path_linux(self, mock_system):
+        self.assertEqual(
+            _constants._get_log_path(), "/var/log/applicationinsights"
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Linux",
+    )
+    def test_status_log_path_linux(self, mock_system):
+        self.assertEqual(
+            _constants._get_log_path(status_log_path=True),
+            "/var/log/applicationinsights",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Windows",
+    )
+    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
+    def test_log_path_windows(self, mock_system, mock_home):
+        self.assertEqual(
+            _constants._get_log_path(),
+            "\\HOME\\DIR\\LogFiles\\ApplicationInsights",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Windows",
+    )
+    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
+    def test_status_log_path_windows(self, mock_system, mock_home):
+        self.assertEqual(
+            _constants._get_log_path(status_log_path=True),
+            "\\HOME\\DIR\\LogFiles\\ApplicationInsights\\status",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Window",
+    )
+    def test_log_path_other(self, mock_platform):
+        self.assertIsNone(_constants._get_log_path())
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="linux",
+    )
+    def test_status_log_path_other(self, mock_platform):
+        self.assertIsNone(_constants._get_log_path(status_log_path=True))
+
+    @patch.dict("os.environ", {"key": "value"})
+    def test_env_var_or_default(self):
+        self.assertEqual(_constants._env_var_or_default("key"), "value")
+
+    @patch.dict("os.environ", {})
+    def test_env_var_or_default_empty(self):
+        self.assertEqual(_constants._env_var_or_default("key"), "")
+
+    @patch.dict("os.environ", {})
+    def test_env_var_or_default_empty_with_defaults(self):
+        self.assertEqual(
+            _constants._env_var_or_default("key", default_val="value"), "value"
+        )
```

