# Comparing `tmp/vectice-23.1.7.0.tar.gz` & `tmp/vectice-23.1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.1.7.0.tar", last modified: Mon Apr  3 08:14:04 2023, max compression
+gzip compressed data, was "vectice-23.1.7.2.tar", last modified: Thu Apr 13 14:28:23 2023, max compression
```

## Comparing `vectice-23.1.7.0.tar` & `vectice-23.1.7.2.tar`

### file list

```diff
@@ -1,119 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.234942 vectice-23.1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 08:13:55.000000 vectice-23.1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-03 08:14:04.234942 vectice-23.1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-03 08:13:55.000000 vectice-23.1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-03 08:13:55.000000 vectice-23.1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-03 08:14:04.234942 vectice-23.1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-03 08:13:55.000000 vectice-23.1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.218942 vectice-23.1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.222942 vectice-23.1.7.0/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.226942 vectice-23.1.7.0/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    25020 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.230942 vectice-23.1.7.0/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.230942 vectice-23.1.7.0/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.230942 vectice-23.1.7.0/src/vectice/models/datasource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.230942 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/file_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.234942 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.234942 vectice-23.1.7.0/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.234942 vectice-23.1.7.0/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    32481 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.234942 vectice-23.1.7.0/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-03 08:13:55.000000 vectice-23.1.7.0/src/vectice/utils/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 08:14:04.222942 vectice-23.1.7.0/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-03 08:14:04.000000 vectice-23.1.7.0/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-03 08:14:04.000000 vectice-23.1.7.0/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 08:14:04.000000 vectice-23.1.7.0/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-03 08:14:04.000000 vectice-23.1.7.0/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-03 08:14:04.000000 vectice-23.1.7.0/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.444666 vectice-23.1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 14:28:10.000000 vectice-23.1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-13 14:28:23.444666 vectice-23.1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 14:28:10.000000 vectice-23.1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-13 14:28:10.000000 vectice-23.1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 14:28:23.444666 vectice-23.1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-04-13 14:28:10.000000 vectice-23.1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.428666 vectice-23.1.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.428666 vectice-23.1.7.2/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.432666 vectice-23.1.7.2/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24867 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.436666 vectice-23.1.7.2/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.440666 vectice-23.1.7.2/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.440666 vectice-23.1.7.2/src/vectice/models/datasource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.440666 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/file_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.440666 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.440666 vectice-23.1.7.2/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.444666 vectice-23.1.7.2/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/metadata/dataframe_column_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33903 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.444666 vectice-23.1.7.2/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-13 14:28:10.000000 vectice-23.1.7.2/src/vectice/utils/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:28:23.432666 vectice-23.1.7.2/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-13 14:28:23.000000 vectice-23.1.7.2/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-13 14:28:23.000000 vectice-23.1.7.2/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:28:23.000000 vectice-23.1.7.2/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-13 14:28:23.000000 vectice-23.1.7.2/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 14:28:23.000000 vectice-23.1.7.2/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.1.7.0/LICENSE` & `vectice-23.1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/PKG-INFO` & `vectice-23.1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.1.7.0
+Version: 23.1.7.2
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.1.7.0/setup.py` & `vectice-23.1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         "requests>=2.5.0",
         "rich",
         "urllib3",
         "gql[requests]",
         "GitPython",
         "packaging",
         "Pillow",
