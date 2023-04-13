# Comparing `tmp/amsterdam-schema-tools-5.9.1.tar.gz` & `tmp/amsterdam-schema-tools-5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amsterdam-schema-tools-5.9.1.tar", last modified: Fri Apr  7 06:44:52 2023, max compression
+gzip compressed data, was "amsterdam-schema-tools-5.9.2.tar", last modified: Thu Apr 13 11:51:53 2023, max compression
```

## Comparing `amsterdam-schema-tools-5.9.1.tar` & `amsterdam-schema-tools-5.9.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/
--rw-rw-r--   0 jan       (1000) jan       (1000)    16725 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/LICENSE
--rw-rw-r--   0 jan       (1000) jan       (1000)     8030 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     7222 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/README.md
--rw-rw-r--   0 jan       (1000) jan       (1000)      385 2022-02-02 10:52:20.000000 amsterdam-schema-tools-5.9.1/pyproject.toml
--rw-rw-r--   0 jan       (1000) jan       (1000)     3215 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/setup.cfg
--rwxrwxr-x   0 jan       (1000) jan       (1000)       38 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/setup.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.854717 amsterdam-schema-tools-5.9.1/src/
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.858717 amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/
--rw-rw-r--   0 jan       (1000) jan       (1000)     8030 2023-04-07 06:44:52.000000 amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     5215 2023-04-07 06:44:52.000000 amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2023-04-07 06:44:52.000000 amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       93 2023-04-07 06:44:52.000000 amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/entry_points.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)      775 2023-04-07 06:44:52.000000 amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/requires.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)       12 2023-04-07 06:44:52.000000 amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/top_level.txt
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.858717 amsterdam-schema-tools-5.9.1/src/schematools/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1533 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.1/src/schematools/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.858717 amsterdam-schema-tools-5.9.1/src/schematools/ckan/
--rw-rw-r--   0 jan       (1000) jan       (1000)      220 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/ckan/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4070 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.1/src/schematools/ckan/_convert.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    36776 2023-04-06 11:46:32.000000 amsterdam-schema-tools-5.9.1/src/schematools/cli.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.858717 amsterdam-schema-tools-5.9.1/src/schematools/contrib/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.858717 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2023-01-25 10:03:29.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2456 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/app_config.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      553 2022-12-19 10:56:22.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/apps.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      671 2021-07-12 15:13:15.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/auth_backend.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1073 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/cli.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      535 2021-04-06 12:58:11.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/db.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    22707 2023-02-07 06:49:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/factories.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.862717 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/
--rw-rw-r--   0 jan       (1000) jan       (1000)     8021 2023-01-23 08:50:49.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1727 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/create.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.862717 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      949 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/date.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1041 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/date_time.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2955 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/geo.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      899 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/integer.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      275 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/nuller.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1141 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/pyfloat.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6839 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/relate.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2625 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/loaders.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.862717 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/__init__.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.862717 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1625 2023-03-02 18:29:52.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4219 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/change_dataset.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1341 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/create_mock_data.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3560 2023-01-25 10:59:12.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/create_tables.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3865 2023-01-23 08:10:48.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/dump_model_mockers.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     9003 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/dump_models.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2478 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/import_profiles.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6682 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/import_schemas.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      609 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/relate_mock_data.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2897 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/remove_schemas.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    13225 2023-01-10 15:37:21.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/sqlmigrate_schema.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      788 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/truncate_tables.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1382 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/managers.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.862717 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/
--rw-rw-r--   0 jan       (1000) jan       (1000)     1309 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0001_initial.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1963 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0002_add_datasettable.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      425 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0003_datasettable_geometry_field_type.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      661 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0004_add_authorization_fields.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1355 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0005_datasetfield.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      899 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0006_remote_datasets.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      396 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0007_datasettable_is_temporal.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1034 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0008_profile.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      822 2021-04-06 12:58:11.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0009_auto_20210330_1659.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      606 2021-04-08 06:18:45.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0010_use_native_jsonfield.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1472 2021-07-06 10:06:37.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0011_auto_20210623_1135.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      580 2021-07-23 06:32:25.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0012_schema_data_as_textfield.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      586 2021-07-23 06:32:25.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0013_profile_schema_data_as_textfield.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      455 2021-11-29 07:59:58.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0014_datasettable_version.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1210 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0015_alter_dataset_id_alter_datasetfield_id_and_more.py
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1099 2023-01-23 08:10:48.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/mockers.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    21013 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/models.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      129 2021-05-12 11:02:03.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/signals.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      733 2021-07-23 06:32:25.000000 amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/validators.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.862717 amsterdam-schema-tools-5.9.1/src/schematools/events/
--rw-rw-r--   0 jan       (1000) jan       (1000)       78 2021-05-19 15:34:33.000000 amsterdam-schema-tools-5.9.1/src/schematools/events/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     9248 2023-04-07 06:12:04.000000 amsterdam-schema-tools-5.9.1/src/schematools/events/full.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      714 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.1/src/schematools/exceptions.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.862717 amsterdam-schema-tools-5.9.1/src/schematools/exports/
--rw-rw-r--   0 jan       (1000) jan       (1000)     3264 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/exports/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1457 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/exports/csv.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2136 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/exports/geopackage.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1799 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/exports/jsonlines.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    18967 2023-01-23 08:50:49.000000 amsterdam-schema-tools-5.9.1/src/schematools/factories.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/importer/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/importer/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    19780 2023-01-19 16:15:40.000000 amsterdam-schema-tools-5.9.1/src/schematools/importer/base.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2680 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/importer/geojson.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12759 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/importer/ndjson.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/introspect/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/introspect/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4277 2023-04-05 13:59:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/introspect/db.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4233 2021-11-29 07:59:58.000000 amsterdam-schema-tools-5.9.1/src/schematools/introspect/geojson.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      912 2023-04-05 13:59:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/introspect/utils.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    23953 2023-02-06 10:16:09.000000 amsterdam-schema-tools-5.9.1/src/schematools/loaders.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/maps/
--rw-rw-r--   0 jan       (1000) jan       (1000)      163 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      415 2021-06-15 08:30:16.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/create.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/maps/generators/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/generators/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3698 2021-06-15 08:30:16.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/generators/mapfile.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1456 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/json_.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/mapfile/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/mapfile/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1169 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/mapfile/serializers.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2842 2021-06-15 08:30:16.000000 amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/mapfile/types.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3663 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/src/schematools/naming.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/permissions/
--rw-rw-r--   0 jan       (1000) jan       (1000)      143 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/permissions/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    12640 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.1/src/schematools/permissions/auth.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    22003 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/permissions/db.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/src/schematools/provenance/
--rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.1/src/schematools/provenance/__init__.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     3240 2021-08-17 11:27:14.000000 amsterdam-schema-tools-5.9.1/src/schematools/provenance/create.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    80372 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/types.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     4566 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.1/src/schematools/utils.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    20868 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/src/schematools/validation.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-07 06:44:52.866717 amsterdam-schema-tools-5.9.1/tests/
--rw-rw-r--   0 jan       (1000) jan       (1000)      936 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/tests/test_ckan.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     7808 2023-04-07 06:12:04.000000 amsterdam-schema-tools-5.9.1/tests/test_events_full.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2550 2023-04-05 13:59:42.000000 amsterdam-schema-tools-5.9.1/tests/test_geojson.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    11861 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/tests/test_import.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    14681 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/tests/test_indexes.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      956 2023-01-23 08:08:35.000000 amsterdam-schema-tools-5.9.1/tests/test_loaders.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     1811 2022-12-19 10:56:22.000000 amsterdam-schema-tools-5.9.1/tests/test_naming.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    20238 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/tests/test_ndjson.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    34499 2023-01-23 08:08:35.000000 amsterdam-schema-tools-5.9.1/tests/test_permissions.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     6552 2023-03-20 13:52:46.000000 amsterdam-schema-tools-5.9.1/tests/test_permissions_auth.py
--rw-rw-r--   0 jan       (1000) jan       (1000)     2763 2021-11-29 07:59:58.000000 amsterdam-schema-tools-5.9.1/tests/test_provenance.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      456 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.1/tests/test_provenancemapper.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    11825 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/tests/test_types.py
--rw-rw-r--   0 jan       (1000) jan       (1000)    11855 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.1/tests/test_validation.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.092576 amsterdam-schema-tools-5.9.2/
+-rw-rw-r--   0 jan       (1000) jan       (1000)    16725 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/LICENSE
+-rw-rw-r--   0 jan       (1000) jan       (1000)     8030 2023-04-13 11:51:53.092576 amsterdam-schema-tools-5.9.2/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7222 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/README.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)      385 2022-02-02 10:52:20.000000 amsterdam-schema-tools-5.9.2/pyproject.toml
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3186 2023-04-13 11:51:53.092576 amsterdam-schema-tools-5.9.2/setup.cfg
+-rwxrwxr-x   0 jan       (1000) jan       (1000)       38 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/setup.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.060577 amsterdam-schema-tools-5.9.2/src/
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.064577 amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     8030 2023-04-13 11:51:53.000000 amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     5215 2023-04-13 11:51:53.000000 amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2023-04-13 11:51:53.000000 amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       93 2023-04-13 11:51:53.000000 amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)      748 2023-04-13 11:51:53.000000 amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/requires.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)       12 2023-04-13 11:51:53.000000 amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/top_level.txt
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.064577 amsterdam-schema-tools-5.9.2/src/schematools/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1533 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.2/src/schematools/__init__.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.064577 amsterdam-schema-tools-5.9.2/src/schematools/ckan/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      220 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/ckan/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4070 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.2/src/schematools/ckan/_convert.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    36758 2023-04-13 11:50:55.000000 amsterdam-schema-tools-5.9.2/src/schematools/cli.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.064577 amsterdam-schema-tools-5.9.2/src/schematools/contrib/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/__init__.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.068577 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2023-01-25 10:03:29.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2456 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/app_config.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      553 2022-12-19 10:56:22.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/apps.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      671 2021-07-12 15:13:15.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/auth_backend.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1073 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/cli.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      535 2021-04-06 12:58:11.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/db.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    22707 2023-02-07 06:49:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/factories.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.068577 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     8021 2023-01-23 08:50:49.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1727 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/create.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.072577 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      949 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/date.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1041 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/date_time.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2955 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/geo.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      899 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/integer.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      275 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/nuller.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1141 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/pyfloat.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6839 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/relate.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2625 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/loaders.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.072577 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/__init__.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.072577 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1625 2023-03-02 18:29:52.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4219 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/change_dataset.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1341 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/create_mock_data.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3560 2023-01-25 10:59:12.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/create_tables.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3865 2023-01-23 08:10:48.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/dump_model_mockers.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     9003 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/dump_models.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2478 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/import_profiles.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6682 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/import_schemas.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      609 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/relate_mock_data.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2897 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/remove_schemas.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    13225 2023-01-10 15:37:21.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/sqlmigrate_schema.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      788 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/truncate_tables.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1382 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/managers.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.076577 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1309 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0001_initial.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1963 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0002_add_datasettable.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      425 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0003_datasettable_geometry_field_type.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      661 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0004_add_authorization_fields.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1355 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0005_datasetfield.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      899 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0006_remote_datasets.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      396 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0007_datasettable_is_temporal.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1034 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0008_profile.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      822 2021-04-06 12:58:11.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0009_auto_20210330_1659.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      606 2021-04-08 06:18:45.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0010_use_native_jsonfield.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1472 2021-07-06 10:06:37.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0011_auto_20210623_1135.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      580 2021-07-23 06:32:25.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0012_schema_data_as_textfield.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      586 2021-07-23 06:32:25.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0013_profile_schema_data_as_textfield.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      455 2021-11-29 07:59:58.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0014_datasettable_version.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1210 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0015_alter_dataset_id_alter_datasetfield_id_and_more.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1099 2023-01-23 08:10:48.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/mockers.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    21013 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/models.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      129 2021-05-12 11:02:03.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/signals.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      733 2021-07-23 06:32:25.000000 amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/validators.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.076577 amsterdam-schema-tools-5.9.2/src/schematools/events/
+-rw-rw-r--   0 jan       (1000) jan       (1000)       78 2021-05-19 15:34:33.000000 amsterdam-schema-tools-5.9.2/src/schematools/events/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     9348 2023-04-13 11:50:55.000000 amsterdam-schema-tools-5.9.2/src/schematools/events/full.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      714 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.2/src/schematools/exceptions.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.080577 amsterdam-schema-tools-5.9.2/src/schematools/exports/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3264 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/exports/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1457 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/exports/csv.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2136 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/exports/geopackage.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1799 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/exports/jsonlines.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    18967 2023-01-23 08:50:49.000000 amsterdam-schema-tools-5.9.2/src/schematools/factories.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.080577 amsterdam-schema-tools-5.9.2/src/schematools/importer/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/importer/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    19780 2023-01-19 16:15:40.000000 amsterdam-schema-tools-5.9.2/src/schematools/importer/base.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2680 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/importer/geojson.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    12764 2023-04-13 11:50:55.000000 amsterdam-schema-tools-5.9.2/src/schematools/importer/ndjson.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.080577 amsterdam-schema-tools-5.9.2/src/schematools/introspect/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/introspect/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4277 2023-04-05 13:59:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/introspect/db.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4233 2021-11-29 07:59:58.000000 amsterdam-schema-tools-5.9.2/src/schematools/introspect/geojson.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      912 2023-04-05 13:59:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/introspect/utils.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    23953 2023-02-06 10:16:09.000000 amsterdam-schema-tools-5.9.2/src/schematools/loaders.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.080577 amsterdam-schema-tools-5.9.2/src/schematools/maps/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      163 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      415 2021-06-15 08:30:16.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/create.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.084576 amsterdam-schema-tools-5.9.2/src/schematools/maps/generators/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/generators/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3698 2021-06-15 08:30:16.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/generators/mapfile.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.084576 amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1456 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/json_.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.084576 amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/mapfile/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/mapfile/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1169 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/mapfile/serializers.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2842 2021-06-15 08:30:16.000000 amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/mapfile/types.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3663 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/src/schematools/naming.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.084576 amsterdam-schema-tools-5.9.2/src/schematools/permissions/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      143 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/permissions/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    12640 2022-10-04 06:57:51.000000 amsterdam-schema-tools-5.9.2/src/schematools/permissions/auth.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    22003 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/permissions/db.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.084576 amsterdam-schema-tools-5.9.2/src/schematools/provenance/
+-rw-rw-r--   0 jan       (1000) jan       (1000)        0 2021-03-25 13:13:42.000000 amsterdam-schema-tools-5.9.2/src/schematools/provenance/__init__.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3240 2021-08-17 11:27:14.000000 amsterdam-schema-tools-5.9.2/src/schematools/provenance/create.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    80372 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/types.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     4566 2023-01-09 16:35:00.000000 amsterdam-schema-tools-5.9.2/src/schematools/utils.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    20868 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/src/schematools/validation.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2023-04-13 11:51:53.092576 amsterdam-schema-tools-5.9.2/tests/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      910 2023-04-13 11:50:55.000000 amsterdam-schema-tools-5.9.2/tests/test_ckan.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     7808 2023-04-07 06:12:04.000000 amsterdam-schema-tools-5.9.2/tests/test_events_full.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2550 2023-04-05 13:59:42.000000 amsterdam-schema-tools-5.9.2/tests/test_geojson.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    11861 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/tests/test_import.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    14681 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/tests/test_indexes.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      956 2023-01-23 08:08:35.000000 amsterdam-schema-tools-5.9.2/tests/test_loaders.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     1811 2022-12-19 10:56:22.000000 amsterdam-schema-tools-5.9.2/tests/test_naming.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    20238 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/tests/test_ndjson.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    34499 2023-01-23 08:08:35.000000 amsterdam-schema-tools-5.9.2/tests/test_permissions.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     6552 2023-03-20 13:52:46.000000 amsterdam-schema-tools-5.9.2/tests/test_permissions_auth.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2763 2021-11-29 07:59:58.000000 amsterdam-schema-tools-5.9.2/tests/test_provenance.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      456 2022-12-12 12:46:30.000000 amsterdam-schema-tools-5.9.2/tests/test_provenancemapper.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    11825 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/tests/test_types.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)    11855 2023-04-05 12:15:27.000000 amsterdam-schema-tools-5.9.2/tests/test_validation.py
```

### Comparing `amsterdam-schema-tools-5.9.1/LICENSE` & `amsterdam-schema-tools-5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/PKG-INFO` & `amsterdam-schema-tools-5.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amsterdam-schema-tools
-Version: 5.9.1
+Version: 5.9.2
 Summary: Tools to work with Amsterdam Schema.
 Home-page: https://github.com/amsterdam/schema-tools
 Author: Team Data Diensten, van het Dataplatform onder de Directie Digitale Voorzieningen (Gemeente Amsterdam)
 Author-email: datapunt@amsterdam.nl
 License: Mozilla Public 2.0
 Keywords: jsonschema,schema,json,amsterdam,validation,code-generation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `amsterdam-schema-tools-5.9.1/README.md` & `amsterdam-schema-tools-5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/setup.cfg` & `amsterdam-schema-tools-5.9.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = amsterdam-schema-tools
-version = 5.9.1
+version = 5.9.2
 url = https://github.com/amsterdam/schema-tools
 license = Mozilla Public 2.0
 author = Team Data Diensten, van het Dataplatform onder de Directie Digitale Voorzieningen (Gemeente Amsterdam)
 author_email = datapunt@amsterdam.nl
 description = Tools to work with Amsterdam Schema.
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -31,16 +31,14 @@
 	geoalchemy2
 	psycopg2
 	pg-grant
 	click
 	deepdiff
 	jsonlines
 	jsonschema[format] >= 3.2.0
-	json-encoder
-	ndjson>=0.3.0
 	shapely>=1.8.0
 	python-string-utils
 	python-dateutil
 	requests
 	jinja2
 	mappyfile
 	methodtools
```

