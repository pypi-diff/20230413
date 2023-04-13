# Comparing `tmp/PyPlumIO-0.3.5.tar.gz` & `tmp/PyPlumIO-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPlumIO-0.3.5.tar", last modified: Fri Feb 17 20:15:50 2023, max compression
+gzip compressed data, was "PyPlumIO-0.4.0.tar", last modified: Thu Apr 13 21:39:08 2023, max compression
```

## Comparing `PyPlumIO-0.3.5.tar` & `PyPlumIO-0.4.0.tar`

### file list

```diff
@@ -1,119 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.489436 PyPlumIO-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24074 2023-02-17 20:15:50.489436 PyPlumIO-0.3.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/PyPlumIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24074 2023-02-17 20:15:50.000000 PyPlumIO-0.3.5/PyPlumIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-02-17 20:15:50.000000 PyPlumIO-0.3.5/PyPlumIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 20:15:50.000000 PyPlumIO-0.3.5/PyPlumIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-17 20:15:50.000000 PyPlumIO-0.3.5/PyPlumIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-17 20:15:50.000000 PyPlumIO-0.3.5/PyPlumIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/images/ecomax.png
--rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/images/rs485.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/pyplumio/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-17 20:15:50.000000 PyPlumIO-0.3.5/pyplumio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/pyplumio/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/devices/ecomax.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/devices/ecoster.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.481436 PyPlumIO-0.3.5/pyplumio/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/frames/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/frames/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/frames/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.485436 PyPlumIO-0.3.5/pyplumio/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/helpers/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.489436 PyPlumIO-0.3.5/pyplumio/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/data_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15728 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/ecomax_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/fan_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/frame_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/fuel_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/lambda_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/mixer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/mixer_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/network_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/output_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/pending_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/product_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/program_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/regulator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/temperatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/thermostat_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/structures/thermostat_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyplumio/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 20:15:50.489436 PyPlumIO-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.489436 PyPlumIO-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17694 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.489436 PyPlumIO-0.3.5/tests/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/frames/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/frames/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/frames/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/frames/test_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 20:15:50.489436 PyPlumIO-0.3.5/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/helpers/test_uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-17 20:15:24.000000 PyPlumIO-0.3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/PyPlumIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/images/ecomax.png
+-rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/images/rs485.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/pyplumio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/pyplumio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/pyplumio/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/ecomax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/ecoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/pyplumio/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.356367 PyPlumIO-0.4.0/pyplumio/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/pyplumio/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/data_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/ecomax_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/fan_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/frame_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/fuel_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/lambda_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/mixer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/mixer_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/network_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/output_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/pending_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/product_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/program_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/regulator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/temperatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/thermostat_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/thermostat_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/tests/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21987 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tox.ini
```

### Comparing `PyPlumIO-0.3.5/.github/CODE_OF_CONDUCT.md` & `PyPlumIO-0.4.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/.github/workflows/ci.yml` & `PyPlumIO-0.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/.github/workflows/codeql-analysis.yml` & `PyPlumIO-0.4.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/.github/workflows/deploy.yml` & `PyPlumIO-0.4.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/.gitignore` & `PyPlumIO-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/.pre-commit-config.yaml` & `PyPlumIO-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/LICENSE` & `PyPlumIO-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/PyPlumIO.egg-info/SOURCES.txt` & `PyPlumIO-0.4.0/PyPlumIO.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,27 @@
 tox.ini
 .github/CODE_OF_CONDUCT.md
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
 .github/workflows/ci.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/deploy.yml
+.github/workflows/documentation.yml
 .vscode/settings.json
 PyPlumIO.egg-info/PKG-INFO
 PyPlumIO.egg-info/SOURCES.txt
 PyPlumIO.egg-info/dependency_links.txt
 PyPlumIO.egg-info/requires.txt
 PyPlumIO.egg-info/top_level.txt
+docs/Makefile
+docs/make.bat
+docs/source/conf.py
+docs/source/index.rst
+docs/source/protocol.rst
+docs/source/usage.rst
 images/ecomax.png
 images/rs485.png
 pyplumio/__init__.py
 pyplumio/__main__.py
 pyplumio/_version.py
 pyplumio/connection.py
 pyplumio/const.py
@@ -31,23 +38,24 @@
 pyplumio/filters.py
 pyplumio/protocol.py
 pyplumio/stream.py
 pyplumio/util.py
 pyplumio/devices/__init__.py
 pyplumio/devices/ecomax.py
 pyplumio/devices/ecoster.py
+pyplumio/devices/mixer.py
+pyplumio/devices/thermostat.py
 pyplumio/frames/__init__.py
 pyplumio/frames/messages.py
 pyplumio/frames/requests.py
 pyplumio/frames/responses.py
 pyplumio/helpers/__init__.py
 pyplumio/helpers/data_types.py
 pyplumio/helpers/event_manager.py
 pyplumio/helpers/factory.py
-pyplumio/helpers/filters.py
 pyplumio/helpers/parameter.py
 pyplumio/helpers/schedule.py
 pyplumio/helpers/task_manager.py
 pyplumio/helpers/timeout.py
 pyplumio/helpers/typing.py
 pyplumio/helpers/uid.py
 pyplumio/structures/__init__.py
@@ -90,13 +98,12 @@
 tests/frames/test_messages.py
 tests/frames/test_requests.py
 tests/frames/test_responses.py
 tests/helpers/__init__.py
 tests/helpers/test_data_types.py
 tests/helpers/test_event_manager.py
 tests/helpers/test_factory.py
-tests/helpers/test_filters.py
 tests/helpers/test_parameter.py
 tests/helpers/test_schedule.py
 tests/helpers/test_task_manager.py
 tests/helpers/test_timeout.py
 tests/helpers/test_uid.py
