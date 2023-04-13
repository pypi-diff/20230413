# Comparing `tmp/PyPlumIO-0.4.0.tar.gz` & `tmp/PyPlumIO-0.4.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPlumIO-0.4.0.tar", last modified: Thu Apr 13 21:39:08 2023, max compression
+gzip compressed data, was "PyPlumIO-0.4.0.post1.tar", last modified: Thu Apr 13 21:49:20 2023, max compression
```

## Comparing `PyPlumIO-0.4.0.tar` & `PyPlumIO-0.4.0.post1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/PyPlumIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/PyPlumIO.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.348367 PyPlumIO-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/protocol.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/images/ecomax.png
--rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/images/rs485.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/pyplumio/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 21:39:08.000000 PyPlumIO-0.4.0/pyplumio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/pyplumio/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/ecomax.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/ecoster.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/devices/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.352367 PyPlumIO-0.4.0/pyplumio/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/frames/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.356367 PyPlumIO-0.4.0/pyplumio/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/helpers/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/pyplumio/structures/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/data_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/ecomax_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/fan_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/frame_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/fuel_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/lambda_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/mixer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/mixer_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/network_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/output_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/pending_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/power.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/product_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/program_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/regulator_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/temperatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/thermostat_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/structures/thermostat_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyplumio/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/tests/frames/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/frames/test_responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:39:08.360367 PyPlumIO-0.4.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/helpers/test_uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    21987 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 21:38:53.000000 PyPlumIO-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.732936 PyPlumIO-0.4.0.post1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/protocol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.736935 PyPlumIO-0.4.0.post1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/images/ecomax.png
+-rw-r--r--   0 runner    (1001) docker     (123)   133458 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/images/rs485.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.740936 PyPlumIO-0.4.0.post1/pyplumio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 21:49:20.000000 PyPlumIO-0.4.0.post1/pyplumio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.740936 PyPlumIO-0.4.0.post1/pyplumio/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/ecomax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/ecoster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/devices/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.740936 PyPlumIO-0.4.0.post1/pyplumio/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/frames/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.744936 PyPlumIO-0.4.0.post1/pyplumio/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/helpers/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.748936 PyPlumIO-0.4.0.post1/pyplumio/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/data_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/ecomax_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/fan_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/frame_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/lambda_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/network_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/output_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/pending_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/product_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/program_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/regulator_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/temperatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyplumio/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.748936 PyPlumIO-0.4.0.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17493 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/tests/frames/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/frames/test_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:49:20.752936 PyPlumIO-0.4.0.post1/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/helpers/test_uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21987 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 21:48:58.000000 PyPlumIO-0.4.0.post1/tox.ini
```

### Comparing `PyPlumIO-0.4.0/.github/CODE_OF_CONDUCT.md` & `PyPlumIO-0.4.0.post1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.github/ISSUE_TEMPLATE/feature_request.yml` & `PyPlumIO-0.4.0.post1/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.github/workflows/ci.yml` & `PyPlumIO-0.4.0.post1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.github/workflows/codeql-analysis.yml` & `PyPlumIO-0.4.0.post1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.github/workflows/deploy.yml` & `PyPlumIO-0.4.0.post1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.github/workflows/documentation.yml` & `PyPlumIO-0.4.0.post1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.gitignore` & `PyPlumIO-0.4.0.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/.pre-commit-config.yaml` & `PyPlumIO-0.4.0.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/LICENSE` & `PyPlumIO-0.4.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/PKG-INFO` & `PyPlumIO-0.4.0.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.4.0
+Version: 0.4.0.post1
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
-Project-URL: Documentation, https://pypulmio.denpa.pro
+Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyPlumIO-0.4.0/PyPlumIO.egg-info/PKG-INFO` & `PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyPlumIO
-Version: 0.4.0
+Version: 0.4.0.post1
 Summary: PyPlumIO is a native ecoNET library for Plum ecoMAX controllers.
 Author-email: Denis Paavilainen <denpa@denpa.pro>
 License: MIT License