### Comparing `amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/PKG-INFO` & `amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amsterdam-schema-tools
-Version: 5.9.1
+Version: 5.9.2
 Summary: Tools to work with Amsterdam Schema.
 Home-page: https://github.com/amsterdam/schema-tools
 Author: Team Data Diensten, van het Dataplatform onder de Directie Digitale Voorzieningen (Gemeente Amsterdam)
 Author-email: datapunt@amsterdam.nl
 License: Mozilla Public 2.0
 Keywords: jsonschema,schema,json,amsterdam,validation,code-generation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/SOURCES.txt` & `amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/amsterdam_schema_tools.egg-info/requires.txt` & `amsterdam-schema-tools-5.9.2/src/amsterdam_schema_tools.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 geoalchemy2
 psycopg2
 pg-grant
 click
 deepdiff
 jsonlines
 jsonschema[format]>=3.2.0
-json-encoder
-ndjson>=0.3.0
 shapely>=1.8.0
 python-string-utils
 python-dateutil
 requests
 jinja2
 mappyfile
 methodtools
```

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/__init__.py` & `amsterdam-schema-tools-5.9.2/src/schematools/__init__.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/ckan/_convert.py` & `amsterdam-schema-tools-5.9.2/src/schematools/ckan/_convert.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/cli.py` & `amsterdam-schema-tools-5.9.2/src/schematools/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Cli tools."""
 from __future__ import annotations
 
 import io
+import json
 import logging
 import operator
 import os
 import sys
 from collections import defaultdict
 from functools import reduce
 from importlib.metadata import version
@@ -13,15 +14,14 @@
 from typing import Any, DefaultDict, Iterable, List
 
 import click
 import jsonschema
 import requests
 import sqlalchemy
 from deepdiff import DeepDiff
-from json_encoder import json
 from jsonschema import draft7_format_checker
 from sqlalchemy import create_engine, inspect
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.schema import CreateTable
 
 from schematools import (
     COMPATIBLE_METASCHEMAS,
```

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/app_config.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/app_config.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/apps.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/auth_backend.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/auth_backend.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/cli.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/cli.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/db.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/db.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/factories.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/factories.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/__init__.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/__init__.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/create.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/create.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/date.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/date.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/date_time.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/date_time.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/geo.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/geo.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/integer.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/integer.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/providers/pyfloat.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/providers/pyfloat.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/faker/relate.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/faker/relate.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/loaders.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/loaders.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/__init__.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/change_dataset.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/change_dataset.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/create_mock_data.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/create_mock_data.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/create_tables.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/create_tables.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/dump_model_mockers.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/dump_model_mockers.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/dump_models.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/dump_models.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/import_profiles.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/import_profiles.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/import_schemas.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/import_schemas.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/relate_mock_data.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/relate_mock_data.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/remove_schemas.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/remove_schemas.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/sqlmigrate_schema.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/sqlmigrate_schema.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/management/commands/truncate_tables.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/management/commands/truncate_tables.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/managers.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/managers.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0001_initial.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0002_add_datasettable.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0002_add_datasettable.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0004_add_authorization_fields.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0004_add_authorization_fields.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0005_datasetfield.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0005_datasetfield.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0006_remote_datasets.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0006_remote_datasets.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0008_profile.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0008_profile.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0009_auto_20210330_1659.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0009_auto_20210330_1659.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0010_use_native_jsonfield.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0010_use_native_jsonfield.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0011_auto_20210623_1135.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0011_auto_20210623_1135.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0012_schema_data_as_textfield.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0012_schema_data_as_textfield.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0013_profile_schema_data_as_textfield.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0013_profile_schema_data_as_textfield.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/migrations/0015_alter_dataset_id_alter_datasetfield_id_and_more.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/migrations/0015_alter_dataset_id_alter_datasetfield_id_and_more.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/mockers.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/mockers.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/models.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/models.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/contrib/django/validators.py` & `amsterdam-schema-tools-5.9.2/src/schematools/contrib/django/validators.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/events/full.py` & `amsterdam-schema-tools-5.9.2/src/schematools/events/full.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,18 +124,21 @@
             dataset_schema = self.datasets[dataset_id]
             schema_table = dataset_schema.get_table_by_id(table_id)
             db_table_name = schema_table.db_name_variant(postfix=FULL_LOAD_TABLE_POSTFIX)
             importer = BaseImporter(dataset_schema, self.conn.engine, logger)
             importer.generate_db_objects(
                 table_id,
                 db_table_name=db_table_name,
-                truncate=event_meta.get("first_of_sequence", False),
                 is_versioned_dataset=importer.is_versioned_dataset,
+                ind_extra_index=False,
             )
 