```

### Comparing `PyPlumIO-0.3.5/images/ecomax.png` & `PyPlumIO-0.4.0/images/ecomax.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/images/rs485.png` & `PyPlumIO-0.4.0/images/rs485.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/__init__.py` & `PyPlumIO-0.4.0/pyplumio/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/connection.py` & `PyPlumIO-0.4.0/pyplumio/connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/const.py` & `PyPlumIO-0.4.0/pyplumio/const.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/devices/__init__.py` & `PyPlumIO-0.4.0/pyplumio/devices/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Contains device representations."""
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import ClassVar
-from warnings import warn
 
 from pyplumio import util
 from pyplumio.const import ATTR_LOADED, DeviceType, FrameType
 from pyplumio.exceptions import ParameterNotFoundError, UnknownDeviceError
 from pyplumio.frames import DataFrameDescription, Frame, Request, get_frame_handler
 from pyplumio.helpers.event_manager import EventManager
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.parameter import SET_RETRIES, Parameter
 from pyplumio.helpers.typing import ParameterValueType
-from pyplumio.structures.network_info import ATTR_NETWORK, NetworkInfo
+from pyplumio.structures.network_info import NetworkInfo
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def _handler_class_path(device_type_name: str) -> str:
     """Return the handler class path for a given device type name."""
     device_type_name = util.to_camelcase(
@@ -49,66 +48,14 @@
     queue: asyncio.Queue
 
     def __init__(self, queue: asyncio.Queue):
         """Initialize the device object."""
         super().__init__()
         self.queue = queue
 
-    async def get_value(self, name: str, timeout: float | None = None):
-        """Return a value."""
-        warn(
-            "get_value() is deprecated and will be removed in v0.4.1. "
-            + "Please use get() or get_nowait().",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        value = await self.get(name, timeout)
-        if isinstance(value, Parameter):
-            return value.value
-
-        return value
-
-    async def get_parameter(self, name: str, timeout: float | None = None):
-        """Return a parameter."""
-        warn(
-            "get_parameter() is deprecated and will be removed in v0.4.1. "
-            + "Please use get() or get_nowait().",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return await self.get(name, timeout)
-
-    async def set_value(
-        self, name: str, value: ParameterValueType, timeout: float | None = None
-    ) -> bool:
-        """Sets a value."""
-        warn(
-            "set_value() is deprecated and will be removed in v0.4.1. "
-            + "Please use set().",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return await self.set(name, value, timeout)
-
-    def set_value_nowait(
-        self, name: str, value: ParameterValueType, timeout: float | None = None
-    ) -> None:
-        """Sets a value without waiting."""
-        warn(
-            "set_value_nowait() is deprecated and will be removed in v0.4.1. "
-            + "Please use set_nowait().",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        self.set_nowait(name, value, timeout)
-
     async def set(
         self,
         name: str,
         value: ParameterValueType,
         timeout: float | None = None,
         retries: int = SET_RETRIES,
     ) -> bool:
@@ -132,30 +79,24 @@
         self.create_task(self.set(name, value, timeout, retries))
 
 
 class Addressable(Device):
     """Represents the addressable device."""
 
     address: ClassVar[int]
-    _network: NetworkInfo
     _frame_types: tuple[DataFrameDescription, ...] = ()
+    _network: NetworkInfo
 
     def __init__(self, queue: asyncio.Queue, network: NetworkInfo):
         """Initialize the addressable object."""
         super().__init__(queue)
         self._network = network
 
     def handle_frame(self, frame: Frame) -> None:
         """Handle received frame."""
-        if isinstance(frame, Request) and frame.frame_type in (
-            FrameType.REQUEST_CHECK_DEVICE,
-            FrameType.REQUEST_PROGRAM_VERSION,
-        ):
-            self.queue.put_nowait(frame.response(data={ATTR_NETWORK: self._network}))
-
         if frame.data is not None:
             for name, value in frame.data.items():
                 self.dispatch_nowait(name, value)
 
     async def async_setup(self) -> bool:
         """Setup addressable device object."""
         try:
@@ -205,15 +146,7 @@
     index: int
 
     def __init__(self, queue: asyncio.Queue, parent: Addressable, index: int = 0):
         """Initialize a new sub-device object."""
         super().__init__(queue)
         self.parent = parent
         self.index = index
-
-
-class Mixer(SubDevice):
-    """Represents the mixer sub-device."""
-
-
-class Thermostat(SubDevice):
-    """Represents the thermostat sub-device."""
```

### Comparing `PyPlumIO-0.3.5/pyplumio/devices/ecomax.py` & `PyPlumIO-0.4.0/pyplumio/devices/ecomax.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Contains ecoMAX device representation."""
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Sequence
+from collections.abc import Generator, Iterable, Sequence
 import logging
 import time
 from typing import ClassVar, Final
 
 from pyplumio.const import (
     ATTR_PASSWORD,
     ATTR_SENSORS,
@@ -14,17 +14,25 @@
     STATE_OFF,
     STATE_ON,
     DeviceState,
     DeviceType,
     FrameType,
     ProductType,
 )
-from pyplumio.devices import Addressable, Mixer, Thermostat
+from pyplumio.devices import Addressable
+from pyplumio.devices.mixer import Mixer
+from pyplumio.devices.thermostat import Thermostat
 from pyplumio.filters import on_change
-from pyplumio.frames import DataFrameDescription, get_frame_handler, is_known_frame_type
+from pyplumio.frames import (
+    DataFrameDescription,
+    Frame,
+    Request,
+    get_frame_handler,
+    is_known_frame_type,
+)
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.schedule import Schedule, ScheduleDay
 from pyplumio.helpers.typing import EventDataType, ParameterDataType
 from pyplumio.structures import StructureDecoder
 from pyplumio.structures.alerts import ATTR_ALERTS
 from pyplumio.structures.data_schema import ATTR_SCHEMA
 from pyplumio.structures.ecomax_parameters import (
@@ -34,34 +42,29 @@
     ECOMAX_I_PARAMETERS,
     ECOMAX_P_PARAMETERS,
     THERMOSTAT_PROFILE_PARAMETER,
     EcomaxParameter,
 )
 from pyplumio.structures.frame_versions import ATTR_FRAME_VERSIONS
 from pyplumio.structures.fuel_consumption import ATTR_FUEL_CONSUMPTION
-from pyplumio.structures.mixer_parameters import (
-    ATTR_MIXER_PARAMETERS,
-    ECOMAX_I_MIXER_PARAMETERS,
-    ECOMAX_P_MIXER_PARAMETERS,
-)
+from pyplumio.structures.mixer_parameters import ATTR_MIXER_PARAMETERS
 from pyplumio.structures.mixer_sensors import ATTR_MIXER_SENSORS
-from pyplumio.structures.network_info import NetworkInfo
+from pyplumio.structures.network_info import ATTR_NETWORK, NetworkInfo
 from pyplumio.structures.product_info import ATTR_PRODUCT
 from pyplumio.structures.regulator_data import ATTR_REGDATA, ATTR_REGDATA_DECODER
 from pyplumio.structures.schedules import (
     ATTR_SCHEDULE_PARAMETERS,
     ATTR_SCHEDULES,
     SCHEDULE_PARAMETERS,
     SCHEDULES,
 )
 from pyplumio.structures.thermostat_parameters import (
     ATTR_THERMOSTAT_PARAMETERS,
     ATTR_THERMOSTAT_PARAMETERS_DECODER,
     ATTR_THERMOSTAT_PROFILE,
-    THERMOSTAT_PARAMETERS,
 )
 from pyplumio.structures.thermostat_sensors import ATTR_THERMOSTAT_SENSORS
 
 ATTR_MIXERS: Final = "mixers"
 ATTR_THERMOSTATS: Final = "thermostats"
 ATTR_FUEL_BURNED: Final = "fuel_burned"
 
@@ -89,15 +92,15 @@
     DataFrameDescription(frame_type=FrameType.REQUEST_PASSWORD, provides=ATTR_PASSWORD),
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class EcoMAX(Addressable):
-    """Represents ecoMAX controller."""
+    """Represents the ecoMAX controller."""
 
     address: ClassVar[int] = DeviceType.ECOMAX
     _frame_versions: dict[int, int]
     _frame_types: tuple[DataFrameDescription, ...] = DATA_FRAME_TYPES
     _fuel_burned_timestamp_ns: int = 0
 
     def __init__(self, queue: asyncio.Queue, network: NetworkInfo):
@@ -123,66 +126,75 @@
         )
 
     async def async_setup(self) -> bool:
         """Setup addressable device object."""
         await self.wait_for(ATTR_SENSORS)
         return await super().async_setup()
 