+        "pandas",
     ],
     extras_require={
         "dev": [
             "black",
             "gitpython",
             "mypy",
             "ruff",
```

### Comparing `vectice-23.1.7.0/src/vectice/__init__.py` & `vectice-23.1.7.2/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/__init__.py` & `vectice-23.1.7.2/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/_auth.py` & `vectice-23.1.7.2/src/vectice/api/_auth.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/_utils.py` & `vectice-23.1.7.2/src/vectice/api/_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/attachment.py` & `vectice-23.1.7.2/src/vectice/api/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,21 @@
         entity_files = []
         try:
             url, model_repr = self._generate_model_url_and_id(model_version)
             if len(files) == 1:
                 response = self._post_attachments(url, files)
                 if response:
                     entity_files.append(response.json())
-                _logger.info(f"Attachment with name: {files[0][1][0]} successfully attached to {model_repr}.")
+                _logger.debug(f"Attachment with name: {files[0][1][0]} successfully attached to {model_repr}.")
             elif len(files) > 1:
                 for file in files:
                     response = self._post_attachments(url, [file])
                     if response:
                         entity_files.append(response.json())
-                _logger.info(
+                _logger.debug(
                     f"Attachments with names: {[f[1][0] for f in files]} successfully attached to {model_repr}."
                 )
             return entity_files
         except HttpError as e:
             self._handle_http_error(e, model_version)
 
     def post_model_predictor(self, model_type: str, model_content: BytesIO, model_version: ModelVersionOutput) -> None:
```

### Comparing `vectice-23.1.7.0/src/vectice/api/client.py` & `vectice-23.1.7.2/src/vectice/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 
         Returns:
             The workspace JSON structure.
         """
         return WorkspaceApi(self.auth).update_workspace(data, workspace)
 
     def list_workspaces(
-        self, search: str | None = None, page_index: int = 1, page_size: int = 20
+        self, search: str | None = None, page_index: int = 1, page_size: int = 100
     ) -> PagedResponse[WorkspaceOutput]:
         """List the workspaces.
 
         Parameters:
             search: A text to search for.
             page_index: The index of the page.
             page_size: The size of the page.
@@ -405,16 +405,17 @@
 
     def list_steps(
         self,
         phase_id: int,
         iteration_index: int | None = None,
         phase_name: str | None = None,
     ) -> list[StepOutput]:
-        if iteration_index:
+        if iteration_index is not None:
             return StepApi(self._gql_client, self.auth).list_steps_for_iteration(phase_id, iteration_index, phase_name)
+
         return StepApi(self._gql_client, self.auth).list_steps(phase_id, phase_name)
 
     def close_step(self, step_id: int, message: str | None = None) -> StepOutput:
         step_update = StepUpdateInput(text=message)
         return StepApi(self._gql_client, self.auth).close_step(step_id, step_update)
 
     def add_iteration_step_artifact(self, step_id: int, step_artifacts: IterationStepArtifactInput) -> StepOutput:
@@ -503,28 +504,25 @@
     def register_dataset(
         self,
         dataset_register_input: DatasetRegisterInput,
         project_id: int | None = None,
         phase_id: int | None = None,
         iteration_id: int | None = None,
     ) -> DatasetRegisterOutput:
-        try:
-            data: DatasetRegisterOutput = GqlDatasetApi(self._gql_client, self.auth).register_dataset(
-                dataset_register_input, project_id, phase_id, iteration_id
-            )
-            _logger.info(
-                f"Successfully registered Dataset("
-                f"name='{dataset_register_input.name}', "
-                f"id={data['datasetVersion']['id']}, "
-                f"version='{data['datasetVersion']['name']}', "
-                f"type={dataset_register_input.type})."
-            )
-            return data
-        except Exception as e:
-            raise ValueError(f"The dataset register failed due to {e}") from e
+        data: DatasetRegisterOutput = GqlDatasetApi(self._gql_client, self.auth).register_dataset(
+            dataset_register_input, project_id, phase_id, iteration_id
+        )
+        _logger.info(
+            f"Successfully registered Dataset("
+            f"name='{dataset_register_input.name}', "
+            f"id={data['datasetVersion']['id']}, "
+            f"version='{data['datasetVersion']['name']}', "
+            f"type={dataset_register_input.type})."
+        )
+        return data
 
     def get_project_and_workspace_references(
         self, project: str | int | None = None, workspace: str | int | None = None
     ):
         if project is None and self.project is not None:
             project = self.project.id
         if workspace is None and self.workspace is not None:
```

### Comparing `vectice-23.1.7.0/src/vectice/api/gql_api.py` & `vectice-23.1.7.2/src/vectice/api/gql_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,31 +25,17 @@
     from vectice.api._auth import Auth
 
 ResultType = TypeVar("ResultType")
 
 
 class Parser:
     def map_type(self, type_name: str) -> Type[ResultType]:
-        types_map = {
-            "Workspace": WorkspaceOutput,
-            "Project": ProjectOutput,
-            "Phase": PhaseOutput,
-            "IterationStep": StepOutput,
-            "Iteration": IterationOutput,
-            "DatasetRegisterResultOutput": DatasetRegisterOutput,
-            "ModelRegisterResultOutput": ModelRegisterOutput,
-            "UserActivity": UserActivity,
-            "Code": CodeOutput,
-            "CodeVersion": CodeVersionOutput,
-            "PublicConfigOutput": PublicConfigOutput,
-            "UserAndDefaultWorkspaceOutput": UserAndDefaultWorkspaceOutput,
-            "StepDefinition": StepOutput,
-        }
+        types_map = self._build_map()
         if type_name in types_map.keys():
-            return types_map[type_name]  # type: ignore[return-value]
+            return types_map[type_name]  # type: ignore[no-any-return]
         else:
             raise RuntimeError("Unknown type: " + type_name)
 
     def parse_item(self, item: dict[str, Any]) -> ResultType:  # type: ignore[type-var]
         clazz: Type[ResultType] = self.map_type(item["__typename"])
         result = clazz(**item)
         return result
@@ -69,14 +55,31 @@
             return self.parse_list(data)
         else:
             if "items" in data and "page" in data and "total" in data:
                 return self.parse_paged_response(data)
             else:
                 return self.parse_item(data)
 
+    def _build_map(self):
+        return {
+            "Workspace": WorkspaceOutput,
+            "Project": ProjectOutput,
+            "Phase": PhaseOutput,
+            "IterationStep": StepOutput,
+            "Iteration": IterationOutput,
+            "DatasetRegisterResultOutput": DatasetRegisterOutput,
+            "ModelRegisterResultOutput": ModelRegisterOutput,
+            "UserActivity": UserActivity,
+            "Code": CodeOutput,
+            "CodeVersion": CodeVersionOutput,
+            "PublicConfigOutput": PublicConfigOutput,
+            "UserAndDefaultWorkspaceOutput": UserAndDefaultWorkspaceOutput,
+            "StepDefinition": StepOutput,
+        }
+
 
 class GqlApi:
     def __init__(self, client: Client, auth: Auth):
         self.client = client
         self.auth = auth
         self._error_handler = ClientErrorHandler()
```

### Comparing `vectice-23.1.7.0/src/vectice/api/gql_code.py` & `vectice-23.1.7.2/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/gql_code_version.py` & `vectice-23.1.7.2/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/gql_dataset.py` & `vectice-23.1.7.2/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/gql_model.py` & `vectice-23.1.7.2/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.1.7.2/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/http_error.py` & `vectice-23.1.7.2/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/http_error_handlers.py` & `vectice-23.1.7.2/src/vectice/api/http_error_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             status_code = -1
         if status_code == 404:
             raise BadReferenceFactory.get_reference(reference_type, reference)
         elif status_code == 401:
             raise ConnectionRefusedError(BAD_OR_MISSING_CREDENTIALS_ERROR_MESSAGE)
         elif status_code == 403:
             raise PermissionError(f"Missing rights to access this {reference_type}")
-        elif status_code == 400:
+        elif status_code == 400 or status_code == 412:
             # backend always adds a "message" to the response
             message = error.errors[0]["message"]  # type: ignore
             raise VecticeException(f"{reference_type}: {message}")
         raise self._graphql_error_formatter(error) from error
 
 
 class BadReferenceFactory:
```

### Comparing `vectice-23.1.7.0/src/vectice/api/iteration.py` & `vectice-23.1.7.2/src/vectice/api/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/__init__.py` & `vectice-23.1.7.2/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/artifact_version.py` & `vectice-23.1.7.2/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/code.py` & `vectice-23.1.7.2/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/code_version.py` & `vectice-23.1.7.2/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/dataset_register.py` & `vectice-23.1.7.2/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/files_metadata.py` & `vectice-23.1.7.2/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/iteration.py` & `vectice-23.1.7.2/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/last_assets.py` & `vectice-23.1.7.2/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/metric.py` & `vectice-23.1.7.2/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/model.py` & `vectice-23.1.7.2/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/model_register.py` & `vectice-23.1.7.2/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/model_version.py` & `vectice-23.1.7.2/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/paged_response.py` & `vectice-23.1.7.2/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/phase.py` & `vectice-23.1.7.2/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/project.py` & `vectice-23.1.7.2/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/property.py` & `vectice-23.1.7.2/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/public_config.py` & `vectice-23.1.7.2/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/step.py` & `vectice-23.1.7.2/src/vectice/api/json/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/json/workspace.py` & `vectice-23.1.7.2/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/last_assets.py` & `vectice-23.1.7.2/src/vectice/api/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/phase.py` & `vectice-23.1.7.2/src/vectice/api/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/project.py` & `vectice-23.1.7.2/src/vectice/api/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/rest_api.py` & `vectice-23.1.7.2/src/vectice/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/step.py` & `vectice-23.1.7.2/src/vectice/api/step.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/version.py` & `vectice-23.1.7.2/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/api/workspace.py` & `vectice-23.1.7.2/src/vectice/api/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             return WorkspaceOutput(**response)
         except HttpError as e:
             self._httpErrorHandler.handle_get_http_error(e, "workspace", workspace)
         except TypeError as error:
             raise ValueError(INVALID_WORKSPACE_MESSAGE) from error
 
     def list_workspaces(
-        self, search: str | None = None, page_index: int = 1, page_size: int = 20
+        self, search: str | None = None, page_index: int = 1, page_size: int = 100
     ) -> PagedResponse[WorkspaceOutput]:
         if search is None or search == "":
             url = f"/metadata/workspace?index={page_index}&size={page_size}"
         else:
             url = f"/metadata/workspace?index={page_index}&size={page_size}&search={search}"
         workspaces = self.get(url)
         return PagedResponse(
```

### Comparing `vectice-23.1.7.0/src/vectice/connection.py` & `vectice-23.1.7.2/src/vectice/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         rich_table.add_column("description", justify="left", no_wrap=True, max_width=50)
 
         for count, workspace in enumerate(workspace_outputs, 1):
             if count > 10:
                 break
             rich_table.add_row(str(workspace.id), workspace.name, format_description(workspace.description))
 
-        description = f"""There are {len(workspace_outputs)} workspaces for user {user_name}."""
+        description = f"""There are {len(workspace_outputs)} workspaces."""
         tips = dedent(
             """
         >> To access your personal workspace, use connection.my_workspace or connect.workspaces[0]
         >> To access a specific workspace, use connection.workspace(Workspace ID)"""
         ).lstrip()
         link = dedent(
             f"""
```

### Comparing `vectice-23.1.7.0/src/vectice/models/__init__.py` & `vectice-23.1.7.2/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/attachment_container.py` & `vectice-23.1.7.2/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/dataset.py` & `vectice-23.1.7.2/src/vectice/models/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from __future__ import annotations
 
 from datetime import datetime
 
+from pandas import DataFrame
+
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
+from vectice.models.resource.metadata.files_metadata import File
 
 
 class Dataset:
     def __init__(
         self,
         type: DatasetType,
         name: str | None = None,
         resource: Resource | None = None,
         training_resource: Resource | None = None,
         testing_resource: Resource | None = None,
         validation_resource: Resource | None = None,
         derived_from: list[int | Dataset] | None = None,
+        dataframe: DataFrame | None = None,
+        training_dataframe: DataFrame | None = None,
+        testing_dataframe: DataFrame | None = None,
+        validation_dataframe: DataFrame | None = None,
         # attachments: str | list[str] | None = None,
         # properties: dict[str, str | int] | list[Property] | Property | None = None,
     ):
         """Initialize a dataset.
 
         Users should not instantiate a dataset directly but rather use the provided static methods
         [`origin()`][vectice.models.dataset.Dataset.origin],
@@ -30,14 +37,18 @@
             type: The type of dataset.
             name: The name of the dataset.
             resource: A single resource (for origin and clean datasets).
             training_resource: The resource for the training set (for modeling datasets).
             testing_resource: The resource for the testing set (for modeling datasets).
             validation_resource: The resource for the validation set (optional, for modeling datasets).
             derived_from: A list of datasets (or ids) from which this dataset is derived.
+            dataframe: A pandas dataframe for clean and origin datasets.
+            training_dataframe: A pandas dataframe for modeling dataset.
+            testing_dataframe: A pandas dataframe for modeling dataset.
+            validation_dataframe: A pandas dataframe for modeling dataset.
         """
         derived_from_ids = []
         for df in derived_from or []:
             if isinstance(df, Dataset):
                 if df.latest_version_id is None:
                     raise ValueError(
                         f"Dataset '{df.name}' does not have a version id. "
@@ -50,29 +61,41 @@
         self._name = name or f"dataset {datetime.time}"
         self._resource = resource
         self._training_resource = training_resource
         self._testing_resource = testing_resource
         self._validation_resource = validation_resource
         self._derived_from = derived_from_ids
         self._latest_version_id: int | None = None
+
         # self._properties = self._format_properties(properties) if properties else None
         # self._attachments = self._format_attachments(attachments) if attachments else None
 
         if self._type is DatasetType.MODELING:
             if self._training_resource is None or self._testing_resource is None:
                 raise ValueError("You cannot create a modeling dataset without both training and testing sets")
+
             self._training_resource.usage = DatasetSourceUsage.TRAINING
             self._testing_resource.usage = DatasetSourceUsage.TESTING
             if self._validation_resource:
                 self._validation_resource.usage = DatasetSourceUsage.VALIDATION
 
+        self._fill_file_dataframe(
+            [
+                (resource, dataframe, "dataframe"),
+                (training_resource, training_dataframe, "training_dataframe"),
+                (testing_resource, testing_dataframe, "testing_dataframe"),
+                (validation_resource, validation_dataframe, "validation_dataframe"),
+            ]
+        )
+
     @staticmethod
     def origin(
         resource: Resource,
         name: str | None = None,
+        dataframe: DataFrame | None = None,
         # properties: dict[str, str | int] | list[Property] | Property | None = None,
         # attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create an origin dataset.
 
         Examples:
             ```python
@@ -83,28 +106,31 @@
                 resource=FileResource(path="origin_dataset.csv"),
             )
             ```
 
         Parameters:
             resource: The resource for the origin dataset.
             name: The name of the dataset.
+            dataframe: A pandas dataframe allowing vectice to compute more metadata about this dataset.
         """
         return Dataset(
             type=DatasetType.ORIGIN,
             name=name,
             resource=resource,
+            dataframe=dataframe,
             # properties=properties,
             # attachments=attachments,
         )
 
     @staticmethod
     def clean(
         resource: Resource,
         name: str | None = None,
         derived_from: list[int | Dataset] | None = None,
+        dataframe: DataFrame | None = None,
         # properties: dict[str, str | int] | list[Property] | Property | None = None,
         # attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create a clean dataset.
 
         Examples:
             ```python
@@ -116,30 +142,35 @@
             )
             ```
 
         Parameters:
             resource: The resource for the clean dataset.
             name: The name of the dataset.
             derived_from: A list of datasets (or ids) from which this dataset is derived.
+            dataframe: A pandas dataframe allowing vectice to compute more metadata about this dataset.
         """
         return Dataset(
             type=DatasetType.CLEAN,
             name=name,
             resource=resource,
             derived_from=derived_from,
+            dataframe=dataframe,
             # properties=properties,
             # attachments=attachments,
         )
 
     @staticmethod
     def modeling(
         training_resource: Resource,
         testing_resource: Resource,
         validation_resource: Resource | None = None,
         name: str | None = None,
+        training_dataframe: DataFrame | None = None,
+        testing_dataframe: DataFrame | None = None,
+        validation_dataframe: DataFrame | None = None,
         # properties: dict[str, str | int] | list[Property] | Property | None = None,
         # attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create a modeling dataset.
 
         Examples:
             ```python
@@ -154,21 +185,27 @@
             ```
 
         Parameters:
             training_resource: The resource for the training set (for modeling datasets).
             testing_resource: The resource for the testing set (for modeling datasets).
             validation_resource: The resource for the validation set (optional, for modeling datasets).
             name: The name of the dataset.
+            training_dataframe: A pandas dataframe allowing vectice to compute more metadata about the training set.
+            testing_dataframe: A pandas dataframe allowing vectice to compute more metadata about the testing set.
+            validation_dataframe: A pandas dataframe allowing vectice to compute more metadata about the validation set.
         """
         return Dataset(
             type=DatasetType.MODELING,
             name=name,
             training_resource=training_resource,
             testing_resource=testing_resource,
             validation_resource=validation_resource,
+            training_dataframe=training_dataframe,
+            testing_dataframe=testing_dataframe,
+            validation_dataframe=validation_dataframe,
             # properties=properties,
             # attachments=attachments,
         )
 
     def __repr__(self):
         return f"Dataset(name={self.name!r}, type={self.type!r})"
 
@@ -299,7 +336,27 @@
     # @staticmethod
     # def _remove_incorrect_properties(properties: list[Property]) -> list[Property]:
     #     for prop in properties:
     #         if not isinstance(prop, Property):
     #             logging.warning(f"Incorrect property '{prop}'. Please check property type.")
     #             properties.remove(prop)
     #     return properties
+
+    def _fill_file_dataframe(self, resources: list[tuple[Resource | None, DataFrame | None, str]]):
+        for resource, dataframe, arg in resources:
+            if dataframe is not None and not isinstance(dataframe, DataFrame):
+                raise ValueError(
+                    f"Argument '{arg}' of type '{type(dataframe)}' is invalid, only pandas DataFrame is supported."
+                )
+            if resource is not None and dataframe is not None:
+                file = self._get_latest_file(resource=resource)
+                if file is not None:
+                    file._dataframe = dataframe
+
+    def _get_latest_file(self, resource: Resource) -> File | None:
+        latest_file = None
+        latest_date = None
+        for file in resource.metadata.files:
+            if latest_date is None or file.updated_date > latest_date:
+                latest_file = file
+                latest_date = file.updated_date
+        return latest_file
```

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/__init__.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/data_wrapper.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/file_data_wrapper.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/file_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/gcs_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/__init__.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/files_metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 from __future__ import annotations
 
+from typing import Any
+
 from vectice.models.resource.metadata.base import (
     DatasetSourceOrigin,
     DatasetSourceType,
     DatasetSourceUsage,
-    DatasetType,
     Metadata,
 )
-from vectice.models.resource.metadata.db_metadata import Column, DBMetadata, MetadataDB
-from vectice.models.resource.metadata.files_metadata import File, FilesMetadata
+from vectice.models.resource.metadata.files_metadata import (
+    File,
+    FilesMetadata,
+)
 from vectice.utils.deprecation import deprecate
 
-__all__ = [
-    "DBMetadata",
-    "Column",
-    "MetadataDB",
-    "DatasetSourceOrigin",
-    "DatasetSourceUsage",
-    "DatasetSourceType",
-    "DatasetType",
-    "File",
-    "FilesMetadata",
-    "Metadata",
-]
+
+def __getattr__(name: str) -> Any:
+    attrs = {
+        "DatasetSourceOrigin": DatasetSourceOrigin,
+        "DatasetSourceType": DatasetSourceType,
+        "DatasetSourceUsage": DatasetSourceUsage,
+        "Metadata": Metadata,
+        "FilesMetadata": FilesMetadata,
+        "File": File,
+    }
+
+    if name in attrs:
+        return attrs[name]
+
+    raise AttributeError(f"'{__name__}' module has no attribute '{name}'")
 
 
 @deprecate(
     warn_at="23.1",
     fail_at="23.3",
     remove_at="23.4",
-    reason="The `vectice.models.datasource.datawrapper.metadata` module "
-    "is deprecated in favor the `vectice.models.resource.metadata` module. "
+    reason="The `vectice.models.datasource.datawrapper.metadata.files_metadata` module "
+    "is deprecated in favor the `vectice.models.resource.metadata.files_metadata` module. "
     "Importing from the deprecated module will fail in v{fail_at}, "
     "and the module will be removed in v{remove_at}.",
 )
 def _warn() -> None:
     pass
```

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/db_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 
 from vectice.models.resource.metadata.base import (
     DatasetSourceOrigin,
     DatasetSourceType,
     DatasetSourceUsage,
     Metadata,
 )
+from vectice.models.resource.metadata.column_metadata import DBColumn
 from vectice.models.resource.metadata.db_metadata import (
-    Column,
     DBMetadata,
     MetadataDB,
 )
 from vectice.utils.deprecation import deprecate
 
 
 def __getattr__(name: str) -> Any:
     attrs = {
         "DatasetSourceOrigin": DatasetSourceOrigin,
         "DatasetSourceType": DatasetSourceType,
         "DatasetSourceUsage": DatasetSourceUsage,
         "Metadata": Metadata,
         "DBMetadata": DBMetadata,
-        "Column": Column,
+        "DBColumn": DBColumn,
         "MetadataDB": MetadataDB,
     }
 
     if name in attrs:
         return attrs[name]
 
     raise AttributeError(f"'{__name__}' module has no attribute '{name}'")
```

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/metadata/metadata.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py` & `vectice-23.1.7.2/src/vectice/models/datasource/datawrapper/s3_data_wrapper.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/git_version.py` & `vectice-23.1.7.2/src/vectice/models/git_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/iteration.py` & `vectice-23.1.7.2/src/vectice/models/iteration.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,15 +323,15 @@
         if not steps_output:
             rich_table.add_row(
                 None,
                 None,
                 None,
                 None,
             )
-        description = f"""There are {len(steps_output)} steps in the iteration {self.index} for user {user_name}."""
+        description = f"""There are {len(steps_output)} steps in iteration {self.index!r}."""
         tips = dedent(
             """
         >> To access a specific step, use iteration.step(Step ID)
         >> To access an array of steps, use iteration.steps"""
         ).lstrip()
         link = dedent(
             f"""
```

### Comparing `vectice-23.1.7.0/src/vectice/models/metric.py` & `vectice-23.1.7.2/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/model.py` & `vectice-23.1.7.2/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/phase.py` & `vectice-23.1.7.2/src/vectice/models/phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -203,31 +203,28 @@
 
     def list_step_definitions(self) -> None:
         """List the step definitions to which this phase has access and print the step definitions in a tabular format.
 
         Returns:
             None
         """
-        steps_output = self._client.list_step_definitions(self.id)
+        steps_output = sorted(self._client.list_step_definitions(self.id), key=lambda x: x.index)
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
         rich_table = Table(expand=True, show_edge=False)
 
-        rich_table.add_column("step def. id", justify="left", no_wrap=True, min_width=5, max_width=5)
+        rich_table.add_column("shortcut", justify="left", no_wrap=True, min_width=3, max_width=20)
         rich_table.add_column("name", justify="left", no_wrap=True, min_width=5, max_width=10)
         rich_table.add_column("description", justify="left", no_wrap=True, min_width=3, max_width=15)
-        rich_table.add_column("shortcut", justify="left", no_wrap=True, min_width=3, max_width=20)
 
-        for count, step in enumerate(reversed(steps_output), 1):
+        for count, step in enumerate(steps_output, 1):
             if count > 10:
                 break
-            rich_table.add_row(str(step.id), f"{count}. {step.name}", format_description(step.description), step.slug)
-        description = (
-            f"""There are {len(steps_output)} step definitions in the phase {self.name} for user {user_name}."""
-        )
+            rich_table.add_row(step.slug, step.name, format_description(step.description))
+        description = f"""There are {len(steps_output)} steps required in the phase {self.name!r}."""
         link = dedent(
             f"""
         For quick access to the list of step definitions in the Vectice web app, visit:
         {self._client.auth._API_BASE_URL}/project/phase/steps?w={self.workspace.id}&pageId={self.id}"""
         ).lstrip()
         _temp_print(description)
         _temp_print(table=rich_table)
@@ -245,15 +242,16 @@
         Returns:
             An iteration.
         """
         if index:
             iteration_output = self._client.get_iteration_by_index(self.id, index)
         else:
             iteration_output = self._client.create_iteration(self.id)
-        _logger.debug(f"Iteration number {iteration_output.index} (id {iteration_output.id}) successfully retrieved.")
+            _logger.info(f"New Iteration number {iteration_output.index!r} created.")
+        _logger.info(f"Iteration number {iteration_output.index!r} successfully retrieved.")
         iteration_object = Iteration(
             id=iteration_output.id,
             index=iteration_output.index,
             phase=self,
             status=iteration_output.status,
         )
         self._current_iteration = iteration_object
```

### Comparing `vectice-23.1.7.0/src/vectice/models/project.py` & `vectice-23.1.7.2/src/vectice/models/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         Parameters:
             phase: The name or id of the phase to get.
 
         Returns:
             The specified phase.
         """
         item = self._client.get_phase(phase, project_id=self._id)
-        _logger.debug(f"Phase with id: {item.id} successfully retrieved.")
+        _logger.info(f"Phase {item.name!r} successfully retrieved.")
         phase_object = Phase(item.id, self, item.name, item.index, item.status)
         self._phase = phase_object
         return phase_object
 
     def list_phases(self) -> None:
         """List the phases to which this project has access and print the phases in a tabular format.
 
@@ -216,15 +216,15 @@
                 str(phase.id),
                 phase.name,
                 phase_owner,
                 phase_status,
                 f"{active_iterations}/{iterations_total}",
                 str(total_phase_steps),
             )
-        description = f"""There are {len(phase_outputs)} phases in the project {self.name} for user {user_name}."""
+        description = f"""There are {len(phase_outputs)} phases in the project {self.name!r}."""
         tips = dedent(
             """
         >> To access a specific phase, use project.phase(PhaseID)
         >> To access an array of phases, use project.phases"""
         ).lstrip()
         link = dedent(
             f"""
```

### Comparing `vectice-23.1.7.0/src/vectice/models/property.py` & `vectice-23.1.7.2/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/__init__.py` & `vectice-23.1.7.2/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/base.py` & `vectice-23.1.7.2/src/vectice/models/resource/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/description.py` & `vectice-23.1.7.2/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/file_resource.py` & `vectice-23.1.7.2/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/gcs_resource.py` & `vectice-23.1.7.2/src/vectice/models/resource/gcs_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.1.7.2/src/vectice/models/resource/metadata/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from vectice.models.resource.metadata.base import (
     DatasetSourceOrigin,
     DatasetSourceType,
     DatasetSourceUsage,
     DatasetType,
     Metadata,
 )
-from vectice.models.resource.metadata.db_metadata import Column, DBMetadata, MetadataDB
+from vectice.models.resource.metadata.column_metadata import Column, DBColumn
+from vectice.models.resource.metadata.db_metadata import DBMetadata, MetadataDB
 from vectice.models.resource.metadata.files_metadata import File, FilesMetadata
 
 __all__ = [
     "DBMetadata",
     "Column",
+    "DBColumn",
     "MetadataDB",
     "DatasetSourceOrigin",
     "DatasetSourceUsage",
     "DatasetSourceType",
     "DatasetType",
     "File",
     "FilesMetadata",
```

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/metadata/base.py` & `vectice-23.1.7.2/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.1.7.2/src/vectice/models/resource/metadata/column_metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,99 @@
 from __future__ import annotations
 
-from vectice.models.resource.metadata.base import (
-    DatasetSourceType,
-    DatasetSourceUsage,
-    Metadata,
-)
+from dataclasses import dataclass
 
+import numpy as np
 
-class DBMetadata(Metadata):
-    """Class that describes metadata of dataset that comes from a database."""
+
+@dataclass
+class StatValue:
+    """Model a key-value pair of a column statistic.
+
+    Parameters:
+        key: The key to identify the statistic.
+        value: The value of the statistic.
+    """
+
+    key: str
+    value: int | float | str
+
+    def __post_init__(self):
+        if isinstance(self.value, np.generic):
+            self.value = self.value.item()
+        if not isinstance(self.value, (int, float, str)):
+            raise TypeError(
+                f"StatValue '{self.key}' value must have type float, integer or string, not {type(self.value).__name__}."
+            )
+
+    def __repr__(self):
+        return f"StatValue(key={self.key!r}, value={self.value!r})"
+
+
+class Column:
+    """Model a column of a dataset."""
 
     def __init__(
         self,
-        dbs: list[MetadataDB],
-        size: int,
-        usage: DatasetSourceUsage | None = None,
-        origin: str | None = None,
+        name: str,
+        data_type: str,
+        stats: list[StatValue] | None = None,
     ):
-        """Initialize a DBMetadata instance.
+        """Initialize a column.
 
         Parameters:
-            dbs: The list of databases.
-            size: The size of the metadata.
-            usage: The usage of the metadata.
-            origin: The origin of the metadata.
+            name: The name of the column.
+            data_type: The type of the data contained in the column.
+            stats: Additional statistics about the column.
         """
-        super().__init__(size=size, type=DatasetSourceType.DB, usage=usage, origin=origin)
-        self.dbs = dbs
+        self.name = name
+        self.data_type = data_type
+        self.stats = stats
 
     def asdict(self) -> dict:
         return {
-            "dbs": [db.asdict() for db in self.dbs],
-            "size": self.size,
-            "filesCount": None,
-            "files": [],
-            "type": self.type.value,
-            "usage": self.usage.value if self.usage else None,
-            "origin": self.origin,
+            "name": self.name,
+            "dataType": self.data_type,
+            "stats": [vars(stat) for stat in self.stats or []],
         }
 
 
-class Column:
+class DBColumn(Column):
     """Model a column of a dataset, like a database column."""
 
     def __init__(
         self,
         name: str,
         data_type: str,
         is_unique: bool | None = None,
         nullable: bool | None = None,
         is_private_key: bool | None = None,
         is_foreign_key: bool | None = None,
+        stats: list[StatValue] | None = None,
     ):
         """Initialize a column.
 
         Parameters:
             name: The name of the column.
             data_type: The type of the data contained in the column.
             is_unique: If the column uniquely defines a record.
             nullable: If the column can contain null value.
             is_private_key: If the column uniquely defines a record,
                 individually or with other columns (can be null).
             is_foreign_key: If the column refers to another one,
                 individually or with other columns (cannot be null).
+            stats: Additional statistics about the column.
         """
-        self.name = name
-        self.data_type = data_type
+        super().__init__(name, data_type, stats)
         self.is_unique = is_unique
         self.nullable = nullable
         self.is_private_key = is_private_key
         self.is_foreign_key = is_foreign_key
 
     def asdict(self) -> dict:
         return {
-            "name": self.name,
-            "dataType": self.data_type,
+            **super().asdict(),
             "isUnique": self.is_unique,
             "nullable": self.nullable,
             "isPK": self.is_private_key,
             "isFK": self.is_foreign_key,
         }
-
-
-class MetadataDB:
-    def __init__(self, name: str, columns: list[Column], rows_number: int, size: int | None = None):
-        """Initialize a MetadataDB instance.
-
-        Parameters:
-            name: The name of the table.
-            columns: The columns that compose the table.
-            rows_number: The number of row of the table.
-            size: The size of the table.
-        """
-        self.name = name
-        self.size = size
-        self.rows_number = rows_number
-        self.columns = columns
-
-    def asdict(self) -> dict:
-        return {
-            "name": self.name,
-            "size": self.size,
-            "rowsNumber": self.rows_number,
-            "columns": [column.asdict() for column in self.columns],
-        }
```

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.1.7.2/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
+from pandas import DataFrame
+
 from vectice.models.resource.metadata.base import (
     DatasetSourceType,
     DatasetSourceUsage,
     Metadata,
 )
+from vectice.models.resource.metadata.column_metadata import Column
+from vectice.models.resource.metadata.dataframe_column_parser import capture_columns
 
 
 class FilesMetadata(Metadata):
     """The metadata of a set of files."""
 
     def __init__(
         self,
@@ -45,34 +49,41 @@
         self,
         name: str,
         size: int,
         fingerprint: str,
         created_date: str | None = None,
         updated_date: str | None = None,
         uri: str | None = None,
+        columns: list[Column] | None = None,
+        dataframe: DataFrame | None = None,
     ):
         """Initialize a file.
 
         Parameters:
             name: The name of the file.
             size: The size of the file.
             fingerprint: The hash of the file.
             created_date: The date of creation of the file.
             updated_date: The date of last update of the file.
             uri: The uri of the file.
+            columns: The columns coming from the dataframe with the statistics.
+            dataframe: A pandas dataframe which will capture the files metadata.
         """
         self.name = name
         self.size = size
         self.fingerprint = fingerprint
         self.created_date = created_date
         self.updated_date = updated_date
         self.uri = uri
+        self.columns = columns
+        self._dataframe = dataframe
 
     def asdict(self) -> dict:
         return {
             "name": self.name,
             "size": self.size,
             "fingerprint": self.fingerprint,
             "createdDate": self.created_date,
             "updatedDate": self.updated_date,
             "uri": self.uri,
+            "columns": capture_columns(init_columns=self.columns, dataframe=self._dataframe),
         }
```

### Comparing `vectice-23.1.7.0/src/vectice/models/resource/s3_resource.py` & `vectice-23.1.7.2/src/vectice/models/resource/s3_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/step.py` & `vectice-23.1.7.2/src/vectice/models/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 from vectice.api.http_error_handlers import VecticeException
 from vectice.api.json.iteration import (
     IterationStatus,
     IterationStepArtifact,
     IterationStepArtifactInput,
     IterationStepArtifactType,
 )
+from vectice.api.json.model_register import ModelRegisterOutput
 from vectice.api.json.model_version import ModelVersionOutput
 from vectice.api.json.step import StepType
 from vectice.models.attachment_container import AttachmentContainer
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata import DatasetType
 from vectice.utils.automatic_link_utils import (
     existing_dataset_logger,
     existing_model_logger,
     link_assets_to_step,
     link_dataset_to_step,
     wrapper_to_dataset,
 )
 from vectice.utils.common_utils import _check_image_path, _check_read_only, _get_image_variables
 from vectice.utils.deprecation import deprecate
+from vectice.utils.last_assets import _register_dataset_logging, _register_model_logging
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.models import Iteration, Phase, Project, Workspace
     from vectice.models.dataset import Dataset
     from vectice.models.datasource.datawrapper.data_wrapper import DataWrapper
     from vectice.models.model import Model
@@ -208,14 +210,15 @@
         self, value: Dataset | Model | int | float | str | None = None
     ) -> Step | StepString | StepNumber | StepDataset:
         # TODO cyclic imports
         from vectice.models.dataset import Dataset
         from vectice.models.model import Model
         from vectice.models.step_dataset import StepDataset
         from vectice.models.step_image import StepImage
+        from vectice.models.step_model import StepModel
         from vectice.models.step_number import StepNumber
         from vectice.models.step_string import StepString
 
         if isinstance(value, (int, float)):
             self._update_iteration_step(StepType.StepNumber, value)
             return StepNumber(step=self, number=value)
 
@@ -230,55 +233,84 @@
             return StepImage(self, value)
 
         if isinstance(value, str):
             self._update_iteration_step(StepType.StepString, value)
             return StepString(self, string=value)
 
         if isinstance(value, Model):
-            self._client.update_iteration_step_artifact(
+            code_version_id = self._get_code_version_id()
+            data = self._client.register_model(
+                model=value,
+                project_id=self.project.id,
+                phase_id=self.phase.id,
+                iteration_id=self.iteration.id,
+                code_version_id=code_version_id,
+            )
+            attachments_output = self._set_model_attachments(value, data.model_version)
+
+            artifacts = self._get_model_artifacts(data, attachments_output)
+            step_output = self._client.update_iteration_step_artifact(
                 self.id,
                 StepType.StepModel,
+                None,
+                artifacts,
             )
+            _register_model_logging(self, data, value, self.name, attachments_output, _logger)
+            self.artifacts = [IterationStepArtifact(modelVersionId=step_output.id, type="ModelVersion")]
             self._warn_step_change(value)
-            self.model = value
-            step = self._refresh_step()
-            step._model = value
-            return step
+            return StepModel(self, self.artifacts[0], value)
 
         if isinstance(value, Dataset):
             code_version_id = self._get_code_version_id()
             data = self._client.register_dataset_from_source(
                 dataset=value,
                 project_id=self.project.id,
                 phase_id=self.phase.id,
                 iteration_id=self.iteration.id,
                 code_version_id=code_version_id,
             )
-            existing_dataset_logger(data, value.name, _logger)
             artifacts = [
                 IterationStepArtifactInput(
                     id=data["datasetVersion"]["id"],
                     type=IterationStepArtifactType.DataSetVersion.name,
                 )
             ]
             step_output = self._client.update_iteration_step_artifact(
                 self.id,
                 StepType.StepDataset,
                 None,
                 artifacts,
             )
-            _logger.info(
-                f"Successfully added Dataset(name='{value.name}', id={data['datasetVersion']['id']}, version='{data['datasetVersion']['name']}', type=MODELING) to {step_output.name}"
-            )
+
+            _register_dataset_logging(self, data, value, step_output, _logger)
             self.artifacts = [IterationStepArtifact(datasetVersionId=step_output.id, type="DataSetVersion")]
             self._warn_step_change(value)
             return StepDataset(self, dataset_version=step_output.artifacts[0])
 
         return self
 
+    def _get_model_artifacts(
+        self, data: ModelRegisterOutput, attachments_output: list[dict] | None = None
+    ) -> list[IterationStepArtifactInput]:
+        attachments = None
+        if attachments_output:
+            attachments = (
+                [IterationStepArtifactInput(id=attach["fileId"], type="EntityFile") for attach in attachments_output]
+                if attachments_output
+                else None
+            )
+        artifacts = [
+            IterationStepArtifactInput(
+                id=data["modelVersion"]["id"],
+                type=IterationStepArtifactType.ModelVersion.name,
+            )
+        ]
+        artifacts += attachments if attachments else []
+        return artifacts
+
     def _create_image_artifact(self, value: str | IOBase | Image) -> tuple[list[IterationStepArtifactInput], str]:
         image, filename = _get_image_variables(value)
         try:
             attachments_output = self._client.create_phase_attachments(
                 [("file", (filename, image))], self.phase.id, self.project.id
             )
             return [
@@ -340,23 +372,23 @@
         # TODO: cyclic import
         from vectice.models.dataset import Dataset
         from vectice.models.model import Model
 
         if self._type is StepType.Step:
             return
         elif self._type is not StepType.StepModel and isinstance(value, Model):
-            _logger.info(f"Step type changed from {self._type.name} to StepModel")
+            _logger.debug(f"Step type changed from {self._type.name} to StepModel")
         elif self._type is not StepType.StepDataset and isinstance(value, Dataset):
-            _logger.info(f"Step type changed from {self._type.name} to StepDataset")
+            _logger.debug(f"Step type changed from {self._type.name} to StepDataset")
         elif self._type is not StepType.StepImage and StepType.StepImage is value:
-            _logger.info(f"Step type changed from {self._type.name} to StepImage")
+            _logger.debug(f"Step type changed from {self._type.name} to StepImage")
         elif self._type is not StepType.StepNumber and isinstance(value, (int, float)):
-            _logger.info(f"Step type changed from {self._type.name} to StepNumber")
+            _logger.debug(f"Step type changed from {self._type.name} to StepNumber")
         elif self._type is not StepType.StepString and isinstance(value, str):
-            _logger.info(f"Step type changed from {self._type.name} to StepString")
+            _logger.debug(f"Step type changed from {self._type.name} to StepString")
 
     @property
     def name(self) -> str:
         """The step's name.
 
         Returns:
             The step's name.
```

### Comparing `vectice-23.1.7.0/src/vectice/models/step_dataset.py` & `vectice-23.1.7.2/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/step_image.py` & `vectice-23.1.7.2/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/step_number.py` & `vectice-23.1.7.2/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/step_string.py` & `vectice-23.1.7.2/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/models/workspace.py` & `vectice-23.1.7.2/src/vectice/models/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         rich_table.add_column("description", justify="left", no_wrap=True, max_width=50)
 
         for count, project in enumerate(project_outputs, 1):
             if count > 10:
                 break
             rich_table.add_row(str(project.id), project.name, format_description(project.description))
 
-        description = f"""There are {len(project_outputs)} projects for user {user_name}."""
+        description = f"""There are {len(project_outputs)} projects in the workspace {self.name!r}."""
         tips = dedent(
             """
         >> To access a specific project, use workspace.project(Project ID)
         >> To access an array of projects, use workspace.projects"""
         ).lstrip()
         link = dedent(
             f"""
```

### Comparing `vectice-23.1.7.0/src/vectice/utils/automatic_link_utils.py` & `vectice-23.1.7.2/src/vectice/utils/automatic_link_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,25 +13,31 @@
 if TYPE_CHECKING:
     from logging import Logger
 
     from vectice.models import Step
     from vectice.models.resource.base import Resource
 
 
-def existing_dataset_logger(data: dict, dataset_name: str, _logger: Logger):
+def existing_dataset_logger(data: dict, dataset_name: str, _logger: Logger) -> str | None:
+    """Identifies if the dataset and it's version exists already."""
     if data["useExistingDataset"]:
         existing_dataset_version = f"Dataset: {dataset_name}"
         if data["useExistingVersion"]:
             existing_dataset_version += f" with Version: {data['datasetVersion']['name']}"
         _logger.debug(f"{existing_dataset_version} already exists.")
+        return existing_dataset_version
+    return None
 
 
 def existing_model_logger(data: dict, model_name: str, _logger: Logger):
     if data["useExistingModel"]:
-        _logger.info(f"Model: {model_name} already exists.")
+        existing_model = f"Model: {model_name} already exists."
+        _logger.debug(existing_model)
+        return existing_model
+    return
 
 
 def link_dataset_to_step(
     step_artifact: IterationStepArtifactInput,
     dataset: Dataset,
     data: dict,
     _logger: Logger,
```

### Comparing `vectice-23.1.7.0/src/vectice/utils/common_utils.py` & `vectice-23.1.7.2/src/vectice/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/utils/configuration.py` & `vectice-23.1.7.2/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/utils/deprecation.py` & `vectice-23.1.7.2/src/vectice/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.1.7.0/src/vectice/utils/logging_utils.py` & `vectice-23.1.7.2/src/vectice/utils/logging_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,25 @@
 
 If you are using a notebook you can call the help by using a Vectice returned object with the builtin notebook "?":
 >> connection?
 
 If you are using an IDE you can call the help() method on any object returned by Vectice:
 >> help(connection)
 
-For quick access to the list of workspaces in the Vectice web app, visit:
-{url}"""
+{logging_output}"""
 
-CONNECTION_WORKSPACE_LOGGING = """Welcome, {user}. You`re now successfully connected to the workspace {workspace_name} in Vectice.
+CONNECTION_WORKSPACE_LOGGING = """Welcome, {user!r}. You`re now successfully connected to the workspace {workspace_name!r} in Vectice.
 
 To access a specific project, use workspace.project(Project ID)
 To get a list of projects you can access and their IDs, use workspace.list_projects()
 
 For quick access to the list of projects in the Vectice web app, visit:
 {url}/workspace/projects?w={workspace_id}"""
 
-CONNECTION_PROJECT_LOGGING = """Welcome, {user}. You`re now successfully connected to the project {project_name} in Vectice.
+CONNECTION_PROJECT_LOGGING = """Welcome, {user!r}. You`re now successfully connected to the project {project_name!r} in Vectice.
 
 To access a specific phase, use project.phase(Phase ID)
 To get a list of phases you can access and their IDs, use project.list_phases()
 
 For quick access to the list of phases in the Vectice web app, visit:
 {url}/project?w={workspace_id}&resourceId={project_id}"""
```

### Comparing `vectice-23.1.7.0/src/vectice.egg-info/PKG-INFO` & `vectice-23.1.7.2/src/vectice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.1.7.0
+Version: 23.1.7.2
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
```

### Comparing `vectice-23.1.7.0/src/vectice.egg-info/SOURCES.txt` & `vectice-23.1.7.2/src/vectice.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 src/vectice/models/model.py
 src/vectice/models/phase.py
 src/vectice/models/project.py
 src/vectice/models/property.py
 src/vectice/models/step.py
 src/vectice/models/step_dataset.py
 src/vectice/models/step_image.py
+src/vectice/models/step_model.py
 src/vectice/models/step_number.py
 src/vectice/models/step_string.py
 src/vectice/models/workspace.py
 src/vectice/models/datasource/__init__.py
 src/vectice/models/datasource/datawrapper/__init__.py
 src/vectice/models/datasource/datawrapper/data_wrapper.py
 src/vectice/models/datasource/datawrapper/file_data_wrapper.py
@@ -90,14 +91,16 @@
 src/vectice/models/resource/base.py
 src/vectice/models/resource/description.py
 src/vectice/models/resource/file_resource.py
 src/vectice/models/resource/gcs_resource.py
 src/vectice/models/resource/s3_resource.py
 src/vectice/models/resource/metadata/__init__.py
 src/vectice/models/resource/metadata/base.py
+src/vectice/models/resource/metadata/column_metadata.py
+src/vectice/models/resource/metadata/dataframe_column_parser.py
 src/vectice/models/resource/metadata/db_metadata.py
 src/vectice/models/resource/metadata/files_metadata.py
 src/vectice/utils/__init__.py
 src/vectice/utils/automatic_link_utils.py
 src/vectice/utils/common_utils.py
 src/vectice/utils/configuration.py
 src/vectice/utils/deprecation.py
```

### Comparing `vectice-23.1.7.0/src/vectice.egg-info/requires.txt` & `vectice-23.1.7.2/src/vectice.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 requests>=2.5.0
 rich
 urllib3
 gql[requests]
 GitPython
 packaging
 Pillow
+pandas
 
 [dev]
 black
 gitpython
 mypy
 ruff
 types-requests
```