+            if event_meta.get("first_of_sequence", False):
+                self.conn.engine.execute(f"TRUNCATE {db_table_name}")
+
             table = importer.tables[table_id]
         else:
             schema_table = self.datasets[dataset_id].get_table_by_id(table_id)
             table = self.tables[dataset_id][to_snake_case(table_id)]
 
         row = self._flatten_event_data(event_data)
```

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/exceptions.py` & `amsterdam-schema-tools-5.9.2/src/schematools/exceptions.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/exports/__init__.py` & `amsterdam-schema-tools-5.9.2/src/schematools/exports/__init__.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/exports/csv.py` & `amsterdam-schema-tools-5.9.2/src/schematools/exports/csv.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/exports/geopackage.py` & `amsterdam-schema-tools-5.9.2/src/schematools/exports/geopackage.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/exports/jsonlines.py` & `amsterdam-schema-tools-5.9.2/src/schematools/exports/jsonlines.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/factories.py` & `amsterdam-schema-tools-5.9.2/src/schematools/factories.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/importer/base.py` & `amsterdam-schema-tools-5.9.2/src/schematools/importer/base.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/importer/geojson.py` & `amsterdam-schema-tools-5.9.2/src/schematools/importer/geojson.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/importer/ndjson.py` & `amsterdam-schema-tools-5.9.2/src/schematools/importer/ndjson.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import json
 from pathlib import PosixPath
 from typing import Any, Iterator
 
-import ndjson
+import orjson
 from shapely.geometry import shape
 
 from schematools.types import DatasetFieldSchema, DatasetTableSchema
 
 from .base import BaseImporter, Provenance, Record
 
 
@@ -17,17 +17,17 @@
 
     def parse_records(
         self, file_name: PosixPath, dataset_table: DatasetTableSchema, **kwargs: Any
     ) -> Iterator[dict[str, list[Record]]]:
         """Provide an iterator the reads the NDJSON records."""
         # Initializes the field mapper once for the table
         field_mapper = TableFieldMapper(dataset_table)
-        with open(file_name) as fh:
-            for row in ndjson.reader(fh):
-                records = field_mapper.parse_object(row)
+        with open(file_name, "rb") as fh:
+            for row in fh:
+                records = field_mapper.parse_object(orjson.loads(row))
                 yield records
 
 
 class TableFieldMapper:
     """Conversion of field names during the import.
     The :meth:`parse_object` returns the database records to create for a given NDJson line.
     """
```

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/introspect/db.py` & `amsterdam-schema-tools-5.9.2/src/schematools/introspect/db.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/introspect/geojson.py` & `amsterdam-schema-tools-5.9.2/src/schematools/introspect/geojson.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/introspect/utils.py` & `amsterdam-schema-tools-5.9.2/src/schematools/introspect/utils.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/loaders.py` & `amsterdam-schema-tools-5.9.2/src/schematools/loaders.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/maps/generators/mapfile.py` & `amsterdam-schema-tools-5.9.2/src/schematools/maps/generators/mapfile.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/json_.py` & `amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/json_.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/mapfile/serializers.py` & `amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/mapfile/serializers.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/maps/interfaces/mapfile/types.py` & `amsterdam-schema-tools-5.9.2/src/schematools/maps/interfaces/mapfile/types.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/naming.py` & `amsterdam-schema-tools-5.9.2/src/schematools/naming.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/permissions/auth.py` & `amsterdam-schema-tools-5.9.2/src/schematools/permissions/auth.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/permissions/db.py` & `amsterdam-schema-tools-5.9.2/src/schematools/permissions/db.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/provenance/create.py` & `amsterdam-schema-tools-5.9.2/src/schematools/provenance/create.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/types.py` & `amsterdam-schema-tools-5.9.2/src/schematools/types.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/utils.py` & `amsterdam-schema-tools-5.9.2/src/schematools/utils.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/src/schematools/validation.py` & `amsterdam-schema-tools-5.9.2/src/schematools/validation.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_ckan.py` & `amsterdam-schema-tools-5.9.2/tests/test_ckan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import json
 import re
 