+    def handle_frame(self, frame: Frame) -> None:
+        """Handle received frame."""
+        if isinstance(frame, Request) and frame.frame_type in (
+            FrameType.REQUEST_CHECK_DEVICE,
+            FrameType.REQUEST_PROGRAM_VERSION,
+        ):
+            self.queue.put_nowait(frame.response(data={ATTR_NETWORK: self._network}))
+
+        super().handle_frame(frame)
+
     async def _update_frame_versions(self, versions: dict[int, int]) -> None:
         """Check versions and fetch outdated frames."""
         for frame_type, version in versions.items():
             if is_known_frame_type(frame_type) and (
                 frame_type not in self._frame_versions
                 or self._frame_versions[frame_type] != version
             ):
                 # We don't have this frame or it's version has changed.
                 request = factory(get_frame_handler(frame_type), recipient=self.address)
                 self.queue.put_nowait(request)
                 self._frame_versions[frame_type] = version
 
-    def _get_mixer(self, index: int, mixer_count: int) -> Mixer:
-        """Get or create a new mixer object and add it to the device."""
-        mixers: dict[int, Mixer] = self.data.setdefault(ATTR_MIXERS, {})
-        try:
-            mixer = mixers[index]
-        except KeyError:
-            mixer = Mixer(self.queue, parent=self, index=index)
-            mixers[index] = mixer
-            if len(mixers) == mixer_count:
-                # All mixers were processed, notify callbacks and getters.
-                self.dispatch_nowait(ATTR_MIXERS, mixers)
-
-        return mixer
-
-    def _get_thermostat(self, index: int, thermostat_count: int) -> Thermostat:
-        """Get or create a new thermostat object and add it to the
-        device."""
-        thermostats: dict[int, Thermostat] = self.data.setdefault(ATTR_THERMOSTATS, {})
-        try:
-            thermostat = thermostats[index]
-        except KeyError:
-            thermostat = Thermostat(self.queue, parent=self, index=index)
-            thermostats[index] = thermostat
-            if len(thermostats) == thermostat_count:
-                # All thermostats were processed, notify callbacks and getters.
-                self.dispatch_nowait(ATTR_THERMOSTATS, thermostats)
+    def _mixers(self, indexes: Iterable[int]) -> Generator[Mixer, None, None]:
+        """Iterates through the mixer indexes. For each index,
+        returns or creates instance of Mixer class.
+        Once done, dispatches the event.
+        """
+        mixers = self.data.setdefault(ATTR_MIXERS, {})
+        for index in indexes:
+            if index not in mixers:
+                mixers[index] = Mixer(self.queue, parent=self, index=index)
+
+            yield mixers[index]
+
+        return self.dispatch_nowait(ATTR_MIXERS, mixers)
+
+    def _thermostats(self, indexes: Iterable[int]) -> Generator[Thermostat, None, None]:
+        """Iterates through the thermostat indexes. For each index,
+        returns or creates instance of Thermostat class.
+        Once done, dispatches the event.
+        """
+        thermostats = self.data.setdefault(ATTR_THERMOSTATS, {})
+        for index in indexes:
+            if index not in thermostats:
+                thermostats[index] = Thermostat(self.queue, parent=self, index=index)
+
+            yield thermostats[index]
 
-        return thermostat
+        return self.dispatch_nowait(ATTR_THERMOSTATS, thermostats)
 
     async def _add_ecomax_sensors(self, sensors: EventDataType) -> bool:
-        """Add ecomax sensor values to the device data."""
+        """Add ecomax sensors."""
         for name, value in sensors.items():
             await self.dispatch(name, value)
 
         return True
 
     async def _add_ecomax_parameters(
         self, parameters: Sequence[tuple[int, ParameterDataType]]
     ) -> bool:
-        """Add ecomax parameters to the device data."""
+        """Add ecomax parameters."""
         product = await self.get(ATTR_PRODUCT)
         for index, value in parameters:
             description = (
                 ECOMAX_P_PARAMETERS[index]
                 if product.type == ProductType.ECOMAX_P
                 else ECOMAX_I_PARAMETERS[index]
             )
@@ -194,89 +206,55 @@
                 min_value=value[1],
                 max_value=value[2],
             )
             await self.dispatch(description.name, parameter)
 
         return True
 
-    async def _add_mixer_sensors(
-        self, sensors: Sequence[tuple[int, EventDataType]]
-    ) -> bool:
-        """set sensor values for the mixer."""
-        for mixer_index, mixer_sensors in sensors:
-            mixer = self._get_mixer(mixer_index, len(sensors))
-            for name, value in mixer_sensors.items():
-                await mixer.dispatch(name, value)
+    async def _add_mixer_sensors(self, sensors: dict[int, EventDataType]) -> bool:
+        """Pass mixer sensors to mixer instances."""
+        for mixer in self._mixers(sensors.keys()):
+            await mixer.dispatch(ATTR_MIXER_SENSORS, sensors[mixer.index])
 
         return True
 
     async def _add_mixer_parameters(
         self,
-        parameters: Sequence[tuple[int, Sequence[tuple[int, ParameterDataType]]]]
-        | None,
+        parameters: dict[int, Sequence[tuple[int, ParameterDataType]]] | None,
     ) -> bool:
-        """set mixer parameters."""
+        """Pass mixer parameters to mixer instances."""
         if parameters is None:
             return False
 
-        product = await self.get(ATTR_PRODUCT)
-        for mixer_index, mixer_parameters in parameters:
-            mixer = self._get_mixer(mixer_index, len(parameters))
-            for index, value in mixer_parameters:
-                description = (
-                    ECOMAX_P_MIXER_PARAMETERS[index]
-                    if product.type == ProductType.ECOMAX_P
-                    else ECOMAX_I_MIXER_PARAMETERS[index]
-                )
-                parameter = description.cls(
-                    device=mixer,
-                    description=description,
-                    index=index,
-                    value=value[0],
-                    min_value=value[1],
-                    max_value=value[2],
-                )
-                await mixer.dispatch(description.name, parameter)
+        for mixer in self._mixers(parameters.keys()):
+            await mixer.dispatch(ATTR_MIXER_PARAMETERS, parameters[mixer.index])
 
         return True
 
-    async def _add_thermostat_sensors(
-        self, sensors: Sequence[tuple[int, EventDataType]]
-    ) -> bool:
-        """set sensor values for the thermostat."""
-        for thermostat_index, thermostat_sensors in sensors:
-            thermostat = self._get_thermostat(thermostat_index, len(sensors))
-            for name, value in thermostat_sensors.items():
-                await thermostat.dispatch(name, value)
+    async def _add_thermostat_sensors(self, sensors: dict[int, EventDataType]) -> bool:
+        """Pass sensors to thermostat instances."""
+        for thermostat in self._thermostats(sensors.keys()):
+            await thermostat.dispatch(
+                ATTR_THERMOSTAT_SENSORS, sensors[thermostat.index]
+            )
 
         return True
 
     async def _add_thermostat_parameters(
         self,
-        parameters: Sequence[tuple[int, Sequence[tuple[int, ParameterDataType]]]]
-        | None,
+        parameters: dict[int, Sequence[tuple[int, ParameterDataType]]] | None,
     ) -> bool:
         """set thermostat parameters."""
         if parameters is None:
             return False
 
