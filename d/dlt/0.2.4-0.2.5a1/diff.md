# Comparing `tmp/dlt-0.2.4.tar.gz` & `tmp/dlt-0.2.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.4.tar", last modified: Thu Apr 13 10:16:22 2023, max compression
+gzip compressed data, was "dlt-0.2.5a1.tar", max compression
```

## Comparing `dlt-0.2.4.tar` & `dlt-0.2.5a1.tar`

### file list

```diff
@@ -1,19 +1,202 @@
-drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-13 10:16:22.515210 dlt-0.2.4/
--rwxr-xr-x   0 burnash    (501) staff       (20)     1085 2018-01-25 03:33:06.000000 dlt-0.2.4/LICENSE.md
--rwxr-xr-x   0 burnash    (501) staff       (20)       37 2018-01-25 03:33:06.000000 dlt-0.2.4/MANIFEST.in
--rw-r--r--   0 burnash    (501) staff       (20)      690 2023-04-13 10:16:22.515334 dlt-0.2.4/PKG-INFO
--rwxr-xr-x   0 burnash    (501) staff       (20)     1920 2018-02-14 14:45:42.000000 dlt-0.2.4/README.md
-drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-13 10:16:22.513721 dlt-0.2.4/dlt/
--rwxr-xr-x   0 burnash    (501) staff       (20)      485 2023-04-13 10:15:44.000000 dlt-0.2.4/dlt/__init__.py
--rwxr-xr-x   0 burnash    (501) staff       (20)     5297 2018-01-30 08:29:01.000000 dlt-0.2.4/dlt/cifar.py
--rwxr-xr-x   0 burnash    (501) staff       (20)     1349 2018-01-25 03:33:06.000000 dlt-0.2.4/dlt/fashion_mnist.py
--rwxr-xr-x   0 burnash    (501) staff       (20)      927 2018-01-30 08:30:39.000000 dlt-0.2.4/dlt/mnist.py
--rwxr-xr-x   0 burnash    (501) staff       (20)    10235 2018-02-14 14:57:07.000000 dlt-0.2.4/dlt/utils.py
-drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-13 10:16:22.515004 dlt-0.2.4/dlt.egg-info/
--rw-r--r--   0 burnash    (501) staff       (20)      690 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/PKG-INFO
--rw-r--r--   0 burnash    (501) staff       (20)      261 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/SOURCES.txt
--rw-r--r--   0 burnash    (501) staff       (20)        1 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/dependency_links.txt
--rw-r--r--   0 burnash    (501) staff       (20)       47 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/requires.txt
--rw-r--r--   0 burnash    (501) staff       (20)        4 2023-04-13 10:16:22.000000 dlt-0.2.4/dlt.egg-info/top_level.txt
--rwxr-xr-x   0 burnash    (501) staff       (20)       70 2023-04-13 10:16:22.515727 dlt-0.2.4/setup.cfg
--rwxr-xr-x   0 burnash    (501) staff       (20)      839 2023-04-13 09:44:49.000000 dlt-0.2.4/setup.py
+-rw-r--r--   0        0        0    11343 2023-04-06 15:20:13.865351 dlt-0.2.5a1/LICENSE.txt
+-rw-r--r--   0        0        0     5277 2023-04-13 12:36:14.969762 dlt-0.2.5a1/README.md
+-rw-r--r--   0        0        0     1661 2023-04-12 17:10:39.598778 dlt-0.2.5a1/dlt/__init__.py
+-rw-r--r--   0        0        0       31 2023-04-06 15:20:13.866512 dlt-0.2.5a1/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    13282 2023-04-06 15:20:13.866661 dlt-0.2.5a1/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3653 2023-04-06 15:20:13.866767 dlt-0.2.5a1/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    16662 2023-04-06 15:20:13.866947 dlt-0.2.5a1/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0     1683 2023-04-06 15:20:13.867073 dlt-0.2.5a1/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-04-06 15:20:13.867191 dlt-0.2.5a1/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18888 2023-04-13 13:06:57.962424 dlt-0.2.5a1/dlt/cli/init_command.py
+-rw-r--r--   0        0        0     6255 2023-04-06 15:20:13.867536 dlt-0.2.5a1/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9419 2023-04-06 15:20:13.867687 dlt-0.2.5a1/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4404 2023-04-06 15:20:13.867805 dlt-0.2.5a1/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1776 2023-04-06 15:20:13.867916 dlt-0.2.5a1/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0      106 2023-04-06 15:20:13.868003 dlt-0.2.5a1/dlt/cli/typing.py
+-rw-r--r--   0        0        0     3662 2023-04-06 15:20:13.868104 dlt-0.2.5a1/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-04-06 15:20:13.868241 dlt-0.2.5a1/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2023-04-06 15:20:13.868339 dlt-0.2.5a1/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      428 2023-04-06 15:20:13.868485 dlt-0.2.5a1/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     4898 2023-04-06 15:20:13.868600 dlt-0.2.5a1/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3448 2023-04-06 15:20:13.868721 dlt-0.2.5a1/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5884 2023-04-06 15:20:13.868843 dlt-0.2.5a1/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7773 2023-04-11 19:17:13.136572 dlt-0.2.5a1/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1198 2023-04-06 15:20:13.869116 dlt-0.2.5a1/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      252 2023-04-06 15:20:13.869256 dlt-0.2.5a1/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1089 2023-04-06 15:20:13.869358 dlt-0.2.5a1/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1193 2023-04-06 15:20:13.869462 dlt-0.2.5a1/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     2050 2023-04-06 15:20:13.869570 dlt-0.2.5a1/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0      758 2023-04-06 15:20:13.869667 dlt-0.2.5a1/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     4922 2023-04-11 20:01:32.767153 dlt-0.2.5a1/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18084 2023-04-12 15:12:05.711413 dlt-0.2.5a1/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      815 2023-04-06 15:20:13.870177 dlt-0.2.5a1/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0    10914 2023-04-11 19:17:13.137158 dlt-0.2.5a1/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     1854 2023-04-06 15:20:13.870453 dlt-0.2.5a1/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     2792 2023-04-06 15:20:13.870561 dlt-0.2.5a1/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1124 2023-04-06 15:20:13.870700 dlt-0.2.5a1/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0     3047 2023-04-06 15:20:13.870845 dlt-0.2.5a1/dlt/common/configuration/specs/gcp_client_credentials.py
+-rw-r--r--   0        0        0      665 2023-04-06 15:20:13.870968 dlt-0.2.5a1/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0      556 2023-04-06 15:20:13.871124 dlt-0.2.5a1/dlt/common/configuration/specs/load_volume_configuration.py
+-rw-r--r--   0        0        0      417 2023-04-06 15:20:13.871244 dlt-0.2.5a1/dlt/common/configuration/specs/normalize_volume_configuration.py
+-rw-r--r--   0        0        0     2769 2023-04-06 15:20:13.871358 dlt-0.2.5a1/dlt/common/configuration/specs/postgres_credentials.py
+-rw-r--r--   0        0        0     2532 2023-04-06 15:20:13.871468 dlt-0.2.5a1/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0      944 2023-04-06 15:20:13.871570 dlt-0.2.5a1/dlt/common/configuration/specs/schema_volume_configuration.py
+-rw-r--r--   0        0        0     5339 2023-04-06 15:20:13.871785 dlt-0.2.5a1/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-04-06 15:20:13.871968 dlt-0.2.5a1/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-04-06 15:20:13.872137 dlt-0.2.5a1/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-04-06 15:20:13.872251 dlt-0.2.5a1/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-04-06 15:20:13.872403 dlt-0.2.5a1/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-04-06 15:20:13.872525 dlt-0.2.5a1/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2395 2023-04-06 15:20:13.872641 dlt-0.2.5a1/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-04-06 15:20:13.872732 dlt-0.2.5a1/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-04-06 15:20:13.872876 dlt-0.2.5a1/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0       97 2023-04-06 15:20:13.873047 dlt-0.2.5a1/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-06 15:20:13.873165 dlt-0.2.5a1/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    10682 2023-04-11 19:17:13.137365 dlt-0.2.5a1/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6439 2023-04-11 19:17:13.137531 dlt-0.2.5a1/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-04-06 15:20:13.873598 dlt-0.2.5a1/dlt/common/git.py
+-rw-r--r--   0        0        0     5248 2023-04-11 19:17:13.137693 dlt-0.2.5a1/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-11 19:17:13.137836 dlt-0.2.5a1/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-11 19:17:13.138015 dlt-0.2.5a1/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0      232 2023-04-06 15:20:13.874188 dlt-0.2.5a1/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1210 2023-04-06 15:20:13.874288 dlt-0.2.5a1/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-04-06 15:20:13.874377 dlt-0.2.5a1/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-11 19:17:13.138171 dlt-0.2.5a1/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13396 2023-04-11 19:17:13.138353 dlt-0.2.5a1/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-04-06 15:20:13.874875 dlt-0.2.5a1/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-04-06 15:20:13.875007 dlt-0.2.5a1/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-04-06 15:20:13.875132 dlt-0.2.5a1/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-04-06 15:20:13.875231 dlt-0.2.5a1/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-06 15:20:13.875343 dlt-0.2.5a1/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-04-06 15:20:13.875460 dlt-0.2.5a1/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-06 15:20:13.875554 dlt-0.2.5a1/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-11 19:17:13.138502 dlt-0.2.5a1/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-04-06 15:20:13.875758 dlt-0.2.5a1/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    14410 2023-04-12 15:12:05.711649 dlt-0.2.5a1/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.876032 dlt-0.2.5a1/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-04-06 15:20:13.876156 dlt-0.2.5a1/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-11 19:17:13.138862 dlt-0.2.5a1/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5117 2023-04-06 15:20:13.876379 dlt-0.2.5a1/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      210 2023-04-06 15:20:13.876517 dlt-0.2.5a1/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0     1079 2023-04-06 15:20:13.876626 dlt-0.2.5a1/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0      939 2023-04-06 15:20:13.876720 dlt-0.2.5a1/dlt/common/runners/init.py
+-rw-r--r--   0        0        0     7832 2023-04-06 15:20:13.876921 dlt-0.2.5a1/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-04-06 15:20:13.877077 dlt-0.2.5a1/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-04-06 15:20:13.877194 dlt-0.2.5a1/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-04-06 15:20:13.877453 dlt-0.2.5a1/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      583 2023-04-06 15:20:13.877558 dlt-0.2.5a1/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5250 2023-04-06 15:20:13.877675 dlt-0.2.5a1/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.877784 dlt-0.2.5a1/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0     3828 2023-04-06 15:20:13.877913 dlt-0.2.5a1/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0     6320 2023-04-06 15:20:13.878085 dlt-0.2.5a1/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2026 2023-04-06 15:20:13.878281 dlt-0.2.5a1/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     6554 2023-04-06 15:20:13.878421 dlt-0.2.5a1/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2479 2023-04-06 15:20:13.878523 dlt-0.2.5a1/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     1943 2023-04-06 15:20:13.878627 dlt-0.2.5a1/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-06 15:20:13.878735 dlt-0.2.5a1/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      989 2023-04-06 15:20:13.878839 dlt-0.2.5a1/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-06 15:20:13.878980 dlt-0.2.5a1/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-04-06 15:20:13.879100 dlt-0.2.5a1/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-04-06 15:20:13.879229 dlt-0.2.5a1/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25175 2023-04-11 19:17:13.139202 dlt-0.2.5a1/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     2976 2023-04-06 15:20:13.879636 dlt-0.2.5a1/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    21530 2023-04-12 15:12:05.712017 dlt-0.2.5a1/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0      410 2023-04-06 15:20:13.880044 dlt-0.2.5a1/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-06 15:20:13.880173 dlt-0.2.5a1/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2804 2023-04-06 15:20:13.880285 dlt-0.2.5a1/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0     9059 2023-04-06 15:20:13.880432 dlt-0.2.5a1/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2685 2023-04-12 15:12:05.712222 dlt-0.2.5a1/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21684 2023-04-06 15:20:13.880777 dlt-0.2.5a1/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2414 2023-04-06 15:20:13.880947 dlt-0.2.5a1/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8508 2023-04-06 15:20:13.881095 dlt-0.2.5a1/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2465 2023-04-06 15:20:13.881225 dlt-0.2.5a1/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2677 2023-04-06 15:20:13.881365 dlt-0.2.5a1/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-06 15:20:13.881494 dlt-0.2.5a1/dlt/common/typing.py
+-rw-r--r--   0        0        0    10588 2023-04-11 19:17:13.139619 dlt-0.2.5a1/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-04-06 15:20:13.881847 dlt-0.2.5a1/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-04-06 15:20:13.882015 dlt-0.2.5a1/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.882122 dlt-0.2.5a1/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-04-06 15:20:13.882326 dlt-0.2.5a1/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-06 15:20:13.882430 dlt-0.2.5a1/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12301 2023-04-11 19:17:13.139861 dlt-0.2.5a1/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      392 2023-04-06 15:20:13.882780 dlt-0.2.5a1/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10169 2023-04-06 15:20:13.882921 dlt-0.2.5a1/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-06 15:20:13.883076 dlt-0.2.5a1/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     5503 2023-04-06 15:20:13.883187 dlt-0.2.5a1/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-04-06 15:20:13.883437 dlt-0.2.5a1/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-06 15:20:13.883566 dlt-0.2.5a1/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-04-06 15:20:13.883757 dlt-0.2.5a1/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-06 15:20:13.883867 dlt-0.2.5a1/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4975 2023-04-06 15:20:13.883996 dlt-0.2.5a1/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-06 15:20:13.884122 dlt-0.2.5a1/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     4983 2023-04-06 15:20:13.884272 dlt-0.2.5a1/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    14398 2023-04-11 19:17:13.140063 dlt-0.2.5a1/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-06 15:20:13.884546 dlt-0.2.5a1/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-04-06 15:20:13.884710 dlt-0.2.5a1/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-06 15:20:13.884806 dlt-0.2.5a1/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0      443 2023-04-06 15:20:13.884893 dlt-0.2.5a1/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-04-06 15:20:13.884988 dlt-0.2.5a1/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6066 2023-04-12 15:12:05.712412 dlt-0.2.5a1/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-06 15:20:13.885239 dlt-0.2.5a1/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-06 15:20:13.885340 dlt-0.2.5a1/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      405 2023-04-06 15:20:13.885474 dlt-0.2.5a1/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-04-06 15:20:13.885590 dlt-0.2.5a1/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     6850 2023-04-06 15:20:13.885722 dlt-0.2.5a1/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10101 2023-04-11 19:17:13.140321 dlt-0.2.5a1/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1933 2023-04-06 15:20:13.885947 dlt-0.2.5a1/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.886049 dlt-0.2.5a1/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    22227 2023-04-11 19:17:13.140593 dlt-0.2.5a1/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12183 2023-04-11 19:17:13.140877 dlt-0.2.5a1/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     7654 2023-04-12 15:12:05.712637 dlt-0.2.5a1/dlt/extract/extract.py
+-rw-r--r--   0        0        0    13689 2023-04-12 15:12:05.712864 dlt-0.2.5a1/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31421 2023-04-12 15:12:05.713134 dlt-0.2.5a1/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     8210 2023-04-12 15:12:05.713430 dlt-0.2.5a1/dlt/extract/schema.py
+-rw-r--r--   0        0        0    30388 2023-04-12 15:12:05.713696 dlt-0.2.5a1/dlt/extract/source.py
+-rw-r--r--   0        0        0     4781 2023-04-12 15:12:05.713893 dlt-0.2.5a1/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 15:20:13.887409 dlt-0.2.5a1/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.887511 dlt-0.2.5a1/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-06 15:20:13.887654 dlt-0.2.5a1/dlt/helpers/dbt/README.md
+-rw-r--r--   0        0        0     2907 2023-04-06 15:20:13.887756 dlt-0.2.5a1/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-06 15:20:13.887882 dlt-0.2.5a1/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-04-06 15:20:13.888012 dlt-0.2.5a1/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-04-06 15:20:13.888126 dlt-0.2.5a1/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-04-06 15:20:13.888232 dlt-0.2.5a1/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    14293 2023-04-06 15:20:13.888399 dlt-0.2.5a1/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2373 2023-04-06 15:20:13.888508 dlt-0.2.5a1/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     1035 2023-04-06 15:20:13.888600 dlt-0.2.5a1/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    12920 2023-04-13 13:08:09.451202 dlt-0.2.5a1/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2023-04-06 15:20:13.888885 dlt-0.2.5a1/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1103 2023-04-06 15:20:13.889003 dlt-0.2.5a1/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-06 15:20:13.889110 dlt-0.2.5a1/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    20447 2023-04-06 15:20:13.889323 dlt-0.2.5a1/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-04-06 15:20:13.889485 dlt-0.2.5a1/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-06 15:20:13.889573 dlt-0.2.5a1/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.889615 dlt-0.2.5a1/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    17989 2023-04-11 19:17:13.142942 dlt-0.2.5a1/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2023-04-06 15:20:13.889985 dlt-0.2.5a1/dlt/pipeline/README.md
+-rw-r--r--   0        0        0    12224 2023-04-12 15:12:05.714087 dlt-0.2.5a1/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1823 2023-04-06 15:20:13.890499 dlt-0.2.5a1/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      342 2023-04-06 15:20:13.890615 dlt-0.2.5a1/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-04-06 15:20:13.890730 dlt-0.2.5a1/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     2537 2023-04-06 15:20:13.890828 dlt-0.2.5a1/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     1497 2023-04-06 15:20:13.890922 dlt-0.2.5a1/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-11 19:17:13.143161 dlt-0.2.5a1/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    58159 2023-04-13 12:59:16.401972 dlt-0.2.5a1/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0     4200 2023-04-11 19:17:13.143762 dlt-0.2.5a1/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-06 15:20:13.891660 dlt-0.2.5a1/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4563 2023-04-06 15:20:13.891788 dlt-0.2.5a1/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-04-06 15:20:13.891882 dlt-0.2.5a1/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.891929 dlt-0.2.5a1/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.892040 dlt-0.2.5a1/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-04-06 15:20:13.892137 dlt-0.2.5a1/dlt/reflection/names.py
+-rw-r--r--   0        0        0     4805 2023-04-06 15:20:13.892251 dlt-0.2.5a1/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-04-06 15:20:13.892405 dlt-0.2.5a1/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      118 2023-04-11 19:17:13.143908 dlt-0.2.5a1/dlt/sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:20:13.892603 dlt-0.2.5a1/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-04-06 15:20:13.892755 dlt-0.2.5a1/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9089 2023-04-06 15:20:13.892883 dlt-0.2.5a1/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-04-06 15:20:13.892983 dlt-0.2.5a1/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-11 19:17:13.144029 dlt-0.2.5a1/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-13 13:00:28.813120 dlt-0.2.5a1/dlt/version.py
+-rw-r--r--   0        0        0     3716 2023-04-13 13:03:11.818599 dlt-0.2.5a1/pyproject.toml
+-rw-r--r--   0        0        0     8423 1970-01-01 00:00:00.000000 dlt-0.2.5a1/PKG-INFO
```