-import json_encoder.json
 import pytest
 
 from schematools import ckan
 from schematools.types import DatasetSchema
 
 
 @pytest.mark.parametrize(
@@ -22,15 +22,15 @@
         "parkeervakken",
         "stadsdelen",
     ],
 )
 def test_convert(here, name):
     filename = here / f"files/datasets/{name}.json"
     with open(filename) as f:
-        schema = DatasetSchema.from_dict(json_encoder.json.load(f))
+        schema = DatasetSchema.from_dict(json.load(f))
 
     data = ckan.from_dataset(schema, name)
 
     for key in ["identifier", "title"]:
         assert data.get(key) and re.match(r"^[a-z0-9_-]", data[key])
     for key in ["language", "theme"]:
         assert isinstance(data.get(key), list) and data[key]
```

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_events_full.py` & `amsterdam-schema-tools-5.9.2/tests/test_events_full.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_geojson.py` & `amsterdam-schema-tools-5.9.2/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_import.py` & `amsterdam-schema-tools-5.9.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_indexes.py` & `amsterdam-schema-tools-5.9.2/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_loaders.py` & `amsterdam-schema-tools-5.9.2/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_naming.py` & `amsterdam-schema-tools-5.9.2/tests/test_naming.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_ndjson.py` & `amsterdam-schema-tools-5.9.2/tests/test_ndjson.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_permissions.py` & `amsterdam-schema-tools-5.9.2/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_permissions_auth.py` & `amsterdam-schema-tools-5.9.2/tests/test_permissions_auth.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_provenance.py` & `amsterdam-schema-tools-5.9.2/tests/test_provenance.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_types.py` & `amsterdam-schema-tools-5.9.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `amsterdam-schema-tools-5.9.1/tests/test_validation.py` & `amsterdam-schema-tools-5.9.2/tests/test_validation.py`

 * *Files identical despite different names*