-        for thermostat_index, thermostat_parameters in parameters:
-            thermostat = self._get_thermostat(thermostat_index, len(parameters))
-            for index, value in thermostat_parameters:
-                description = THERMOSTAT_PARAMETERS[index]
-                parameter = description.cls(
-                    device=thermostat,
-                    description=description,
-                    index=index,
-                    value=value[0],
-                    min_value=value[1],
-                    max_value=value[2],
-                    offset=(thermostat_index * len(thermostat_parameters)),
-                )
-                await thermostat.dispatch(description.name, parameter)
+        for thermostat in self._thermostats(parameters.keys()):
+            await thermostat.dispatch(
+                ATTR_THERMOSTAT_PARAMETERS, parameters[thermostat.index]
+            )
 
         return True
 
     async def _add_thermostat_profile_parameter(
         self, parameter: ParameterDataType
     ) -> EcomaxParameter | None:
         """Add thermostat profile parameter to the device instance."""
@@ -335,14 +313,15 @@
                 continue
 
         return True
 
     async def _add_schedule_parameters(
         self, parameters: Sequence[tuple[int, ParameterDataType]]
     ) -> bool:
+        """Add schedule parameter."""
         for index, value in parameters:
             description = SCHEDULE_PARAMETERS[index]
             parameter = description.cls(
                 device=self,
                 description=description,
                 index=index,
                 value=value[0],
```

### Comparing `PyPlumIO-0.3.5/pyplumio/exceptions.py` & `PyPlumIO-0.4.0/pyplumio/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/filters.py` & `PyPlumIO-0.4.0/pyplumio/filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/frames/__init__.py` & `PyPlumIO-0.4.0/pyplumio/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/frames/messages.py` & `PyPlumIO-0.4.0/pyplumio/frames/messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/frames/requests.py` & `PyPlumIO-0.4.0/pyplumio/frames/requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/frames/responses.py` & `PyPlumIO-0.4.0/pyplumio/frames/responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/data_types.py` & `PyPlumIO-0.4.0/pyplumio/helpers/data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/event_manager.py` & `PyPlumIO-0.4.0/pyplumio/helpers/event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/factory.py` & `PyPlumIO-0.4.0/pyplumio/helpers/factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/parameter.py` & `PyPlumIO-0.4.0/pyplumio/helpers/parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/schedule.py` & `PyPlumIO-0.4.0/pyplumio/helpers/schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/task_manager.py` & `PyPlumIO-0.4.0/pyplumio/helpers/task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/timeout.py` & `PyPlumIO-0.4.0/pyplumio/helpers/timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/helpers/uid.py` & `PyPlumIO-0.4.0/pyplumio/helpers/uid.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/protocol.py` & `PyPlumIO-0.4.0/pyplumio/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Contains protocol representation."""
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Awaitable, Callable
 import logging
 from typing import Final
-from warnings import warn
 
 from pyplumio.const import ATTR_CONNECTED, DeviceType
 from pyplumio.devices import Addressable, get_device_handler
 from pyplumio.exceptions import (
     FrameError,
     ReadError,
     UnknownDeviceError,
@@ -163,22 +162,11 @@
             device.dispatch_nowait(ATTR_CONNECTED, True)
             self.create_task(device.async_setup())
             self.data[name] = device
             self.set_event(name)
 
         return self.data[name]
 
-    async def get_device(self, name: str, timeout: float | None = None):
-        """Return a device."""
-        warn(
-            "get_device() is deprecated and will be removed in v0.4.1. "
-            + "Please use get() or get_nowait().",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return await self.get(name, timeout)
-
     @property
     def queues(self) -> tuple[asyncio.Queue, asyncio.Queue]:
         """Return protocol queues."""
         return self._queues
```

### Comparing `PyPlumIO-0.3.5/pyplumio/stream.py` & `PyPlumIO-0.4.0/pyplumio/stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/__init__.py` & `PyPlumIO-0.4.0/pyplumio/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/alerts.py` & `PyPlumIO-0.4.0/pyplumio/structures/alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/data_schema.py` & `PyPlumIO-0.4.0/pyplumio/structures/data_schema.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/ecomax_parameters.py` & `PyPlumIO-0.4.0/pyplumio/structures/ecomax_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,31 +24,32 @@
     device: Addressable
     description: EcomaxParameterDescription
 
     async def set(self, value: ParameterValueType, retries: int = 5) -> bool:
         """set parameter value."""
         if isinstance(value, (int, float)):
             value *= self.description.multiplier
+            value -= self.description.offset
 
         return await super().set(value, retries)
 
     @property
     def value(self) -> ParameterValueType:
         """Return parameter value."""
-        return self._value / self.description.multiplier
+        return (self._value + self.description.offset) / self.description.multiplier
 
     @property
     def min_value(self) -> ParameterValueType:
         """Return minimum allowed value."""
-        return self._min_value / self.description.multiplier
+        return (self._min_value + self.description.offset) / self.description.multiplier
 
     @property
     def max_value(self) -> ParameterValueType:
         """Return maximum allowed value."""
-        return self._max_value / self.description.multiplier
+        return (self._max_value + self.description.offset) / self.description.multiplier
 
     @property
     def request(self) -> Request:
         """Return request to change the parameter."""
 
         if self.description.name == ATTR_ECOMAX_CONTROL:
             return factory(
@@ -83,18 +84,19 @@
 
 class EcomaxBinaryParameter(BinaryParameter, EcomaxParameter):
     """Represents ecoMAX binary parameter."""
 
 
 @dataclass
 class EcomaxParameterDescription(ParameterDescription):
-    """Represent thermostat parameter description."""
+    """Represent ecoMAX parameter description."""
 
     cls: type[EcomaxParameter] = EcomaxParameter
     multiplier: int = 1
+    offset: int = 0
 
 
 ECOMAX_P_PARAMETERS: tuple[EcomaxParameterDescription, ...] = (
     EcomaxParameterDescription(name="airflow_power_100"),
     EcomaxParameterDescription(name="airflow_power_50"),
     EcomaxParameterDescription(name="airflow_power_30"),
     EcomaxParameterDescription(name="power_100"),
@@ -200,15 +202,15 @@
     EcomaxParameterDescription(name="pause_term"),
     EcomaxParameterDescription(name="work_term"),
     EcomaxParameterDescription(name="increase_heating_temp_for_water_heater"),
     EcomaxParameterDescription(
         name="heating_weather_control", cls=EcomaxBinaryParameter
     ),
     EcomaxParameterDescription(name="heating_heat_curve", multiplier=10),
-    EcomaxParameterDescription(name="heating_heat_curve_shift", multiplier=10),
+    EcomaxParameterDescription(name="heating_heat_curve_shift", offset=-20),
     EcomaxParameterDescription(name="weather_factor"),
     EcomaxParameterDescription(name="term_boiler_operation"),
     EcomaxParameterDescription(name="term_boiler_mode", cls=EcomaxBinaryParameter),
     EcomaxParameterDescription(name="decrease_set_heating_term"),
     EcomaxParameterDescription(name="term_pump_off"),
     EcomaxParameterDescription(name="boiler_alert_temp"),
     EcomaxParameterDescription(name="max_feeder_temp"),
```

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/fan_power.py` & `PyPlumIO-0.4.0/pyplumio/structures/fan_power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/frame_versions.py` & `PyPlumIO-0.4.0/pyplumio/structures/frame_versions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/fuel_consumption.py` & `PyPlumIO-0.4.0/pyplumio/structures/fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/fuel_level.py` & `PyPlumIO-0.4.0/pyplumio/structures/fuel_level.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/lambda_sensor.py` & `PyPlumIO-0.4.0/pyplumio/structures/lambda_sensor.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/load.py` & `PyPlumIO-0.4.0/pyplumio/structures/load.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/mixer_parameters.py` & `PyPlumIO-0.4.0/pyplumio/structures/mixer_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Contains mixer parameter structure decoder."""
 from __future__ import annotations
 
 from collections.abc import Iterable
 from dataclasses import dataclass
-from typing import Final
+from typing import TYPE_CHECKING, Final
 
 from pyplumio import util
 from pyplumio.const import ATTR_DEVICE_INDEX, ATTR_INDEX, ATTR_VALUE
-from pyplumio.devices import Mixer
 from pyplumio.frames import Request
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.parameter import BinaryParameter, Parameter, ParameterDescription
 from pyplumio.helpers.typing import EventDataType, ParameterDataType, ParameterValueType
 from pyplumio.structures import StructureDecoder, ensure_device_data
 
+if TYPE_CHECKING:
+    from pyplumio.devices.mixer import Mixer
+
 ATTR_MIXER_PARAMETERS: Final = "mixer_parameters"
 
 
 class MixerParameter(Parameter):
     """Represents mixer parameter."""
 
     device: Mixer
@@ -138,23 +140,23 @@
     ) -> tuple[EventDataType, int]:
         """Decode bytes and return message data and offset."""
         first_index = message[offset + 1]
         last_index = message[offset + 2]
         mixer_count = message[offset + 3]
         parameter_count_per_mixer = first_index + last_index
         offset += 4