-Project-URL: Documentation, https://pypulmio.denpa.pro
+Project-URL: Documentation, https://pyplumio.denpa.pro
 Project-URL: Source Code, https://github.com/denpamusic/PyPlumIO
 Project-URL: Bug Tracker, https://github.com/denpamusic/PyPlumIO/issues
 Keywords: home,automation,heating
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyPlumIO-0.4.0/PyPlumIO.egg-info/SOURCES.txt` & `PyPlumIO-0.4.0.post1/PyPlumIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/README.md` & `PyPlumIO-0.4.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/docs/Makefile` & `PyPlumIO-0.4.0.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/docs/make.bat` & `PyPlumIO-0.4.0.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/docs/source/conf.py` & `PyPlumIO-0.4.0.post1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/docs/source/index.rst` & `PyPlumIO-0.4.0.post1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/docs/source/protocol.rst` & `PyPlumIO-0.4.0.post1/docs/source/protocol.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/docs/source/usage.rst` & `PyPlumIO-0.4.0.post1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/images/ecomax.png` & `PyPlumIO-0.4.0.post1/images/ecomax.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/images/rs485.png` & `PyPlumIO-0.4.0.post1/images/rs485.png`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/__init__.py` & `PyPlumIO-0.4.0.post1/pyplumio/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/connection.py` & `PyPlumIO-0.4.0.post1/pyplumio/connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/const.py` & `PyPlumIO-0.4.0.post1/pyplumio/const.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/devices/__init__.py` & `PyPlumIO-0.4.0.post1/pyplumio/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/devices/ecomax.py` & `PyPlumIO-0.4.0.post1/pyplumio/devices/ecomax.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/devices/mixer.py` & `PyPlumIO-0.4.0.post1/pyplumio/devices/mixer.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/devices/thermostat.py` & `PyPlumIO-0.4.0.post1/pyplumio/devices/thermostat.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/exceptions.py` & `PyPlumIO-0.4.0.post1/pyplumio/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/filters.py` & `PyPlumIO-0.4.0.post1/pyplumio/filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/frames/__init__.py` & `PyPlumIO-0.4.0.post1/pyplumio/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/frames/messages.py` & `PyPlumIO-0.4.0.post1/pyplumio/frames/messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/frames/requests.py` & `PyPlumIO-0.4.0.post1/pyplumio/frames/requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/frames/responses.py` & `PyPlumIO-0.4.0.post1/pyplumio/frames/responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/data_types.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/event_manager.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/factory.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/parameter.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/schedule.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/task_manager.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/timeout.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/helpers/uid.py` & `PyPlumIO-0.4.0.post1/pyplumio/helpers/uid.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/protocol.py` & `PyPlumIO-0.4.0.post1/pyplumio/protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/stream.py` & `PyPlumIO-0.4.0.post1/pyplumio/stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/__init__.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/alerts.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/data_schema.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/data_schema.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/ecomax_parameters.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/ecomax_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/fan_power.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/fan_power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/frame_versions.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/frame_versions.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/fuel_consumption.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/fuel_level.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/fuel_level.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/lambda_sensor.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/lambda_sensor.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/load.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/load.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/mixer_parameters.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/mixer_sensors.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/mixer_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/modules.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/modules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/network_info.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/network_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/output_flags.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/output_flags.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/outputs.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/outputs.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/pending_alerts.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/pending_alerts.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/power.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/power.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/product_info.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/product_info.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/program_version.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/program_version.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/regulator_data.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/regulator_data.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/schedules.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/schedules.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/statuses.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/statuses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/temperatures.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/temperatures.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/thermostat_parameters.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_parameters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/structures/thermostat_sensors.py` & `PyPlumIO-0.4.0.post1/pyplumio/structures/thermostat_sensors.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyplumio/util.py` & `PyPlumIO-0.4.0.post1/pyplumio/util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/pyproject.toml` & `PyPlumIO-0.4.0.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 dependencies = [
     "pyserial-asyncio==0.6",
 ]
 dynamic = ["version"]
 
 [project.urls]
-"Documentation" = "https://pypulmio.denpa.pro"
+"Documentation" = "https://pyplumio.denpa.pro"
 "Source Code" = "https://github.com/denpamusic/PyPlumIO"
 "Bug Tracker" = "https://github.com/denpamusic/PyPlumIO/issues"
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `PyPlumIO-0.4.0/tests/conftest.py` & `PyPlumIO-0.4.0.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/frames/test_init.py` & `PyPlumIO-0.4.0.post1/tests/frames/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/frames/test_messages.py` & `PyPlumIO-0.4.0.post1/tests/frames/test_messages.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/frames/test_requests.py` & `PyPlumIO-0.4.0.post1/tests/frames/test_requests.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/frames/test_responses.py` & `PyPlumIO-0.4.0.post1/tests/frames/test_responses.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/helpers/test_data_types.py` & `PyPlumIO-0.4.0.post1/tests/helpers/test_data_types.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/helpers/test_event_manager.py` & `PyPlumIO-0.4.0.post1/tests/helpers/test_event_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/helpers/test_factory.py` & `PyPlumIO-0.4.0.post1/tests/helpers/test_factory.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/helpers/test_parameter.py` & `PyPlumIO-0.4.0.post1/tests/helpers/test_parameter.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/helpers/test_schedule.py` & `PyPlumIO-0.4.0.post1/tests/helpers/test_schedule.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/helpers/test_task_manager.py` & `PyPlumIO-0.4.0.post1/tests/helpers/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/helpers/test_timeout.py` & `PyPlumIO-0.4.0.post1/tests/helpers/test_timeout.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_connection.py` & `PyPlumIO-0.4.0.post1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_devices.py` & `PyPlumIO-0.4.0.post1/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_filters.py` & `PyPlumIO-0.4.0.post1/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_init.py` & `PyPlumIO-0.4.0.post1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_main.py` & `PyPlumIO-0.4.0.post1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_protocol.py` & `PyPlumIO-0.4.0.post1/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_stream.py` & `PyPlumIO-0.4.0.post1/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tests/test_util.py` & `PyPlumIO-0.4.0.post1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `PyPlumIO-0.4.0/tox.ini` & `PyPlumIO-0.4.0.post1/tox.ini`

 * *Files identical despite different names*