-        mixer_parameters: list[tuple[int, list[tuple[int, ParameterDataType]]]] = []
+        mixer_parameters: dict[int, list[tuple[int, ParameterDataType]]] = {}
         for index in range(mixer_count):
             parameters, offset = _decode_mixer_parameters(
                 message,
                 offset,
                 range(first_index, parameter_count_per_mixer),
             )
             if parameters:
-                mixer_parameters.append((index, parameters))
+                mixer_parameters[index] = parameters
 
         if not mixer_parameters:
             # No mixer parameters detected.
             return ensure_device_data(data, {ATTR_MIXER_PARAMETERS: None}), offset
 
         return (
             ensure_device_data(data, {ATTR_MIXER_PARAMETERS: mixer_parameters}),
```

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/mixer_sensors.py` & `PyPlumIO-0.4.0/pyplumio/structures/mixer_sensors.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
     def decode(
         self, message: bytearray, offset: int = 0, data: EventDataType | None = None
     ) -> tuple[EventDataType, int]:
         """Decode bytes and return message data and offset."""
         mixer_count = message[offset]
         offset += 1
-        mixer_sensors: list[tuple[int, EventDataType]] = []
+        mixer_sensors: dict[int, EventDataType] = {}
         for index in range(mixer_count):
             current_temp = util.unpack_float(message[offset : offset + 4])[0]
             if not math.isnan(current_temp):
                 sensors: EventDataType = {}
                 sensors[ATTR_CURRENT_TEMP] = current_temp
                 sensors[ATTR_TARGET_TEMP] = message[offset + 4]
                 outputs = message[offset + 6]
                 sensors[ATTR_PUMP] = bool(outputs & 0x01)
-                mixer_sensors.append((index, sensors))
+                mixer_sensors[index] = sensors
 
             offset += 8
 
         if not mixer_sensors:
             # No mixer sensors detected.
             return ensure_device_data(data), offset
```

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/modules.py` & `PyPlumIO-0.4.0/pyplumio/structures/modules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/network_info.py` & `PyPlumIO-0.4.0/pyplumio/structures/network_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/output_flags.py` & `PyPlumIO-0.4.0/pyplumio/structures/output_flags.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/outputs.py` & `PyPlumIO-0.4.0/pyplumio/structures/outputs.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/pending_alerts.py` & `PyPlumIO-0.4.0/pyplumio/structures/pending_alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/power.py` & `PyPlumIO-0.4.0/pyplumio/structures/power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/product_info.py` & `PyPlumIO-0.4.0/pyplumio/structures/product_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/program_version.py` & `PyPlumIO-0.4.0/pyplumio/structures/program_version.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/regulator_data.py` & `PyPlumIO-0.4.0/pyplumio/structures/regulator_data.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/schedules.py` & `PyPlumIO-0.4.0/pyplumio/structures/schedules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/statuses.py` & `PyPlumIO-0.4.0/pyplumio/structures/statuses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/temperatures.py` & `PyPlumIO-0.4.0/pyplumio/structures/temperatures.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/thermostat_parameters.py` & `PyPlumIO-0.4.0/pyplumio/structures/thermostat_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """Contains thermostat parameter structure decoder."""
 from __future__ import annotations
 
 from collections.abc import Iterable
 from dataclasses import dataclass
-from typing import Final
+from typing import TYPE_CHECKING, Final
 
 from pyplumio import util
 from pyplumio.const import ATTR_INDEX, ATTR_OFFSET, ATTR_SIZE, ATTR_VALUE
-from pyplumio.devices import Thermostat
 from pyplumio.frames import Request
 from pyplumio.helpers.factory import factory
 from pyplumio.helpers.parameter import BinaryParameter, Parameter, ParameterDescription
 from pyplumio.helpers.typing import EventDataType, ParameterDataType, ParameterValueType
 from pyplumio.structures import StructureDecoder, ensure_device_data
 from pyplumio.structures.thermostat_sensors import ATTR_THERMOSTAT_COUNT
 
 ATTR_THERMOSTAT_PROFILE: Final = "thermostat_profile"
 ATTR_THERMOSTAT_PARAMETERS: Final = "thermostat_parameters"
 ATTR_THERMOSTAT_PARAMETERS_DECODER: Final = "thermostat_parameters_decoder"
 
+if TYPE_CHECKING:
+    from pyplumio.devices.thermostat import Thermostat
+
 
 class ThermostatParameter(Parameter):
     """Represents thermostat parameter."""
 
     device: Thermostat
     description: ThermostatParameterDescription
     offset: int
@@ -140,25 +142,23 @@
             )
 
         first_index = message[offset + 1]
         last_index = message[offset + 2]
         thermostat_profile = util.unpack_parameter(message, offset + 3)
         parameter_count_per_thermostat = (first_index + last_index) // thermostat_count
         offset += 6
-        thermostat_parameters: list[
-            tuple[int, list[tuple[int, ParameterDataType]]]
-        ] = []
+        thermostat_parameters: dict[int, list[tuple[int, ParameterDataType]]] = {}
         for index in range(thermostat_count):
             parameters, offset = _decode_thermostat_parameters(
                 message,
                 offset,
                 range(first_index, parameter_count_per_thermostat),
             )
             if parameters:
-                thermostat_parameters.append((index, parameters))
+                thermostat_parameters[index] = parameters
 
         if not thermostat_parameters:
             # No thermostat parameters detected.
             return (
                 ensure_device_data(
                     data,
                     {ATTR_THERMOSTAT_PARAMETERS: None, ATTR_THERMOSTAT_PROFILE: None},
```

### Comparing `PyPlumIO-0.3.5/pyplumio/structures/thermostat_sensors.py` & `PyPlumIO-0.4.0/pyplumio/structures/thermostat_sensors.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,26 +31,26 @@
             return ensure_device_data(data), offset + 1
 
         contacts = message[offset]
         thermostat_count = message[offset + 1]
         offset += 2
         contact_mask = 1
         schedule_mask = 1 << 3
-        thermostat_sensors: list[tuple[int, EventDataType]] = []
+        thermostat_sensors: dict[int, EventDataType] = {}
         for index in range(thermostat_count):
             current_temp = util.unpack_float(message[offset + 1 : offset + 5])[0]
             target_temp = util.unpack_float(message[offset + 5 : offset + 9])[0]
             if not math.isnan(current_temp) and target_temp > 0:
                 sensors: EventDataType = {}
                 sensors[ATTR_STATE] = message[offset]
                 sensors[ATTR_CURRENT_TEMP] = current_temp
                 sensors[ATTR_TARGET_TEMP] = target_temp
                 sensors[ATTR_CONTACTS] = bool(contacts & contact_mask)
                 sensors[ATTR_SCHEDULE] = bool(contacts & schedule_mask)
-                thermostat_sensors.append((index, sensors))
+                thermostat_sensors[index] = sensors
 
             contact_mask = contact_mask << 1
             schedule_mask = schedule_mask << 1
             offset += 9
 
         return (
             ensure_device_data(
```

### Comparing `PyPlumIO-0.3.5/pyplumio/util.py` & `PyPlumIO-0.4.0/pyplumio/util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/pyproject.toml` & `PyPlumIO-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ]
 dependencies = [
     "pyserial-asyncio==0.6",
 ]
 dynamic = ["version"]
 
 [project.urls]
+"Documentation" = "https://pypulmio.denpa.pro"
 "Source Code" = "https://github.com/denpamusic/PyPlumIO"
 "Bug Tracker" = "https://github.com/denpamusic/PyPlumIO/issues"
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
@@ -46,15 +47,15 @@
 
 [tool.isort]
 profile = "black"
 force_sort_within_sections = true
 combine_as_imports = true
 
 [tool.flake8]
-exclude = ".git,.tox,.mypy_cache,build"
+exclude = ".git,.tox,.mypy_cache,build,docs"
 max-complexity = 25
 ignore = [
     "E501",
     "W503",
     "E203",
     "D202",
     "W504",
@@ -92,20 +93,21 @@
     "duplicate-code",
 ]
 
 [tool.pylint.REPORTS]
 score = false
 
 [tool.codespell]
-skip = ".git,.tox,.mypy_cache,build"
+skip = ".git,.tox,.mypy_cache,build,docs"
 
 [tool.mypy]
 ignore_missing_imports = true
 no_strict_optional = true
 exclude = [
+    "docs",
     "build",
     ".tox",
     ".git",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
```

### Comparing `PyPlumIO-0.3.5/tests/conftest.py` & `PyPlumIO-0.4.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,50 +183,44 @@
                 (125, (0, 0, 2)),
                 (126, (16, 5, 30)),
                 (127, (10, 1, 15)),
                 (128, (3, 0, 99)),
             ]
         },
         FrameType.RESPONSE_MIXER_PARAMETERS: {
-            ATTR_MIXER_PARAMETERS: [
-                (
-                    0,
-                    [
-                        (0, (40, 30, 60)),
-                        (1, (20, 30, 40)),
-                        (2, (80, 70, 90)),
-                        (3, (20, 10, 30)),
-                        (4, (1, 0, 1)),
-                        (5, (13, 10, 30)),
-                    ],
-                )
-            ]
+            ATTR_MIXER_PARAMETERS: {
+                0: [
+                    (0, (40, 30, 60)),
+                    (1, (20, 30, 40)),
+                    (2, (80, 70, 90)),
+                    (3, (20, 10, 30)),
+                    (4, (1, 0, 1)),
+                    (5, (13, 10, 30)),
+                ],
+            }
         },
         FrameType.RESPONSE_THERMOSTAT_PARAMETERS: {
             ATTR_THERMOSTAT_COUNT: 3,
             ATTR_THERMOSTAT_PROFILE: (0, 0, 5),
-            ATTR_THERMOSTAT_PARAMETERS: [
-                (
-                    0,
-                    [
-                        (0, (0, 0, 7)),
-                        (1, (220, 100, 350)),
-                        (2, (150, 100, 350)),
-                        (3, (100, 60, 140)),
-                        (4, (2, 0, 60)),
-                        (5, (1, 0, 60)),
-                        (6, (1, 0, 60)),
-                        (7, (10, 0, 60)),
-                        (8, (9, 0, 50)),
-                        (9, (222, 100, 350)),
-                        (10, (212, 100, 350)),
-                        (11, (90, 50, 300)),
-                    ],
-                )
-            ],
+            ATTR_THERMOSTAT_PARAMETERS: {
+                0: [
+                    (0, (0, 0, 7)),
+                    (1, (220, 100, 350)),
+                    (2, (150, 100, 350)),
+                    (3, (100, 60, 140)),
+                    (4, (2, 0, 60)),
+                    (5, (1, 0, 60)),
+                    (6, (1, 0, 60)),
+                    (7, (10, 0, 60)),
+                    (8, (9, 0, 50)),
+                    (9, (222, 100, 350)),
+                    (10, (212, 100, 350)),
+                    (11, (90, 50, 300)),
+                ]
+            },
         },
         FrameType.RESPONSE_ALERTS: {
             ATTR_ALERTS: [
                 Alert(
                     code=26,
                     from_dt=datetime(2022, 7, 23, 16, 27),
                     to_dt=datetime(2022, 7, 23, 16, 32, 27),
```

### Comparing `PyPlumIO-0.3.5/tests/frames/test_init.py` & `PyPlumIO-0.4.0/tests/frames/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/frames/test_messages.py` & `PyPlumIO-0.4.0/tests/frames/test_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,36 +91,30 @@
     assert not data[ATTR_HEATING_PUMP]
     assert data[ATTR_HEATING_STATUS] == 0
     assert data[ATTR_MODULES].module_a == "18.11.58.K1"
     assert data[ATTR_MODULES].panel == "18.10.72"
     assert data[ATTR_LAMBDA_LEVEL] == 4.0
     assert data[ATTR_PENDING_ALERTS] == 0
     assert data[ATTR_FUEL_LEVEL] == 32
-    assert data[ATTR_MIXER_SENSORS] == [
-        (
-            4,
-            {
-                ATTR_CURRENT_TEMP: 20.0,
-                ATTR_TARGET_TEMP: 40,
-                ATTR_PUMP: False,
-            },
-        )
-    ]
-    assert data[ATTR_THERMOSTAT_SENSORS] == [
-        (
-            0,
-            {
-                ATTR_STATE: 3,
-                ATTR_CURRENT_TEMP: 43.5,
-                ATTR_TARGET_TEMP: 50.0,
-                ATTR_CONTACTS: True,
-                ATTR_SCHEDULE: False,
-            },
-        )
-    ]
+    assert data[ATTR_MIXER_SENSORS] == {
+        4: {
+            ATTR_CURRENT_TEMP: 20.0,
+            ATTR_TARGET_TEMP: 40,
+            ATTR_PUMP: False,
+        },
+    }
+    assert data[ATTR_THERMOSTAT_SENSORS] == {
+        0: {
+            ATTR_STATE: 3,
+            ATTR_CURRENT_TEMP: 43.5,
+            ATTR_TARGET_TEMP: 50.0,
+            ATTR_CONTACTS: True,
+            ATTR_SCHEDULE: False,
+        },
+    }
 
     # Test with the unknown state.
     test_message[INDEX_STATE] = 12
     frame = SensorDataMessage(message=test_message)
     assert frame.data[ATTR_SENSORS][ATTR_STATE] == 12
```

### Comparing `PyPlumIO-0.3.5/tests/frames/test_requests.py` & `PyPlumIO-0.4.0/tests/frames/test_requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/frames/test_responses.py` & `PyPlumIO-0.4.0/tests/frames/test_responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/helpers/test_data_types.py` & `PyPlumIO-0.4.0/tests/helpers/test_data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/helpers/test_event_manager.py` & `PyPlumIO-0.4.0/tests/helpers/test_event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/helpers/test_factory.py` & `PyPlumIO-0.4.0/tests/helpers/test_factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/helpers/test_parameter.py` & `PyPlumIO-0.4.0/tests/helpers/test_parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/helpers/test_schedule.py` & `PyPlumIO-0.4.0/tests/helpers/test_schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/helpers/test_task_manager.py` & `PyPlumIO-0.4.0/tests/helpers/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/helpers/test_timeout.py` & `PyPlumIO-0.4.0/tests/helpers/test_timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/test_connection.py` & `PyPlumIO-0.4.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/test_devices.py` & `PyPlumIO-0.4.0/tests/test_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Contains tests for devices."""
 
 import asyncio
 from unittest.mock import AsyncMock, Mock, call, patch
-import warnings
 
 import pytest
 
 from pyplumio.const import (
     ATTR_DEVICE_INDEX,
     ATTR_INDEX,
     ATTR_LOADED,
@@ -18,23 +17,25 @@
     ATTR_TYPE,
     ATTR_VALUE,
     STATE_OFF,
     STATE_ON,
     DeviceType,
     FrameType,
 )
-from pyplumio.devices import Mixer, Thermostat, get_device_handler
+from pyplumio.devices import get_device_handler
 from pyplumio.devices.ecomax import (
     ATTR_FUEL_BURNED,
     ATTR_MIXERS,
     ATTR_THERMOSTATS,
     DATA_FRAME_TYPES,
     EcoMAX,
 )
 from pyplumio.devices.ecoster import EcoSTER
+from pyplumio.devices.mixer import Mixer
+from pyplumio.devices.thermostat import Thermostat
 from pyplumio.exceptions import ParameterNotFoundError, UnknownDeviceError
 from pyplumio.frames import Response
 from pyplumio.frames.messages import RegulatorDataMessage, SensorDataMessage
 from pyplumio.frames.requests import (
     AlertsRequest,
     DataSchemaRequest,
     EcomaxControlRequest,
@@ -48,15 +49,14 @@
 from pyplumio.frames.responses import (
     DataSchemaResponse,
     EcomaxParametersResponse,
     MixerParametersResponse,
     SchedulesResponse,
     ThermostatParametersResponse,
 )
-from pyplumio.helpers.parameter import Parameter
 from pyplumio.helpers.schedule import Schedule
 from pyplumio.helpers.typing import EventDataType
 from pyplumio.structures.ecomax_parameters import (
     ATTR_ECOMAX_CONTROL,
     EcomaxBinaryParameter,
 )
 from pyplumio.structures.frame_versions import ATTR_FRAME_VERSIONS
@@ -101,70 +101,14 @@
 
 
 def test_ecoster(ecoster: EcoSTER) -> None:
     """Test ecoster instance."""
     assert isinstance(ecoster, EcoSTER)
 
 
-async def test_deprecated_get_value(ecomax: EcoMAX) -> None:
-    """Test deprecated get_value method."""
-    mock_parameter = Mock(spec=Parameter)
-    with patch(
-        "pyplumio.devices.Device.get",
-        new_callable=AsyncMock,
-        side_effect=(None, mock_parameter),
-    ) as mock_get, warnings.catch_warnings(record=True) as warn:
-        warnings.simplefilter("always")
-        assert await ecomax.get_value("test") is None
-        assert await ecomax.get_value("test") == mock_parameter.value
-        assert len(warn) == 2
-        assert issubclass(warn[-1].category, DeprecationWarning)
-        assert "deprecated" in str(warn[-1].message)
-        mock_get.assert_any_await("test", None)
-
-
-async def test_deprecated_get_parameter(ecomax: EcoMAX) -> None:
-    """Test deprecated get_parameter method."""
-    with patch(
-        "pyplumio.devices.Device.get", new_callable=AsyncMock
-    ) as mock_get, warnings.catch_warnings(record=True) as warn:
-        warnings.simplefilter("always")
-        await ecomax.get_parameter("test")
-        assert len(warn) == 1
-        assert issubclass(warn[-1].category, DeprecationWarning)
-        assert "deprecated" in str(warn[-1].message)
-        mock_get.assert_awaited_once_with("test", None)
-
-
-async def test_deprecated_set_value(ecomax: EcoMAX) -> None:
-    """Test deprecated set_value method."""
-    with patch(
-        "pyplumio.devices.Device.set", new_callable=AsyncMock
-    ) as mock_set, warnings.catch_warnings(record=True) as warn:
-        warnings.simplefilter("always")
-        await ecomax.set_value("test", 1)
-        assert len(warn) == 1
-        assert issubclass(warn[-1].category, DeprecationWarning)
-        assert "deprecated" in str(warn[-1].message)
-        mock_set.assert_awaited_once_with("test", 1, None)
-
-
-def test_deprecated_set_value_nowait(ecomax: EcoMAX) -> None:
-    """Test deprecated set_value_nowait method."""
-    with patch(
-        "pyplumio.devices.Device.set_nowait"
-    ) as mock_set_nowait, warnings.catch_warnings(record=True) as warn:
-        warnings.simplefilter("always")
-        ecomax.set_value_nowait("test", 1)
-        assert len(warn) == 1
-        assert issubclass(warn[-1].category, DeprecationWarning)
-        assert "deprecated" in str(warn[-1].message)
-        mock_set_nowait.assert_called_once_with("test", 1, None)
-
-
 async def test_async_setup() -> None:
     """Test requesting initial data frames."""
     ecomax = EcoMAX(asyncio.Queue(), network=NetworkInfo())
 
     with patch("pyplumio.devices.ecomax.EcoMAX.wait_for"), patch(
         "pyplumio.devices.ecomax.EcoMAX.request",
         side_effect=(True, True, True, True, True, True, True, True),
@@ -245,18 +189,41 @@
     fuzzy_logic_value = await ecomax.get("fuzzy_logic")
     assert fuzzy_logic_value == STATE_ON
     assert fuzzy_logic.request.data == {
         ATTR_INDEX: 18,
         ATTR_VALUE: 1,
     }
 
-    airflow_power_50 = await ecomax.get("airflow_power_50")
-    assert airflow_power_50.value == 60.0
-    assert airflow_power_50.min_value == 41.0
-    assert airflow_power_50.max_value == 60.0
+    # Test parameter with the multiplier (heating_heat_curve)
+    heating_heat_curve = await ecomax.get("heating_heat_curve")
+    assert heating_heat_curve.value == 1.3
+    assert heating_heat_curve.min_value == 0.1
+    assert heating_heat_curve.max_value == 4.0
+
+    # Test setting parameter with the multiplier.
+    with patch(
+        "pyplumio.structures.ecomax_parameters.Parameter.set", new_callable=AsyncMock
+    ) as mock_set:
+        await heating_heat_curve.set(2.5)
+
+    mock_set.assert_awaited_once_with(25, 5)
+
+    # Test parameter with the offset (heating_heat_curve_shift)
+    heating_heat_curve_shift = await ecomax.get("heating_heat_curve_shift")
+    assert heating_heat_curve_shift.value == 0.0
+    assert heating_heat_curve_shift.min_value == -20.0
+    assert heating_heat_curve_shift.max_value == 20.0
+
+    # Test setting the parameter with the offset.
+    with patch(
+        "pyplumio.structures.ecomax_parameters.Parameter.set", new_callable=AsyncMock
+    ) as mock_set:
+        await heating_heat_curve_shift.set(1)
+
+    mock_set.assert_awaited_once_with(21, 5)
 
 
 @patch(
     "time.perf_counter_ns",
     side_effect=(0, 10 * 1000000000, 600 * 1000000000, 610 * 1000000000),
 )
 async def test_fuel_consumption_callbacks(mock_time, caplog) -> None:
@@ -312,15 +279,20 @@
     )
     await ecomax.wait_until_done()
     mixers = await ecomax.get(ATTR_MIXERS)
     assert len(mixers) == 1
     mixer = mixers[4]
     assert isinstance(mixer, Mixer)
     assert mixer.index == 4
-    assert mixer.data == {"current_temp": 20.0, "target_temp": 40, "pump": False}
+    assert mixer.data == {
+        "current_temp": 20.0,
+        "target_temp": 40,
+        "pump": False,
+        "mixer_sensors": True,
+    }
 
 
 async def test_thermostat_sensors_callbacks(
     ecomax: EcoMAX, messages: dict[FrameType, bytearray]
 ) -> None:
     """Test callbacks that are dispatchd on receiving thermostat sensors info."""
     ecomax.handle_frame(
@@ -334,14 +306,15 @@
     assert thermostat.index == 0
     assert thermostat.data == {
         "state": 3,
         "current_temp": 43.5,
         "target_temp": 50.0,
         "contacts": True,
         "schedule": False,
+        "thermostat_sensors": True,
     }
     thermostat_count = await ecomax.get(ATTR_THERMOSTAT_COUNT)
     assert thermostat_count == 1
 
 
 async def test_thermostat_parameters_callbacks(
     ecomax: EcoMAX, messages: dict[FrameType, bytearray]
@@ -353,15 +326,15 @@
             message=messages[FrameType.RESPONSE_THERMOSTAT_PARAMETERS]
         )
     )
     await ecomax.wait_until_done()
     thermostats = await ecomax.get(ATTR_THERMOSTATS)
     assert len(thermostats) == 1
     thermostat = thermostats[0]
-    assert len(thermostat.data) == 12
+    assert len(thermostat.data) == 13
     party_target_temp = await thermostat.get("party_target_temp")
     assert isinstance(party_target_temp, ThermostatParameter)
     assert isinstance(party_target_temp.request, SetThermostatParameterRequest)
     assert isinstance(party_target_temp.device, Thermostat)
     assert party_target_temp.value == 22.0
     assert party_target_temp.min_value == 10.0
     assert party_target_temp.max_value == 35.0
@@ -427,15 +400,15 @@
     ecomax.handle_frame(
         MixerParametersResponse(message=messages[FrameType.RESPONSE_MIXER_PARAMETERS])
     )
     await ecomax.wait_until_done()
     mixers = await ecomax.get(ATTR_MIXERS)
     assert len(mixers) == 1
     mixer = mixers[0]
-    assert len(mixer.data) == 6
+    assert len(mixer.data) == 7
     mixer_target_temp = await mixer.get("mixer_target_temp")
     assert isinstance(mixer_target_temp, MixerParameter)
     assert isinstance(mixer_target_temp.request, SetMixerParameterRequest)
     assert isinstance(mixer_target_temp.device, Mixer)
     assert mixer_target_temp.value == 40.0
     assert mixer_target_temp.min_value == 30.0
     assert mixer_target_temp.max_value == 60.0
@@ -614,16 +587,16 @@
 async def test_shutdown(ecomax: EcoMAX, messages: dict[FrameType, bytearray]) -> None:
     """Test device tasks shutdown."""
     ecomax.handle_frame(
         SensorDataMessage(message=messages[FrameType.MESSAGE_SENSOR_DATA])
     )
     await ecomax.wait_until_done()
 
-    with patch("pyplumio.devices.Mixer.shutdown") as mock_mixer_shutdown, patch(
-        "pyplumio.devices.Thermostat.shutdown"
+    with patch("pyplumio.devices.mixer.Mixer.shutdown") as mock_mixer_shutdown, patch(
+        "pyplumio.devices.thermostat.Thermostat.shutdown"
     ) as mock_thermostat_shutdown, patch(
         "pyplumio.devices.Device.cancel_tasks"
     ) as mock_cancel_tasks, patch(
         "pyplumio.devices.Device.wait_until_done"
     ) as mock_wait_until_done:
         await ecomax.shutdown()
```

### Comparing `PyPlumIO-0.3.5/tests/test_filters.py` & `PyPlumIO-0.4.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/test_init.py` & `PyPlumIO-0.4.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/test_main.py` & `PyPlumIO-0.4.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/test_protocol.py` & `PyPlumIO-0.4.0/tests/test_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Contains tests for protocol."""
 
 import asyncio
 import logging
 from unittest.mock import AsyncMock, Mock, PropertyMock, call, patch
-import warnings
 
 import pytest
 
 from pyplumio.const import ATTR_CONNECTED, DeviceType, EncryptionType
 from pyplumio.devices.ecomax import EcoMAX
 from pyplumio.exceptions import (
     FrameError,
@@ -279,27 +278,14 @@
         await protocol.connection_lost()
 
     # Check that devices were notified and callback was called.
     mock_ecomax.dispatch.assert_called_once_with(ATTR_CONNECTED, False)
     mock_connection_lost_callback.assert_called_once()
 
 
-async def test_deprecated_get_device(protocol: Protocol) -> None:
-    """Test deprecated get_device method."""
-    with patch(
-        "pyplumio.protocol.Protocol.get", new_callable=AsyncMock
-    ) as mock_get, warnings.catch_warnings(record=True) as warn:
-        warnings.simplefilter("always")
-        await protocol.get_device("test")
-        assert len(warn) == 1
-        assert issubclass(warn[-1].category, DeprecationWarning)
-        assert "deprecated" in str(warn[-1].message)
-        mock_get.assert_awaited_once_with("test", None)
-
-
 @patch("asyncio.wait")
 @patch("asyncio.gather", new_callable=AsyncMock)
 @patch("pyplumio.protocol.Protocol.cancel_tasks")
 @patch("pyplumio.devices.ecomax.EcoMAX.shutdown")
 async def test_shutdown(
     mock_shutdown,
     mock_cancel_tasks,
```

### Comparing `PyPlumIO-0.3.5/tests/test_stream.py` & `PyPlumIO-0.4.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tests/test_util.py` & `PyPlumIO-0.4.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.3.5/tox.ini` & `PyPlumIO-0.4.0/tox.ini`

 * *Files identical despite different names*

