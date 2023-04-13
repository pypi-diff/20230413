# Comparing `tmp/mindfoundry.client.analyze-1.20.4.tar.gz` & `tmp/mindfoundry.client.analyze-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindfoundry.client.analyze-1.20.4.tar", last modified: Thu Apr 13 11:22:12 2023, max compression
+gzip compressed data, was "mindfoundry.client.analyze-1.9.2.tar", last modified: Tue Jul 19 16:01:05 2022, max compression
```

## Comparing `mindfoundry.client.analyze-1.20.4.tar` & `mindfoundry.client.analyze-1.9.2.tar`

### file list

```diff
@@ -1,298 +1,297 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.225782 mindfoundry.client.analyze-1.20.4/
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2157 2023-04-13 11:22:12.226784 mindfoundry.client.analyze-1.20.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-04-13 11:22:12.227786 mindfoundry.client.analyze-1.20.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2018 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.121601 mindfoundry.client.analyze-1.20.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.121601 mindfoundry.client.analyze-1.20.4/src/mindfoundry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.122603 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.227786 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/
--rw-rw-rw-   0 root         (0) root         (0)      601 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/__init__.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-04-13 11:22:12.227786 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4375 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/client.py
--rw-rw-rw-   0 root         (0) root         (0)    40956 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/project_api_swagger_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.134624 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/
--rw-rw-rw-   0 root         (0) root         (0)      394 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2661 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/connection.py
--rw-rw-rw-   0 root         (0) root         (0)     7571 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/data_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.135626 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.136627 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/classifier/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/classifier/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7711 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/classifier/analyze_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)     3513 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/classifier/local.py
--rw-rw-rw-   0 root         (0) root         (0)     1628 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/load_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.138631 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/regressor/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/regressor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8009 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/regressor/analyze_regressor.py
--rw-rw-rw-   0 root         (0) root         (0)     3660 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/regressor/local.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.140634 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6425 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/analyze_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2169 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/local.py
--rw-rw-rw-   0 root         (0) root         (0)     6670 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/remote.py
--rw-rw-rw-   0 root         (0) root         (0)     6271 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     6084 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.141636 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.142638 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.149650 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4473 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/create_model_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4607 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/create_model_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     4674 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/create_pipeline_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4774 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/create_pipeline_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_model_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_model_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_pipeline_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_pipeline_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     4184 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_model_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4423 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_pipeline_api.py
--rw-rw-rw-   0 root         (0) root         (0)     3643 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3614 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api_clients.py
--rw-rw-rw-   0 root         (0) root         (0)     3062 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_apis.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4054 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3781 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_clients.py
--rw-rw-rw-   0 root         (0) root         (0)     3217 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_apis.py
--rw-rw-rw-   0 root         (0) root         (0)     4165 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/replace_model_api.py
--rw-rw-rw-   0 root         (0) root         (0)     4318 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/replace_pipeline_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.154659 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/apply_data_prep_steps.py
--rw-rw-rw-   0 root         (0) root         (0)     4312 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/create_cloud_data_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4292 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/create_db_data_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4393 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/create_file_data_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4284 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/create_http_data_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4271 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/delete_data_prep_steps.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/delete_data_set.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/edit_data_set.py
--rw-rw-rw-   0 root         (0) root         (0)     3240 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_set.py
--rw-rw-rw-   0 root         (0) root         (0)     2827 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     3245 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets_csv_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets_parquet_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.155660 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/deprecated/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/deprecated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4343 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/deprecated/create_data_set.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.161671 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4318 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/configure_decisioning_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4172 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_auto_clustering_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4271 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_classification_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4035 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_clustering_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_decisioning_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4007 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_forecasting_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4172 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_multi_forecasting_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4191 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_regression_model.py
--rw-rw-rw-   0 root         (0) root         (0)     1693 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/delete_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3857 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/edit_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3444 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_model_result_csv_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2006 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_model_result_parquet_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2802 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4257 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/optimize_decisioning_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4441 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/save_model_result.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/stop_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.162673 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/other/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/other/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2872 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/other/get_future.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.164676 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3916 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/create_data_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/delete_data_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4010 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/edit_data_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/get_data_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     2981 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/get_data_pipelines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.167681 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3857 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/create_prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/delete_prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     4022 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/edit_prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3314 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction.py
--rw-rw-rw-   0 root         (0) root         (0)     3456 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_forecast.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_result_csv_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1782 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_result_parquet_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_predictions.py
--rw-rw-rw-   0 root         (0) root         (0)     3963 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/save_prediction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.171688 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3659 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/create_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/delete_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3824 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/edit_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3182 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/get_test.py
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_csv_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_parquet_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2780 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/get_tests.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/save_test.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.222777 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/
--rw-rw-rw-   0 root         (0) root         (0)     8634 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/api_column_level.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/api_column_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2581 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/api_history_response.py
--rw-rw-rw-   0 root         (0) root         (0)    12773 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/apply_data_prep_steps_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/apply_formula_step.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/apply_formula_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/cadence.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/classification_model_type.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/classification_scorers.py
--rw-rw-rw-   0 root         (0) root         (0)     2108 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/combine_step.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/combine_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/configure_decisioning_request.py
--rw-rw-rw-   0 root         (0) root         (0)     3716 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_auto_clustering_request.py
--rw-rw-rw-   0 root         (0) root         (0)     8204 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_classification_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5372 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_cloud_data_set_request.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_cloud_data_set_request_cloud_type.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_cloud_data_set_request_data_origin.py
--rw-rw-rw-   0 root         (0) root         (0)     3455 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_clustering_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2689 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_data_set_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4459 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request_data_origin.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request_db_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3007 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_decisioning_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_deployed_api_client_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_deployed_model_api_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1999 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_deployed_pipeline_api_request.py
--rw-rw-rw-   0 root         (0) root         (0)     3445 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_file_data_set_request.py
--rw-rw-rw-   0 root         (0) root         (0)     3385 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_forecasting_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4344 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_http_data_set_request.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_http_data_set_request_data_origin.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_model_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3753 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_multi_forecasting_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2207 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_prediction_request.py
--rw-rw-rw-   0 root         (0) root         (0)     9063 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_regression_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2177 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4115 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/csv_parse_options.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/csv_parse_options_file_type.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_partition_method.py
--rw-rw-rw-   0 root         (0) root         (0)     1606 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_pipeline_create_request.py
--rw-rw-rw-   0 root         (0) root         (0)    12226 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_pipeline_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_pipelines_response.py
--rw-rw-rw-   0 root         (0) root         (0)    10650 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_prep_step_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_set_column_metadata_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4644 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_set_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_sets_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3592 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/decisioning_decision.py
--rw-rw-rw-   0 root         (0) root         (0)     1576 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/decisioning_reward.py
--rw-rw-rw-   0 root         (0) root         (0)     1537 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/decisioning_threshold.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/delete_data_prep_steps_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_create_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2108 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2391 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3192 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2496 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)     3207 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2414 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/discriminators.py
--rw-rw-rw-   0 root         (0) root         (0)     3022 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/discriminators_column_values_item.py
--rw-rw-rw-   0 root         (0) root         (0)     1680 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/drop_step.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/drop_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1392 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_data_pipeline_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_data_set_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_deployed_model_api_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_deployed_pipeline_api_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1592 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_model_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1617 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_prediction_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2661 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/excel_parse_options.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/excel_parse_options_file_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2034 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/filter_rows_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/filter_rows_rule_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/filter_rows_step.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/filter_rows_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2857 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/future.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/future_output_of_your_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1977 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/group_by_aggregation.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/group_by_aggregation_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2458 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/group_by_step.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/group_by_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/id_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1556 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/json_parse_options.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/json_parse_options_file_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/merge_columns_step.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/merge_columns_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_health.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_influence.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)    14843 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_score.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_status.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_validation_method.py
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/nlp_language.py
--rw-rw-rw-   0 root         (0) root         (0)     2049 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/normalize_text_step.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/normalize_text_step_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/normalize_text_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/null_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2297 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response_model_forecasts_item.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_response.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_response_problem_type.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_response_task_status.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/problem_type.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/regression_model_type.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/regression_scorers.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/rename_step.py
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/rename_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/replace_step.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/replace_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/save_model_results_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1617 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/save_prediction_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/save_test_request.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/score_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2106 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/sentiment_analysis_step.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/sentiment_analysis_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1974 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_column_level_step.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_column_level_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_column_type_step.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_column_type_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_time_index_step.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_time_index_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     4445 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simple_forecast.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simple_forecast_cadence.py
--rw-rw-rw-   0 root         (0) root         (0)     1997 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simplify_categories_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     1969 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simplify_categories_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2948 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simplify_categories_step.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simplify_categories_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1950 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/split_column_step.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/split_column_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/status.py
--rw-rw-rw-   0 root         (0) root         (0)      193 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/target_distributions.py
--rw-rw-rw-   0 root         (0) root         (0)     1990 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/test_list_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5778 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/test_response_problem_type.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/test_response_task_status.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/transform_text_step.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/transform_text_step_if_no_match.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/transform_text_step_replace_existing_column.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/transform_text_step_step_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/update_deployed_model_api_request.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/update_deployed_pipeline_api_request.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.225782 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3024 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_cached_response.py
--rw-rw-rw-   0 root         (0) root         (0)     2882 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_polling.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_refreshable_access_token.py
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_swagger_response_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_token_authenticated_client.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_url_validation.py
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 11:22:12.131619 mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2157 2023-04-13 11:22:12.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    19030 2023-04-13 11:22:12.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 11:22:12.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 11:22:12.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      348 2023-04-13 11:22:12.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-13 11:22:12.000000 mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    69992 2023-04-13 11:22:07.000000 mindfoundry.client.analyze-1.20.4/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.601630 mindfoundry.client.analyze-1.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       83 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2156 2022-07-19 16:01:05.601630 mindfoundry.client.analyze-1.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      381 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      357 2022-07-19 16:01:05.601630 mindfoundry.client.analyze-1.9.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.433629 mindfoundry.client.analyze-1.9.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.433629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.433629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.601630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/
+-rw-rw-rw-   0 root         (0) root         (0)      601 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2022-07-19 16:01:05.601630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/client.py
+-rw-rw-rw-   0 root         (0) root         (0)    40356 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/project_api_swagger_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.441629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/
+-rw-rw-rw-   0 root         (0) root         (0)      394 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2661 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/data_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.445629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/
+-rw-rw-rw-   0 root         (0) root         (0)      689 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.445629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/classifier/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/classifier/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7412 2022-07-07 10:27:09.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/classifier/analyze_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     3356 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/classifier/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/load_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.449629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/regressor/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/regressor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7337 2022-07-07 10:27:09.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/regressor/analyze_regressor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3340 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/regressor/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.449629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/
+-rw-rw-rw-   0 root         (0) root         (0)      130 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6310 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/analyze_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2169 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     6608 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     6271 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     6084 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.453629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.453629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.465629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3364 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/create_model_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3454 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/create_model_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3449 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/create_pipeline_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3531 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/create_pipeline_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2643 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_model_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2688 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_model_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_pipeline_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_pipeline_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_model_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3460 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_pipeline_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2915 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api_clients.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_apis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3062 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2895 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_clients.py
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_apis.py
+-rw-rw-rw-   0 root         (0) root         (0)     3224 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/replace_model_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3317 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/replace_pipeline_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.469629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/apply_data_prep_steps.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_cloud_data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_db_data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_file_data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     3027 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_http_data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/delete_data_prep_steps.py
+-rw-rw-rw-   0 root         (0) root         (0)     2472 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/delete_data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/edit_data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     2654 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/get_data_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     2281 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets_csv_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2559 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets_parquet_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.473630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/deprecated/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/deprecated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/deprecated/create_data_set.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.481629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3439 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/configure_decisioning_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3249 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_auto_clustering_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3344 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_classification_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_clustering_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_decisioning_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3250 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_forecasting_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3317 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_multi_forecasting_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3304 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_regression_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/delete_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/edit_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2524 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/get_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/get_model_result_csv_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2734 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/get_model_result_parquet_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2276 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/get_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3350 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/optimize_decisioning_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/save_model_result.py
+-rw-rw-rw-   0 root         (0) root         (0)     2681 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/stop_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.481629 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/other/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/other/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2288 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/other/get_future.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.485630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3121 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/create_data_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/delete_data_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3145 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/edit_data_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2774 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/get_data_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/get_data_pipelines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.489630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/create_prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/delete_prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3125 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/edit_prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2594 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_forecast.py
+-rw-rw-rw-   0 root         (0) root         (0)     3673 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_result_csv_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_result_parquet_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2336 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_predictions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3068 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/save_prediction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.493630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2874 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/create_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/delete_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/edit_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/get_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_csv_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_parquet_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/get_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/save_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1575 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.593630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/
+-rw-rw-rw-   0 root         (0) root         (0)     8527 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/api_history_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2547 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/apply_data_prep_steps_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1875 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/apply_formula_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/apply_formula_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)      481 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/classification_model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/classification_scorers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/combine_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/combine_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/configure_decisioning_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3377 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_auto_clustering_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6958 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_classification_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_cloud_data_set_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_cloud_data_set_request_cloud_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_cloud_data_set_request_data_origin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3145 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_clustering_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_data_set_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3968 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request_data_origin.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request_db_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2767 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_decisioning_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_deployed_api_client_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_deployed_model_api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1900 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_deployed_pipeline_api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_file_data_set_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3109 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_forecasting_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_http_data_set_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_http_data_set_request_data_origin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_model_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3434 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_multi_forecasting_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_prediction_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     6906 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_regression_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2041 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     3264 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/csv_parse_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/csv_parse_options_file_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_partition_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_pipeline_create_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_pipeline_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2061 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_pipelines_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_prep_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1923 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_prep_step_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_set_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1775 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_sets_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     3185 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/decisioning_decision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1506 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/decisioning_reward.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/decisioning_threshold.py
+-rw-rw-rw-   0 root         (0) root         (0)     1656 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/delete_data_prep_steps_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_create_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2174 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2384 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2984 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/discriminators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/discriminators_column_values_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/drop_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/drop_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_data_pipeline_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_data_set_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1576 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_deployed_model_api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_deployed_pipeline_api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_model_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_prediction_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2380 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/excel_parse_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/excel_parse_options_file_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/filter_rows_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/filter_rows_rule_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/filter_rows_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/filter_rows_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/future.py
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/future_outputofyourrequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/group_by_aggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/group_by_aggregation_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/group_by_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/group_by_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/id_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/json_parse_options.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/json_parse_options_file_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/merge_columns_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/merge_columns_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_health.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_influence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1940 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)    12200 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1479 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_score.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_validation_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/nlp_language.py
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/normalize_text_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/normalize_text_step_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/normalize_text_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/null_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/parse_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response_model_forecasts_item.py
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     4634 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_response_problem_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      274 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_response_task_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/problem_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/regression_model_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/regression_scorers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/rename_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/rename_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/replace_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/replace_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1553 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/save_model_results_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/save_prediction_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/save_test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/score_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/sentiment_analysis_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/sentiment_analysis_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_column_level_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      150 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_column_level_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3383 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_column_type_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_column_type_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2105 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_time_index_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_time_index_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     4009 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simple_forecast.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simple_forecast_cadence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simplify_categories_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     1844 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simplify_categories_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     2756 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simplify_categories_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simplify_categories_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/split_column_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/split_column_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      216 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/test_list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     5118 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/test_response_problem_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/test_response_task_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/transform_text_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/transform_text_step_if_no_match.py
+-rw-rw-rw-   0 root         (0) root         (0)      196 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/transform_text_step_replace_existing_column.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/transform_text_step_step_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/update_deployed_model_api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/update_deployed_pipeline_api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      981 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.601630 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      566 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3024 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_cached_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     2882 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_polling.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_refreshable_access_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_swagger_response_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_token_authenticated_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_url_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 16:01:05.437629 mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2156 2022-07-19 16:01:05.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18930 2022-07-19 16:01:05.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 16:01:05.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-07-19 16:01:05.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      341 2022-07-19 16:01:05.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2022-07-19 16:01:05.000000 mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    70144 2022-01-27 12:51:44.000000 mindfoundry.client.analyze-1.9.2/versioneer.py
```

### Comparing `mindfoundry.client.analyze-1.20.4/LICENSE` & `mindfoundry.client.analyze-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/PKG-INFO` & `mindfoundry.client.analyze-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindfoundry.client.analyze
-Version: 1.20.4
+Version: 1.9.2
 Summary: Mind Foundry Analyze Python Client
 Home-page: https://www.mindfoundry.ai/platform
 Author: Mind Foundry Ltd
 Author-email: support@mindfoundry.ai
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mindfoundry.client.analyze-1.20.4/README.rst` & `mindfoundry.client.analyze-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/setup.py` & `mindfoundry.client.analyze-1.9.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import find_namespace_packages, setup
 
 import versioneer
 
 install_requires = [
     "attrs",
-    "httpx>=0.22,<0.23.1",
+    "httpx<0.19.0",  # Generated swagger doesn't support this version at the moment
     "pandas",
     "pyarrow",
     "requests",
 ]  # etc
 
 dev_extras = [
     "black",
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/__init__.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,12 +103,12 @@
 
         return response.json()
 
     def _request(self, *args, **kwargs):
         kwargs["headers"] = {
             "Authorization": "Bearer " + self._token_generator.get_token()
         }
-        response = requests.request(*args, **kwargs, timeout=60)
+        response = requests.request(*args, **kwargs)
         if response.ok:
             return response
         else:
             raise Exception(response.text)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/project_api_swagger_client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/project_api_swagger_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,16 +121,14 @@
     dto.SetColumnTypeStep,
     dto.SetTimeIndexStep,
     dto.SimplifyCategoriesStep,
     dto.SplitColumnStep,
     dto.TransformTextStep,
 ]
 
-ParseOptions = Union[dto.CsvParseOptions, dto.ExcelParseOptions, dto.JsonParseOptions]
-
 
 # pylint: disable=too-many-public-methods
 class AnalyzeSwaggerClientWrapper:
     def __init__(self, client: Client):
         self._client = client
 
     ###############
@@ -138,15 +136,15 @@
     ###############
 
     def create_file_data_set(
         self,
         data: Union[pd.DataFrame, str, io.TextIOBase, io.BytesIO],
         name: str,
         description: Optional[str] = None,
-        parse_options: Optional[ParseOptions] = None,
+        parse_options: Optional[dto.ParseOptions] = None,
     ) -> int:
         with get_data_file(data) as data_file:
             response = create_file_data_set.sync_detailed(
                 client=self._client,
                 multipart_data=dto.CreateFileDataSetRequest(
                     name=name,
                     data=data_file,
@@ -163,15 +161,15 @@
         name: str,
         description: str,
         cloud_type: dto.CreateCloudDataSetRequestCloudType,
         access_key: str,
         secret_key: str,
         bucket_name: str,
         path: str,
-        parse_options: Optional[ParseOptions] = None,
+        parse_options: Optional[dto.ParseOptions] = None,
     ) -> int:
         payload = dto.CreateCloudDataSetRequest(
             name=name,
             description=description,
             data_origin=dto.CreateCloudDataSetRequestDataOrigin.CLOUD,
             cloud_type=cloud_type,
             access_key=access_key,
@@ -189,15 +187,15 @@
         ]
 
     def create_http_data_set(
         self,
         name: str,
         description: str,
         url: str,
-        parse_options: Optional[ParseOptions] = None,
+        parse_options: Optional[dto.ParseOptions] = None,
     ) -> int:
         payload = dto.CreateHttpDataSetRequest(
             name=name,
             description=description,
             data_origin=dto.CreateHttpDataSetRequestDataOrigin.HTTP,
             url=url,
             parse_options=parse_options or UNSET,
@@ -251,15 +249,15 @@
             check_exists(get_data_sets.sync(client=self._client)).data_sets
         )
 
     def get_data_set(self, data_set_id: int) -> dto.DataSetResponse:
         return check_exists(get_data_set.sync(client=self._client, id=data_set_id))
 
     def edit_data_set(
-        self, data_set_id: int, name: str, description: Optional[str] = None
+        self, data_set_id: int, name: str, description: str = None
     ) -> dto.DataSetResponse:
         payload = dto.EditDataSetRequest(name=name, description=description)
         return check_exists(
             edit_data_set.sync(client=self._client, id=data_set_id, json_body=payload)
         )
 
     def download_data_set_as_csv(
@@ -302,15 +300,15 @@
             file.write(parquet_bytes)
 
     def get_data_set_as_pandas(self, data_set_id: int) -> pd.DataFrame:
         stream = io.BytesIO(self._get_data_set_bytes_as_parquet(data_set_id))
         return pd.read_parquet(stream)
 
     def delete_data_set(self, data_set_id: int) -> None:
-        delete_data_set.sync_detailed(client=self._client, id=data_set_id)
+        delete_data_set.sync(client=self._client, id=data_set_id)
 
     def apply_saved_data_preparation_steps(
         self,
         data_set_id: int,
         data_preparation_step_id: int,
         insertion_index: Optional[int] = None,
     ) -> int:
@@ -373,15 +371,15 @@
             check_exists(get_data_pipelines.sync(client=self._client)).pipelines
         )
 
     def get_data_pipeline(self, pipeline_id: int) -> dto.DataPipelineResponse:
         return check_exists(get_data_pipeline.sync(client=self._client, id=pipeline_id))
 
     def delete_data_pipeline(self, pipeline_id: int) -> None:
-        delete_data_pipeline.sync_detailed(client=self._client, id=pipeline_id)
+        delete_data_pipeline.sync(client=self._client, id=pipeline_id)
 
     def create_data_pipeline(self, data_set_id: int, name: str) -> int:
         payload = dto.DataPipelineCreateRequest(
             data_set_id=data_set_id,
             name=name,
         )
         return check_exists(
@@ -407,15 +405,15 @@
             check_exists(get_models.sync(client=self._client)).models
         )
 
     def get_model(self, model_id: int) -> dto.ModelResponse:
         return check_exists(get_model.sync(client=self._client, id=model_id))
 
     def delete_model(self, model_id: int):
-        delete_model.sync_detailed(client=self._client, id=model_id)
+        delete_model.sync(client=self._client, id=model_id)
 
     # pylint: disable=too-many-arguments,too-many-locals
     def create_classification_model(
         self,
         name: str,
         data_set_id: int,
         target_column: str,
@@ -424,15 +422,14 @@
         description: Optional[str] = None,
         draft_mode: bool = False,
         number_of_evaluations: int = 300,
         nlp_language: dto.NlpLanguage = dto.NlpLanguage.AUTO_DETECT,
         model_validation_method: dto.ModelValidationMethod = dto.ModelValidationMethod.FIVE_FOLD_CROSS,
         no_mixing_columns: Optional[List[str]] = None,
         data_partition_method: dto.DataPartitionMethod = dto.DataPartitionMethod.RANDOM,
-        hold_out_percentage: Optional[float] = 10.0,
         partition_column: Optional[str] = None,
         order_by_column: Optional[str] = None,
         weight_column: Optional[str] = None,
         wait_until_complete: bool = True,
         model_types: Optional[List[dto.ClassificationModelType]] = None,
     ) -> int:
         payload = dto.CreateClassificationRequest(
@@ -443,15 +440,14 @@
             model_validation_method=model_validation_method,
             data_partition_method=data_partition_method,
             number_of_evaluations=number_of_evaluations,
             description=description or UNSET,
             excluded_columns=excluded_columns or UNSET,
             nlp_language=nlp_language,
             draft_mode=draft_mode,
-            hold_out_percentage=hold_out_percentage or UNSET,
             no_mixing_columns=no_mixing_columns or UNSET,
             partition_column=partition_column or UNSET,
             order_by_column=order_by_column or UNSET,
             weight_column=weight_column or UNSET,
             model_types=model_types or UNSET,
         )
 
@@ -466,45 +462,41 @@
 
     # pylint: disable=too-many-arguments,too-many-locals
     def create_regression_model(
         self,
         name: str,
         data_set_id: int,
         target_column: str,
-        target_distribution: Optional[dto.TargetDistributions] = None,
         score_to_optimize: dto.RegressionScorers = dto.RegressionScorers.RMSE,
         excluded_columns: Optional[List[str]] = None,
         description: Optional[str] = None,
         number_of_evaluations: int = 300,
         nlp_language: dto.NlpLanguage = dto.NlpLanguage.AUTO_DETECT,
         draft_mode: bool = False,
         model_validation_method: dto.ModelValidationMethod = dto.ModelValidationMethod.FIVE_FOLD_CROSS,
         no_mixing_columns: Optional[List[str]] = None,
         data_partition_method: dto.DataPartitionMethod = dto.DataPartitionMethod.RANDOM,
-        hold_out_percentage: Optional[float] = 10.0,
         partition_column: Optional[str] = None,
         order_by_column: Optional[str] = None,
         weight_column: Optional[str] = None,
         wait_until_complete: bool = True,
         model_types: Optional[List[dto.RegressionModelType]] = None,
     ) -> int:
         payload = dto.CreateRegressionRequest(
             name=name,
             data_set_id=data_set_id,
             target_column=target_column,
-            target_distribution=target_distribution or UNSET,
             score_to_optimize=score_to_optimize,
             model_validation_method=model_validation_method,
             data_partition_method=data_partition_method,
             number_of_evaluations=number_of_evaluations,
             description=description or UNSET,
             excluded_columns=excluded_columns or UNSET,
             nlp_language=nlp_language,
             draft_mode=draft_mode,
-            hold_out_percentage=hold_out_percentage or UNSET,
             no_mixing_columns=no_mixing_columns or UNSET,
             partition_column=partition_column or UNSET,
             order_by_column=order_by_column or UNSET,
             weight_column=weight_column or UNSET,
             model_types=model_types or UNSET,
         )
         model_id = check_exists(
@@ -521,14 +513,15 @@
         data_set_id: int,
         number_of_clusters: int,
         description: Optional[str] = None,
         nlp_language: dto.NlpLanguage = dto.NlpLanguage.AUTO_DETECT,
         excluded_columns: Optional[List[str]] = None,
         wait_until_complete: bool = True,
     ) -> int:
+
         payload = dto.CreateClusteringRequest(
             name=name,
             data_set_id=data_set_id,
             description=description or UNSET,
             excluded_columns=excluded_columns or UNSET,
             nlp_language=nlp_language,
             number_of_clusters=number_of_clusters,
@@ -713,15 +706,15 @@
     ) -> dto.ModelResponse:
         payload = dto.EditModelRequest(name=name, description=description)
         return check_exists(
             edit_model.sync(client=self._client, id=model_id, json_body=payload)
         )
 
     def stop_optimization(self, model_id: int):
-        stop_model.sync_detailed(client=self._client, id=model_id)
+        stop_model.sync(client=self._client, id=model_id)
 
     def download_model_results_as_csv(
         self,
         model_id: int,
         output_file: Union[str, PathLike],
         separator: str = ",",
         quote_char: str = '"',
@@ -775,15 +768,15 @@
     ###############
 
     def create_prediction(
         self,
         model_id: int,
         data_set_id: int,
         name: str,
-        description: Optional[str] = None,
+        description: str = None,
         wait_until_complete: bool = True,
     ) -> int:
         prediction_id = check_exists(
             create_prediction.sync(
                 client=self._client,
                 json_body=dto.CreatePredictionRequest(
                     model_id=model_id,
@@ -795,15 +788,15 @@
         ).id
         if not wait_until_complete:
             return prediction_id
 
         return wait_for_prediction_to_complete(self._client, prediction_id)
 
     def edit_prediction(
-        self, prediction_id: int, name: str, description: Optional[str] = None
+        self, prediction_id: int, name: str, description: str = None
     ) -> dto.PredictionResponse:
         payload = dto.EditPredictionRequest(name=name, description=description)
         return check_exists(
             edit_prediction.sync(
                 client=self._client, id=prediction_id, json_body=payload
             )
         )
@@ -865,15 +858,15 @@
             file.write(parquet_bytes)
 
     def get_prediction_result_as_pandas(self, prediction_id: int) -> pd.DataFrame:
         stream = io.BytesIO(self._get_prediction_bytes_as_parquet(prediction_id))
         return pd.read_parquet(stream)
 
     def delete_prediction(self, prediction_id: int) -> None:
-        delete_prediction.sync_detailed(client=self._client, id=prediction_id)
+        delete_prediction.sync(client=self._client, id=prediction_id)
 
     def save_prediction_result_as_data_set(
         self, prediction_id: int, name: str, description: Optional[str] = None
     ) -> int:
         payload = dto.SavePredictionRequest(name=name, description=description)
         return check_exists(
             save_prediction.sync(
@@ -886,15 +879,15 @@
     ###############
 
     def create_test(
         self,
         model_id: int,
         data_set_id: int,
         name: str,
-        description: Optional[str] = None,
+        description: str = None,
         wait_until_complete: bool = True,
     ) -> int:
         test_id = check_exists(
             create_test.sync(
                 client=self._client,
                 json_body=dto.CreateTestRequest(
                     model_id=model_id,
@@ -906,15 +899,15 @@
         ).id
         if not wait_until_complete:
             return test_id
 
         return wait_for_test_to_complete(self._client, test_id)
 
     def edit_test(
-        self, test_id: int, name: str, description: Optional[str] = None
+        self, test_id: int, name: str, description: str = None
     ) -> dto.TestResponse:
         payload = dto.EditTestRequest(name=name, description=description)
         return check_exists(
             edit_test.sync(client=self._client, id=test_id, json_body=payload)
         )
 
     def get_test_overview(self, test_id: int) -> dto.TestResponse:
@@ -965,15 +958,15 @@
     def get_test_result_as_pandas(self, test_id: int) -> pd.DataFrame:
         with tempfile.TemporaryFile() as file:
             file.write(self._get_test_bytes_as_parquet(test_id))
             file.seek(0)
             return pd.read_parquet(path=file)
 
     def delete_test(self, test_id: int) -> None:
-        delete_test.sync_detailed(client=self._client, id=test_id)
+        delete_test.sync(client=self._client, id=test_id)
 
     def save_test_result_as_data_set(
         self, test_id: int, name: str, description: Optional[str] = None
     ) -> int:
         payload = dto.SaveTestRequest(name=name, description=description)
         return check_exists(
             save_test.sync(client=self._client, id=test_id, json_body=payload)
@@ -985,15 +978,15 @@
 
     def list_model_apis(self) -> List[dto.DeployedModelApiResponse]:
         return check_not_unset(
             check_exists(get_model_apis.sync(client=self._client)).published_models
         )
 
     def delete_model_api(self, model_api_id: int) -> None:
-        delete_model_api.sync_detailed(client=self._client, model_api_id=model_api_id)
+        delete_model_api.sync(client=self._client, model_api_id=model_api_id)
 
     def create_model_api(
         self, model_id: int, name: str, description: Optional[str] = None
     ) -> int:
         response = create_model_api.sync_detailed(
             client=self._client,
             json_body=dto.CreateDeployedModelApiRequest(
@@ -1039,15 +1032,15 @@
         return check_not_unset(
             check_exists(
                 get_model_api_clients.sync(client=self._client, model_api_id=api_id)
             ).api_clients
         )
 
     def delete_model_api_client(self, model_api_id: int, client_id: str) -> None:
-        delete_model_api_client.sync_detailed(
+        delete_model_api_client.sync(
             client=self._client, model_api_id=model_api_id, client_id=client_id
         )
 
     def create_model_api_client(
         self, api_id: int, name: str
     ) -> dto.DeployedApiClientCreateResponse:
         return check_exists(
@@ -1075,17 +1068,15 @@
         return check_not_unset(
             check_exists(
                 get_pipeline_apis.sync(client=self._client)
             ).published_pipelines
         )
 
     def delete_pipeline_api(self, pipeline_api_id: int) -> None:
-        delete_pipeline_api.sync_detailed(
-            client=self._client, pipeline_api_id=pipeline_api_id
-        )
+        delete_pipeline_api.sync(client=self._client, pipeline_api_id=pipeline_api_id)
 
     def create_pipeline_api(
         self, pipeline_id: int, name: str, description: Optional[str] = None
     ) -> int:
         response = create_pipeline_api.sync_detailed(
             client=self._client,
             json_body=dto.CreateDeployedPipelineApiRequest(
@@ -1133,15 +1124,15 @@
                 get_pipeline_api_clients.sync(
                     client=self._client, pipeline_api_id=api_id
                 )
             ).api_clients
         )
 
     def delete_pipeline_api_client(self, pipeline_api_id: int, client_id: str) -> None:
-        delete_pipeline_api_client.sync_detailed(
+        delete_pipeline_api_client.sync(
             client=self._client, pipeline_api_id=pipeline_api_id, client_id=client_id
         )
 
     def create_pipeline_api_client(
         self, api_id: int, name: str
     ) -> dto.DeployedApiClientCreateResponse:
         return check_exists(
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/connection.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/connection.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/data_set.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/data_set.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/__init__.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Re-export these so they can be accessed from this package
 from mindfoundry.client.analyze.swagger.models import (
-    ClassificationModelType,
     ClassificationScorers,
     CreateAutoClusteringRequest,
     CreateClassificationRequest,
     CreateClusteringRequest,
     CreateForecastingRequest,
     CreateMultiForecastingRequest,
     CreateRegressionRequest,
@@ -13,16 +12,14 @@
     ModelInfluence,
     ModelResponse,
     ModelScore,
     ModelStatus,
     ModelValidationMethod,
     NlpLanguage,
     ProblemType,
-    RegressionModelType,
     RegressionScorers,
     ScoreType,
-    TargetDistributions,
 )
 
 from .classifier import AnalyzeClassifier
 from .load_model import load_model, load_model_from_server
 from .regressor import AnalyzeRegressor
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/classifier/analyze_classifier.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/classifier/analyze_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,83 +124,77 @@
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Classification specific fit parameters
         sample_weight: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
     ) -> "AnalyzeClassifier":
         """Fit the classification model using random data partitioning"""
 
     @overload
     def fit(
         self,
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Classification specific fit parameters
         sample_weight: Optional[str] = None,
         order_by: str,
-        hold_out_percentage: Optional[float] = 10.0,
     ) -> "AnalyzeClassifier":
         """Fit the classification model using ordered data partitioning"""
 
     @overload
     def fit(
         self,
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Classification specific fit parameters
         partition_by: str,
         sample_weight: Optional[str] = None,
-        hold_out_percentage=None,
     ) -> "AnalyzeClassifier":
         """Fit the classification model using manual data partitioning"""
 
     @overload
     def fit(
         self,
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Classification specific fit parameters
         sample_weight: Optional[str] = None,
         no_mixing: List[str],
-        hold_out_percentage: Optional[float] = 10.0,
     ) -> "AnalyzeClassifier":
         """Fit the classification model using a no-mixing column data partitioning"""
 
     def fit(
         self,
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Classification specific fit parameters
         sample_weight: Optional[str] = None,
         order_by: Optional[str] = None,
         partition_by: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
         no_mixing: Optional[List[str]] = None,
     ) -> "AnalyzeClassifier":
         """Internal method - DO NOT USE"""
         super()._fit(
             data,
             target,
             excluded_columns,
             wait_until_complete=wait_until_complete,
             order_by=order_by,
             partition_by=partition_by,
             no_mixing=no_mixing,
             sample_weight=sample_weight,
-            hold_out_percentage=hold_out_percentage,
         )
         return self
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/classifier/local.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/classifier/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ClassificationScorers,
     CreateClassificationRequest,
     DataPartitionMethod,
     ModelValidationMethod,
     NlpLanguage,
 )
 from ....swagger.types import UNSET
-from ....utils import check_response
+from ....utils import check_exists
 from ...connection import ConnectionLike, client_from_connectionlike
 from ...data_set import DataLike, get_dataset_from_datalike
 from ..shared import BaseModel, LocalModel, RemoteModel
 
 
 @attr.s(auto_attribs=True)
 class InitialConfig:
@@ -50,17 +50,17 @@
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         sample_weight: Optional[str] = None,
         order_by: Optional[str] = None,
         partition_by: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
         no_mixing: Optional[List[str]] = None,
     ) -> BaseModel:
+
         # data_partition_method - determine based on whether there are orderby/partitionby/nomixing names
         if not order_by is None:
             data_partition_method = DataPartitionMethod.ORDERED
         elif not partition_by is None:
             data_partition_method = DataPartitionMethod.MANUAL
         elif not no_mixing is None:
             data_partition_method = DataPartitionMethod.NO_MIXING
@@ -82,16 +82,13 @@
             nlp_language=self._initial_config.nlp_language,
             draft_mode=self._initial_config.draft_mode,
             no_mixing_columns=no_mixing or UNSET,
             partition_column=partition_by or UNSET,
             order_by_column=order_by or UNSET,
             weight_column=sample_weight or UNSET,
             model_types=self._initial_config.model_types or UNSET,
-            hold_out_percentage=hold_out_percentage or UNSET,
         )
 
-        model_id = check_response(
-            create_classification_model.sync_detailed(
-                client=self._client, json_body=payload
-            )
+        model_id = check_exists(
+            create_classification_model.sync(client=self._client, json_body=payload)
         ).id
         return RemoteModel(self._connection, model_id)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/load_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/load_model.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/regressor/analyze_regressor.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/regressor/analyze_regressor.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from ....swagger.models import (
     ModelValidationMethod,
     NlpLanguage,
     ProblemType,
     RegressionModelType,
     RegressionScorers,
-    TargetDistributions,
 )
 from ....utils.typing import UNSET, PathLike, Unset
 from ...connection import ConnectionLike, from_connectionlike
 from ...data_set import DataLike
 from ..serialization import parse_model_from_path
 from ..shared import AnalyzeModel, BaseModel, RemoteModel
 from .local import InitialConfig, LocalRegressor
@@ -28,18 +27,14 @@
         scorer: RegressionScorers = RegressionScorers.RMSE,
         model_validation_method: ModelValidationMethod = ModelValidationMethod.FIVE_FOLD_CROSS,
         name: Optional[str] = None,
         description: Optional[str] = None,
         number_of_evaluations: int = 300,
         nlp_language: NlpLanguage = NlpLanguage.AUTO_DETECT,
         draft_mode: bool = False,
-        model_types: Optional[List[RegressionModelType]] = None,
-        target_distribution: Optional[
-            TargetDistributions
-        ] = TargetDistributions.GAUSSIAN,
         *,
         connection: ConnectionLike,
     ):
         """
         Create a new Analyze regression model
         :param scorer: The scorer to use to determine the optimal model
         :param model_validation_method: The method to use to validate the model
@@ -61,17 +56,14 @@
         model_validation_method: ModelValidationMethod = ModelValidationMethod.FIVE_FOLD_CROSS,
         name: Optional[str] = None,
         description: Optional[str] = None,
         number_of_evaluations: int = 300,
         nlp_language: NlpLanguage = NlpLanguage.AUTO_DETECT,
         draft_mode: bool = False,
         model_types: Optional[List[RegressionModelType]] = None,
-        target_distribution: Optional[
-            TargetDistributions
-        ] = TargetDistributions.GAUSSIAN,
         *,
         connection: Union[ConnectionLike, Unset] = UNSET,
         _internal_model: Union[BaseModel, Unset] = UNSET,
     ):
         """Internal constructor - DO NOT USE"""
         if not isinstance(_internal_model, Unset):
             # Default to using the regressor if it was specified
@@ -87,15 +79,14 @@
                 model_validation_method=model_validation_method,
                 name=name if name is not None else _default_model_name(),
                 description=description,
                 number_of_evaluations=number_of_evaluations,
                 nlp_language=nlp_language,
                 draft_mode=draft_mode,
                 model_types=model_types,
-                target_distribution=target_distribution,
             )
             super().__init__(_internal_model=LocalRegressor(connection, initial_config))
 
     @classmethod
     def load_model(
         cls, path: PathLike, *, connection: ConnectionLike
     ) -> "AnalyzeRegressor":
@@ -132,60 +123,56 @@
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Regression specific fit parameters
         sample_weight: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
     ) -> "AnalyzeRegressor":
         """Fit the regression model using random data partitioning"""
 
     @overload
     def fit(
         self,
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Regression specific fit parameters
         sample_weight: Optional[str] = None,
         order_by: str,
-        hold_out_percentage: Optional[float] = 10.0,
     ) -> "AnalyzeRegressor":
         """Fit the regression model using ordered data partitioning"""
 
     @overload
     def fit(
         self,
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Regression specific fit parameters
         sample_weight: Optional[str] = None,
         partition_by: str,
-        hold_out_percentage=None,
     ) -> "AnalyzeRegressor":
         """Fit the regression model using manual data partitioning"""
 
     @overload
     def fit(
         self,
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Regression specific fit parameters
         sample_weight: Optional[str] = None,
         no_mixing: List[str],
-        hold_out_percentage: Optional[float] = 10.0,
     ) -> "AnalyzeRegressor":
         """Fit the regression model using a no-mixing column data partitioning"""
 
     def fit(
         self,
         data: DataLike,
         target: str,
@@ -193,23 +180,21 @@
         *,
         wait_until_complete: bool = True,
         # Regression specific fit parameters
         sample_weight: Optional[str] = None,
         order_by: Optional[str] = None,
         partition_by: Optional[str] = None,
         no_mixing: Optional[List[str]] = None,
-        hold_out_percentage: Optional[float] = 10.0,
     ) -> "AnalyzeRegressor":
         """Internal method - DO NOT USE"""
         # Fit must explicitly override the model with the new fitted model
         super()._fit(
             data,
             target,
             excluded_columns,
             wait_until_complete=wait_until_complete,
             order_by=order_by,
             partition_by=partition_by,
             no_mixing=no_mixing,
             sample_weight=sample_weight,
-            hold_out_percentage=hold_out_percentage,
         )
         return self
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/regressor/local.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/regressor/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 from ....swagger.models import (
     CreateRegressionRequest,
     DataPartitionMethod,
     ModelValidationMethod,
     NlpLanguage,
     RegressionModelType,
     RegressionScorers,
-    TargetDistributions,
 )
 from ....swagger.types import UNSET
-from ....utils import check_response
+from ....utils import check_exists
 from ...connection import ConnectionLike, client_from_connectionlike
 from ...data_set import DataLike, get_dataset_from_datalike
 from ..shared import BaseModel, LocalModel, RemoteModel
 
 
 @attr.s(auto_attribs=True)
 class InitialConfig:
@@ -25,15 +24,14 @@
     model_validation_method: ModelValidationMethod
     name: str
     description: Optional[str]
     number_of_evaluations: int
     nlp_language: NlpLanguage
     draft_mode: bool
     model_types: Optional[List[RegressionModelType]]
-    target_distribution: Optional[TargetDistributions]
 
 
 class LocalRegressor(LocalModel):
     """
     A regressor that has not yet been saved to Analyze (and thus hasn't been fitted)
     """
 
@@ -52,17 +50,17 @@
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         # Regression specific fit parameters
         sample_weight: Optional[str] = None,
         order_by: Optional[str] = None,
         partition_by: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
         no_mixing: Optional[List[str]] = None,
     ) -> BaseModel:
+
         # data_partition_method - determine based on whether there are orderby/partitionby/nomixing names
         if not order_by is None:
             data_partition_method = DataPartitionMethod.ORDERED
         elif not partition_by is None:
             data_partition_method = DataPartitionMethod.MANUAL
         elif not no_mixing is None:
             data_partition_method = DataPartitionMethod.NO_MIXING
@@ -70,31 +68,27 @@
             data_partition_method = DataPartitionMethod.RANDOM
 
         data_set = get_dataset_from_datalike(data, connection=self._connection)
 
         payload = CreateRegressionRequest(
             name=self._initial_config.name,
             data_set_id=data_set.data_set_id,
-            target_distribution=self._initial_config.target_distribution or UNSET,
             target_column=target,
             score_to_optimize=self._initial_config.scorer,
             model_validation_method=self._initial_config.model_validation_method,
             data_partition_method=data_partition_method,
-            hold_out_percentage=hold_out_percentage or UNSET,
             number_of_evaluations=self._initial_config.number_of_evaluations,
             description=self._initial_config.description or UNSET,
             excluded_columns=excluded_columns or UNSET,
             nlp_language=self._initial_config.nlp_language,
             draft_mode=self._initial_config.draft_mode,
             no_mixing_columns=no_mixing or UNSET,
             partition_column=partition_by or UNSET,
             order_by_column=order_by or UNSET,
             weight_column=sample_weight or UNSET,
             model_types=self._initial_config.model_types or UNSET,
         )
 
-        model_id = check_response(
-            create_regression_model.sync_detailed(
-                client=self._client, json_body=payload
-            )
+        model_id = check_exists(
+            create_regression_model.sync(client=self._client, json_body=payload)
         ).id
         return RemoteModel(self._connection, model_id)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/serialization.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/serialization.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/analyze_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/analyze_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,28 +34,26 @@
         excluded_columns: Optional[List[str]] = None,
         *,
         wait_until_complete: bool = True,
         # Classification and Regression specific fit parameters
         sample_weight: Optional[str] = None,
         order_by: Optional[str] = None,
         partition_by: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
         no_mixing: Optional[List[str]] = None,
     ) -> "AnalyzeModel":
         """Internal method - DO NOT USE"""
         # Fit must explicitly override the model with the new fitted model
         self._internal_model = self._internal_model.fit(
             data,
             target,
             excluded_columns,
             order_by=order_by,
             partition_by=partition_by,
             no_mixing=no_mixing,
             sample_weight=sample_weight,
-            hold_out_percentage=hold_out_percentage,
         )
         if wait_until_complete:
             self._internal_model.wait_until_fitted()
         return self
 
     ########################################################
     # Generic methods passed through to the internal model #
@@ -164,12 +162,11 @@
         test, for clustering it is the clustered data."""
         return self._internal_model.results_as_df()
 
     def save_results_as_dataset(
         self, *, name: Optional[str] = None, description: Optional[str] = None
     ) -> DataSet:
         """Save the model results data as a data set to allow use in other places in the system - For classification & regression
-        this result is the result of hold-out test, for clustering it is the clustered data.
-        """
+        this result is the result of hold-out test, for clustering it is the clustered data."""
         return self._internal_model.save_results_as_dataset(
             name=name, description=description
         )
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/base.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         # Classification and Regression specific fit parameters
         sample_weight: Optional[str] = None,
         order_by: Optional[str] = None,
         partition_by: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
         no_mixing: Optional[List[str]] = None,
     ) -> "BaseModel":
         """Fit the model and return a fitted version"""
 
     @property
     @abc.abstractmethod
     def model_id(self) -> int:
@@ -88,9 +87,8 @@
         test, for clustering it is the clustered data."""
 
     @abc.abstractmethod
     def save_results_as_dataset(
         self, *, name: Optional[str] = None, description: Optional[str] = None
     ) -> DataSet:
         """Save the model results data as a data set to allow use in other places in the system - For classification & regression
-        this result is the result of hold-out test, for clustering it is the clustered data.
-        """
+        this result is the result of hold-out test, for clustering it is the clustered data."""
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/local.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/local.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/model/shared/remote.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/model/shared/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,15 @@
 
         return pd.read_parquet(BytesIO(response.content))
 
     def save_results_as_dataset(
         self, *, name: Optional[str] = None, description: Optional[str] = None
     ) -> DataSet:
         """Save the model results data as a data set to allow use in other places in the system - For classification & regression
-        this result is the result of hold-out test, for clustering it is the clustered data.
-        """
+        this result is the result of hold-out test, for clustering it is the clustered data."""
 
         name = name or _default_saved_results_dataset_name(self.model_info().name)
         payload = SaveModelResultsRequest(name=name, description=description)
         data_set_id = check_exists(
             save_model_result.sync(
                 client=self._client, id=self.model_id, json_body=payload
             )
@@ -178,11 +177,10 @@
         data: DataLike,
         target: str,
         excluded_columns: Optional[List[str]] = None,
         *,
         sample_weight: Optional[str] = None,
         order_by: Optional[str] = None,
         partition_by: Optional[str] = None,
-        hold_out_percentage: Optional[float] = 10.0,
         no_mixing: Optional[List[str]] = None,
     ) -> BaseModel:
         raise Exception("Model is already fitted - cannot refit")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/prediction.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/prediction.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/sklearn_client/test.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/sklearn_client/test.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/create_model_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/apply_data_prep_steps.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,189 +1,165 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.create_deployed_model_api_request import CreateDeployedModelApiRequest
+from ...models.apply_data_prep_steps_request import ApplyDataPrepStepsRequest
 from ...models.future import Future
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: CreateDeployedModelApiRequest,
+    id: int,
+    json_body: ApplyDataPrepStepsRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/modelApis".format(
-        client.base_url)
+    url = "{}/v1/dataSets/{id}/dataPrepSteps".format(
+        client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Future]]:
-    if response.status_code == 201:
-        response_201 = Future.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    Future,
+    None,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = Future.from_dict(response.json())
 
 
 
-        return response_201
+        return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
-    if response.status_code == 403:
-        response_403 = cast(Any, None)
-        return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Future]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    Future,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: CreateDeployedModelApiRequest,
-
-) -> Response[Union[Any, Future]]:
-    """Publish a model as an API
-
-     Deploy a model API for the specified model. The response will contain a `futureId` which you can use
-    with the `/futures` endpoint to check the progress of the deployment. Upon completion the future
-    will give you information about the resulting deployment.
-
-    Args:
-        json_body (CreateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+    id: int,
+    json_body: ApplyDataPrepStepsRequest,
 
+) -> Response[Union[
+    Future,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
+id=id,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
-    json_body: CreateDeployedModelApiRequest,
-
-) -> Optional[Union[Any, Future]]:
-    """Publish a model as an API
-
-     Deploy a model API for the specified model. The response will contain a `futureId` which you can use
-    with the `/futures` endpoint to check the progress of the deployment. Upon completion the future
-    will give you information about the resulting deployment.
-
-    Args:
-        json_body (CreateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
+    id: int,
+    json_body: ApplyDataPrepStepsRequest,
 
+) -> Optional[Union[
+    Future,
+    None,
+    None
+]]:
+    """ The data steps will start to be applied immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your step application. Upon completion the future will give you information about the resulting data set. """
 
     return sync_detailed(
         client=client,
+id=id,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: CreateDeployedModelApiRequest,
-
-) -> Response[Union[Any, Future]]:
-    """Publish a model as an API
-
-     Deploy a model API for the specified model. The response will contain a `futureId` which you can use
-    with the `/futures` endpoint to check the progress of the deployment. Upon completion the future
-    will give you information about the resulting deployment.
-
-    Args:
-        json_body (CreateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+    id: int,
+    json_body: ApplyDataPrepStepsRequest,
 
+) -> Response[Union[
+    Future,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
+id=id,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
-    json_body: CreateDeployedModelApiRequest,
-
-) -> Optional[Union[Any, Future]]:
-    """Publish a model as an API
-
-     Deploy a model API for the specified model. The response will contain a `futureId` which you can use
-    with the `/futures` endpoint to check the progress of the deployment. Upon completion the future
-    will give you information about the resulting deployment.
-
-    Args:
-        json_body (CreateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
+    id: int,
+    json_body: ApplyDataPrepStepsRequest,
 
+) -> Optional[Union[
+    Future,
+    None,
+    None
+]]:
+    """ The data steps will start to be applied immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your step application. Upon completion the future will give you information about the resulting data set. """
 
     return (await asyncio_detailed(
         client=client,
+id=id,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/create_pipeline_api_client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/create_pipeline_api_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,197 +1,167 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.create_deployed_api_client_request import CreateDeployedApiClientRequest
 from ...models.deployed_api_client_create_response import (
     DeployedApiClientCreateResponse,
 )
 from ...types import Response
 
 
 def _get_kwargs(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: CreateDeployedApiClientRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/pipelineApis/{pipelineApiId}/clients".format(
         client.base_url,pipelineApiId=pipeline_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedApiClientCreateResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
     if response.status_code == 201:
         response_201 = DeployedApiClientCreateResponse.from_dict(response.json())
 
 
 
         return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedApiClientCreateResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: CreateDeployedApiClientRequest,
 
-) -> Response[Union[Any, DeployedApiClientCreateResponse]]:
-    """Create a new client for a published data prep pipeline
-
-     Create a new client to access and use a given published data prep pipeline api and returns its new
-    credentials (client id and secret)
-
-    Args:
-        pipeline_api_id (int):
-        json_body (CreateDeployedApiClientRequest):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientCreateResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: CreateDeployedApiClientRequest,
 
-) -> Optional[Union[Any, DeployedApiClientCreateResponse]]:
-    """Create a new client for a published data prep pipeline
-
-     Create a new client to access and use a given published data prep pipeline api and returns its new
-    credentials (client id and secret)
-
-    Args:
-        pipeline_api_id (int):
-        json_body (CreateDeployedApiClientRequest):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientCreateResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
+    """ Create a new client to access and use a given published data prep pipeline api and returns its new credentials (client id and secret) """
 
     return sync_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: CreateDeployedApiClientRequest,
 
-) -> Response[Union[Any, DeployedApiClientCreateResponse]]:
-    """Create a new client for a published data prep pipeline
-
-     Create a new client to access and use a given published data prep pipeline api and returns its new
-    credentials (client id and secret)
-
-    Args:
-        pipeline_api_id (int):
-        json_body (CreateDeployedApiClientRequest):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientCreateResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: CreateDeployedApiClientRequest,
 
-) -> Optional[Union[Any, DeployedApiClientCreateResponse]]:
-    """Create a new client for a published data prep pipeline
-
-     Create a new client to access and use a given published data prep pipeline api and returns its new
-    credentials (client id and secret)
-
-    Args:
-        pipeline_api_id (int):
-        json_body (CreateDeployedApiClientRequest):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientCreateResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
+    """ Create a new client to access and use a given published data prep pipeline api and returns its new credentials (client id and secret) """
 
     return (await asyncio_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_model_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,161 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.deployed_api_client_response import DeployedApiClientResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    model_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
+    client_id: str,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/modelApis/{modelApiId}".format(
-        client.base_url,modelApiId=model_api_id)
+    url = "{}/v1/modelApis/{modelApiId}/clients/{clientId}".format(
+        client.base_url,modelApiId=model_api_id,clientId=client_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = DeployedApiClientResponse.from_dict(response.json())
+
+
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    if response.status_code == 404:
+        response_404 = None
 
+        return response_404
+    return None
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    model_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
+    client_id: str,
 
-) -> Response[Any]:
-    """Deletes the specified published model
-
-     Deletes the specified published model
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
+client_id=client_id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    model_api_id: int,
+def sync(
     *,
     client: Client,
+    model_api_id: int,
+    client_id: str,
 
-) -> Response[Any]:
-    """Deletes the specified published model
-
-     Deletes the specified published model
-
-    Args:
-        model_api_id (int):
+) -> Optional[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
+    """ Gets an overview of the published model api client """
+
+    return sync_detailed(
+        client=client,
+model_api_id=model_api_id,
+client_id=client_id,
 
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    model_api_id: int,
+    client_id: str,
 
+) -> Response[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
+client_id=client_id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    model_api_id: int,
+    client_id: str,
+
+) -> Optional[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
+    """ Gets an overview of the published model api client """
+
+    return (await asyncio_detailed(
+        client=client,
+model_api_id=model_api_id,
+client_id=client_id,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_model_api_client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_model_api_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,120 +1,158 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...types import Response
 
 
 def _get_kwargs(
-    model_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    model_api_id: int,
+    client_id: str,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/modelApis/{modelApiId}/clients/{clientId}".format(
         client.base_url,modelApiId=model_api_id,clientId=client_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-
-
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 204:
+        response_204 = None
+
+        return response_204
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    if response.status_code == 404:
+        response_404 = None
+
+        return response_404
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    model_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    model_api_id: int,
+    client_id: str,
 
-) -> Response[Any]:
-    """Delete a model api client
-
-     Delete a model api client
-
-    Args:
-        model_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
+        client=client,
+model_api_id=model_api_id,
 client_id=client_id,
-client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.delete(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    model_api_id: int,
-    client_id: str,
+def sync(
     *,
     client: Client,
+    model_api_id: int,
+    client_id: str,
 
-) -> Response[Any]:
-    """Delete a model api client
-
-     Delete a model api client
+) -> Optional[Union[
+    None,
+    None,
+    None
+]]:
+    """ Delete a model api client """
+
+    return sync_detailed(
+        client=client,
+model_api_id=model_api_id,
+client_id=client_id,
 
-    Args:
-        model_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    model_api_id: int,
+    client_id: str,
 
+) -> Response[Union[
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
+        client=client,
+model_api_id=model_api_id,
 client_id=client_id,
-client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.delete(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    model_api_id: int,
+    client_id: str,
+
+) -> Optional[Union[
+    None,
+    None,
+    None
+]]:
+    """ Delete a model api client """
+
+    return (await asyncio_detailed(
+        client=client,
+model_api_id=model_api_id,
+client_id=client_id,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_pipeline_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_pipeline_api_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,158 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...types import Response
 
 
 def _get_kwargs(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/pipelineApis/{pipelineApiId}".format(
-        client.base_url,pipelineApiId=pipeline_api_id)
+    url = "{}/v1/pipelineApis/{pipelineApiId}/clients/{clientId}".format(
+        client.base_url,pipelineApiId=pipeline_api_id,clientId=client_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-
-
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 204:
+        response_204 = None
+
+        return response_204
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    if response.status_code == 404:
+        response_404 = None
+
+        return response_404
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
-) -> Response[Any]:
-    """Deletes the specified published data prep pipeline
-
-     Deletes the specified published data prep pipeline
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
+client_id=client_id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.delete(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    pipeline_api_id: int,
+def sync(
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
-) -> Response[Any]:
-    """Deletes the specified published data prep pipeline
-
-     Deletes the specified published data prep pipeline
-
-    Args:
-        pipeline_api_id (int):
+) -> Optional[Union[
+    None,
+    None,
+    None
+]]:
+    """ Delete a data prep pipeline api client """
+
+    return sync_detailed(
+        client=client,
+pipeline_api_id=pipeline_api_id,
+client_id=client_id,
 
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
+) -> Response[Union[
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
+client_id=client_id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.delete(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    pipeline_api_id: int,
+    client_id: str,
+
+) -> Optional[Union[
+    None,
+    None,
+    None
+]]:
+    """ Delete a data prep pipeline api client """
+
+    return (await asyncio_detailed(
+        client=client,
+pipeline_api_id=pipeline_api_id,
+client_id=client_id,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/delete_pipeline_api_client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_clients.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,152 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.deployed_api_client_list_response import DeployedApiClientListResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    pipeline_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    pipeline_api_id: int,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/pipelineApis/{pipelineApiId}/clients/{clientId}".format(
-        client.base_url,pipelineApiId=pipeline_api_id,clientId=client_id)
+    url = "{}/v1/pipelineApis/{pipelineApiId}/clients".format(
+        client.base_url,pipelineApiId=pipeline_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = DeployedApiClientListResponse.from_dict(response.json())
+
+
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    if response.status_code == 404:
+        response_404 = None
 
+        return response_404
+    return None
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    pipeline_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    pipeline_api_id: int,
 
-) -> Response[Any]:
-    """Delete a data prep pipeline api client
-
-     Delete a data prep pipeline api client
-
-    Args:
-        pipeline_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client_id=client_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    pipeline_api_id: int,
-    client_id: str,
+def sync(
     *,
     client: Client,
+    pipeline_api_id: int,
 
-) -> Response[Any]:
-    """Delete a data prep pipeline api client
-
-     Delete a data prep pipeline api client
+) -> Optional[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
+    """ Returns a list of all clients for a published data prep pipeline api """
+
+    return sync_detailed(
+        client=client,
+pipeline_api_id=pipeline_api_id,
 
-    Args:
-        pipeline_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    pipeline_api_id: int,
 
+) -> Response[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client_id=client_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    pipeline_api_id: int,
+
+) -> Optional[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
+    """ Returns a list of all clients for a published data prep pipeline api """
+
+    return (await asyncio_detailed(
+        client=client,
+pipeline_api_id=pipeline_api_id,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_model_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_model_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,194 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.deployed_model_api_response import DeployedModelApiResponse
 from ...models.edit_deployed_model_api_request import EditDeployedModelApiRequest
 from ...types import Response
 
 
 def _get_kwargs(
-    model_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
     json_body: EditDeployedModelApiRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/modelApis/{modelApiId}".format(
         client.base_url,modelApiId=model_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedModelApiResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
         response_200 = DeployedModelApiResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedModelApiResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    model_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
     json_body: EditDeployedModelApiRequest,
 
-) -> Response[Union[Any, DeployedModelApiResponse]]:
-    """Edit the specified published model
-
-     Edits the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (EditDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    model_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
     json_body: EditDeployedModelApiRequest,
 
-) -> Optional[Union[Any, DeployedModelApiResponse]]:
-    """Edit the specified published model
-
-     Edits the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (EditDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edits the specified published model """
 
     return sync_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    model_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
     json_body: EditDeployedModelApiRequest,
 
-) -> Response[Union[Any, DeployedModelApiResponse]]:
-    """Edit the specified published model
-
-     Edits the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (EditDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    model_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
     json_body: EditDeployedModelApiRequest,
 
-) -> Optional[Union[Any, DeployedModelApiResponse]]:
-    """Edit the specified published model
-
-     Edits the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (EditDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edits the specified published model """
 
     return (await asyncio_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_pipeline_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/edit_pipeline_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,194 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.deployed_pipeline_api_response import DeployedPipelineApiResponse
 from ...models.edit_deployed_pipeline_api_request import EditDeployedPipelineApiRequest
 from ...types import Response
 
 
 def _get_kwargs(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: EditDeployedPipelineApiRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/pipelineApis/{pipelineApiId}".format(
         client.base_url,pipelineApiId=pipeline_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedPipelineApiResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
         response_200 = DeployedPipelineApiResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedPipelineApiResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: EditDeployedPipelineApiRequest,
 
-) -> Response[Union[Any, DeployedPipelineApiResponse]]:
-    """Edit the specified published data prep pipeline
-
-     Edits the specified published data prep pipeline
-
-    Args:
-        pipeline_api_id (int):
-        json_body (EditDeployedPipelineApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: EditDeployedPipelineApiRequest,
 
-) -> Optional[Union[Any, DeployedPipelineApiResponse]]:
-    """Edit the specified published data prep pipeline
-
-     Edits the specified published data prep pipeline
-
-    Args:
-        pipeline_api_id (int):
-        json_body (EditDeployedPipelineApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edits the specified published data prep pipeline """
 
     return sync_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: EditDeployedPipelineApiRequest,
 
-) -> Response[Union[Any, DeployedPipelineApiResponse]]:
-    """Edit the specified published data prep pipeline
-
-     Edits the specified published data prep pipeline
-
-    Args:
-        pipeline_api_id (int):
-        json_body (EditDeployedPipelineApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
     json_body: EditDeployedPipelineApiRequest,
 
-) -> Optional[Union[Any, DeployedPipelineApiResponse]]:
-    """Edit the specified published data prep pipeline
-
-     Edits the specified published data prep pipeline
-
-    Args:
-        pipeline_api_id (int):
-        json_body (EditDeployedPipelineApiRequest):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edits the specified published data prep pipeline """
 
     return (await asyncio_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/save_model_result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.deployed_model_api_response import DeployedModelApiResponse
+from ...models.id_response import IdResponse
+from ...models.save_model_results_request import SaveModelResultsRequest
 from ...types import Response
 
 
 def _get_kwargs(
-    model_api_id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SaveModelResultsRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/modelApis/{modelApiId}".format(
-        client.base_url,modelApiId=model_api_id)
+    url = "{}/v1/models/{id}/results/save".format(
+        client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedModelApiResponse]]:
-    if response.status_code == 200:
-        response_200 = DeployedModelApiResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = IdResponse.from_dict(response.json())
 
 
 
-        return response_200
+        return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedModelApiResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    model_api_id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SaveModelResultsRequest,
 
-) -> Response[Union[Any, DeployedModelApiResponse]]:
-    """Gets an overview of the published model api
-
-     Gets general information about the published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
-
+) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    model_api_id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SaveModelResultsRequest,
 
-) -> Optional[Union[Any, DeployedModelApiResponse]]:
-    """Gets an overview of the published model api
-
-     Gets general information about the published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
+) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    """ Save the results of the specified model as a new data set - For classification & regression this result is the result of hold-out test, for clustering it is the clustered data. """
 
     return sync_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    model_api_id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SaveModelResultsRequest,
 
-) -> Response[Union[Any, DeployedModelApiResponse]]:
-    """Gets an overview of the published model api
-
-     Gets general information about the published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
-
+) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    model_api_id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SaveModelResultsRequest,
 
-) -> Optional[Union[Any, DeployedModelApiResponse]]:
-    """Gets an overview of the published model api
-
-     Gets general information about the published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedModelApiResponse]]
-    """
-
+) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    """ Save the results of the specified model as a new data set - For classification & regression this result is the result of hold-out test, for clustering it is the clustered data. """
 
     return (await asyncio_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api_clients.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_forecasting_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,174 +1,176 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.deployed_api_client_list_response import DeployedApiClientListResponse
+from ...models.create_forecasting_request import CreateForecastingRequest
+from ...models.create_model_response import CreateModelResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    model_api_id: int,
     *,
     client: Client,
+    json_body: CreateForecastingRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/modelApis/{modelApiId}/clients".format(
-        client.base_url,modelApiId=model_api_id)
+    url = "{}/v1/models/forecasting".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedApiClientListResponse]]:
-    if response.status_code == 200:
-        response_200 = DeployedApiClientListResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = CreateModelResponse.from_dict(response.json())
+
 
 
+        return response_201
+    if response.status_code == 400:
+        response_400 = None
 
-        return response_200
+        return response_400
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
+    if response.status_code == 403:
+        response_403 = None
+
+        return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedApiClientListResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    model_api_id: int,
     *,
     client: Client,
+    json_body: CreateForecastingRequest,
 
-) -> Response[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published model api
-
-     Returns a list of all clients for a published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    model_api_id: int,
     *,
     client: Client,
+    json_body: CreateForecastingRequest,
 
-) -> Optional[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published model api
-
-     Returns a list of all clients for a published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new time-series forecasting model with the supplied configuration. """
 
     return sync_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    model_api_id: int,
     *,
     client: Client,
+    json_body: CreateForecastingRequest,
 
-) -> Response[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published model api
-
-     Returns a list of all clients for a published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    model_api_id: int,
     *,
     client: Client,
+    json_body: CreateForecastingRequest,
 
-) -> Optional[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published model api
-
-     Returns a list of all clients for a published model api
-
-    Args:
-        model_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new time-series forecasting model with the supplied configuration. """
 
     return (await asyncio_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
+json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_apis.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_apis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.deployed_model_api_list_response import DeployedModelApiListResponse
 from ...types import Response
 
@@ -11,140 +11,123 @@
     *,
     client: Client,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/modelApis".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedModelApiListResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedModelApiListResponse,
+    None
+]]:
     if response.status_code == 200:
         response_200 = DeployedModelApiListResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedModelApiListResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedModelApiListResponse,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, DeployedModelApiListResponse]]:
-    """List all published model apis
-
-     Returns a list of all published model apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedModelApiListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedModelApiListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
 
-) -> Optional[Union[Any, DeployedModelApiListResponse]]:
-    """List all published model apis
-
-     Returns a list of all published model apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedModelApiListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedModelApiListResponse,
+    None
+]]:
+    """ Returns a list of all published model apis in the current project """
 
     return sync_detailed(
         client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, DeployedModelApiListResponse]]:
-    """List all published model apis
-
-     Returns a list of all published model apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedModelApiListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedModelApiListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
 
-) -> Optional[Union[Any, DeployedModelApiListResponse]]:
-    """List all published model apis
-
-     Returns a list of all published model apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedModelApiListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedModelApiListResponse,
+    None
+]]:
+    """ Returns a list of all published model apis in the current project """
 
     return (await asyncio_detailed(
         client=client,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,162 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.deployed_pipeline_api_response import DeployedPipelineApiResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/pipelineApis/{pipelineApiId}".format(
         client.base_url,pipelineApiId=pipeline_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedPipelineApiResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
         response_200 = DeployedPipelineApiResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedPipelineApiResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
 
-) -> Response[Union[Any, DeployedPipelineApiResponse]]:
-    """Gets an overview of the published data prep pipeline api
-
-     Gets general information about the published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
 
-) -> Optional[Union[Any, DeployedPipelineApiResponse]]:
-    """Gets an overview of the published data prep pipeline api
-
-     Gets general information about the published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Gets general information about the published data prep pipeline api """
 
     return sync_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 
     ).parsed
 
 async def asyncio_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
 
-) -> Response[Union[Any, DeployedPipelineApiResponse]]:
-    """Gets an overview of the published data prep pipeline api
-
-     Gets general information about the published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    pipeline_api_id: int,
     *,
     client: Client,
+    pipeline_api_id: int,
 
-) -> Optional[Union[Any, DeployedPipelineApiResponse]]:
-    """Gets an overview of the published data prep pipeline api
-
-     Gets general information about the published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedPipelineApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Gets general information about the published data prep pipeline api """
 
     return (await asyncio_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,161 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.deployed_api_client_response import DeployedApiClientResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    pipeline_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/pipelineApis/{pipelineApiId}/clients/{clientId}".format(
         client.base_url,pipelineApiId=pipeline_api_id,clientId=client_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedApiClientResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
     if response.status_code == 200:
         response_200 = DeployedApiClientResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedApiClientResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    pipeline_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
-) -> Response[Union[Any, DeployedApiClientResponse]]:
-    """Gets an overview of the published data prep pipeline api client
-
-     Gets an overview of the published data prep pipeline api client
-
-    Args:
-        pipeline_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 client_id=client_id,
-client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    pipeline_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
-) -> Optional[Union[Any, DeployedApiClientResponse]]:
-    """Gets an overview of the published data prep pipeline api client
-
-     Gets an overview of the published data prep pipeline api client
-
-    Args:
-        pipeline_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
+    """ Gets an overview of the published data prep pipeline api client """
 
     return sync_detailed(
-        pipeline_api_id=pipeline_api_id,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 client_id=client_id,
-client=client,
 
     ).parsed
 
 async def asyncio_detailed(
-    pipeline_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
-) -> Response[Union[Any, DeployedApiClientResponse]]:
-    """Gets an overview of the published data prep pipeline api client
-
-     Gets an overview of the published data prep pipeline api client
-
-    Args:
-        pipeline_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 client_id=client_id,
-client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    pipeline_api_id: int,
-    client_id: str,
     *,
     client: Client,
+    pipeline_api_id: int,
+    client_id: str,
 
-) -> Optional[Union[Any, DeployedApiClientResponse]]:
-    """Gets an overview of the published data prep pipeline api client
-
-     Gets an overview of the published data prep pipeline api client
-
-    Args:
-        pipeline_api_id (int):
-        client_id (str):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientResponse,
+    None,
+    None
+]]:
+    """ Gets an overview of the published data prep pipeline api client """
 
     return (await asyncio_detailed(
-        pipeline_api_id=pipeline_api_id,
+        client=client,
+pipeline_api_id=pipeline_api_id,
 client_id=client_id,
-client=client,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_api_clients.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/create_model_api_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,174 +1,167 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.deployed_api_client_list_response import DeployedApiClientListResponse
+from ...models.create_deployed_api_client_request import CreateDeployedApiClientRequest
+from ...models.deployed_api_client_create_response import (
+    DeployedApiClientCreateResponse,
+)
 from ...types import Response
 
 
 def _get_kwargs(
-    pipeline_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
+    json_body: CreateDeployedApiClientRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/pipelineApis/{pipelineApiId}/clients".format(
-        client.base_url,pipelineApiId=pipeline_api_id)
+    url = "{}/v1/modelApis/{modelApiId}/clients".format(
+        client.base_url,modelApiId=model_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedApiClientListResponse]]:
-    if response.status_code == 200:
-        response_200 = DeployedApiClientListResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = DeployedApiClientCreateResponse.from_dict(response.json())
 
 
 
-        return response_200
+        return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedApiClientListResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
+    json_body: CreateDeployedApiClientRequest,
 
-) -> Response[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published data prep pipeline api
-
-     Returns a list of all clients for a published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    pipeline_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
+    json_body: CreateDeployedApiClientRequest,
 
-) -> Optional[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published data prep pipeline api
-
-     Returns a list of all clients for a published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
+    """ Create a new client to access and use a given published model api and returns its new credentials (client id and secret) """
 
     return sync_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
+json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    pipeline_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
+    json_body: CreateDeployedApiClientRequest,
 
-) -> Response[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published data prep pipeline api
-
-     Returns a list of all clients for a published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    pipeline_api_id: int,
     *,
     client: Client,
+    model_api_id: int,
+    json_body: CreateDeployedApiClientRequest,
 
-) -> Optional[Union[Any, DeployedApiClientListResponse]]:
-    """List all clients for a published data prep pipeline api
-
-     Returns a list of all clients for a published data prep pipeline api
-
-    Args:
-        pipeline_api_id (int):
-
-    Returns:
-        Response[Union[Any, DeployedApiClientListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientCreateResponse,
+    None,
+    None
+]]:
+    """ Create a new client to access and use a given published model api and returns its new credentials (client id and secret) """
 
     return (await asyncio_detailed(
-        pipeline_api_id=pipeline_api_id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
+json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_apis.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_pipeline_apis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.deployed_pipeline_api_list_response import (
     DeployedPipelineApiListResponse,
 )
@@ -13,140 +13,123 @@
     *,
     client: Client,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/pipelineApis".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DeployedPipelineApiListResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedPipelineApiListResponse,
+    None
+]]:
     if response.status_code == 200:
         response_200 = DeployedPipelineApiListResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DeployedPipelineApiListResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedPipelineApiListResponse,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, DeployedPipelineApiListResponse]]:
-    """List all published data prep pipeline apis
-
-     Returns a list of all published data prep pipeline apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedPipelineApiListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
 
-) -> Optional[Union[Any, DeployedPipelineApiListResponse]]:
-    """List all published data prep pipeline apis
-
-     Returns a list of all published data prep pipeline apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedPipelineApiListResponse,
+    None
+]]:
+    """ Returns a list of all published data prep pipeline apis in the current project """
 
     return sync_detailed(
         client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, DeployedPipelineApiListResponse]]:
-    """List all published data prep pipeline apis
-
-     Returns a list of all published data prep pipeline apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedPipelineApiListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
 
-) -> Optional[Union[Any, DeployedPipelineApiListResponse]]:
-    """List all published data prep pipeline apis
-
-     Returns a list of all published data prep pipeline apis in the current project
-
-    Returns:
-        Response[Union[Any, DeployedPipelineApiListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedPipelineApiListResponse,
+    None
+]]:
+    """ Returns a list of all published data prep pipeline apis in the current project """
 
     return (await asyncio_detailed(
         client=client,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/ap_is/replace_model_api.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_decisioning_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,194 +1,176 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.future import Future
-from ...models.update_deployed_model_api_request import UpdateDeployedModelApiRequest
+from ...models.create_decisioning_request import CreateDecisioningRequest
+from ...models.create_model_response import CreateModelResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    model_api_id: int,
     *,
     client: Client,
-    json_body: UpdateDeployedModelApiRequest,
+    json_body: CreateDecisioningRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/modelApis/{modelApiId}/replace".format(
-        client.base_url,modelApiId=model_api_id)
+    url = "{}/v1/models/decisioning".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Future]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 201:
-        response_201 = Future.from_dict(response.json())
+        response_201 = CreateModelResponse.from_dict(response.json())
 
 
 
         return response_201
+    if response.status_code == 400:
+        response_400 = None
+
+        return response_400
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Future]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    model_api_id: int,
     *,
     client: Client,
-    json_body: UpdateDeployedModelApiRequest,
-
-) -> Response[Union[Any, Future]]:
-    """Update the model being published by the specified published model
-
-     Updates the model for the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (UpdateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+    json_body: CreateDecisioningRequest,
 
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    model_api_id: int,
     *,
     client: Client,
-    json_body: UpdateDeployedModelApiRequest,
-
-) -> Optional[Union[Any, Future]]:
-    """Update the model being published by the specified published model
-
-     Updates the model for the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (UpdateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
+    json_body: CreateDecisioningRequest,
 
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new decisioning model. Also configures the model if a configuration is supplied. If no configuration is supplied the model can later be configured by calling the '/v1/models/decisioning/{modelId}/configure' endpoint. """
 
     return sync_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    model_api_id: int,
     *,
     client: Client,
-    json_body: UpdateDeployedModelApiRequest,
-
-) -> Response[Union[Any, Future]]:
-    """Update the model being published by the specified published model
-
-     Updates the model for the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (UpdateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+    json_body: CreateDecisioningRequest,
 
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    model_api_id: int,
     *,
     client: Client,
-    json_body: UpdateDeployedModelApiRequest,
-
-) -> Optional[Union[Any, Future]]:
-    """Update the model being published by the specified published model
-
-     Updates the model for the specified published model
-
-    Args:
-        model_api_id (int):
-        json_body (UpdateDeployedModelApiRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
+    json_body: CreateDecisioningRequest,
 
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new decisioning model. Also configures the model if a configuration is supplied. If no configuration is supplied the model can later be configured by calling the '/v1/models/decisioning/{modelId}/configure' endpoint. """
 
     return (await asyncio_detailed(
-        model_api_id=model_api_id,
-client=client,
+        client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/create_http_data_set.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_http_data_set.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.create_http_data_set_request import CreateHttpDataSetRequest
 from ...models.future import Future
 from ...types import Response
@@ -13,171 +13,134 @@
     client: Client,
     json_body: CreateHttpDataSetRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/dataSets/http".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Future]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    Future,
+    None
+]]:
     if response.status_code == 201:
         response_201 = Future.from_dict(response.json())
 
 
 
         return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Future]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    Future,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     json_body: CreateHttpDataSetRequest,
 
-) -> Response[Union[Any, Future]]:
-    """Create a new data set from a file at a URL
-
-     Your data will start being imported immediately. The response will contain a `futureId` which you
-    can use with the `/futures` endpoint to check the progress of your import. Upon completion the
-    future will give you information about the resulting data set.
-
-    Args:
-        json_body (CreateHttpDataSetRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
-
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
     json_body: CreateHttpDataSetRequest,
 
-) -> Optional[Union[Any, Future]]:
-    """Create a new data set from a file at a URL
-
-     Your data will start being imported immediately. The response will contain a `futureId` which you
-    can use with the `/futures` endpoint to check the progress of your import. Upon completion the
-    future will give you information about the resulting data set.
-
-    Args:
-        json_body (CreateHttpDataSetRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
     json_body: CreateHttpDataSetRequest,
 
-) -> Response[Union[Any, Future]]:
-    """Create a new data set from a file at a URL
-
-     Your data will start being imported immediately. The response will contain a `futureId` which you
-    can use with the `/futures` endpoint to check the progress of your import. Upon completion the
-    future will give you information about the resulting data set.
-
-    Args:
-        json_body (CreateHttpDataSetRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
-
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
     json_body: CreateHttpDataSetRequest,
 
-) -> Optional[Union[Any, Future]]:
-    """Create a new data set from a file at a URL
-
-     Your data will start being imported immediately. The response will contain a `futureId` which you
-    can use with the `/futures` endpoint to check the progress of your import. Upon completion the
-    future will give you information about the resulting data set.
-
-    Args:
-        json_body (CreateHttpDataSetRequest):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/delete_data_set.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,113 +1,133 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.data_sets_response import DataSetsResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataSets/{id}".format(
-        client.base_url,id=id)
+    url = "{}/v1/dataSets".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DataSetsResponse,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = DataSetsResponse.from_dict(response.json())
+
+
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DataSetsResponse,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
 
-) -> Response[Any]:
-    """Deletes the specified data set
-
-     Deletes the specified data set
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    DataSetsResponse,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
 
-) -> Response[Any]:
-    """Deletes the specified data set
-
-     Deletes the specified data set
+) -> Optional[Union[
+    DataSetsResponse,
+    None
+]]:
+    """ Returns a list of all the datasets in the current project """
 
-    Args:
-        id (int):
+    return sync_detailed(
+        client=client,
 
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
 
+) -> Response[Union[
+    DataSetsResponse,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+
+) -> Optional[Union[
+    DataSetsResponse,
+    None
+]]:
+    """ Returns a list of all the datasets in the current project """
+
+    return (await asyncio_detailed(
+        client=client,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/edit_data_set.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_classification_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,194 +1,176 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.data_set_response import DataSetResponse
-from ...models.edit_data_set_request import EditDataSetRequest
+from ...models.create_classification_request import CreateClassificationRequest
+from ...models.create_model_response import CreateModelResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
-    json_body: EditDataSetRequest,
+    json_body: CreateClassificationRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataSets/{id}".format(
-        client.base_url,id=id)
+    url = "{}/v1/models/classification".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DataSetResponse]]:
-    if response.status_code == 200:
-        response_200 = DataSetResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = CreateModelResponse.from_dict(response.json())
+
 
 
+        return response_201
+    if response.status_code == 400:
+        response_400 = None
 
-        return response_200
+        return response_400
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DataSetResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
-    json_body: EditDataSetRequest,
-
-) -> Response[Union[Any, DataSetResponse]]:
-    """Edit the specified data set
-
-     Edits the specified data set
-
-    Args:
-        id (int):
-        json_body (EditDataSetRequest):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
-
+    json_body: CreateClassificationRequest,
 
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
-    json_body: EditDataSetRequest,
-
-) -> Optional[Union[Any, DataSetResponse]]:
-    """Edit the specified data set
-
-     Edits the specified data set
-
-    Args:
-        id (int):
-        json_body (EditDataSetRequest):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
+    json_body: CreateClassificationRequest,
 
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new classification model with the supplied configuration and starts the model search process process. """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
-    json_body: EditDataSetRequest,
-
-) -> Response[Union[Any, DataSetResponse]]:
-    """Edit the specified data set
-
-     Edits the specified data set
-
-    Args:
-        id (int):
-        json_body (EditDataSetRequest):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
-
+    json_body: CreateClassificationRequest,
 
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
-    json_body: EditDataSetRequest,
-
-) -> Optional[Union[Any, DataSetResponse]]:
-    """Edit the specified data set
-
-     Edits the specified data set
-
-    Args:
-        id (int):
-        json_body (EditDataSetRequest):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
+    json_body: CreateClassificationRequest,
 
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new classification model with the supplied configuration and starts the model search process process. """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_set.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,177 +1,152 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.data_set_response import DataSetResponse
+from ...models.prediction_response import PredictionResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    id: int,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataSets/{id}".format(
+    url = "{}/v1/predictions/{id}".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DataSetResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = DataSetResponse.from_dict(response.json())
+        response_200 = PredictionResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
-    if response.status_code == 403:
-        response_403 = cast(Any, None)
-        return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DataSetResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Response[Union[Any, DataSetResponse]]:
-    """Gets an overview of the data set
-
-     Gets general information about the data set
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
-
-
+) -> Response[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Optional[Union[Any, DataSetResponse]]:
-    """Gets an overview of the data set
-
-     Gets general information about the data set
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
-
+) -> Optional[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
+    """ Gets general information about the prediction, including the current status """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Response[Union[Any, DataSetResponse]]:
-    """Gets an overview of the data set
-
-     Gets general information about the data set
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
-
-
+) -> Response[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Optional[Union[Any, DataSetResponse]]:
-    """Gets an overview of the data set
-
-     Gets general information about the data set
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataSetResponse]]
-    """
-
+) -> Optional[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
+    """ Gets general information about the prediction, including the current status """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/get_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,133 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.data_sets_response import DataSetsResponse
+from ...models.test_list_response import TestListResponse
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataSets".format(
+    url = "{}/v1/tests".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DataSetsResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    TestListResponse,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = DataSetsResponse.from_dict(response.json())
+        response_200 = TestListResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DataSetsResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    TestListResponse,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, DataSetsResponse]]:
-    """List all data sets
-
-     Returns a list of all the datasets in the current project
-
-    Returns:
-        Response[Union[Any, DataSetsResponse]]
-    """
-
-
+) -> Response[Union[
+    TestListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
 
-) -> Optional[Union[Any, DataSetsResponse]]:
-    """List all data sets
-
-     Returns a list of all the datasets in the current project
-
-    Returns:
-        Response[Union[Any, DataSetsResponse]]
-    """
-
+) -> Optional[Union[
+    TestListResponse,
+    None
+]]:
+    """ Returns a list of all tests in the current project """
 
     return sync_detailed(
         client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, DataSetsResponse]]:
-    """List all data sets
-
-     Returns a list of all the datasets in the current project
-
-    Returns:
-        Response[Union[Any, DataSetsResponse]]
-    """
-
-
+) -> Response[Union[
+    TestListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
 
-) -> Optional[Union[Any, DataSetsResponse]]:
-    """List all data sets
-
-     Returns a list of all the datasets in the current project
-
-    Returns:
-        Response[Union[Any, DataSetsResponse]]
-    """
-
+) -> Optional[Union[
+    TestListResponse,
+    None
+]]:
+    """ Returns a list of all tests in the current project """
 
     return (await asyncio_detailed(
         client=client,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets_csv_data.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_result_csv_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,157 +1,193 @@
-from typing import Any, Dict, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataSets/{id}/data/csv".format(
+    url = "{}/v1/predictions/{id}/data/csv".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
-    params: Dict[str, Any] = {}
-    params["separator"] = separator
-
-
-    params["quoteChar"] = quote_char
-
-
-    params["escapeChar"] = escape_char
-
-
-    params["charset"] = charset
-
-
-
+    params: Dict[str, Any] = {
+        "separator": separator,
+        "quoteChar": quote_char,
+        "escapeChar": escape_char,
+    }
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-
-
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    None,
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = None
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    if response.status_code == 403:
+        response_403 = None
+
+        return response_403
+    if response.status_code == 404:
+        response_404 = None
+
+        return response_404
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
-
-) -> Response[Any]:
-    """Get the data in CSV format
-
-     Get the data from the latest version of the data set as a csv file
-
-    Args:
-        id (int):
-        separator (Union[Unset, None, str]):
-        quote_char (Union[Unset, None, str]):
-        escape_char (Union[Unset, None, str]):
-        charset (Union[Unset, None, str]):  Default: 'UTF-8'.
-
-    Returns:
-        Response[Any]
-    """
-
-
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Response[Union[
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 separator=separator,
 quote_char=quote_char,
 escape_char=escape_char,
-charset=charset,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
-
-) -> Response[Any]:
-    """Get the data in CSV format
-
-     Get the data from the latest version of the data set as a csv file
-
-    Args:
-        id (int):
-        separator (Union[Unset, None, str]):
-        quote_char (Union[Unset, None, str]):
-        escape_char (Union[Unset, None, str]):
-        charset (Union[Unset, None, str]):  Default: 'UTF-8'.
-
-    Returns:
-        Response[Any]
-    """
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Optional[Union[
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Get the prediction result as a csv file """
+
+    return sync_detailed(
+        client=client,
+id=id,
+separator=separator,
+quote_char=quote_char,
+escape_char=escape_char,
 
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Response[Union[
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 separator=separator,
 quote_char=quote_char,
 escape_char=escape_char,
-charset=charset,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Optional[Union[
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Get the prediction result as a csv file """
+
+    return (await asyncio_detailed(
+        client=client,
+id=id,
+separator=separator,
+quote_char=quote_char,
+escape_char=escape_char,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/data/get_data_sets_parquet_data.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/get_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,113 +1,133 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.model_list_response import ModelListResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataSets/{id}/data/parquet".format(
-        client.base_url,id=id)
+    url = "{}/v1/models".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    ModelListResponse,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = ModelListResponse.from_dict(response.json())
+
+
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    ModelListResponse,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
 
-) -> Response[Any]:
-    """Get the data in parquet file format
-
-     Get the data from the latest version of the data set as a parquet file
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    ModelListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
 
-) -> Response[Any]:
-    """Get the data in parquet file format
-
-     Get the data from the latest version of the data set as a parquet file
+) -> Optional[Union[
+    ModelListResponse,
+    None
+]]:
+    """ Returns a list of all models in the current project """
 
-    Args:
-        id (int):
+    return sync_detailed(
+        client=client,
 
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
 
+) -> Response[Union[
+    ModelListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+
+) -> Optional[Union[
+    ModelListResponse,
+    None
+]]:
+    """ Returns a list of all models in the current project """
+
+    return (await asyncio_detailed(
+        client=client,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_auto_clustering_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_auto_clustering_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.create_auto_clustering_request import CreateAutoClusteringRequest
 from ...models.create_model_response import CreateModelResponse
 from ...types import Response
@@ -13,172 +13,164 @@
     client: Client,
     json_body: CreateAutoClusteringRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/models/autoclustering".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, CreateModelResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 201:
         response_201 = CreateModelResponse.from_dict(response.json())
 
 
 
         return response_201
     if response.status_code == 400:
-        response_400 = cast(Any, None)
+        response_400 = None
+
         return response_400
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, CreateModelResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     json_body: CreateAutoClusteringRequest,
 
-) -> Response[Union[Any, CreateModelResponse]]:
-    """Create a clustering model, automatically determining the optimal number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateAutoClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
     json_body: CreateAutoClusteringRequest,
 
-) -> Optional[Union[Any, CreateModelResponse]]:
-    """Create a clustering model, automatically determining the optimal number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateAutoClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new clustering model with the supplied configuration. """
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
     json_body: CreateAutoClusteringRequest,
 
-) -> Response[Union[Any, CreateModelResponse]]:
-    """Create a clustering model, automatically determining the optimal number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateAutoClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
     json_body: CreateAutoClusteringRequest,
 
-) -> Optional[Union[Any, CreateModelResponse]]:
-    """Create a clustering model, automatically determining the optimal number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateAutoClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new clustering model with the supplied configuration. """
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_clustering_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_clustering_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.create_clustering_request import CreateClusteringRequest
 from ...models.create_model_response import CreateModelResponse
 from ...types import Response
@@ -13,172 +13,164 @@
     client: Client,
     json_body: CreateClusteringRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/models/clustering".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, CreateModelResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 201:
         response_201 = CreateModelResponse.from_dict(response.json())
 
 
 
         return response_201
     if response.status_code == 400:
-        response_400 = cast(Any, None)
+        response_400 = None
+
         return response_400
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, CreateModelResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     json_body: CreateClusteringRequest,
 
-) -> Response[Union[Any, CreateModelResponse]]:
-    """Create a clustering model with a specified number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
     json_body: CreateClusteringRequest,
 
-) -> Optional[Union[Any, CreateModelResponse]]:
-    """Create a clustering model with a specified number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new clustering model with the supplied configuration. """
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
     json_body: CreateClusteringRequest,
 
-) -> Response[Union[Any, CreateModelResponse]]:
-    """Create a clustering model with a specified number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
     json_body: CreateClusteringRequest,
 
-) -> Optional[Union[Any, CreateModelResponse]]:
-    """Create a clustering model with a specified number of clusters.
-
-     Creates a new clustering model with the supplied configuration.
-
-    Args:
-        json_body (CreateClusteringRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new clustering model with the supplied configuration. """
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/create_regression_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/create_regression_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.create_model_response import CreateModelResponse
 from ...models.create_regression_request import CreateRegressionRequest
 from ...types import Response
@@ -13,176 +13,164 @@
     client: Client,
     json_body: CreateRegressionRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/models/regression".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, CreateModelResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 201:
         response_201 = CreateModelResponse.from_dict(response.json())
 
 
 
         return response_201
     if response.status_code == 400:
-        response_400 = cast(Any, None)
+        response_400 = None
+
         return response_400
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, CreateModelResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     json_body: CreateRegressionRequest,
 
-) -> Response[Union[Any, CreateModelResponse]]:
-    """Create a regression model and start the model search.
-
-     Creates a new regression model with the supplied configuration and starts the model search process
-    process.
-
-    Args:
-        json_body (CreateRegressionRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
     json_body: CreateRegressionRequest,
 
-) -> Optional[Union[Any, CreateModelResponse]]:
-    """Create a regression model and start the model search.
-
-     Creates a new regression model with the supplied configuration and starts the model search process
-    process.
-
-    Args:
-        json_body (CreateRegressionRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new regression model with the supplied configuration and starts the model search process process. """
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
     json_body: CreateRegressionRequest,
 
-) -> Response[Union[Any, CreateModelResponse]]:
-    """Create a regression model and start the model search.
-
-     Creates a new regression model with the supplied configuration and starts the model search process
-    process.
-
-    Args:
-        json_body (CreateRegressionRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
     json_body: CreateRegressionRequest,
 
-) -> Optional[Union[Any, CreateModelResponse]]:
-    """Create a regression model and start the model search.
-
-     Creates a new regression model with the supplied configuration and starts the model search process
-    process.
-
-    Args:
-        json_body (CreateRegressionRequest):
-
-    Returns:
-        Response[Union[Any, CreateModelResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Creates a new regression model with the supplied configuration and starts the model search process process. """
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/edit_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/delete_data_prep_steps.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.edit_model_request import EditModelRequest
-from ...models.model_response import ModelResponse
+from ...models.delete_data_prep_steps_request import DeleteDataPrepStepsRequest
+from ...models.future import Future
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
-    json_body: EditModelRequest,
+    id: int,
+    json_body: DeleteDataPrepStepsRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/models/{id}".format(
+    url = "{}/v1/dataSets/{id}/dataPrepSteps".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ModelResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    Future,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = ModelResponse.from_dict(response.json())
+        response_200 = Future.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ModelResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    Future,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
-    json_body: EditModelRequest,
-
-) -> Response[Union[Any, ModelResponse]]:
-    """Edit the name and description of the specified model
-
-     Edit the name and description of the specified model
-
-    Args:
-        id (int):
-        json_body (EditModelRequest):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
-
+    id: int,
+    json_body: DeleteDataPrepStepsRequest,
 
+) -> Response[Union[
+    Future,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.delete(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
-    json_body: EditModelRequest,
-
-) -> Optional[Union[Any, ModelResponse]]:
-    """Edit the name and description of the specified model
-
-     Edit the name and description of the specified model
-
-    Args:
-        id (int):
-        json_body (EditModelRequest):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
+    id: int,
+    json_body: DeleteDataPrepStepsRequest,
 
+) -> Optional[Union[
+    Future,
+    None,
+    None,
+    None
+]]:
+    """ Deletes the specified data prep steps from the dataset. This may take some time as later steps need to be reapplied so a future is returned. """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
-    json_body: EditModelRequest,
-
-) -> Response[Union[Any, ModelResponse]]:
-    """Edit the name and description of the specified model
-
-     Edit the name and description of the specified model
-
-    Args:
-        id (int):
-        json_body (EditModelRequest):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
-
+    id: int,
+    json_body: DeleteDataPrepStepsRequest,
 
+) -> Response[Union[
+    Future,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.delete(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
-    json_body: EditModelRequest,
-
-) -> Optional[Union[Any, ModelResponse]]:
-    """Edit the name and description of the specified model
-
-     Edit the name and description of the specified model
-
-    Args:
-        id (int):
-        json_body (EditModelRequest):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
+    id: int,
+    json_body: DeleteDataPrepStepsRequest,
 
+) -> Optional[Union[
+    Future,
+    None,
+    None,
+    None
+]]:
+    """ Deletes the specified data prep steps from the dataset. This may take some time as later steps need to be reapplied so a future is returned. """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api_clients.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,174 +1,152 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.model_response import ModelResponse
+from ...models.deployed_api_client_list_response import DeployedApiClientListResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    model_api_id: int,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/models/{id}".format(
-        client.base_url,id=id)
+    url = "{}/v1/modelApis/{modelApiId}/clients".format(
+        client.base_url,modelApiId=model_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ModelResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = ModelResponse.from_dict(response.json())
+        response_200 = DeployedApiClientListResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ModelResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Response[Union[Any, ModelResponse]]:
-    """Get information about a model
-
-     Returns information about a specific model in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Optional[Union[Any, ModelResponse]]:
-    """Get information about a model
-
-     Returns information about a specific model in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
+    """ Returns a list of all clients for a published model api """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Response[Union[Any, ModelResponse]]:
-    """Get information about a model
-
-     Returns information about a specific model in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Optional[Union[Any, ModelResponse]]:
-    """Get information about a model
-
-     Returns information about a specific model in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, ModelResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedApiClientListResponse,
+    None,
+    None
+]]:
+    """ Returns a list of all clients for a published model api """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+model_api_id=model_api_id,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_model_result_csv_data.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_csv_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,193 @@
-from typing import Any, Dict, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/models/{id}/results/csv".format(
+    url = "{}/v1/tests/{id}/data/csv".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
-    params: Dict[str, Any] = {}
-    params["separator"] = separator
-
-
-    params["quoteChar"] = quote_char
-
-
-    params["escapeChar"] = escape_char
-
-
-    params["charset"] = charset
-
-
-
+    params: Dict[str, Any] = {
+        "separator": separator,
+        "quoteChar": quote_char,
+        "escapeChar": escape_char,
+    }
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-
-
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    None,
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = None
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    if response.status_code == 403:
+        response_403 = None
+
+        return response_403
+    if response.status_code == 404:
+        response_404 = None
+
+        return response_404
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
-
-) -> Response[Any]:
-    """Get the model result in CSV format
-
-     Get the model result as a csv file - For classification & regression this result is the result of
-    hold-out test, for clustering it is the clustered data.
-
-    Args:
-        id (int):
-        separator (Union[Unset, None, str]):
-        quote_char (Union[Unset, None, str]):
-        escape_char (Union[Unset, None, str]):
-        charset (Union[Unset, None, str]):  Default: 'UTF-8'.
-
-    Returns:
-        Response[Any]
-    """
-
-
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Response[Union[
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 separator=separator,
 quote_char=quote_char,
 escape_char=escape_char,
-charset=charset,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
-
-) -> Response[Any]:
-    """Get the model result in CSV format
-
-     Get the model result as a csv file - For classification & regression this result is the result of
-    hold-out test, for clustering it is the clustered data.
-
-    Args:
-        id (int):
-        separator (Union[Unset, None, str]):
-        quote_char (Union[Unset, None, str]):
-        escape_char (Union[Unset, None, str]):
-        charset (Union[Unset, None, str]):  Default: 'UTF-8'.
-
-    Returns:
-        Response[Any]
-    """
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Optional[Union[
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Get the test result as a csv file """
+
+    return sync_detailed(
+        client=client,
+id=id,
+separator=separator,
+quote_char=quote_char,
+escape_char=escape_char,
 
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Response[Union[
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 separator=separator,
 quote_char=quote_char,
 escape_char=escape_char,
-charset=charset,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    id: int,
+    separator: Union[Unset, str] = UNSET,
+    quote_char: Union[Unset, str] = UNSET,
+    escape_char: Union[Unset, str] = UNSET,
+
+) -> Optional[Union[
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Get the test result as a csv file """
+
+    return (await asyncio_detailed(
+        client=client,
+id=id,
+separator=separator,
+quote_char=quote_char,
+escape_char=escape_char,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_model_result_parquet_data.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_db_data_set.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,115 +1,146 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.create_db_data_set_request import CreateDbDataSetRequest
+from ...models.future import Future
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    json_body: CreateDbDataSetRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/models/{id}/results/parquet".format(
-        client.base_url,id=id)
+    url = "{}/v1/dataSets/db".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    Future,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = Future.from_dict(response.json())
+
+
+
+        return response_201
+    if response.status_code == 401:
+        response_401 = None
 
+        return response_401
+    return None
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    Future,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    json_body: CreateDbDataSetRequest,
 
-) -> Response[Any]:
-    """Get the model result in parquet file format
-
-     Get the model result as a parquet file - For classification & regression this result is the result
-    of hold-out test, for clustering it is the clustered data.
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
+    json_body: CreateDbDataSetRequest,
 
-) -> Response[Any]:
-    """Get the model result in parquet file format
-
-     Get the model result as a parquet file - For classification & regression this result is the result
-    of hold-out test, for clustering it is the clustered data.
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
+
+    return sync_detailed(
+        client=client,
+json_body=json_body,
 
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    json_body: CreateDbDataSetRequest,
 
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    json_body: CreateDbDataSetRequest,
+
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
+
+    return (await asyncio_detailed(
+        client=client,
+json_body=json_body,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/get_models.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/pipelines/get_data_pipelines.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,150 +1,133 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.model_list_response import ModelListResponse
+from ...models.data_pipelines_response import DataPipelinesResponse
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/models".format(
+    url = "{}/v1/dataPipelines".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, ModelListResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DataPipelinesResponse,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = ModelListResponse.from_dict(response.json())
+        response_200 = DataPipelinesResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, ModelListResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DataPipelinesResponse,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, ModelListResponse]]:
-    """List all models
-
-     Returns a list of all models in the current project
-
-    Returns:
-        Response[Union[Any, ModelListResponse]]
-    """
-
-
+) -> Response[Union[
+    DataPipelinesResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
 
-) -> Optional[Union[Any, ModelListResponse]]:
-    """List all models
-
-     Returns a list of all models in the current project
-
-    Returns:
-        Response[Union[Any, ModelListResponse]]
-    """
-
+) -> Optional[Union[
+    DataPipelinesResponse,
+    None
+]]:
+    """ Returns a list of all the data prep pipelines in the current project """
 
     return sync_detailed(
         client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
 
-) -> Response[Union[Any, ModelListResponse]]:
-    """List all models
-
-     Returns a list of all models in the current project
-
-    Returns:
-        Response[Union[Any, ModelListResponse]]
-    """
-
-
+) -> Response[Union[
+    DataPipelinesResponse,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
 
-) -> Optional[Union[Any, ModelListResponse]]:
-    """List all models
-
-     Returns a list of all models in the current project
-
-    Returns:
-        Response[Union[Any, ModelListResponse]]
-    """
-
+) -> Optional[Union[
+    DataPipelinesResponse,
+    None
+]]:
+    """ Returns a list of all the data prep pipelines in the current project """
 
     return (await asyncio_detailed(
         client=client,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/models/stop_model.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/deprecated/create_data_set.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,144 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.create_data_set_request import CreateDataSetRequest
+from ...models.future import Future
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    multipart_data: CreateDataSetRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/models/{id}/stop".format(
-        client.base_url,id=id)
+    url = "{}/v1/dataSets".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "files": multipart_data.to_dict(),
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    Future,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = Future.from_dict(response.json())
+
+
+
+        return response_201
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    Future,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    multipart_data: CreateDataSetRequest,
 
-) -> Response[Any]:
-    """Complete the model optimization process.
-
-     Complete the model optimization process, taking the current best result as the final model. Post
-    build analysis steps will still be run
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+multipart_data=multipart_data,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
+    multipart_data: CreateDataSetRequest,
 
-) -> Response[Any]:
-    """Complete the model optimization process.
-
-     Complete the model optimization process, taking the current best result as the final model. Post
-    build analysis steps will still be run
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
+
+    return sync_detailed(
+        client=client,
+multipart_data=multipart_data,
 
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    multipart_data: CreateDataSetRequest,
 
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+multipart_data=multipart_data,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    multipart_data: CreateDataSetRequest,
+
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
+
+    return (await asyncio_detailed(
+        client=client,
+multipart_data=multipart_data,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/other/get_future.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/save_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,163 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.future import Future
+from ...models.id_response import IdResponse
+from ...models.save_test_request import SaveTestRequest
 from ...types import Response
 
 
 def _get_kwargs(
-    future_id: str,
     *,
     client: Client,
+    id: int,
+    json_body: SaveTestRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/futures/{futureId}".format(
-        client.base_url,futureId=future_id)
+    url = "{}/v1/tests/{id}/save".format(
+        client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, Future]]:
-    if response.status_code == 200:
-        response_200 = Future.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = IdResponse.from_dict(response.json())
 
 
 
-        return response_200
+        return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
+    if response.status_code == 403:
+        response_403 = None
+
+        return response_403
+    if response.status_code == 404:
+        response_404 = None
+
+        return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, Future]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    future_id: str,
     *,
     client: Client,
+    id: int,
+    json_body: SaveTestRequest,
 
-) -> Response[Union[Any, Future]]:
-    """Check on the progress of your request
-
-    Args:
-        future_id (str):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
-
+) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        future_id=future_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    future_id: str,
     *,
     client: Client,
+    id: int,
+    json_body: SaveTestRequest,
 
-) -> Optional[Union[Any, Future]]:
-    """Check on the progress of your request
-
-    Args:
-        future_id (str):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    """ Save the results of the specified test as a new data set """
 
     return sync_detailed(
-        future_id=future_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    future_id: str,
     *,
     client: Client,
+    id: int,
+    json_body: SaveTestRequest,
 
-) -> Response[Union[Any, Future]]:
-    """Check on the progress of your request
-
-    Args:
-        future_id (str):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
-
+) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        future_id=future_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    future_id: str,
     *,
     client: Client,
+    id: int,
+    json_body: SaveTestRequest,
 
-) -> Optional[Union[Any, Future]]:
-    """Check on the progress of your request
-
-    Args:
-        future_id (str):
-
-    Returns:
-        Response[Union[Any, Future]]
-    """
-
+) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    """ Save the results of the specified test as a new data set """
 
     return (await asyncio_detailed(
-        future_id=future_id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/delete_data_pipeline.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_predictions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,133 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.prediction_list_response import PredictionListResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataPipelines/{id}".format(
-        client.base_url,id=id)
+    url = "{}/v1/predictions".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    PredictionListResponse,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = PredictionListResponse.from_dict(response.json())
+
+
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    PredictionListResponse,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
 
-) -> Response[Any]:
-    """Deletes the specified data prep pipeline
-
-     Deletes the specified data prep pipeline
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    PredictionListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
 
-) -> Response[Any]:
-    """Deletes the specified data prep pipeline
-
-     Deletes the specified data prep pipeline
+) -> Optional[Union[
+    PredictionListResponse,
+    None
+]]:
+    """ Returns a list of all predictions in the current project """
 
-    Args:
-        id (int):
+    return sync_detailed(
+        client=client,
 
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
 
+) -> Response[Union[
+    PredictionListResponse,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+
+) -> Optional[Union[
+    PredictionListResponse,
+    None
+]]:
+    """ Returns a list of all predictions in the current project """
+
+    return (await asyncio_detailed(
+        client=client,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/pipelines/get_data_pipeline.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/edit_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,177 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.data_pipeline_response import DataPipelineResponse
+from ...models.edit_test_request import EditTestRequest
+from ...models.test_response import TestResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: EditTestRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/dataPipelines/{id}".format(
+    url = "{}/v1/tests/{id}".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, DataPipelineResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    TestResponse,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = DataPipelineResponse.from_dict(response.json())
+        response_200 = TestResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, DataPipelineResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    TestResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: EditTestRequest,
 
-) -> Response[Union[Any, DataPipelineResponse]]:
-    """Get information about a data prep pipeline
-
-     Returns information about a specific data prep pipeline in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataPipelineResponse]]
-    """
-
-
+) -> Response[Union[
+    TestResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: EditTestRequest,
 
-) -> Optional[Union[Any, DataPipelineResponse]]:
-    """Get information about a data prep pipeline
-
-     Returns information about a specific data prep pipeline in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataPipelineResponse]]
-    """
-
+) -> Optional[Union[
+    TestResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edit the name and description of the specified test """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: EditTestRequest,
 
-) -> Response[Union[Any, DataPipelineResponse]]:
-    """Get information about a data prep pipeline
-
-     Returns information about a specific data prep pipeline in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataPipelineResponse]]
-    """
-
-
+) -> Response[Union[
+    TestResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: EditTestRequest,
 
-) -> Optional[Union[Any, DataPipelineResponse]]:
-    """Get information about a data prep pipeline
-
-     Returns information about a specific data prep pipeline in the current project
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, DataPipelineResponse]]
-    """
-
+) -> Optional[Union[
+    TestResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edit the name and description of the specified test """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/create_prediction.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/create_prediction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.create_prediction_request import CreatePredictionRequest
 from ...models.prediction_response import PredictionResponse
 from ...types import Response
@@ -13,170 +13,144 @@
     client: Client,
     json_body: CreatePredictionRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/predictions".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, PredictionResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     if response.status_code == 201:
         response_201 = PredictionResponse.from_dict(response.json())
 
 
 
         return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, PredictionResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     json_body: CreatePredictionRequest,
 
-) -> Response[Union[Any, PredictionResponse]]:
-    """Create a new prediction
-
-     Create a new prediction using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreatePredictionRequest):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
-
+) -> Response[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
     json_body: CreatePredictionRequest,
 
-) -> Optional[Union[Any, PredictionResponse]]:
-    """Create a new prediction
-
-     Create a new prediction using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreatePredictionRequest):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
+) -> Optional[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
+    """ Create a new prediction using the model identified by the modelId and the data set identified by the dataSetId """
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
     json_body: CreatePredictionRequest,
 
-) -> Response[Union[Any, PredictionResponse]]:
-    """Create a new prediction
-
-     Create a new prediction using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreatePredictionRequest):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
-
+) -> Response[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
     json_body: CreatePredictionRequest,
 
-) -> Optional[Union[Any, PredictionResponse]]:
-    """Create a new prediction
-
-     Create a new prediction using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreatePredictionRequest):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
+) -> Optional[Union[
+    PredictionResponse,
+    None,
+    None
+]]:
+    """ Create a new prediction using the model identified by the modelId and the data set identified by the dataSetId """
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/save_prediction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,174 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.prediction_response import PredictionResponse
+from ...models.id_response import IdResponse
+from ...models.save_prediction_request import SavePredictionRequest
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SavePredictionRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/predictions/{id}".format(
+    url = "{}/v1/predictions/{id}/save".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, PredictionResponse]]:
-    if response.status_code == 200:
-        response_200 = PredictionResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = IdResponse.from_dict(response.json())
 
 
 
-        return response_200
+        return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
+    if response.status_code == 403:
+        response_403 = None
+
+        return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, PredictionResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SavePredictionRequest,
 
-) -> Response[Union[Any, PredictionResponse]]:
-    """Gets an overview of the prediction
-
-     Gets general information about the prediction, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
-
+) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SavePredictionRequest,
 
-) -> Optional[Union[Any, PredictionResponse]]:
-    """Gets an overview of the prediction
-
-     Gets general information about the prediction, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
+) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    """ Save the results of the specified prediction as a new data set """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SavePredictionRequest,
 
-) -> Response[Union[Any, PredictionResponse]]:
-    """Gets an overview of the prediction
-
-     Gets general information about the prediction, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
-
+) -> Response[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: SavePredictionRequest,
 
-) -> Optional[Union[Any, PredictionResponse]]:
-    """Gets an overview of the prediction
-
-     Gets general information about the prediction, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionResponse]]
-    """
-
+) -> Optional[Union[
+    IdResponse,
+    None,
+    None,
+    None
+]]:
+    """ Save the results of the specified prediction as a new data set """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_forecast.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/get_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,174 +1,152 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.prediction_forecast_response import PredictionForecastResponse
+from ...models.test_response import TestResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    id: int,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/predictions/{id}/forecast".format(
+    url = "{}/v1/tests/{id}".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, PredictionForecastResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    TestResponse,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = PredictionForecastResponse.from_dict(response.json())
+        response_200 = TestResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, PredictionForecastResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    TestResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Response[Union[Any, PredictionForecastResponse]]:
-    """Gets the forecast produced by a prediction
-
-     Obtains the forecast information for the specified prediction if available
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionForecastResponse]]
-    """
-
-
+) -> Response[Union[
+    TestResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Optional[Union[Any, PredictionForecastResponse]]:
-    """Gets the forecast produced by a prediction
-
-     Obtains the forecast information for the specified prediction if available
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionForecastResponse]]
-    """
-
+) -> Optional[Union[
+    TestResponse,
+    None,
+    None
+]]:
+    """ Gets general information about the test, including the current status """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Response[Union[Any, PredictionForecastResponse]]:
-    """Gets the forecast produced by a prediction
-
-     Obtains the forecast information for the specified prediction if available
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionForecastResponse]]
-    """
-
-
+) -> Response[Union[
+    TestResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Optional[Union[Any, PredictionForecastResponse]]:
-    """Gets the forecast produced by a prediction
-
-     Obtains the forecast information for the specified prediction if available
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, PredictionForecastResponse]]
-    """
-
+) -> Optional[Union[
+    TestResponse,
+    None,
+    None
+]]:
+    """ Gets general information about the test, including the current status """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_result_csv_data.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_cloud_data_set.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,146 @@
-from typing import Any, Dict, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...types import UNSET, Response, Unset
+from ...models.create_cloud_data_set_request import CreateCloudDataSetRequest
+from ...models.future import Future
+from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
+    json_body: CreateCloudDataSetRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/predictions/{id}/data/csv".format(
-        client.base_url,id=id)
+    url = "{}/v1/dataSets/cloud".format(
+        client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
-    params: Dict[str, Any] = {}
-    params["separator"] = separator
-
-
-    params["quoteChar"] = quote_char
-
-
-    params["escapeChar"] = escape_char
-
-
-    params["charset"] = charset
-
-
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
+    
 
+    json_json_body = json_body.to_dict()
 
-    
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "params": params,
+        "json": json_json_body,
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    Future,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = Future.from_dict(response.json())
+
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+        return response_201
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    Future,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
-
-) -> Response[Any]:
-    """Get the prediction result in CSV format
-
-     Get the prediction result as a csv file
-
-    Args:
-        id (int):
-        separator (Union[Unset, None, str]):
-        quote_char (Union[Unset, None, str]):
-        escape_char (Union[Unset, None, str]):
-        charset (Union[Unset, None, str]):  Default: 'UTF-8'.
-
-    Returns:
-        Response[Any]
-    """
-
+    json_body: CreateCloudDataSetRequest,
 
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
-separator=separator,
-quote_char=quote_char,
-escape_char=escape_char,
-charset=charset,
+        client=client,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
+def sync(
+    *,
+    client: Client,
+    json_body: CreateCloudDataSetRequest,
+
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
+
+    return sync_detailed(
+        client=client,
+json_body=json_body,
+
+    ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
-    separator: Union[Unset, None, str] = UNSET,
-    quote_char: Union[Unset, None, str] = UNSET,
-    escape_char: Union[Unset, None, str] = UNSET,
-    charset: Union[Unset, None, str] = 'UTF-8',
-
-) -> Response[Any]:
-    """Get the prediction result in CSV format
-
-     Get the prediction result as a csv file
-
-    Args:
-        id (int):
-        separator (Union[Unset, None, str]):
-        quote_char (Union[Unset, None, str]):
-        escape_char (Union[Unset, None, str]):
-        charset (Union[Unset, None, str]):  Default: 'UTF-8'.
-
-    Returns:
-        Response[Any]
-    """
-
+    json_body: CreateCloudDataSetRequest,
 
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
-separator=separator,
-quote_char=quote_char,
-escape_char=escape_char,
-charset=charset,
+        client=client,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    json_body: CreateCloudDataSetRequest,
+
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
+
+    return (await asyncio_detailed(
+        client=client,
+json_body=json_body,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/predictions/get_predictions.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/create_file_data_set.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,150 +1,144 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.prediction_list_response import PredictionListResponse
+from ...models.create_file_data_set_request import CreateFileDataSetRequest
+from ...models.future import Future
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
+    multipart_data: CreateFileDataSetRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/predictions".format(
+    url = "{}/v1/dataSets/file".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "files": multipart_data.to_dict(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, PredictionListResponse]]:
-    if response.status_code == 200:
-        response_200 = PredictionListResponse.from_dict(response.json())
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    Future,
+    None
+]]:
+    if response.status_code == 201:
+        response_201 = Future.from_dict(response.json())
 
 
 
-        return response_200
+        return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, PredictionListResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    Future,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
+    multipart_data: CreateFileDataSetRequest,
 
-) -> Response[Union[Any, PredictionListResponse]]:
-    """List all predictions
-
-     Returns a list of all predictions in the current project
-
-    Returns:
-        Response[Union[Any, PredictionListResponse]]
-    """
-
-
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
+multipart_data=multipart_data,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
+    multipart_data: CreateFileDataSetRequest,
 
-) -> Optional[Union[Any, PredictionListResponse]]:
-    """List all predictions
-
-     Returns a list of all predictions in the current project
-
-    Returns:
-        Response[Union[Any, PredictionListResponse]]
-    """
-
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
 
     return sync_detailed(
         client=client,
+multipart_data=multipart_data,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
+    multipart_data: CreateFileDataSetRequest,
 
-) -> Response[Union[Any, PredictionListResponse]]:
-    """List all predictions
-
-     Returns a list of all predictions in the current project
-
-    Returns:
-        Response[Union[Any, PredictionListResponse]]
-    """
-
-
+) -> Response[Union[
+    Future,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
+multipart_data=multipart_data,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
+    multipart_data: CreateFileDataSetRequest,
 
-) -> Optional[Union[Any, PredictionListResponse]]:
-    """List all predictions
-
-     Returns a list of all predictions in the current project
-
-    Returns:
-        Response[Union[Any, PredictionListResponse]]
-    """
-
+) -> Optional[Union[
+    Future,
+    None
+]]:
+    """ Your data will start being imported immediately. The response will contain a `futureId` which you can use with the `/futures` endpoint to check the progress of your import. Upon completion the future will give you information about the resulting data set. """
 
     return (await asyncio_detailed(
         client=client,
+multipart_data=multipart_data,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/create_test.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/tests/create_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
 from ...models.create_test_request import CreateTestRequest
 from ...models.test_response import TestResponse
 from ...types import Response
@@ -13,170 +13,144 @@
     client: Client,
     json_body: CreateTestRequest,
 
 ) -> Dict[str, Any]:
     url = "{}/v1/tests".format(
         client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, TestResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    TestResponse,
+    None,
+    None
+]]:
     if response.status_code == 201:
         response_201 = TestResponse.from_dict(response.json())
 
 
 
         return response_201
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, TestResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    TestResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     json_body: CreateTestRequest,
 
-) -> Response[Union[Any, TestResponse]]:
-    """Create a new test
-
-     Create a new test using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreateTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
-
+) -> Response[Union[
+    TestResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
     json_body: CreateTestRequest,
 
-) -> Optional[Union[Any, TestResponse]]:
-    """Create a new test
-
-     Create a new test using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreateTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
+) -> Optional[Union[
+    TestResponse,
+    None,
+    None
+]]:
+    """ Create a new test using the model identified by the modelId and the data set identified by the dataSetId """
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
     json_body: CreateTestRequest,
 
-) -> Response[Union[Any, TestResponse]]:
-    """Create a new test
-
-     Create a new test using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreateTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
-
+) -> Response[Union[
+    TestResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
     json_body: CreateTestRequest,
 
-) -> Optional[Union[Any, TestResponse]]:
-    """Create a new test
-
-     Create a new test using the model identified by the modelId and the data set identified by the
-    dataSetId
-
-    Args:
-        json_body (CreateTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
+) -> Optional[Union[
+    TestResponse,
+    None,
+    None
+]]:
+    """ Create a new test using the model identified by the modelId and the data set identified by the dataSetId """
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/edit_test.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/data/edit_data_set.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,194 +1,175 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.edit_test_request import EditTestRequest
-from ...models.test_response import TestResponse
+from ...models.data_set_response import DataSetResponse
+from ...models.edit_data_set_request import EditDataSetRequest
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
-    json_body: EditTestRequest,
+    id: int,
+    json_body: EditDataSetRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/tests/{id}".format(
+    url = "{}/v1/dataSets/{id}".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     json_json_body = json_body.to_dict()
 
 
 
-    
-
     return {
-	    "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, TestResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DataSetResponse,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = TestResponse.from_dict(response.json())
+        response_200 = DataSetResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
     if response.status_code == 403:
-        response_403 = cast(Any, None)
+        response_403 = None
+
         return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, TestResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DataSetResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
-    json_body: EditTestRequest,
-
-) -> Response[Union[Any, TestResponse]]:
-    """Edit the name and description of the specified test
-
-     Edit the name and description of the specified test
-
-    Args:
-        id (int):
-        json_body (EditTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
+    id: int,
+    json_body: EditDataSetRequest,
 
+) -> Response[Union[
+    DataSetResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
-    json_body: EditTestRequest,
-
-) -> Optional[Union[Any, TestResponse]]:
-    """Edit the name and description of the specified test
-
-     Edit the name and description of the specified test
-
-    Args:
-        id (int):
-        json_body (EditTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
+    id: int,
+    json_body: EditDataSetRequest,
 
+) -> Optional[Union[
+    DataSetResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edits the specified data set """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
-    json_body: EditTestRequest,
-
-) -> Response[Union[Any, TestResponse]]:
-    """Edit the name and description of the specified test
-
-     Edit the name and description of the specified test
-
-    Args:
-        id (int):
-        json_body (EditTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
+    id: int,
+    json_body: EditDataSetRequest,
 
+) -> Response[Union[
+    DataSetResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
-    json_body: EditTestRequest,
-
-) -> Optional[Union[Any, TestResponse]]:
-    """Edit the name and description of the specified test
-
-     Edit the name and description of the specified test
-
-    Args:
-        id (int):
-        json_body (EditTestRequest):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
+    id: int,
+    json_body: EditDataSetRequest,
 
+) -> Optional[Union[
+    DataSetResponse,
+    None,
+    None,
+    None
+]]:
+    """ Edits the specified data set """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
 json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/get_test.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/models/configure_decisioning_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,185 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.test_response import TestResponse
+from ...models.configure_decisioning_request import ConfigureDecisioningRequest
+from ...models.create_model_response import CreateModelResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: ConfigureDecisioningRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/tests/{id}".format(
+    url = "{}/v1/models/decisioning/{id}/configure".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
-    
+    json_json_body = json_body.to_dict()
+
 
-    
 
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, TestResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = TestResponse.from_dict(response.json())
+        response_200 = CreateModelResponse.from_dict(response.json())
 
 
 
         return response_200
+    if response.status_code == 400:
+        response_400 = None
+
+        return response_400
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
+    if response.status_code == 403:
+        response_403 = None
+
+        return response_403
     if response.status_code == 404:
-        response_404 = cast(Any, None)
+        response_404 = None
+
         return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, TestResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: ConfigureDecisioningRequest,
 
-) -> Response[Union[Any, TestResponse]]:
-    """Gets an overview of the test
-
-     Gets general information about the test, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.post(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: ConfigureDecisioningRequest,
 
-) -> Optional[Union[Any, TestResponse]]:
-    """Gets an overview of the test
-
-     Gets general information about the test, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Configures an existing decisioning model. Will return an error if the model has already been configured """
 
     return sync_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: ConfigureDecisioningRequest,
 
-) -> Response[Union[Any, TestResponse]]:
-    """Gets an overview of the test
-
-     Gets general information about the test, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
-
+) -> Response[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.post(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
-    id: int,
     *,
     client: Client,
+    id: int,
+    json_body: ConfigureDecisioningRequest,
 
-) -> Optional[Union[Any, TestResponse]]:
-    """Gets an overview of the test
-
-     Gets general information about the test, including the current status
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Union[Any, TestResponse]]
-    """
-
+) -> Optional[Union[
+    CreateModelResponse,
+    None,
+    None,
+    None,
+    None
+]]:
+    """ Configures an existing decisioning model. Will return an error if the model has already been configured """
 
     return (await asyncio_detailed(
-        id=id,
-client=client,
+        client=client,
+id=id,
+json_body=json_body,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_parquet_data.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/predictions/get_prediction_forecast.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,152 @@
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
+from ...models.prediction_forecast_response import PredictionForecastResponse
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
     *,
     client: Client,
+    id: int,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/tests/{id}/data/parquet".format(
+    url = "{}/v1/predictions/{id}/forecast".format(
         client.base_url,id=id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    PredictionForecastResponse,
+    None,
+    None
+]]:
+    if response.status_code == 200:
+        response_200 = PredictionForecastResponse.from_dict(response.json())
+
+
+
+        return response_200
+    if response.status_code == 401:
+        response_401 = None
+
+        return response_401
+    if response.status_code == 404:
+        response_404 = None
 
+        return response_404
+    return None
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    PredictionForecastResponse,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    id: int,
     *,
     client: Client,
+    id: int,
 
-) -> Response[Any]:
-    """Get the test result in parquet file format
-
-     Get the test result as a parquet file
-
-    Args:
-        id (int):
-
-    Returns:
-        Response[Any]
-    """
-
-
+) -> Response[Union[
+    PredictionForecastResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
-
-async def asyncio_detailed(
-    id: int,
+def sync(
     *,
     client: Client,
+    id: int,
 
-) -> Response[Any]:
-    """Get the test result in parquet file format
-
-     Get the test result as a parquet file
-
-    Args:
-        id (int):
+) -> Optional[Union[
+    PredictionForecastResponse,
+    None,
+    None
+]]:
+    """ Obtains the forecast information for the specified prediction if available """
+
+    return sync_detailed(
+        client=client,
+id=id,
 
-    Returns:
-        Response[Any]
-    """
+    ).parsed
 
+async def asyncio_detailed(
+    *,
+    client: Client,
+    id: int,
 
+) -> Response[Union[
+    PredictionForecastResponse,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
-        id=id,
-client=client,
+        client=client,
+id=id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
+async def asyncio(
+    *,
+    client: Client,
+    id: int,
+
+) -> Optional[Union[
+    PredictionForecastResponse,
+    None,
+    None
+]]:
+    """ Obtains the forecast information for the specified prediction if available """
+
+    return (await asyncio_detailed(
+        client=client,
+id=id,
+
+    )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/api/tests/get_tests.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/api/ap_is/get_model_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,162 @@
-from typing import Any, Dict, Optional, Union, cast
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.test_list_response import TestListResponse
+from ...models.deployed_model_api_response import DeployedModelApiResponse
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
+    model_api_id: int,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/tests".format(
-        client.base_url)
+    url = "{}/v1/modelApis/{modelApiId}".format(
+        client.base_url,modelApiId=model_api_id)
 
-    headers: Dict[str, str] = client.get_headers()
+    headers: Dict[str, Any] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
     
 
     
 
     
 
-    
-
     return {
-	    "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[Union[Any, TestListResponse]]:
+def _parse_response(*, response: httpx.Response) -> Optional[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     if response.status_code == 200:
-        response_200 = TestListResponse.from_dict(response.json())
+        response_200 = DeployedModelApiResponse.from_dict(response.json())
 
 
 
         return response_200
     if response.status_code == 401:
-        response_401 = cast(Any, None)
+        response_401 = None
+
         return response_401
+    if response.status_code == 403:
+        response_403 = None
+
+        return response_403
+    if response.status_code == 404:
+        response_404 = None
+
+        return response_404
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[Union[Any, TestListResponse]]:
+def _build_response(*, response: httpx.Response) -> Response[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Response[Union[Any, TestListResponse]]:
-    """List all tests
-
-     Returns a list of all tests in the current project
-
-    Returns:
-        Response[Union[Any, TestListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
+model_api_id=model_api_id,
 
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = httpx.get(
         **kwargs,
     )
 
     return _build_response(response=response)
 
 def sync(
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Optional[Union[Any, TestListResponse]]:
-    """List all tests
-
-     Returns a list of all tests in the current project
-
-    Returns:
-        Response[Union[Any, TestListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Gets general information about the published model api """
 
     return sync_detailed(
         client=client,
+model_api_id=model_api_id,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Response[Union[Any, TestListResponse]]:
-    """List all tests
-
-     Returns a list of all tests in the current project
-
-    Returns:
-        Response[Union[Any, TestListResponse]]
-    """
-
-
+) -> Response[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
     kwargs = _get_kwargs(
         client=client,
+model_api_id=model_api_id,
 
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(
+    async with httpx.AsyncClient() as _client:
+        response = await _client.get(
             **kwargs
         )
 
     return _build_response(response=response)
 
 async def asyncio(
     *,
     client: Client,
+    model_api_id: int,
 
-) -> Optional[Union[Any, TestListResponse]]:
-    """List all tests
-
-     Returns a list of all tests in the current project
-
-    Returns:
-        Response[Union[Any, TestListResponse]]
-    """
-
+) -> Optional[Union[
+    DeployedModelApiResponse,
+    None,
+    None,
+    None
+]]:
+    """ Gets general information about the published model api """
 
     return (await asyncio_detailed(
         client=client,
+model_api_id=model_api_id,
 
     )).parsed
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import ssl
-from typing import Dict, Union
+from typing import Dict
 
 import attr
 
 
 @attr.s(auto_attribs=True)
 class Client:
     """ A class for keeping track of data related to the API """
 
     base_url: str
     cookies: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
     headers: Dict[str, str] = attr.ib(factory=dict, kw_only=True)
     timeout: float = attr.ib(5.0, kw_only=True)
-    verify_ssl: Union[str, bool, ssl.SSLContext] = attr.ib(True, kw_only=True)
 
     def get_headers(self) -> Dict[str, str]:
         """ Get headers to be used in all endpoints """
         return {**self.headers}
 
     def with_headers(self, headers: Dict[str, str]) -> "Client":
         """ Get a new client matching this one with additional headers """
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/__init__.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """ Contains all the data models used in inputs/outputs """
 
-from .api_column_level import ApiColumnLevel
-from .api_column_type import ApiColumnType
 from .api_history_response import ApiHistoryResponse
 from .apply_data_prep_steps_request import ApplyDataPrepStepsRequest
 from .apply_formula_step import ApplyFormulaStep
 from .apply_formula_step_step_type import ApplyFormulaStepStepType
 from .cadence import Cadence
 from .classification_model_type import ClassificationModelType
 from .classification_scorers import ClassificationScorers
@@ -39,18 +37,19 @@
 from .create_test_request import CreateTestRequest
 from .csv_parse_options import CsvParseOptions
 from .csv_parse_options_file_type import CsvParseOptionsFileType
 from .data_partition_method import DataPartitionMethod
 from .data_pipeline_create_request import DataPipelineCreateRequest
 from .data_pipeline_response import DataPipelineResponse
 from .data_pipelines_response import DataPipelinesResponse
+from .data_prep_step import DataPrepStep
 from .data_prep_step_response import DataPrepStepResponse
-from .data_set_column_metadata_response import DataSetColumnMetadataResponse
 from .data_set_response import DataSetResponse
 from .data_sets_response import DataSetsResponse
+from .data_value import DataValue
 from .decisioning_decision import DecisioningDecision
 from .decisioning_reward import DecisioningReward
 from .decisioning_threshold import DecisioningThreshold
 from .delete_data_prep_steps_request import DeleteDataPrepStepsRequest
 from .deployed_api_client_create_response import DeployedApiClientCreateResponse
 from .deployed_api_client_list_response import DeployedApiClientListResponse
 from .deployed_api_client_response import DeployedApiClientResponse
@@ -74,15 +73,15 @@
 from .fill_missing_value_step import FillMissingValueStep
 from .fill_missing_value_step_step_type import FillMissingValueStepStepType
 from .filter_rows_rule import FilterRowsRule
 from .filter_rows_rule_rule import FilterRowsRuleRule
 from .filter_rows_step import FilterRowsStep
 from .filter_rows_step_step_type import FilterRowsStepStepType
 from .future import Future
-from .future_output_of_your_request import FutureOutputOfYourRequest
+from .future_outputofyourrequest import FutureOutputofyourrequest
 from .group_by_aggregation import GroupByAggregation
 from .group_by_aggregation_rule import GroupByAggregationRule
 from .group_by_step import GroupByStep
 from .group_by_step_step_type import GroupByStepStepType
 from .id_response import IdResponse
 from .json_parse_options import JsonParseOptions
 from .json_parse_options_file_type import JsonParseOptionsFileType
@@ -96,14 +95,15 @@
 from .model_status import ModelStatus
 from .model_validation_method import ModelValidationMethod
 from .nlp_language import NlpLanguage
 from .normalize_text_step import NormalizeTextStep
 from .normalize_text_step_rule import NormalizeTextStepRule
 from .normalize_text_step_step_type import NormalizeTextStepStepType
 from .null_request import NullRequest
+from .parse_options import ParseOptions
 from .prediction_forecast_response import PredictionForecastResponse
 from .prediction_forecast_response_model_forecasts_item import (
     PredictionForecastResponseModelForecastsItem,
 )
 from .prediction_list_response import PredictionListResponse
 from .prediction_response import PredictionResponse
 from .prediction_response_problem_type import PredictionResponseProblemType
@@ -132,15 +132,14 @@
 from .simplify_categories_definition import SimplifyCategoriesDefinition
 from .simplify_categories_rule import SimplifyCategoriesRule
 from .simplify_categories_step import SimplifyCategoriesStep
 from .simplify_categories_step_step_type import SimplifyCategoriesStepStepType
 from .split_column_step import SplitColumnStep
 from .split_column_step_step_type import SplitColumnStepStepType
 from .status import Status
-from .target_distributions import TargetDistributions
 from .test_list_response import TestListResponse
 from .test_response import TestResponse
 from .test_response_problem_type import TestResponseProblemType
 from .test_response_task_status import TestResponseTaskStatus
 from .transform_text_step import TransformTextStep
 from .transform_text_step_if_no_match import TransformTextStepIfNoMatch
 from .transform_text_step_replace_existing_column import (
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/api_history_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/api_history_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,57 +4,46 @@
 import attr
 from dateutil.parser import isoparse
 
 T = TypeVar("T", bound="ApiHistoryResponse")
 
 @attr.s(auto_attribs=True)
 class ApiHistoryResponse:
-    """
-    Attributes:
-        version_number (int):
-        created_at (datetime.datetime):
-        note (Optional[str]):
-        created_by (Optional[str]):
-        entity_id (Optional[int]):
-        entity_name (Optional[str]):
-    """
-
+    """  """
     version_number: int
     created_at: datetime.datetime
     note: Optional[str]
     created_by: Optional[str]
     entity_id: Optional[int]
     entity_name: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        version_number = self.version_number
+        version_number =  self.version_number
         created_at = self.created_at.isoformat()
 
-        note = self.note
-        created_by = self.created_by
-        entity_id = self.entity_id
-        entity_name = self.entity_name
+        note =  self.note
+        created_by =  self.created_by
+        entity_id =  self.entity_id
+        entity_name =  self.entity_name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "versionNumber": version_number,
             "createdAt": created_at,
             "note": note,
             "createdBy": created_by,
             "entityId": entity_id,
             "entityName": entity_name,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         version_number = d.pop("versionNumber")
 
         created_at = isoparse(d.pop("createdAt"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/apply_formula_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/rename_step.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,60 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.apply_formula_step_step_type import ApplyFormulaStepStepType
+from ..models.rename_step_step_type import RenameStepStepType
 
-T = TypeVar("T", bound="ApplyFormulaStep")
+T = TypeVar("T", bound="RenameStep")
 
 @attr.s(auto_attribs=True)
-class ApplyFormulaStep:
-    """
-    Attributes:
-        formula (str):
-        result_column_name (str):
-        step_type (ApplyFormulaStepStepType):
-    """
-
-    formula: str
-    result_column_name: str
-    step_type: ApplyFormulaStepStepType
+class RenameStep:
+    """  """
+    column: str
+    new_column_name: str
+    step_type: RenameStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        formula = self.formula
-        result_column_name = self.result_column_name
+        column =  self.column
+        new_column_name =  self.new_column_name
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "formula": formula,
-            "resultColumnName": result_column_name,
+            "column": column,
+            "newColumnName": new_column_name,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        formula = d.pop("formula")
+        column = d.pop("column")
 
-        result_column_name = d.pop("resultColumnName")
+        new_column_name = d.pop("newColumnName")
 
-        step_type = ApplyFormulaStepStepType(d.pop("stepType"))
+        step_type = RenameStepStepType(d.pop("stepType"))
 
 
 
 
-        apply_formula_step = cls(
-            formula=formula,
-            result_column_name=result_column_name,
+        rename_step = cls(
+            column=column,
+            new_column_name=new_column_name,
             step_type=step_type,
         )
 
-        apply_formula_step.additional_properties = d
-        return apply_formula_step
+        rename_step.additional_properties = d
+        return rename_step
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/combine_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/combine_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,49 +4,40 @@
 
 from ..models.combine_step_step_type import CombineStepStepType
 
 T = TypeVar("T", bound="CombineStep")
 
 @attr.s(auto_attribs=True)
 class CombineStep:
-    """
-    Attributes:
-        column (str):
-        data_set_column (str):
-        data_set_id (int):
-        step_type (CombineStepStepType):
-    """
-
+    """  """
     column: str
     data_set_column: str
     data_set_id: int
     step_type: CombineStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column = self.column
-        data_set_column = self.data_set_column
-        data_set_id = self.data_set_id
+        column =  self.column
+        data_set_column =  self.data_set_column
+        data_set_id =  self.data_set_id
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "column": column,
             "dataSetColumn": data_set_column,
             "dataSetId": data_set_id,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         column = d.pop("column")
 
         data_set_column = d.pop("dataSetColumn")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/configure_decisioning_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/configure_decisioning_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,22 @@
 
 from ..models.decisioning_decision import DecisioningDecision
 
 T = TypeVar("T", bound="ConfigureDecisioningRequest")
 
 @attr.s(auto_attribs=True)
 class ConfigureDecisioningRequest:
-    """
-    Attributes:
-        target_class (str):
-        decisions (List[DecisioningDecision]):
-    """
-
+    """  """
     target_class: str
     decisions: List[DecisioningDecision]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        target_class = self.target_class
+        target_class =  self.target_class
         decisions = []
         for decisions_item_data in self.decisions:
             decisions_item = decisions_item_data.to_dict()
 
             decisions.append(decisions_item)
 
 
@@ -36,16 +31,14 @@
         field_dict.update({
             "targetClass": target_class,
             "decisions": decisions,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         target_class = d.pop("targetClass")
 
         decisions = []
         _decisions = d.pop("decisions")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_auto_clustering_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_auto_clustering_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,51 +5,41 @@
 from ..models.nlp_language import NlpLanguage
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateAutoClusteringRequest")
 
 @attr.s(auto_attribs=True)
 class CreateAutoClusteringRequest:
-    """
-    Attributes:
-        name (str):
-        data_set_id (int):
-        minimum_clusters (int):
-        maximum_clusters (int):
-        description (Union[Unset, str]):
-        excluded_columns (Union[Unset, List[str]]):
-        nlp_language (Union[Unset, NlpLanguage]):  Default: NlpLanguage.AUTO_DETECT.
-    """
-
+    """  """
     name: str
     data_set_id: int
     minimum_clusters: int
     maximum_clusters: int
     description: Union[Unset, str] = UNSET
     excluded_columns: Union[Unset, List[str]] = UNSET
     nlp_language: Union[Unset, NlpLanguage] = NlpLanguage.AUTO_DETECT
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data_set_id = self.data_set_id
-        minimum_clusters = self.minimum_clusters
-        maximum_clusters = self.maximum_clusters
-        description = self.description
-        excluded_columns: Union[Unset, List[str]] = UNSET
+        name =  self.name
+        data_set_id =  self.data_set_id
+        minimum_clusters =  self.minimum_clusters
+        maximum_clusters =  self.maximum_clusters
+        description =  self.description
+        excluded_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.excluded_columns, Unset):
             excluded_columns = self.excluded_columns
 
 
 
 
-        nlp_language: Union[Unset, str] = UNSET
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         if not isinstance(self.nlp_language, Unset):
-            nlp_language = self.nlp_language.value
+            nlp_language = self.nlp_language
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "dataSetId": data_set_id,
@@ -61,16 +51,14 @@
         if excluded_columns is not UNSET:
             field_dict["excludedColumns"] = excluded_columns
         if nlp_language is not UNSET:
             field_dict["nlpLanguage"] = nlp_language
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         data_set_id = d.pop("dataSetId")
 
@@ -79,19 +67,17 @@
         maximum_clusters = d.pop("maximumClusters")
 
         description = d.pop("description", UNSET)
 
         excluded_columns = cast(List[str], d.pop("excludedColumns", UNSET))
 
 
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         _nlp_language = d.pop("nlpLanguage", UNSET)
-        nlp_language: Union[Unset, NlpLanguage]
-        if isinstance(_nlp_language,  Unset):
-            nlp_language = UNSET
-        else:
+        if not isinstance(_nlp_language,  Unset):
             nlp_language = NlpLanguage(_nlp_language)
 
 
 
 
         create_auto_clustering_request = cls(
             name=name,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_classification_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_classification_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,91 +9,69 @@
 from ..models.nlp_language import NlpLanguage
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateClassificationRequest")
 
 @attr.s(auto_attribs=True)
 class CreateClassificationRequest:
-    """
-    Attributes:
-        name (str):
-        data_set_id (int):
-        target_column (str):
-        score_to_optimize (ClassificationScorers):
-        model_validation_method (ModelValidationMethod):
-        data_partition_method (DataPartitionMethod):
-        number_of_evaluations (int):
-        description (Union[Unset, str]):
-        excluded_columns (Union[Unset, List[str]]):
-        nlp_language (Union[Unset, NlpLanguage]):  Default: NlpLanguage.AUTO_DETECT.
-        draft_mode (Union[Unset, bool]):
-        hold_out_percentage (Union[Unset, float]):  Default: 10.0.
-        no_mixing_columns (Union[Unset, List[str]]):
-        partition_column (Union[Unset, str]):
-        order_by_column (Union[Unset, str]):
-        weight_column (Union[Unset, str]):
-        model_types (Union[Unset, List[ClassificationModelType]]): If omitted - all eligable model types are chosen.
-    """
-
+    """  """
     name: str
     data_set_id: int
     target_column: str
     score_to_optimize: ClassificationScorers
     model_validation_method: ModelValidationMethod
     data_partition_method: DataPartitionMethod
     number_of_evaluations: int
     description: Union[Unset, str] = UNSET
     excluded_columns: Union[Unset, List[str]] = UNSET
     nlp_language: Union[Unset, NlpLanguage] = NlpLanguage.AUTO_DETECT
     draft_mode: Union[Unset, bool] = UNSET
-    hold_out_percentage: Union[Unset, float] = 10.0
     no_mixing_columns: Union[Unset, List[str]] = UNSET
     partition_column: Union[Unset, str] = UNSET
     order_by_column: Union[Unset, str] = UNSET
     weight_column: Union[Unset, str] = UNSET
     model_types: Union[Unset, List[ClassificationModelType]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data_set_id = self.data_set_id
-        target_column = self.target_column
+        name =  self.name
+        data_set_id =  self.data_set_id
+        target_column =  self.target_column
         score_to_optimize = self.score_to_optimize.value
 
         model_validation_method = self.model_validation_method.value
 
         data_partition_method = self.data_partition_method.value
 
-        number_of_evaluations = self.number_of_evaluations
-        description = self.description
-        excluded_columns: Union[Unset, List[str]] = UNSET
+        number_of_evaluations =  self.number_of_evaluations
+        description =  self.description
+        excluded_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.excluded_columns, Unset):
             excluded_columns = self.excluded_columns
 
 
 
 
-        nlp_language: Union[Unset, str] = UNSET
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         if not isinstance(self.nlp_language, Unset):
-            nlp_language = self.nlp_language.value
+            nlp_language = self.nlp_language
 
-        draft_mode = self.draft_mode
-        hold_out_percentage = self.hold_out_percentage
-        no_mixing_columns: Union[Unset, List[str]] = UNSET
+        draft_mode =  self.draft_mode
+        no_mixing_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.no_mixing_columns, Unset):
             no_mixing_columns = self.no_mixing_columns
 
 
 
 
-        partition_column = self.partition_column
-        order_by_column = self.order_by_column
-        weight_column = self.weight_column
-        model_types: Union[Unset, List[str]] = UNSET
+        partition_column =  self.partition_column
+        order_by_column =  self.order_by_column
+        weight_column =  self.weight_column
+        model_types: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.model_types, Unset):
             model_types = []
             for model_types_item_data in self.model_types:
                 model_types_item = model_types_item_data.value
 
                 model_types.append(model_types_item)
 
@@ -116,31 +94,27 @@
             field_dict["description"] = description
         if excluded_columns is not UNSET:
             field_dict["excludedColumns"] = excluded_columns
         if nlp_language is not UNSET:
             field_dict["nlpLanguage"] = nlp_language
         if draft_mode is not UNSET:
             field_dict["draftMode"] = draft_mode
-        if hold_out_percentage is not UNSET:
-            field_dict["holdOutPercentage"] = hold_out_percentage
         if no_mixing_columns is not UNSET:
             field_dict["noMixingColumns"] = no_mixing_columns
         if partition_column is not UNSET:
             field_dict["partitionColumn"] = partition_column
         if order_by_column is not UNSET:
             field_dict["orderByColumn"] = order_by_column
         if weight_column is not UNSET:
             field_dict["weightColumn"] = weight_column
         if model_types is not UNSET:
             field_dict["modelTypes"] = model_types
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         data_set_id = d.pop("dataSetId")
 
@@ -164,28 +138,24 @@
         number_of_evaluations = d.pop("numberOfEvaluations")
 
         description = d.pop("description", UNSET)
 
         excluded_columns = cast(List[str], d.pop("excludedColumns", UNSET))
 
 
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         _nlp_language = d.pop("nlpLanguage", UNSET)
-        nlp_language: Union[Unset, NlpLanguage]
-        if isinstance(_nlp_language,  Unset):
-            nlp_language = UNSET
-        else:
+        if not isinstance(_nlp_language,  Unset):
             nlp_language = NlpLanguage(_nlp_language)
 
 
 
 
         draft_mode = d.pop("draftMode", UNSET)
 
-        hold_out_percentage = d.pop("holdOutPercentage", UNSET)
-
         no_mixing_columns = cast(List[str], d.pop("noMixingColumns", UNSET))
 
 
         partition_column = d.pop("partitionColumn", UNSET)
 
         order_by_column = d.pop("orderByColumn", UNSET)
 
@@ -209,15 +179,14 @@
             model_validation_method=model_validation_method,
             data_partition_method=data_partition_method,
             number_of_evaluations=number_of_evaluations,
             description=description,
             excluded_columns=excluded_columns,
             nlp_language=nlp_language,
             draft_mode=draft_mode,
-            hold_out_percentage=hold_out_percentage,
             no_mixing_columns=no_mixing_columns,
             partition_column=partition_column,
             order_by_column=order_by_column,
             weight_column=weight_column,
             model_types=model_types,
         )
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_clustering_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_clustering_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,48 +5,39 @@
 from ..models.nlp_language import NlpLanguage
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateClusteringRequest")
 
 @attr.s(auto_attribs=True)
 class CreateClusteringRequest:
-    """
-    Attributes:
-        name (str):
-        data_set_id (int):
-        number_of_clusters (int):
-        description (Union[Unset, str]):
-        excluded_columns (Union[Unset, List[str]]):
-        nlp_language (Union[Unset, NlpLanguage]):  Default: NlpLanguage.AUTO_DETECT.
-    """
-
+    """  """
     name: str
     data_set_id: int
     number_of_clusters: int
     description: Union[Unset, str] = UNSET
     excluded_columns: Union[Unset, List[str]] = UNSET
     nlp_language: Union[Unset, NlpLanguage] = NlpLanguage.AUTO_DETECT
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data_set_id = self.data_set_id
-        number_of_clusters = self.number_of_clusters
-        description = self.description
-        excluded_columns: Union[Unset, List[str]] = UNSET
+        name =  self.name
+        data_set_id =  self.data_set_id
+        number_of_clusters =  self.number_of_clusters
+        description =  self.description
+        excluded_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.excluded_columns, Unset):
             excluded_columns = self.excluded_columns
 
 
 
 
-        nlp_language: Union[Unset, str] = UNSET
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         if not isinstance(self.nlp_language, Unset):
-            nlp_language = self.nlp_language.value
+            nlp_language = self.nlp_language
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "dataSetId": data_set_id,
@@ -57,35 +48,31 @@
         if excluded_columns is not UNSET:
             field_dict["excludedColumns"] = excluded_columns
         if nlp_language is not UNSET:
             field_dict["nlpLanguage"] = nlp_language
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         data_set_id = d.pop("dataSetId")
 
         number_of_clusters = d.pop("numberOfClusters")
 
         description = d.pop("description", UNSET)
 
         excluded_columns = cast(List[str], d.pop("excludedColumns", UNSET))
 
 
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         _nlp_language = d.pop("nlpLanguage", UNSET)
-        nlp_language: Union[Unset, NlpLanguage]
-        if isinstance(_nlp_language,  Unset):
-            nlp_language = UNSET
-        else:
+        if not isinstance(_nlp_language,  Unset):
             nlp_language = NlpLanguage(_nlp_language)
 
 
 
 
         create_clustering_request = cls(
             name=name,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_data_set_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_prediction_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,64 @@
-from io import BytesIO
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
-from ..types import UNSET, File, Unset
+from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateDataSetRequest")
+T = TypeVar("T", bound="CreatePredictionRequest")
 
 @attr.s(auto_attribs=True)
-class CreateDataSetRequest:
-    """
-    Attributes:
-        name (str):
-        data (File):
-        description (Union[Unset, str]):
-    """
-
-    name: str
-    data: File
-    description: Union[Unset, str] = UNSET
+class CreatePredictionRequest:
+    """  """
+    model_id: int
+    data_set_id: int
+    name: Union[Unset, str] = UNSET
+    description: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data = self.data.to_tuple()
-
-        description = self.description
+        model_id =  self.model_id
+        data_set_id =  self.data_set_id
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "name": name,
-            "data": data,
-        })
-        if description is not UNSET:
-            field_dict["description"] = description
-
-        return field_dict
-
-
-    def to_multipart(self) -> Dict[str, Any]:
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-        data = self.data.to_tuple()
-
-        description = self.description if isinstance(self.description, Unset) else (None, str(self.description).encode(), "text/plain")
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update({
-            key: (None, str(value).encode(), "text/plain")
-            for key, value in self.additional_properties.items()
-        })
-        field_dict.update({
-            "name": name,
-            "data": data,
+            "modelId": model_id,
+            "dataSetId": data_set_id,
         })
+        if name is not UNSET:
+            field_dict["name"] = name
         if description is not UNSET:
             field_dict["description"] = description
 
         return field_dict
 
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
-
-        data = File(
-             payload = BytesIO(d.pop("data"))
-        )
-
+        model_id = d.pop("modelId")
 
+        data_set_id = d.pop("dataSetId")
 
+        name = d.pop("name", UNSET)
 
         description = d.pop("description", UNSET)
 
-        create_data_set_request = cls(
+        create_prediction_request = cls(
+            model_id=model_id,
+            data_set_id=data_set_id,
             name=name,
-            data=data,
             description=description,
         )
 
-        create_data_set_request.additional_properties = d
-        return create_data_set_request
+        create_prediction_request.additional_properties = d
+        return create_prediction_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_db_data_set_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,15 @@
 from ..models.create_db_data_set_request_db_type import CreateDbDataSetRequestDbType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateDbDataSetRequest")
 
 @attr.s(auto_attribs=True)
 class CreateDbDataSetRequest:
-    """
-    Attributes:
-        name (str):
-        db_type (CreateDbDataSetRequestDbType):
-        query (str):
-        data_origin (CreateDbDataSetRequestDataOrigin):
-        description (Union[Unset, str]):
-        username (Union[Unset, str]):
-        password (Union[Unset, str]):
-        host (Union[Unset, str]):
-        port (Union[Unset, str]):
-        db_name (Union[Unset, str]):
-        custom_db_url (Union[Unset, bool]):
-        db_url (Union[Unset, str]): required if customDbUrl is true
-    """
-
+    """  """
     name: str
     db_type: CreateDbDataSetRequestDbType
     query: str
     data_origin: CreateDbDataSetRequestDataOrigin
     description: Union[Unset, str] = UNSET
     username: Union[Unset, str] = UNSET
     password: Union[Unset, str] = UNSET
@@ -40,28 +25,28 @@
     db_name: Union[Unset, str] = UNSET
     custom_db_url: Union[Unset, bool] = False
     db_url: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
+        name =  self.name
         db_type = self.db_type.value
 
-        query = self.query
+        query =  self.query
         data_origin = self.data_origin.value
 
-        description = self.description
-        username = self.username
-        password = self.password
-        host = self.host
-        port = self.port
-        db_name = self.db_name
-        custom_db_url = self.custom_db_url
-        db_url = self.db_url
+        description =  self.description
+        username =  self.username
+        password =  self.password
+        host =  self.host
+        port =  self.port
+        db_name =  self.db_name
+        custom_db_url =  self.custom_db_url
+        db_url =  self.db_url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "dbType": db_type,
             "query": query,
@@ -82,16 +67,14 @@
         if custom_db_url is not UNSET:
             field_dict["customDbUrl"] = custom_db_url
         if db_url is not UNSET:
             field_dict["dbUrl"] = db_url
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         db_type = CreateDbDataSetRequestDbType(d.pop("dbType"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_decisioning_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_decisioning_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,36 +5,28 @@
 from ..models.configure_decisioning_request import ConfigureDecisioningRequest
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateDecisioningRequest")
 
 @attr.s(auto_attribs=True)
 class CreateDecisioningRequest:
-    """
-    Attributes:
-        name (str):
-        data_set_id (int):
-        parent_model_id (int):
-        description (Union[Unset, str]):
-        configuration (Union[Unset, ConfigureDecisioningRequest]):
-    """
-
+    """  """
     name: str
     data_set_id: int
     parent_model_id: int
     description: Union[Unset, str] = UNSET
-    configuration: Union[Unset, ConfigureDecisioningRequest] = UNSET
+    configuration: Union[ConfigureDecisioningRequest, Unset] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data_set_id = self.data_set_id
-        parent_model_id = self.parent_model_id
-        description = self.description
+        name =  self.name
+        data_set_id =  self.data_set_id
+        parent_model_id =  self.parent_model_id
+        description =  self.description
         configuration: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.configuration, Unset):
             configuration = self.configuration.to_dict()
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
@@ -46,32 +38,28 @@
         if description is not UNSET:
             field_dict["description"] = description
         if configuration is not UNSET:
             field_dict["configuration"] = configuration
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         data_set_id = d.pop("dataSetId")
 
         parent_model_id = d.pop("parentModelId")
 
         description = d.pop("description", UNSET)
 
+        configuration: Union[ConfigureDecisioningRequest, Unset] = UNSET
         _configuration = d.pop("configuration", UNSET)
-        configuration: Union[Unset, ConfigureDecisioningRequest]
-        if isinstance(_configuration,  Unset):
-            configuration = UNSET
-        else:
+        if not isinstance(_configuration,  Unset):
             configuration = ConfigureDecisioningRequest.from_dict(_configuration)
 
 
 
 
         create_decisioning_request = cls(
             name=name,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_deployed_api_client_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_data_pipeline_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateDeployedApiClientRequest")
+T = TypeVar("T", bound="EditDataPipelineRequest")
 
 @attr.s(auto_attribs=True)
-class CreateDeployedApiClientRequest:
-    """
-    Attributes:
-        name (str):
-    """
-
+class EditDataPipelineRequest:
+    """  """
     name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
+        name =  self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
-        create_deployed_api_client_request = cls(
+        edit_data_pipeline_request = cls(
             name=name,
         )
 
-        create_deployed_api_client_request.additional_properties = d
-        return create_deployed_api_client_request
+        edit_data_pipeline_request.additional_properties = d
+        return edit_data_pipeline_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_deployed_model_api_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_deployed_model_api_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,40 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateDeployedModelApiRequest")
 
 @attr.s(auto_attribs=True)
 class CreateDeployedModelApiRequest:
-    """
-    Attributes:
-        model_id (int):
-        name (str):
-        description (Union[Unset, None, str]):
-    """
-
+    """  """
     model_id: int
     name: str
-    description: Union[Unset, None, str] = UNSET
+    description: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        model_id = self.model_id
-        name = self.name
-        description = self.description
+        model_id =  self.model_id
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "modelId": model_id,
             "name": name,
         })
         if description is not UNSET:
             field_dict["description"] = description
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         model_id = d.pop("modelId")
 
         name = d.pop("name")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_deployed_pipeline_api_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_data_set_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,48 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="CreateDeployedPipelineApiRequest")
+T = TypeVar("T", bound="EditDataSetRequest")
 
 @attr.s(auto_attribs=True)
-class CreateDeployedPipelineApiRequest:
-    """
-    Attributes:
-        pipeline_id (int):
-        name (str):
-        description (Union[Unset, None, str]):
-    """
-
-    pipeline_id: int
+class EditDataSetRequest:
+    """  """
     name: str
-    description: Union[Unset, None, str] = UNSET
+    description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        pipeline_id = self.pipeline_id
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "pipelineId": pipeline_id,
             "name": name,
+            "description": description,
         })
-        if description is not UNSET:
-            field_dict["description"] = description
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        pipeline_id = d.pop("pipelineId")
-
         name = d.pop("name")
 
-        description = d.pop("description", UNSET)
+        description = d.pop("description")
 
-        create_deployed_pipeline_api_request = cls(
-            pipeline_id=pipeline_id,
+        edit_data_set_request = cls(
             name=name,
             description=description,
         )
 
-        create_deployed_pipeline_api_request.additional_properties = d
-        return create_deployed_pipeline_api_request
+        edit_data_set_request.additional_properties = d
+        return edit_data_set_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_file_data_set_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_http_data_set_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,86 @@
-from io import BytesIO
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..types import UNSET, File, Unset
+from ..models.create_http_data_set_request_data_origin import (
+    CreateHttpDataSetRequestDataOrigin,
+)
+from ..models.parse_options import ParseOptions
+from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateFileDataSetRequest")
+T = TypeVar("T", bound="CreateHttpDataSetRequest")
 
 @attr.s(auto_attribs=True)
-class CreateFileDataSetRequest:
-    """
-    Attributes:
-        name (str):
-        data (File):
-        description (Union[Unset, str]):
-        parse_options (Union[Unset, str]): This parameter is a string for multipart-form compatibility. If provided it
-            should be string of JSON matching the appropriate ParseOptions (CSV or Parquet) schema
-    """
-
+class CreateHttpDataSetRequest:
+    """  """
     name: str
-    data: File
-    description: Union[Unset, str] = UNSET
-    parse_options: Union[Unset, str] = UNSET
+    description: str
+    url: str
+    data_origin: CreateHttpDataSetRequestDataOrigin
+    parse_options: Union[ParseOptions, Unset] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data = self.data.to_tuple()
+        name =  self.name
+        description =  self.description
+        url =  self.url
+        data_origin = self.data_origin.value
+
+        parse_options: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.parse_options, Unset):
+            parse_options = self.parse_options.to_dict()
 
-        description = self.description
-        parse_options = self.parse_options
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
-            "data": data,
+            "description": description,
+            "url": url,
+            "dataOrigin": data_origin,
         })
-        if description is not UNSET:
-            field_dict["description"] = description
         if parse_options is not UNSET:
             field_dict["parseOptions"] = parse_options
 
         return field_dict
 
-
-    def to_multipart(self) -> Dict[str, Any]:
-        name = self.name if isinstance(self.name, Unset) else (None, str(self.name).encode(), "text/plain")
-        data = self.data.to_tuple()
-
-        description = self.description if isinstance(self.description, Unset) else (None, str(self.description).encode(), "text/plain")
-        parse_options = self.parse_options if isinstance(self.parse_options, Unset) else (None, str(self.parse_options).encode(), "text/plain")
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update({
-            key: (None, str(value).encode(), "text/plain")
-            for key, value in self.additional_properties.items()
-        })
-        field_dict.update({
-            "name": name,
-            "data": data,
-        })
-        if description is not UNSET:
-            field_dict["description"] = description
-        if parse_options is not UNSET:
-            field_dict["parseOptions"] = parse_options
-
-        return field_dict
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
-        data = File(
-             payload = BytesIO(d.pop("data"))
-        )
+        description = d.pop("description")
+
+        url = d.pop("url")
+
+        data_origin = CreateHttpDataSetRequestDataOrigin(d.pop("dataOrigin"))
+
+
 
 
+        parse_options: Union[ParseOptions, Unset] = UNSET
+        _parse_options = d.pop("parseOptions", UNSET)
+        if not isinstance(_parse_options,  Unset):
+            parse_options = ParseOptions.from_dict(_parse_options)
 
 
-        description = d.pop("description", UNSET)
 
-        parse_options = d.pop("parseOptions", UNSET)
 
-        create_file_data_set_request = cls(
+        create_http_data_set_request = cls(
             name=name,
-            data=data,
             description=description,
+            url=url,
+            data_origin=data_origin,
             parse_options=parse_options,
         )
 
-        create_file_data_set_request.additional_properties = d
-        return create_file_data_set_request
+        create_http_data_set_request.additional_properties = d
+        return create_http_data_set_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_forecasting_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_multi_forecasting_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..models.cadence import Cadence
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateForecastingRequest")
+T = TypeVar("T", bound="CreateMultiForecastingRequest")
 
 @attr.s(auto_attribs=True)
-class CreateForecastingRequest:
-    """
-    Attributes:
-        name (str):
-        data_set_id (int):
-        target_column (str):
-        time_index_column (str):
-        cadence (Cadence):
-        horizons (List[int]):
-        description (Union[Unset, str]):
-        excluded_columns (Union[Unset, List[str]]):
-    """
-
+class CreateMultiForecastingRequest:
+    """  """
     name: str
     data_set_id: int
     target_column: str
     time_index_column: str
     cadence: Cadence
     horizons: List[int]
+    discriminator_columns: List[str]
     description: Union[Unset, str] = UNSET
     excluded_columns: Union[Unset, List[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data_set_id = self.data_set_id
-        target_column = self.target_column
-        time_index_column = self.time_index_column
+        name =  self.name
+        data_set_id =  self.data_set_id
+        target_column =  self.target_column
+        time_index_column =  self.time_index_column
         cadence = self.cadence.value
 
         horizons = self.horizons
 
 
 
 
-        description = self.description
-        excluded_columns: Union[Unset, List[str]] = UNSET
+        discriminator_columns = self.discriminator_columns
+
+
+
+
+        description =  self.description
+        excluded_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.excluded_columns, Unset):
             excluded_columns = self.excluded_columns
 
 
 
 
 
@@ -58,24 +53,23 @@
         field_dict.update({
             "name": name,
             "dataSetId": data_set_id,
             "targetColumn": target_column,
             "timeIndexColumn": time_index_column,
             "cadence": cadence,
             "horizons": horizons,
+            "discriminatorColumns": discriminator_columns,
         })
         if description is not UNSET:
             field_dict["description"] = description
         if excluded_columns is not UNSET:
             field_dict["excludedColumns"] = excluded_columns
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         data_set_id = d.pop("dataSetId")
 
@@ -87,32 +81,36 @@
 
 
 
 
         horizons = cast(List[int], d.pop("horizons"))
 
 
+        discriminator_columns = cast(List[str], d.pop("discriminatorColumns"))
+
+
         description = d.pop("description", UNSET)
 
         excluded_columns = cast(List[str], d.pop("excludedColumns", UNSET))
 
 
-        create_forecasting_request = cls(
+        create_multi_forecasting_request = cls(
             name=name,
             data_set_id=data_set_id,
             target_column=target_column,
             time_index_column=time_index_column,
             cadence=cadence,
             horizons=horizons,
+            discriminator_columns=discriminator_columns,
             description=description,
             excluded_columns=excluded_columns,
         )
 
-        create_forecasting_request.additional_properties = d
-        return create_forecasting_request
+        create_multi_forecasting_request.additional_properties = d
+        return create_multi_forecasting_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_model_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/id_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,42 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="CreateModelResponse")
+T = TypeVar("T", bound="IdResponse")
 
 @attr.s(auto_attribs=True)
-class CreateModelResponse:
-    """
-    Attributes:
-        id (int):
-    """
-
+class IdResponse:
+    """  """
     id: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
+        id =  self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "id": id,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
-        create_model_response = cls(
+        id_response = cls(
             id=id,
         )
 
-        create_model_response.additional_properties = d
-        return create_model_response
+        id_response.additional_properties = d
+        return id_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_multi_forecasting_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_forecasting_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,44 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..models.cadence import Cadence
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateMultiForecastingRequest")
+T = TypeVar("T", bound="CreateForecastingRequest")
 
 @attr.s(auto_attribs=True)
-class CreateMultiForecastingRequest:
-    """
-    Attributes:
-        name (str):
-        data_set_id (int):
-        target_column (str):
-        time_index_column (str):
-        cadence (Cadence):
-        horizons (List[int]):
-        discriminator_columns (List[str]):
-        description (Union[Unset, str]):
-        excluded_columns (Union[Unset, List[str]]):
-    """
-
+class CreateForecastingRequest:
+    """  """
     name: str
     data_set_id: int
     target_column: str
     time_index_column: str
     cadence: Cadence
     horizons: List[int]
-    discriminator_columns: List[str]
     description: Union[Unset, str] = UNSET
     excluded_columns: Union[Unset, List[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data_set_id = self.data_set_id
-        target_column = self.target_column
-        time_index_column = self.time_index_column
+        name =  self.name
+        data_set_id =  self.data_set_id
+        target_column =  self.target_column
+        time_index_column =  self.time_index_column
         cadence = self.cadence.value
 
         horizons = self.horizons
 
 
 
 
-        discriminator_columns = self.discriminator_columns
-
-
-
-
-        description = self.description
-        excluded_columns: Union[Unset, List[str]] = UNSET
+        description =  self.description
+        excluded_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.excluded_columns, Unset):
             excluded_columns = self.excluded_columns
 
 
 
 
 
@@ -65,25 +47,22 @@
         field_dict.update({
             "name": name,
             "dataSetId": data_set_id,
             "targetColumn": target_column,
             "timeIndexColumn": time_index_column,
             "cadence": cadence,
             "horizons": horizons,
-            "discriminatorColumns": discriminator_columns,
         })
         if description is not UNSET:
             field_dict["description"] = description
         if excluded_columns is not UNSET:
             field_dict["excludedColumns"] = excluded_columns
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         data_set_id = d.pop("dataSetId")
 
@@ -95,36 +74,32 @@
 
 
 
 
         horizons = cast(List[int], d.pop("horizons"))
 
 
-        discriminator_columns = cast(List[str], d.pop("discriminatorColumns"))
-
-
         description = d.pop("description", UNSET)
 
         excluded_columns = cast(List[str], d.pop("excludedColumns", UNSET))
 
 
-        create_multi_forecasting_request = cls(
+        create_forecasting_request = cls(
             name=name,
             data_set_id=data_set_id,
             target_column=target_column,
             time_index_column=time_index_column,
             cadence=cadence,
             horizons=horizons,
-            discriminator_columns=discriminator_columns,
             description=description,
             excluded_columns=excluded_columns,
         )
 
-        create_multi_forecasting_request.additional_properties = d
-        return create_multi_forecasting_request
+        create_forecasting_request.additional_properties = d
+        return create_forecasting_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_prediction_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_test_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,64 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreatePredictionRequest")
+T = TypeVar("T", bound="CreateTestRequest")
 
 @attr.s(auto_attribs=True)
-class CreatePredictionRequest:
-    """
-    Attributes:
-        model_id (int):
-        data_set_id (int):
-        name (Union[Unset, str]):
-        description (Union[Unset, None, str]):
-    """
-
+class CreateTestRequest:
+    """  """
     model_id: int
     data_set_id: int
     name: Union[Unset, str] = UNSET
-    description: Union[Unset, None, str] = UNSET
+    description: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        model_id = self.model_id
-        data_set_id = self.data_set_id
-        name = self.name
-        description = self.description
+        model_id =  self.model_id
+        data_set_id =  self.data_set_id
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "modelId": model_id,
             "dataSetId": data_set_id,
         })
         if name is not UNSET:
             field_dict["name"] = name
         if description is not UNSET:
             field_dict["description"] = description
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         model_id = d.pop("modelId")
 
         data_set_id = d.pop("dataSetId")
 
         name = d.pop("name", UNSET)
 
         description = d.pop("description", UNSET)
 
-        create_prediction_request = cls(
+        create_test_request = cls(
             model_id=model_id,
             data_set_id=data_set_id,
             name=name,
             description=description,
         )
 
-        create_prediction_request.additional_properties = d
-        return create_prediction_request
+        create_test_request.additional_properties = d
+        return create_test_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_regression_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_regression_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,104 +3,75 @@
 import attr
 
 from ..models.data_partition_method import DataPartitionMethod
 from ..models.model_validation_method import ModelValidationMethod
 from ..models.nlp_language import NlpLanguage
 from ..models.regression_model_type import RegressionModelType
 from ..models.regression_scorers import RegressionScorers
-from ..models.target_distributions import TargetDistributions
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="CreateRegressionRequest")
 
 @attr.s(auto_attribs=True)
 class CreateRegressionRequest:
-    """
-    Attributes:
-        name (str):
-        data_set_id (int):
-        target_column (str):
-        score_to_optimize (RegressionScorers):
-        model_validation_method (ModelValidationMethod):
-        data_partition_method (DataPartitionMethod):
-        number_of_evaluations (int):
-        description (Union[Unset, str]):
-        target_distribution (Union[Unset, TargetDistributions]):  Default: TargetDistributions.GAUSSIAN.
-        excluded_columns (Union[Unset, List[str]]):
-        nlp_language (Union[Unset, NlpLanguage]):  Default: NlpLanguage.AUTO_DETECT.
-        draft_mode (Union[Unset, bool]):
-        hold_out_percentage (Union[Unset, float]):  Default: 10.0.
-        no_mixing_columns (Union[Unset, List[str]]):
-        partition_column (Union[Unset, str]):
-        order_by_column (Union[Unset, str]):
-        weight_column (Union[Unset, str]):
-        model_types (Union[Unset, List[RegressionModelType]]): If omitted - all eligable model types are chosen.
-    """
-
+    """  """
     name: str
     data_set_id: int
     target_column: str
     score_to_optimize: RegressionScorers
     model_validation_method: ModelValidationMethod
     data_partition_method: DataPartitionMethod
     number_of_evaluations: int
     description: Union[Unset, str] = UNSET
-    target_distribution: Union[Unset, TargetDistributions] = TargetDistributions.GAUSSIAN
     excluded_columns: Union[Unset, List[str]] = UNSET
     nlp_language: Union[Unset, NlpLanguage] = NlpLanguage.AUTO_DETECT
     draft_mode: Union[Unset, bool] = UNSET
-    hold_out_percentage: Union[Unset, float] = 10.0
     no_mixing_columns: Union[Unset, List[str]] = UNSET
     partition_column: Union[Unset, str] = UNSET
     order_by_column: Union[Unset, str] = UNSET
     weight_column: Union[Unset, str] = UNSET
     model_types: Union[Unset, List[RegressionModelType]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        data_set_id = self.data_set_id
-        target_column = self.target_column
+        name =  self.name
+        data_set_id =  self.data_set_id
+        target_column =  self.target_column
         score_to_optimize = self.score_to_optimize.value
 
         model_validation_method = self.model_validation_method.value
 
         data_partition_method = self.data_partition_method.value
 
-        number_of_evaluations = self.number_of_evaluations
-        description = self.description
-        target_distribution: Union[Unset, str] = UNSET
-        if not isinstance(self.target_distribution, Unset):
-            target_distribution = self.target_distribution.value
-
-        excluded_columns: Union[Unset, List[str]] = UNSET
+        number_of_evaluations =  self.number_of_evaluations
+        description =  self.description
+        excluded_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.excluded_columns, Unset):
             excluded_columns = self.excluded_columns
 
 
 
 
-        nlp_language: Union[Unset, str] = UNSET
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         if not isinstance(self.nlp_language, Unset):
-            nlp_language = self.nlp_language.value
+            nlp_language = self.nlp_language
 
-        draft_mode = self.draft_mode
-        hold_out_percentage = self.hold_out_percentage
-        no_mixing_columns: Union[Unset, List[str]] = UNSET
+        draft_mode =  self.draft_mode
+        no_mixing_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.no_mixing_columns, Unset):
             no_mixing_columns = self.no_mixing_columns
 
 
 
 
-        partition_column = self.partition_column
-        order_by_column = self.order_by_column
-        weight_column = self.weight_column
-        model_types: Union[Unset, List[str]] = UNSET
+        partition_column =  self.partition_column
+        order_by_column =  self.order_by_column
+        weight_column =  self.weight_column
+        model_types: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.model_types, Unset):
             model_types = []
             for model_types_item_data in self.model_types:
                 model_types_item = model_types_item_data.value
 
                 model_types.append(model_types_item)
 
@@ -117,39 +88,33 @@
             "scoreToOptimize": score_to_optimize,
             "modelValidationMethod": model_validation_method,
             "dataPartitionMethod": data_partition_method,
             "numberOfEvaluations": number_of_evaluations,
         })
         if description is not UNSET:
             field_dict["description"] = description
-        if target_distribution is not UNSET:
-            field_dict["targetDistribution"] = target_distribution
         if excluded_columns is not UNSET:
             field_dict["excludedColumns"] = excluded_columns
         if nlp_language is not UNSET:
             field_dict["nlpLanguage"] = nlp_language
         if draft_mode is not UNSET:
             field_dict["draftMode"] = draft_mode
-        if hold_out_percentage is not UNSET:
-            field_dict["holdOutPercentage"] = hold_out_percentage
         if no_mixing_columns is not UNSET:
             field_dict["noMixingColumns"] = no_mixing_columns
         if partition_column is not UNSET:
             field_dict["partitionColumn"] = partition_column
         if order_by_column is not UNSET:
             field_dict["orderByColumn"] = order_by_column
         if weight_column is not UNSET:
             field_dict["weightColumn"] = weight_column
         if model_types is not UNSET:
             field_dict["modelTypes"] = model_types
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         data_set_id = d.pop("dataSetId")
 
@@ -170,41 +135,27 @@
 
 
 
         number_of_evaluations = d.pop("numberOfEvaluations")
 
         description = d.pop("description", UNSET)
 
-        _target_distribution = d.pop("targetDistribution", UNSET)
-        target_distribution: Union[Unset, TargetDistributions]
-        if isinstance(_target_distribution,  Unset):
-            target_distribution = UNSET
-        else:
-            target_distribution = TargetDistributions(_target_distribution)
-
-
-
-
         excluded_columns = cast(List[str], d.pop("excludedColumns", UNSET))
 
 
+        nlp_language: Union[Unset, NlpLanguage] = UNSET
         _nlp_language = d.pop("nlpLanguage", UNSET)
-        nlp_language: Union[Unset, NlpLanguage]
-        if isinstance(_nlp_language,  Unset):
-            nlp_language = UNSET
-        else:
+        if not isinstance(_nlp_language,  Unset):
             nlp_language = NlpLanguage(_nlp_language)
 
 
 
 
         draft_mode = d.pop("draftMode", UNSET)
 
-        hold_out_percentage = d.pop("holdOutPercentage", UNSET)
-
         no_mixing_columns = cast(List[str], d.pop("noMixingColumns", UNSET))
 
 
         partition_column = d.pop("partitionColumn", UNSET)
 
         order_by_column = d.pop("orderByColumn", UNSET)
 
@@ -225,19 +176,17 @@
             data_set_id=data_set_id,
             target_column=target_column,
             score_to_optimize=score_to_optimize,
             model_validation_method=model_validation_method,
             data_partition_method=data_partition_method,
             number_of_evaluations=number_of_evaluations,
             description=description,
-            target_distribution=target_distribution,
             excluded_columns=excluded_columns,
             nlp_language=nlp_language,
             draft_mode=draft_mode,
-            hold_out_percentage=hold_out_percentage,
             no_mixing_columns=no_mixing_columns,
             partition_column=partition_column,
             order_by_column=order_by_column,
             weight_column=weight_column,
             model_types=model_types,
         )
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/create_test_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_file_data_set_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,71 @@
+from io import BytesIO
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..types import UNSET, Unset
+from ..types import UNSET, File, Unset
 
-T = TypeVar("T", bound="CreateTestRequest")
+T = TypeVar("T", bound="CreateFileDataSetRequest")
 
 @attr.s(auto_attribs=True)
-class CreateTestRequest:
-    """
-    Attributes:
-        model_id (int):
-        data_set_id (int):
-        name (Union[Unset, str]):
-        description (Union[Unset, None, str]):
-    """
-
-    model_id: int
-    data_set_id: int
-    name: Union[Unset, str] = UNSET
-    description: Union[Unset, None, str] = UNSET
+class CreateFileDataSetRequest:
+    """  """
+    name: str
+    data: File
+    description: Union[Unset, str] = UNSET
+    parse_options: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        model_id = self.model_id
-        data_set_id = self.data_set_id
-        name = self.name
-        description = self.description
+        name =  self.name
+        data = self.data.to_tuple()
+
+        description =  self.description
+        parse_options =  self.parse_options
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "modelId": model_id,
-            "dataSetId": data_set_id,
+            "name": name,
+            "data": data,
         })
-        if name is not UNSET:
-            field_dict["name"] = name
         if description is not UNSET:
             field_dict["description"] = description
+        if parse_options is not UNSET:
+            field_dict["parseOptions"] = parse_options
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        model_id = d.pop("modelId")
+        name = d.pop("name")
+
+        data = File(
+             payload = BytesIO(d.pop("data"))
+        )
+
 
-        data_set_id = d.pop("dataSetId")
 
-        name = d.pop("name", UNSET)
 
         description = d.pop("description", UNSET)
 
-        create_test_request = cls(
-            model_id=model_id,
-            data_set_id=data_set_id,
+        parse_options = d.pop("parseOptions", UNSET)
+
+        create_file_data_set_request = cls(
             name=name,
+            data=data,
             description=description,
+            parse_options=parse_options,
         )
 
-        create_test_request.additional_properties = d
-        return create_test_request
+        create_file_data_set_request.additional_properties = d
+        return create_file_data_set_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_pipeline_create_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_pipeline_create_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import attr
 
 T = TypeVar("T", bound="DataPipelineCreateRequest")
 
 @attr.s(auto_attribs=True)
 class DataPipelineCreateRequest:
-    """
-    Attributes:
-        data_set_id (int):
-        name (str):
-    """
-
+    """  """
     data_set_id: int
     name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        data_set_id = self.data_set_id
-        name = self.name
+        data_set_id =  self.data_set_id
+        name =  self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "dataSetId": data_set_id,
             "name": name,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         data_set_id = d.pop("dataSetId")
 
         name = d.pop("name")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_pipelines_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_pipelines_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from ..models.data_pipeline_response import DataPipelineResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DataPipelinesResponse")
 
 @attr.s(auto_attribs=True)
 class DataPipelinesResponse:
-    """
-    Attributes:
-        pipelines (Union[Unset, List[DataPipelineResponse]]):
-    """
-
+    """  """
     pipelines: Union[Unset, List[DataPipelineResponse]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        pipelines: Union[Unset, List[Dict[str, Any]]] = UNSET
+        pipelines: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.pipelines, Unset):
             pipelines = []
             for pipelines_item_data in self.pipelines:
                 pipelines_item = pipelines_item_data.to_dict()
 
                 pipelines.append(pipelines_item)
 
@@ -36,16 +32,14 @@
         field_dict.update({
         })
         if pipelines is not UNSET:
             field_dict["pipelines"] = pipelines
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         pipelines = []
         _pipelines = d.pop("pipelines", UNSET)
         for pipelines_item_data in (_pipelines or []):
             pipelines_item = DataPipelineResponse.from_dict(pipelines_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_set_column_metadata_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_data_set_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,64 @@
-from typing import Any, Dict, List, Type, TypeVar
+from io import BytesIO
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
-from ..models.api_column_level import ApiColumnLevel
-from ..models.api_column_type import ApiColumnType
+from ..types import UNSET, File, Unset
 
-T = TypeVar("T", bound="DataSetColumnMetadataResponse")
+T = TypeVar("T", bound="CreateDataSetRequest")
 
 @attr.s(auto_attribs=True)
-class DataSetColumnMetadataResponse:
-    """
-    Attributes:
-        name (str):
-        type (ApiColumnType):
-        level (ApiColumnLevel):
-    """
-
+class CreateDataSetRequest:
+    """  """
     name: str
-    type: ApiColumnType
-    level: ApiColumnLevel
+    data: File
+    description: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        type = self.type.value
-
-        level = self.level.value
+        name =  self.name
+        data = self.data.to_tuple()
 
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
-            "type": type,
-            "level": level,
+            "data": data,
         })
+        if description is not UNSET:
+            field_dict["description"] = description
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
-        type = ApiColumnType(d.pop("type"))
-
-
-
+        data = File(
+             payload = BytesIO(d.pop("data"))
+        )
 
-        level = ApiColumnLevel(d.pop("level"))
 
 
 
+        description = d.pop("description", UNSET)
 
-        data_set_column_metadata_response = cls(
+        create_data_set_request = cls(
             name=name,
-            type=type,
-            level=level,
+            data=data,
+            description=description,
         )
 
-        data_set_column_metadata_response.additional_properties = d
-        return data_set_column_metadata_response
+        create_data_set_request.additional_properties = d
+        return create_data_set_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/data_sets_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_sets_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 
 from ..models.data_set_response import DataSetResponse
 
 T = TypeVar("T", bound="DataSetsResponse")
 
 @attr.s(auto_attribs=True)
 class DataSetsResponse:
-    """
-    Attributes:
-        data_sets (List[DataSetResponse]):
-    """
-
+    """  """
     data_sets: List[DataSetResponse]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         data_sets = []
         for data_sets_item_data in self.data_sets:
@@ -32,16 +28,14 @@
         field_dict.update(self.additional_properties)
         field_dict.update({
             "dataSets": data_sets,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         data_sets = []
         _data_sets = d.pop("dataSets")
         for data_sets_item_data in (_data_sets):
             data_sets_item = DataSetResponse.from_dict(data_sets_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/decisioning_decision.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/decisioning_decision.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,43 +6,36 @@
 from ..models.decisioning_threshold import DecisioningThreshold
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DecisioningDecision")
 
 @attr.s(auto_attribs=True)
 class DecisioningDecision:
-    """
-    Attributes:
-        label (str):
-        rewards (List[DecisioningReward]):
-        chosen_threshold (Optional[DecisioningThreshold]):
-        optimal_threshold (Union[Unset, None, DecisioningThreshold]):
-    """
-
+    """  """
     label: str
     rewards: List[DecisioningReward]
     chosen_threshold: Optional[DecisioningThreshold]
-    optimal_threshold: Union[Unset, None, DecisioningThreshold] = UNSET
+    optimal_threshold: Union[Optional[DecisioningThreshold], Unset] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        label = self.label
+        label =  self.label
         rewards = []
         for rewards_item_data in self.rewards:
             rewards_item = rewards_item_data.to_dict()
 
             rewards.append(rewards_item)
 
 
 
 
         chosen_threshold = self.chosen_threshold.to_dict() if self.chosen_threshold else None
 
-        optimal_threshold: Union[Unset, None, Dict[str, Any]] = UNSET
+        optimal_threshold: Union[None, Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.optimal_threshold, Unset):
             optimal_threshold = self.optimal_threshold.to_dict() if self.optimal_threshold else None
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
@@ -51,16 +44,14 @@
             "chosenThreshold": chosen_threshold,
         })
         if optimal_threshold is not UNSET:
             field_dict["optimalThreshold"] = optimal_threshold
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         label = d.pop("label")
 
         rewards = []
         _rewards = d.pop("rewards")
@@ -68,31 +59,25 @@
             rewards_item = DecisioningReward.from_dict(rewards_item_data)
 
 
 
             rewards.append(rewards_item)
 
 
+        chosen_threshold = None
         _chosen_threshold = d.pop("chosenThreshold")
-        chosen_threshold: Optional[DecisioningThreshold]
-        if _chosen_threshold is None:
-            chosen_threshold = None
-        else:
+        if _chosen_threshold is not None:
             chosen_threshold = DecisioningThreshold.from_dict(_chosen_threshold)
 
 
 
 
+        optimal_threshold = None
         _optimal_threshold = d.pop("optimalThreshold", UNSET)
-        optimal_threshold: Union[Unset, None, DecisioningThreshold]
-        if _optimal_threshold is None:
-            optimal_threshold = None
-        elif isinstance(_optimal_threshold,  Unset):
-            optimal_threshold = UNSET
-        else:
+        if _optimal_threshold is not None and not isinstance(_optimal_threshold,  Unset):
             optimal_threshold = DecisioningThreshold.from_dict(_optimal_threshold)
 
 
 
 
         decisioning_decision = cls(
             label=label,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/decisioning_reward.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/decisioning_reward.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import attr
 
 T = TypeVar("T", bound="DecisioningReward")
 
 @attr.s(auto_attribs=True)
 class DecisioningReward:
-    """
-    Attributes:
-        class_name (str):
-        reward (float):
-    """
-
+    """  """
     class_name: str
     reward: float
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        class_name = self.class_name
-        reward = self.reward
+        class_name =  self.class_name
+        reward =  self.reward
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "className": class_name,
             "reward": reward,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         class_name = d.pop("className")
 
         reward = d.pop("reward")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/decisioning_threshold.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/decisioning_threshold.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import attr
 
 T = TypeVar("T", bound="DecisioningThreshold")
 
 @attr.s(auto_attribs=True)
 class DecisioningThreshold:
-    """
-    Attributes:
-        upper (float):
-        lower (float):
-    """
-
+    """  """
     upper: float
     lower: float
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        upper = self.upper
-        lower = self.lower
+        upper =  self.upper
+        lower =  self.lower
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "upper": upper,
             "lower": lower,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         upper = d.pop("upper")
 
         lower = d.pop("lower")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/delete_data_prep_steps_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/delete_data_prep_steps_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import attr
 
 T = TypeVar("T", bound="DeleteDataPrepStepsRequest")
 
 @attr.s(auto_attribs=True)
 class DeleteDataPrepStepsRequest:
-    """
-    Attributes:
-        delete_index (int): Index of the step to delete
-        delete_children (bool): If true, also delete all subsequent steps
-    """
-
+    """  """
     delete_index: int
     delete_children: bool
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        delete_index = self.delete_index
-        delete_children = self.delete_children
+        delete_index =  self.delete_index
+        delete_children =  self.delete_children
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "deleteIndex": delete_index,
             "deleteChildren": delete_children,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         delete_index = d.pop("deleteIndex")
 
         delete_children = d.pop("deleteChildren")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_create_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_create_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,56 +2,45 @@
 
 import attr
 
 T = TypeVar("T", bound="DeployedApiClientCreateResponse")
 
 @attr.s(auto_attribs=True)
 class DeployedApiClientCreateResponse:
-    """
-    Attributes:
-        id (str):
-        project_id (str):
-        name (str):
-        created_at (str):
-        created_by (str):
-        secret (str):
-    """
-
+    """  """
     id: str
     project_id: str
     name: str
     created_at: str
     created_by: str
     secret: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        project_id = self.project_id
-        name = self.name
-        created_at = self.created_at
-        created_by = self.created_by
-        secret = self.secret
+        id =  self.id
+        project_id =  self.project_id
+        name =  self.name
+        created_at =  self.created_at
+        created_by =  self.created_by
+        secret =  self.secret
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "id": id,
             "projectId": project_id,
             "name": name,
             "createdAt": created_at,
             "createdBy": created_by,
             "secret": secret,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         project_id = d.pop("projectId")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_list_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from ..models.deployed_api_client_response import DeployedApiClientResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DeployedApiClientListResponse")
 
 @attr.s(auto_attribs=True)
 class DeployedApiClientListResponse:
-    """
-    Attributes:
-        api_clients (Union[Unset, List[DeployedApiClientResponse]]):
-    """
-
+    """  """
     api_clients: Union[Unset, List[DeployedApiClientResponse]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        api_clients: Union[Unset, List[Dict[str, Any]]] = UNSET
+        api_clients: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.api_clients, Unset):
             api_clients = []
             for api_clients_item_data in self.api_clients:
                 api_clients_item = api_clients_item_data.to_dict()
 
                 api_clients.append(api_clients_item)
 
@@ -36,16 +32,14 @@
         field_dict.update({
         })
         if api_clients is not UNSET:
             field_dict["apiClients"] = api_clients
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         api_clients = []
         _api_clients = d.pop("apiClients", UNSET)
         for api_clients_item_data in (_api_clients or []):
             api_clients_item = DeployedApiClientResponse.from_dict(api_clients_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_api_client_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,52 +2,42 @@
 
 import attr
 
 T = TypeVar("T", bound="DeployedApiClientResponse")
 
 @attr.s(auto_attribs=True)
 class DeployedApiClientResponse:
-    """
-    Attributes:
-        id (str):
-        project_id (str):
-        name (str):
-        created_at (str):
-        created_by (str):
-    """
-
+    """  """
     id: str
     project_id: str
     name: str
     created_at: str
     created_by: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        project_id = self.project_id
-        name = self.name
-        created_at = self.created_at
-        created_by = self.created_by
+        id =  self.id
+        project_id =  self.project_id
+        name =  self.name
+        created_at =  self.created_at
+        created_by =  self.created_by
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "id": id,
             "projectId": project_id,
             "name": name,
             "createdAt": created_at,
             "createdBy": created_by,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         project_id = d.pop("projectId")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_list_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from ..models.deployed_model_api_response import DeployedModelApiResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DeployedModelApiListResponse")
 
 @attr.s(auto_attribs=True)
 class DeployedModelApiListResponse:
-    """
-    Attributes:
-        published_models (Union[Unset, List[DeployedModelApiResponse]]):
-    """
-
+    """  """
     published_models: Union[Unset, List[DeployedModelApiResponse]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        published_models: Union[Unset, List[Dict[str, Any]]] = UNSET
+        published_models: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.published_models, Unset):
             published_models = []
             for published_models_item_data in self.published_models:
                 published_models_item = published_models_item_data.to_dict()
 
                 published_models.append(published_models_item)
 
@@ -36,16 +32,14 @@
         field_dict.update({
         })
         if published_models is not UNSET:
             field_dict["publishedModels"] = published_models
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         published_models = []
         _published_models = d.pop("publishedModels", UNSET)
         for published_models_item_data in (_published_models or []):
             published_models_item = DeployedModelApiResponse.from_dict(published_models_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_model_api_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,45 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
 from ..models.api_history_response import ApiHistoryResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DeployedModelApiResponse")
 
 @attr.s(auto_attribs=True)
 class DeployedModelApiResponse:
-    """
-    Attributes:
-        id (int):
-        project_id (int):
-        name (str):
-        api_endpoint (str):
-        documentation_endpoint (str):
-        history (List[ApiHistoryResponse]):
-        description (Union[Unset, None, str]):
-    """
-
+    """  """
     id: int
     project_id: int
     name: str
     api_endpoint: str
     documentation_endpoint: str
     history: List[ApiHistoryResponse]
-    description: Union[Unset, None, str] = UNSET
+    description: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        project_id = self.project_id
-        name = self.name
-        api_endpoint = self.api_endpoint
-        documentation_endpoint = self.documentation_endpoint
+        id =  self.id
+        project_id =  self.project_id
+        name =  self.name
+        api_endpoint =  self.api_endpoint
+        documentation_endpoint =  self.documentation_endpoint
         history = []
         for history_item_data in self.history:
             history_item = history_item_data.to_dict()
 
             history.append(history_item)
 
 
 
 
-        description = self.description
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "id": id,
             "projectId": project_id,
             "name": name,
@@ -58,16 +48,14 @@
             "history": history,
         })
         if description is not UNSET:
             field_dict["description"] = description
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         project_id = d.pop("projectId")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_list_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_list_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from ..models.deployed_pipeline_api_response import DeployedPipelineApiResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DeployedPipelineApiListResponse")
 
 @attr.s(auto_attribs=True)
 class DeployedPipelineApiListResponse:
-    """
-    Attributes:
-        published_pipelines (Union[Unset, List[DeployedPipelineApiResponse]]):
-    """
-
+    """  """
     published_pipelines: Union[Unset, List[DeployedPipelineApiResponse]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        published_pipelines: Union[Unset, List[Dict[str, Any]]] = UNSET
+        published_pipelines: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.published_pipelines, Unset):
             published_pipelines = []
             for published_pipelines_item_data in self.published_pipelines:
                 published_pipelines_item = published_pipelines_item_data.to_dict()
 
                 published_pipelines.append(published_pipelines_item)
 
@@ -36,16 +32,14 @@
         field_dict.update({
         })
         if published_pipelines is not UNSET:
             field_dict["publishedPipelines"] = published_pipelines
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         published_pipelines = []
         _published_pipelines = d.pop("publishedPipelines", UNSET)
         for published_pipelines_item_data in (_published_pipelines or []):
             published_pipelines_item = DeployedPipelineApiResponse.from_dict(published_pipelines_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/deployed_pipeline_api_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,45 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
 from ..models.api_history_response import ApiHistoryResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DeployedPipelineApiResponse")
 
 @attr.s(auto_attribs=True)
 class DeployedPipelineApiResponse:
-    """
-    Attributes:
-        id (int):
-        project_id (int):
-        name (str):
-        api_endpoint (str):
-        documentation_endpoint (str):
-        history (List[ApiHistoryResponse]):
-        description (Union[Unset, None, str]):
-    """
-
+    """  """
     id: int
     project_id: int
     name: str
     api_endpoint: str
     documentation_endpoint: str
     history: List[ApiHistoryResponse]
-    description: Union[Unset, None, str] = UNSET
+    description: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        project_id = self.project_id
-        name = self.name
-        api_endpoint = self.api_endpoint
-        documentation_endpoint = self.documentation_endpoint
+        id =  self.id
+        project_id =  self.project_id
+        name =  self.name
+        api_endpoint =  self.api_endpoint
+        documentation_endpoint =  self.documentation_endpoint
         history = []
         for history_item_data in self.history:
             history_item = history_item_data.to_dict()
 
             history.append(history_item)
 
 
 
 
-        description = self.description
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "id": id,
             "projectId": project_id,
             "name": name,
@@ -58,16 +48,14 @@
             "history": history,
         })
         if description is not UNSET:
             field_dict["description"] = description
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         project_id = d.pop("projectId")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/discriminators.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/discriminators.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,23 @@
 from ..models.discriminators_column_values_item import DiscriminatorsColumnValuesItem
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="Discriminators")
 
 @attr.s(auto_attribs=True)
 class Discriminators:
-    """
-    Attributes:
-        empty (bool):
-        column_values (Union[Unset, List[DiscriminatorsColumnValuesItem]]):
-    """
-
+    """  """
     empty: bool
     column_values: Union[Unset, List[DiscriminatorsColumnValuesItem]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        empty = self.empty
-        column_values: Union[Unset, List[Dict[str, Any]]] = UNSET
+        empty =  self.empty
+        column_values: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.column_values, Unset):
             column_values = []
             for column_values_item_data in self.column_values:
                 column_values_item = column_values_item_data.to_dict()
 
                 column_values.append(column_values_item)
 
@@ -40,16 +35,14 @@
             "empty": empty,
         })
         if column_values is not UNSET:
             field_dict["columnValues"] = column_values
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         empty = d.pop("empty")
 
         column_values = []
         _column_values = d.pop("columnValues", UNSET)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/discriminators_column_values_item.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/discriminators_column_values_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,31 +6,25 @@
 
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="DiscriminatorsColumnValuesItem")
 
 @attr.s(auto_attribs=True)
 class DiscriminatorsColumnValuesItem:
-    """
-    Attributes:
-        column_name (Union[Unset, str]):
-        value (Union[Unset, datetime.datetime, float, int, str]):
-    """
-
+    """  """
     column_name: Union[Unset, str] = UNSET
-    value: Union[Unset, datetime.datetime, float, int, str] = UNSET
+    value: Union[Unset, str, float, int, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column_name = self.column_name
-        value: Union[Unset, float, int, str]
+        column_name =  self.column_name
+        value: Union[Unset, str, float, int, datetime.datetime]
         if isinstance(self.value, Unset):
             value = UNSET
-
         elif isinstance(self.value, datetime.datetime):
             value = UNSET
             if not isinstance(self.value, Unset):
                 value = self.value.isoformat()
 
         else:
             value = self.value
@@ -44,40 +38,34 @@
         if column_name is not UNSET:
             field_dict["columnName"] = column_name
         if value is not UNSET:
             field_dict["value"] = value
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         column_name = d.pop("columnName", UNSET)
 
-        def _parse_value(data: object) -> Union[Unset, datetime.datetime, float, int, str]:
-            if isinstance(data, Unset):
-                return data
+        def _parse_value(data: Any) -> Union[Unset, str, float, int, datetime.datetime]:
+            data = None if isinstance(data, Unset) else data
+            value: Union[Unset, str, float, int, datetime.datetime]
             try:
-                if not isinstance(data, str):
-                    raise TypeError()
-                _value_type_3 = data
-                value_type_3: Union[Unset, datetime.datetime]
-                if isinstance(_value_type_3,  Unset):
-                    value_type_3 = UNSET
-                else:
-                    value_type_3 = isoparse(_value_type_3)
+                value = UNSET
+                _value = data
+                if not isinstance(_value,  Unset):
+                    value = isoparse(_value)
 
 
 
-                return value_type_3
+                return value
             except: # noqa: E722
                 pass
-            return cast(Union[Unset, datetime.datetime, float, int, str], data)
+            return cast(Union[Unset, str, float, int, datetime.datetime], data)
 
         value = _parse_value(d.pop("value", UNSET))
 
 
         discriminators_column_values_item = cls(
             column_name=column_name,
             value=value,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/drop_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/drop_step.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,15 @@
 
 from ..models.drop_step_step_type import DropStepStepType
 
 T = TypeVar("T", bound="DropStep")
 
 @attr.s(auto_attribs=True)
 class DropStep:
-    """
-    Attributes:
-        columns (List[str]):
-        step_type (DropStepStepType):
-    """
-
+    """  """
     columns: List[str]
     step_type: DropStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         columns = self.columns
@@ -33,16 +28,14 @@
         field_dict.update({
             "columns": columns,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         columns = cast(List[str], d.pop("columns"))
 
 
         step_type = DropStepStepType(d.pop("stepType"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_data_pipeline_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_prep_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="EditDataPipelineRequest")
+T = TypeVar("T", bound="DataPrepStep")
 
 @attr.s(auto_attribs=True)
-class EditDataPipelineRequest:
-    """
-    Attributes:
-        name (str):
-    """
-
-    name: str
+class DataPrepStep:
+    """  """
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "name": name,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
-
-        edit_data_pipeline_request = cls(
-            name=name,
+        data_prep_step = cls(
         )
 
-        edit_data_pipeline_request.additional_properties = d
-        return edit_data_pipeline_request
+        data_prep_step.additional_properties = d
+        return data_prep_step
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_data_set_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_test_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="EditDataSetRequest")
+T = TypeVar("T", bound="EditTestRequest")
 
 @attr.s(auto_attribs=True)
-class EditDataSetRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
+class EditTestRequest:
+    """  """
     name: str
     description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
 
-        edit_data_set_request = cls(
+        edit_test_request = cls(
             name=name,
             description=description,
         )
 
-        edit_data_set_request.additional_properties = d
-        return edit_data_set_request
+        edit_test_request.additional_properties = d
+        return edit_test_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_deployed_model_api_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_model_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="EditDeployedModelApiRequest")
+T = TypeVar("T", bound="EditModelRequest")
 
 @attr.s(auto_attribs=True)
-class EditDeployedModelApiRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
+class EditModelRequest:
+    """  """
     name: str
     description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
 
-        edit_deployed_model_api_request = cls(
+        edit_model_request = cls(
             name=name,
             description=description,
         )
 
-        edit_deployed_model_api_request.additional_properties = d
-        return edit_deployed_model_api_request
+        edit_model_request.additional_properties = d
+        return edit_model_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_deployed_pipeline_api_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_deployed_model_api_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="EditDeployedPipelineApiRequest")
+T = TypeVar("T", bound="EditDeployedModelApiRequest")
 
 @attr.s(auto_attribs=True)
-class EditDeployedPipelineApiRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
+class EditDeployedModelApiRequest:
+    """  """
     name: str
     description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
 
-        edit_deployed_pipeline_api_request = cls(
+        edit_deployed_model_api_request = cls(
             name=name,
             description=description,
         )
 
-        edit_deployed_pipeline_api_request.additional_properties = d
-        return edit_deployed_pipeline_api_request
+        edit_deployed_model_api_request.additional_properties = d
+        return edit_deployed_model_api_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_model_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/save_prediction_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="EditModelRequest")
+T = TypeVar("T", bound="SavePredictionRequest")
 
 @attr.s(auto_attribs=True)
-class EditModelRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
+class SavePredictionRequest:
+    """  """
     name: str
     description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
 
-        edit_model_request = cls(
+        save_prediction_request = cls(
             name=name,
             description=description,
         )
 
-        edit_model_request.additional_properties = d
-        return edit_model_request
+        save_prediction_request.additional_properties = d
+        return save_prediction_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_prediction_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/edit_prediction_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import attr
 
 T = TypeVar("T", bound="EditPredictionRequest")
 
 @attr.s(auto_attribs=True)
 class EditPredictionRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
+    """  """
     name: str
     description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/edit_test_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/save_test_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,48 @@
 from typing import Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="EditTestRequest")
+T = TypeVar("T", bound="SaveTestRequest")
 
 @attr.s(auto_attribs=True)
-class EditTestRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
+class SaveTestRequest:
+    """  """
     name: str
     description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
 
-        edit_test_request = cls(
+        save_test_request = cls(
             name=name,
             description=description,
         )
 
-        edit_test_request.additional_properties = d
-        return edit_test_request
+        save_test_request.additional_properties = d
+        return save_test_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/excel_parse_options.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/excel_parse_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,28 @@
 from ..models.excel_parse_options_file_type import ExcelParseOptionsFileType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ExcelParseOptions")
 
 @attr.s(auto_attribs=True)
 class ExcelParseOptions:
-    """
-    Attributes:
-        file_type (ExcelParseOptionsFileType):
-        column_names_in_header (Union[Unset, bool]): The first row contains column names
-        skip_top (Union[Unset, int]): Ignore the first n rows
-        skip_bottom (Union[Unset, int]): Ignore the last n rows
-    """
-
+    """  """
     file_type: ExcelParseOptionsFileType
     column_names_in_header: Union[Unset, bool] = False
     skip_top: Union[Unset, int] = 0
     skip_bottom: Union[Unset, int] = 0
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         file_type = self.file_type.value
 
-        column_names_in_header = self.column_names_in_header
-        skip_top = self.skip_top
-        skip_bottom = self.skip_bottom
+        column_names_in_header =  self.column_names_in_header
+        skip_top =  self.skip_top
+        skip_bottom =  self.skip_bottom
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "fileType": file_type,
         })
         if column_names_in_header is not UNSET:
@@ -41,16 +34,14 @@
         if skip_top is not UNSET:
             field_dict["skipTop"] = skip_top
         if skip_bottom is not UNSET:
             field_dict["skipBottom"] = skip_bottom
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         file_type = ExcelParseOptionsFileType(d.pop("fileType"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,49 +4,41 @@
 
 from ..models.fill_missing_value_step_step_type import FillMissingValueStepStepType
 
 T = TypeVar("T", bound="FillMissingValueStep")
 
 @attr.s(auto_attribs=True)
 class FillMissingValueStep:
-    """
-    Attributes:
-        columns (List[str]):
-        default_value (str):
-        step_type (FillMissingValueStepStepType):
-    """
-
+    """  """
     columns: List[str]
     default_value: str
     step_type: FillMissingValueStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         columns = self.columns
 
 
 
 
-        default_value = self.default_value
+        default_value =  self.default_value
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "columns": columns,
             "defaultValue": default_value,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         columns = cast(List[str], d.pop("columns"))
 
 
         default_value = d.pop("defaultValue")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/filter_rows_rule.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/filter_rows_rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,35 +5,28 @@
 from ..models.filter_rows_rule_rule import FilterRowsRuleRule
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="FilterRowsRule")
 
 @attr.s(auto_attribs=True)
 class FilterRowsRule:
-    """
-    Attributes:
-        rule (FilterRowsRuleRule):
-        value1 (Union[Unset, str]):
-        inclusive (Union[Unset, bool]):
-        inclusive_between (Union[Unset, bool]):
-    """
-
+    """  """
     rule: FilterRowsRuleRule
     value1: Union[Unset, str] = UNSET
     inclusive: Union[Unset, bool] = UNSET
     inclusive_between: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         rule = self.rule.value
 
-        value1 = self.value1
-        inclusive = self.inclusive
-        inclusive_between = self.inclusive_between
+        value1 =  self.value1
+        inclusive =  self.inclusive
+        inclusive_between =  self.inclusive_between
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "rule": rule,
         })
         if value1 is not UNSET:
@@ -41,16 +34,14 @@
         if inclusive is not UNSET:
             field_dict["inclusive"] = inclusive
         if inclusive_between is not UNSET:
             field_dict["inclusiveBetween"] = inclusive_between
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         rule = FilterRowsRuleRule(d.pop("rule"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/filter_rows_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/filter_rows_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 from ..models.filter_rows_rule import FilterRowsRule
 from ..models.filter_rows_step_step_type import FilterRowsStepStepType
 
 T = TypeVar("T", bound="FilterRowsStep")
 
 @attr.s(auto_attribs=True)
 class FilterRowsStep:
-    """
-    Attributes:
-        rules (List[FilterRowsRule]):
-        step_type (FilterRowsStepStepType):
-    """
-
+    """  """
     rules: List[FilterRowsRule]
     step_type: FilterRowsStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         rules = []
@@ -38,16 +33,14 @@
         field_dict.update({
             "rules": rules,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         rules = []
         _rules = d.pop("rules")
         for rules_item_data in (_rules):
             rules_item = FilterRowsRule.from_dict(rules_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/future.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/future.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
-from ..models.future_output_of_your_request import FutureOutputOfYourRequest
+from ..models.future_outputofyourrequest import FutureOutputofyourrequest
 from ..models.status import Status
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="Future")
 
 @attr.s(auto_attribs=True)
 class Future:
-    """
-    Attributes:
-        future_id (Union[Unset, str]):
-        status (Union[Unset, Status]):
-        response (Union[Unset, None, FutureOutputOfYourRequest]):
-    """
-
+    """  """
     future_id: Union[Unset, str] = UNSET
     status: Union[Unset, Status] = UNSET
-    response: Union[Unset, None, FutureOutputOfYourRequest] = UNSET
+    response: Union[Optional[FutureOutputofyourrequest], Unset] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        future_id = self.future_id
-        status: Union[Unset, str] = UNSET
+        future_id =  self.future_id
+        status: Union[Unset, Status] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
 
-        response: Union[Unset, None, Dict[str, Any]] = UNSET
+        response: Union[None, Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.response, Unset):
             response = self.response.to_dict() if self.response else None
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
@@ -43,39 +37,31 @@
         if status is not UNSET:
             field_dict["status"] = status
         if response is not UNSET:
             field_dict["response"] = response
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         future_id = d.pop("futureId", UNSET)
 
+        status: Union[Unset, Status] = UNSET
         _status = d.pop("status", UNSET)
-        status: Union[Unset, Status]
-        if isinstance(_status,  Unset):
-            status = UNSET
-        else:
+        if not isinstance(_status,  Unset):
             status = Status(_status)
 
 
 
 
+        response = None
         _response = d.pop("response", UNSET)
-        response: Union[Unset, None, FutureOutputOfYourRequest]
-        if _response is None:
-            response = None
-        elif isinstance(_response,  Unset):
-            response = UNSET
-        else:
-            response = FutureOutputOfYourRequest.from_dict(_response)
+        if _response is not None and not isinstance(_response,  Unset):
+            response = FutureOutputofyourrequest.from_dict(_response)
 
 
 
 
         future = cls(
             future_id=future_id,
             status=status,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/future_output_of_your_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_score.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="FutureOutputOfYourRequest")
+from ..models.score_type import ScoreType
 
-@attr.s(auto_attribs=True)
-class FutureOutputOfYourRequest:
-    """
-    """
+T = TypeVar("T", bound="ModelScore")
 
+@attr.s(auto_attribs=True)
+class ModelScore:
+    """  """
+    value: float
+    type: ScoreType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        
+        value =  self.value
+        type = self.type.value
+
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
+            "value": value,
+            "type": type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        future_output_of_your_request = cls(
+        value = d.pop("value")
+
+        type = ScoreType(d.pop("type"))
+
+
+
+
+        model_score = cls(
+            value=value,
+            type=type,
         )
 
-        future_output_of_your_request.additional_properties = d
-        return future_output_of_your_request
+        model_score.additional_properties = d
+        return model_score
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/group_by_aggregation.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/group_by_aggregation.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,45 +4,37 @@
 
 from ..models.group_by_aggregation_rule import GroupByAggregationRule
 
 T = TypeVar("T", bound="GroupByAggregation")
 
 @attr.s(auto_attribs=True)
 class GroupByAggregation:
-    """
-    Attributes:
-        target_column (str):
-        new_column_name (str):
-        rule (GroupByAggregationRule):
-    """
-
+    """  """
     target_column: str
     new_column_name: str
     rule: GroupByAggregationRule
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        target_column = self.target_column
-        new_column_name = self.new_column_name
+        target_column =  self.target_column
+        new_column_name =  self.new_column_name
         rule = self.rule.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "targetColumn": target_column,
             "newColumnName": new_column_name,
             "rule": rule,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         target_column = d.pop("targetColumn")
 
         new_column_name = d.pop("newColumnName")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/group_by_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/group_by_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,15 @@
 from ..models.group_by_aggregation import GroupByAggregation
 from ..models.group_by_step_step_type import GroupByStepStepType
 
 T = TypeVar("T", bound="GroupByStep")
 
 @attr.s(auto_attribs=True)
 class GroupByStep:
-    """
-    Attributes:
-        key_columns (List[str]):
-        aggregations (List[GroupByAggregation]):
-        step_type (GroupByStepStepType):
-    """
-
+    """  """
     key_columns: List[str]
     aggregations: List[GroupByAggregation]
     step_type: GroupByStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
@@ -46,16 +40,14 @@
             "keyColumns": key_columns,
             "aggregations": aggregations,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         key_columns = cast(List[str], d.pop("keyColumns"))
 
 
         aggregations = []
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/id_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/parse_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,36 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="IdResponse")
+T = TypeVar("T", bound="ParseOptions")
 
 @attr.s(auto_attribs=True)
-class IdResponse:
-    """
-    Attributes:
-        id (int):
-    """
-
-    id: int
+class ParseOptions:
+    """  """
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "id": id,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        id = d.pop("id")
-
-        id_response = cls(
-            id=id,
+        parse_options = cls(
         )
 
-        id_response.additional_properties = d
-        return id_response
+        parse_options.additional_properties = d
+        return parse_options
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/json_parse_options.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/json_parse_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,15 @@
 
 from ..models.json_parse_options_file_type import JsonParseOptionsFileType
 
 T = TypeVar("T", bound="JsonParseOptions")
 
 @attr.s(auto_attribs=True)
 class JsonParseOptions:
-    """
-    Attributes:
-        file_type (JsonParseOptionsFileType):
-    """
-
+    """  """
     file_type: JsonParseOptionsFileType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         file_type = self.file_type.value
 
@@ -25,16 +21,14 @@
         field_dict.update(self.additional_properties)
         field_dict.update({
             "fileType": file_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         file_type = JsonParseOptionsFileType(d.pop("fileType"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/merge_columns_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/merge_columns_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,41 @@
 
 from ..models.merge_columns_step_step_type import MergeColumnsStepStepType
 
 T = TypeVar("T", bound="MergeColumnsStep")
 
 @attr.s(auto_attribs=True)
 class MergeColumnsStep:
-    """
-    Attributes:
-        columns (List[str]):
-        merged_column_name (str):
-        step_type (MergeColumnsStepStepType):
-    """
-
+    """  """
     columns: List[str]
     merged_column_name: str
     step_type: MergeColumnsStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         columns = self.columns
 
 
 
 
-        merged_column_name = self.merged_column_name
+        merged_column_name =  self.merged_column_name
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "columns": columns,
             "mergedColumnName": merged_column_name,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         columns = cast(List[str], d.pop("columns"))
 
 
         merged_column_name = d.pop("mergedColumnName")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_influence.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_influence.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import attr
 
 T = TypeVar("T", bound="ModelInfluence")
 
 @attr.s(auto_attribs=True)
 class ModelInfluence:
-    """
-    Attributes:
-        name (str):
-        value (float):
-    """
-
+    """  """
     name: str
     value: float
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        value = self.value
+        name =  self.name
+        value =  self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "value": value,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         value = d.pop("value")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_list_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/model_list_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from ..models.model_response import ModelResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ModelListResponse")
 
 @attr.s(auto_attribs=True)
 class ModelListResponse:
-    """
-    Attributes:
-        models (Union[Unset, List[ModelResponse]]):
-    """
-
+    """  """
     models: Union[Unset, List[ModelResponse]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        models: Union[Unset, List[Dict[str, Any]]] = UNSET
+        models: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.models, Unset):
             models = []
             for models_item_data in self.models:
                 models_item = models_item_data.to_dict()
 
                 models.append(models_item)
 
@@ -36,16 +32,14 @@
         field_dict.update({
         })
         if models is not UNSET:
             field_dict["models"] = models
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         models = []
         _models = d.pop("models", UNSET)
         for models_item_data in (_models or []):
             models_item = ModelResponse.from_dict(models_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/model_score.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/update_deployed_model_api_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,51 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
-from ..models.score_type import ScoreType
+from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ModelScore")
+T = TypeVar("T", bound="UpdateDeployedModelApiRequest")
 
 @attr.s(auto_attribs=True)
-class ModelScore:
-    """
-    Attributes:
-        value (float):
-        type (ScoreType):
-    """
-
-    value: float
-    type: ScoreType
+class UpdateDeployedModelApiRequest:
+    """  """
+    new_model_id: int
+    notes: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        value = self.value
-        type = self.type.value
-
+        new_model_id =  self.new_model_id
+        notes =  self.notes
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "value": value,
-            "type": type,
+            "newModelId": new_model_id,
         })
+        if notes is not UNSET:
+            field_dict["notes"] = notes
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        value = d.pop("value")
-
-        type = ScoreType(d.pop("type"))
-
-
+        new_model_id = d.pop("newModelId")
 
+        notes = d.pop("notes", UNSET)
 
-        model_score = cls(
-            value=value,
-            type=type,
+        update_deployed_model_api_request = cls(
+            new_model_id=new_model_id,
+            notes=notes,
         )
 
-        model_score.additional_properties = d
-        return model_score
+        update_deployed_model_api_request.additional_properties = d
+        return update_deployed_model_api_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/nlp_language.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/nlp_language.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/normalize_text_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/normalize_text_step.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,15 @@
 from ..models.normalize_text_step_rule import NormalizeTextStepRule
 from ..models.normalize_text_step_step_type import NormalizeTextStepStepType
 
 T = TypeVar("T", bound="NormalizeTextStep")
 
 @attr.s(auto_attribs=True)
 class NormalizeTextStep:
-    """
-    Attributes:
-        columns (List[str]):
-        rule (NormalizeTextStepRule):
-        step_type (NormalizeTextStepStepType):
-    """
-
+    """  """
     columns: List[str]
     rule: NormalizeTextStepRule
     step_type: NormalizeTextStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
@@ -39,16 +33,14 @@
             "columns": columns,
             "rule": rule,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         columns = cast(List[str], d.pop("columns"))
 
 
         rule = NormalizeTextStepRule(d.pop("rule"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/null_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/null_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,37 +4,31 @@
 
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="NullRequest")
 
 @attr.s(auto_attribs=True)
 class NullRequest:
-    """
-    Attributes:
-        non_existant_property (Union[Unset, int]):
-    """
-
+    """  """
     non_existant_property: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        non_existant_property = self.non_existant_property
+        non_existant_property =  self.non_existant_property
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
         })
         if non_existant_property is not UNSET:
             field_dict["nonExistantProperty"] = non_existant_property
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         non_existant_property = d.pop("nonExistantProperty", UNSET)
 
         null_request = cls(
             non_existant_property=non_existant_property,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,22 @@
     PredictionForecastResponseModelForecastsItem,
 )
 
 T = TypeVar("T", bound="PredictionForecastResponse")
 
 @attr.s(auto_attribs=True)
 class PredictionForecastResponse:
-    """
-    Attributes:
-        id (int):
-        model_forecasts (List[PredictionForecastResponseModelForecastsItem]):
-    """
-
+    """  """
     id: int
     model_forecasts: List[PredictionForecastResponseModelForecastsItem]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
+        id =  self.id
         model_forecasts = []
         for model_forecasts_item_data in self.model_forecasts:
             model_forecasts_item = model_forecasts_item_data.to_dict()
 
             model_forecasts.append(model_forecasts_item)
 
 
@@ -38,16 +33,14 @@
         field_dict.update({
             "id": id,
             "modelForecasts": model_forecasts,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         model_forecasts = []
         _model_forecasts = d.pop("modelForecasts")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response_model_forecasts_item.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response_model_forecasts_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 from ..models.discriminators import Discriminators
 from ..models.simple_forecast import SimpleForecast
 
 T = TypeVar("T", bound="PredictionForecastResponseModelForecastsItem")
 
 @attr.s(auto_attribs=True)
 class PredictionForecastResponseModelForecastsItem:
-    """
-    Attributes:
-        discriminators (Discriminators):
-        simple_forecasts (List[SimpleForecast]):
-    """
-
+    """  """
     discriminators: Discriminators
     simple_forecasts: List[SimpleForecast]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         discriminators = self.discriminators.to_dict()
@@ -38,16 +33,14 @@
         field_dict.update({
             "discriminators": discriminators,
             "simpleForecasts": simple_forecasts,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         discriminators = Discriminators.from_dict(d.pop("discriminators"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_list_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_list_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from ..models.prediction_response import PredictionResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="PredictionListResponse")
 
 @attr.s(auto_attribs=True)
 class PredictionListResponse:
-    """
-    Attributes:
-        predictions (Union[Unset, List[PredictionResponse]]):
-    """
-
+    """  """
     predictions: Union[Unset, List[PredictionResponse]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        predictions: Union[Unset, List[Dict[str, Any]]] = UNSET
+        predictions: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.predictions, Unset):
             predictions = []
             for predictions_item_data in self.predictions:
                 predictions_item = predictions_item_data.to_dict()
 
                 predictions.append(predictions_item)
 
@@ -36,16 +32,14 @@
         field_dict.update({
         })
         if predictions is not UNSET:
             field_dict["predictions"] = predictions
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         predictions = []
         _predictions = d.pop("predictions", UNSET)
         for predictions_item_data in (_predictions or []):
             predictions_item = PredictionResponse.from_dict(predictions_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/prediction_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/prediction_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,54 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
 from ..models.prediction_response_problem_type import PredictionResponseProblemType
 from ..models.prediction_response_task_status import PredictionResponseTaskStatus
 from ..models.status import Status
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="PredictionResponse")
 
 @attr.s(auto_attribs=True)
 class PredictionResponse:
-    """
-    Attributes:
-        id (int):
-        name (str):
-        problem_type (PredictionResponseProblemType):
-        task_status (PredictionResponseTaskStatus):
-        description (Union[Unset, None, str]):
-        project_id (Union[Unset, None, int]):
-        model_id (Union[Unset, None, int]):
-        data_set_id (Union[Unset, None, int]):
-        is_multi_series (Union[Unset, None, bool]):
-        status (Union[Unset, Status]):
-        failure_details (Union[Unset, None, str]):
-        prediction_column_name (Union[Unset, None, str]):
-    """
-
+    """  """
     id: int
     name: str
     problem_type: PredictionResponseProblemType
     task_status: PredictionResponseTaskStatus
-    description: Union[Unset, None, str] = UNSET
-    project_id: Union[Unset, None, int] = UNSET
-    model_id: Union[Unset, None, int] = UNSET
-    data_set_id: Union[Unset, None, int] = UNSET
-    is_multi_series: Union[Unset, None, bool] = UNSET
+    description: Union[Unset, Optional[str]] = UNSET
+    project_id: Union[Unset, Optional[int]] = UNSET
+    model_id: Union[Unset, Optional[int]] = UNSET
+    data_set_id: Union[Unset, Optional[int]] = UNSET
+    is_multi_series: Union[Unset, Optional[bool]] = UNSET
     status: Union[Unset, Status] = UNSET
-    failure_details: Union[Unset, None, str] = UNSET
-    prediction_column_name: Union[Unset, None, str] = UNSET
+    failure_details: Union[Unset, Optional[str]] = UNSET
+    prediction_column_name: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        name = self.name
+        id =  self.id
+        name =  self.name
         problem_type = self.problem_type.value
 
         task_status = self.task_status.value
 
-        description = self.description
-        project_id = self.project_id
-        model_id = self.model_id
-        data_set_id = self.data_set_id
-        is_multi_series = self.is_multi_series
-        status: Union[Unset, str] = UNSET
+        description =  self.description
+        project_id =  self.project_id
+        model_id =  self.model_id
+        data_set_id =  self.data_set_id
+        is_multi_series =  self.is_multi_series
+        status: Union[Unset, Status] = UNSET
         if not isinstance(self.status, Unset):
-            status = self.status.value
+            status = self.status
 
-        failure_details = self.failure_details
-        prediction_column_name = self.prediction_column_name
+        failure_details =  self.failure_details
+        prediction_column_name =  self.prediction_column_name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "id": id,
             "name": name,
             "problemType": problem_type,
@@ -84,16 +69,14 @@
         if failure_details is not UNSET:
             field_dict["failureDetails"] = failure_details
         if prediction_column_name is not UNSET:
             field_dict["predictionColumnName"] = prediction_column_name
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         name = d.pop("name")
 
@@ -113,19 +96,17 @@
 
         model_id = d.pop("modelId", UNSET)
 
         data_set_id = d.pop("dataSetId", UNSET)
 
         is_multi_series = d.pop("isMultiSeries", UNSET)
 
+        status: Union[Unset, Status] = UNSET
         _status = d.pop("status", UNSET)
-        status: Union[Unset, Status]
-        if isinstance(_status,  Unset):
-            status = UNSET
-        else:
+        if not isinstance(_status,  Unset):
             status = Status(_status)
 
 
 
 
         failure_details = d.pop("failureDetails", UNSET)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/rename_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/replace_step.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar, cast
 
 import attr
 
-from ..models.rename_step_step_type import RenameStepStepType
+from ..models.replace_step_step_type import ReplaceStepStepType
 
-T = TypeVar("T", bound="RenameStep")
+T = TypeVar("T", bound="ReplaceStep")
 
 @attr.s(auto_attribs=True)
-class RenameStep:
-    """
-    Attributes:
-        column (str):
-        new_column_name (str):
-        step_type (RenameStepStepType):
-    """
-
-    column: str
-    new_column_name: str
-    step_type: RenameStepStepType
+class ReplaceStep:
+    """  """
+    columns: List[str]
+    old_value: str
+    new_value: str
+    step_type: ReplaceStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column = self.column
-        new_column_name = self.new_column_name
+        columns = self.columns
+
+
+
+
+        old_value =  self.old_value
+        new_value =  self.new_value
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "column": column,
-            "newColumnName": new_column_name,
+            "columns": columns,
+            "oldValue": old_value,
+            "newValue": new_value,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        column = d.pop("column")
+        columns = cast(List[str], d.pop("columns"))
+
+
+        old_value = d.pop("oldValue")
 
-        new_column_name = d.pop("newColumnName")
+        new_value = d.pop("newValue")
 
-        step_type = RenameStepStepType(d.pop("stepType"))
+        step_type = ReplaceStepStepType(d.pop("stepType"))
 
 
 
 
-        rename_step = cls(
-            column=column,
-            new_column_name=new_column_name,
+        replace_step = cls(
+            columns=columns,
+            old_value=old_value,
+            new_value=new_value,
             step_type=step_type,
         )
 
-        rename_step.additional_properties = d
-        return rename_step
+        replace_step.additional_properties = d
+        return replace_step
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/replace_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/create_deployed_api_client_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,42 @@
-from typing import Any, Dict, List, Type, TypeVar, cast
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..models.replace_step_step_type import ReplaceStepStepType
-
-T = TypeVar("T", bound="ReplaceStep")
+T = TypeVar("T", bound="CreateDeployedApiClientRequest")
 
 @attr.s(auto_attribs=True)
-class ReplaceStep:
-    """
-    Attributes:
-        columns (List[str]):
-        old_value (str):
-        new_value (str):
-        step_type (ReplaceStepStepType):
-    """
-
-    columns: List[str]
-    old_value: str
-    new_value: str
-    step_type: ReplaceStepStepType
+class CreateDeployedApiClientRequest:
+    """  """
+    name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        columns = self.columns
-
-
-
-
-        old_value = self.old_value
-        new_value = self.new_value
-        step_type = self.step_type.value
-
+        name =  self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "columns": columns,
-            "oldValue": old_value,
-            "newValue": new_value,
-            "stepType": step_type,
+            "name": name,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        columns = cast(List[str], d.pop("columns"))
-
-
-        old_value = d.pop("oldValue")
-
-        new_value = d.pop("newValue")
-
-        step_type = ReplaceStepStepType(d.pop("stepType"))
-
-
-
+        name = d.pop("name")
 
-        replace_step = cls(
-            columns=columns,
-            old_value=old_value,
-            new_value=new_value,
-            step_type=step_type,
+        create_deployed_api_client_request = cls(
+            name=name,
         )
 
-        replace_step.additional_properties = d
-        return replace_step
+        create_deployed_api_client_request.additional_properties = d
+        return create_deployed_api_client_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/save_model_results_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/save_model_results_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,40 +2,33 @@
 
 import attr
 
 T = TypeVar("T", bound="SaveModelResultsRequest")
 
 @attr.s(auto_attribs=True)
 class SaveModelResultsRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
+    """  """
     name: str
     description: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
+        name =  self.name
+        description =  self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         name = d.pop("name")
 
         description = d.pop("description")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/save_prediction_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/future_outputofyourrequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,36 @@
-from typing import Any, Dict, List, Optional, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SavePredictionRequest")
+T = TypeVar("T", bound="FutureOutputofyourrequest")
 
 @attr.s(auto_attribs=True)
-class SavePredictionRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
-    name: str
-    description: Optional[str]
+class FutureOutputofyourrequest:
+    """  """
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "name": name,
-            "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
-
-        description = d.pop("description")
-
-        save_prediction_request = cls(
-            name=name,
-            description=description,
+        future_outputofyourrequest = cls(
         )
 
-        save_prediction_request.additional_properties = d
-        return save_prediction_request
+        future_outputofyourrequest.additional_properties = d
+        return future_outputofyourrequest
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/save_test_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/data_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,36 @@
-from typing import Any, Dict, List, Optional, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="SaveTestRequest")
+T = TypeVar("T", bound="DataValue")
 
 @attr.s(auto_attribs=True)
-class SaveTestRequest:
-    """
-    Attributes:
-        name (str):
-        description (Optional[str]):
-    """
-
-    name: str
-    description: Optional[str]
+class DataValue:
+    """  """
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        description = self.description
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "name": name,
-            "description": description,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        name = d.pop("name")
-
-        description = d.pop("description")
-
-        save_test_request = cls(
-            name=name,
-            description=description,
+        data_value = cls(
         )
 
-        save_test_request.additional_properties = d
-        return save_test_request
+        data_value.additional_properties = d
+        return data_value
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/score_type.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/score_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,11 +24,10 @@
     CLUSTERS = "CLUSTERS"
     SILHOUETTE_COEF = "SILHOUETTE_COEF"
     F1_SINGLE_CLASS = "F1_SINGLE_CLASS"
     RECALL_SINGLE_CLASS = "RECALL_SINGLE_CLASS"
     PRECISION_SINGLE_CLASS = "PRECISION_SINGLE_CLASS"
     F5_SINGLE_CLASS = "F5_SINGLE_CLASS"
     EXPECTED_REWARD = "EXPECTED_REWARD"
-    GINI = "GINI"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/sentiment_analysis_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/sentiment_analysis_step.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,45 +4,37 @@
 
 from ..models.sentiment_analysis_step_step_type import SentimentAnalysisStepStepType
 
 T = TypeVar("T", bound="SentimentAnalysisStep")
 
 @attr.s(auto_attribs=True)
 class SentimentAnalysisStep:
-    """
-    Attributes:
-        column (str):
-        new_sentiment_column_name (str):
-        step_type (SentimentAnalysisStepStepType):
-    """
-
+    """  """
     column: str
     new_sentiment_column_name: str
     step_type: SentimentAnalysisStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column = self.column
-        new_sentiment_column_name = self.new_sentiment_column_name
+        column =  self.column
+        new_sentiment_column_name =  self.new_sentiment_column_name
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "column": column,
             "newSentimentColumnName": new_sentiment_column_name,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         column = d.pop("column")
 
         new_sentiment_column_name = d.pop("newSentimentColumnName")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_column_level_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_column_level_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,49 +4,41 @@
 
 from ..models.set_column_level_step_step_type import SetColumnLevelStepStepType
 
 T = TypeVar("T", bound="SetColumnLevelStep")
 
 @attr.s(auto_attribs=True)
 class SetColumnLevelStep:
-    """
-    Attributes:
-        columns (List[str]):
-        new_level (str):
-        step_type (SetColumnLevelStepStepType):
-    """
-
+    """  """
     columns: List[str]
     new_level: str
     step_type: SetColumnLevelStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         columns = self.columns
 
 
 
 
-        new_level = self.new_level
+        new_level =  self.new_level
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "columns": columns,
             "newLevel": new_level,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         columns = cast(List[str], d.pop("columns"))
 
 
         new_level = d.pop("newLevel")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_column_type_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_column_type_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,15 @@
 from ..models.set_column_type_step_step_type import SetColumnTypeStepStepType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="SetColumnTypeStep")
 
 @attr.s(auto_attribs=True)
 class SetColumnTypeStep:
-    """
-    Attributes:
-        columns (List[str]):
-        new_type (str):
-        step_type (SetColumnTypeStepStepType):
-        epoch (Union[Unset, str]):
-        invalid (Union[Unset, str]):
-        not_int (Union[Unset, str]):
-        default_not_int (Union[Unset, str]):
-        datetime_format (Union[Unset, str]):
-        default_value (Union[Unset, str]):
-    """
-
+    """  """
     columns: List[str]
     new_type: str
     step_type: SetColumnTypeStepStepType
     epoch: Union[Unset, str] = UNSET
     invalid: Union[Unset, str] = UNSET
     not_int: Union[Unset, str] = UNSET
     default_not_int: Union[Unset, str] = UNSET
@@ -36,23 +24,23 @@
 
     def to_dict(self) -> Dict[str, Any]:
         columns = self.columns
 
 
 
 
-        new_type = self.new_type
+        new_type =  self.new_type
         step_type = self.step_type.value
 
-        epoch = self.epoch
-        invalid = self.invalid
-        not_int = self.not_int
-        default_not_int = self.default_not_int
-        datetime_format = self.datetime_format
-        default_value = self.default_value
+        epoch =  self.epoch
+        invalid =  self.invalid
+        not_int =  self.not_int
+        default_not_int =  self.default_not_int
+        datetime_format =  self.datetime_format
+        default_value =  self.default_value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "columns": columns,
             "newType": new_type,
             "stepType": step_type,
@@ -68,16 +56,14 @@
         if datetime_format is not UNSET:
             field_dict["datetimeFormat"] = datetime_format
         if default_value is not UNSET:
             field_dict["defaultValue"] = default_value
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         columns = cast(List[str], d.pop("columns"))
 
 
         new_type = d.pop("newType")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/set_time_index_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/set_time_index_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,26 @@
 from ..models.set_time_index_step_step_type import SetTimeIndexStepStepType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="SetTimeIndexStep")
 
 @attr.s(auto_attribs=True)
 class SetTimeIndexStep:
-    """
-    Attributes:
-        column (str):
-        step_type (SetTimeIndexStepStepType):
-        series_columns (Union[Unset, List[str]]):
-    """
-
+    """  """
     column: str
     step_type: SetTimeIndexStepStepType
     series_columns: Union[Unset, List[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column = self.column
+        column =  self.column
         step_type = self.step_type.value
 
-        series_columns: Union[Unset, List[str]] = UNSET
+        series_columns: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.series_columns, Unset):
             series_columns = self.series_columns
 
 
 
 
 
@@ -41,16 +35,14 @@
             "stepType": step_type,
         })
         if series_columns is not UNSET:
             field_dict["seriesColumns"] = series_columns
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         column = d.pop("column")
 
         step_type = SetTimeIndexStepStepType(d.pop("stepType"))
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simple_forecast.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simple_forecast.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,52 +7,41 @@
 from ..models.simple_forecast_cadence import SimpleForecastCadence
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="SimpleForecast")
 
 @attr.s(auto_attribs=True)
 class SimpleForecast:
-    """
-    Attributes:
-        horizon (Union[Unset, int]):
-        cadence (Union[Unset, SimpleForecastCadence]):
-        index (Union[Unset, datetime.datetime]):
-        predicted_value (Union[Unset, float]):
-        lower_bound (Union[Unset, float]):
-        upper_bound (Union[Unset, float]):
-        historic_rmse_score (Union[Unset, float]):
-        historic_r2_score (Union[Unset, float]):
-    """
-
+    """  """
     horizon: Union[Unset, int] = UNSET
     cadence: Union[Unset, SimpleForecastCadence] = UNSET
     index: Union[Unset, datetime.datetime] = UNSET
     predicted_value: Union[Unset, float] = UNSET
     lower_bound: Union[Unset, float] = UNSET
     upper_bound: Union[Unset, float] = UNSET
     historic_rmse_score: Union[Unset, float] = UNSET
     historic_r2_score: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        horizon = self.horizon
-        cadence: Union[Unset, str] = UNSET
+        horizon =  self.horizon
+        cadence: Union[Unset, SimpleForecastCadence] = UNSET
         if not isinstance(self.cadence, Unset):
-            cadence = self.cadence.value
+            cadence = self.cadence
 
         index: Union[Unset, str] = UNSET
         if not isinstance(self.index, Unset):
             index = self.index.isoformat()
 
-        predicted_value = self.predicted_value
-        lower_bound = self.lower_bound
-        upper_bound = self.upper_bound
-        historic_rmse_score = self.historic_rmse_score
-        historic_r2_score = self.historic_r2_score
+        predicted_value =  self.predicted_value
+        lower_bound =  self.lower_bound
+        upper_bound =  self.upper_bound
+        historic_rmse_score =  self.historic_rmse_score
+        historic_r2_score =  self.historic_r2_score
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
         })
         if horizon is not UNSET:
             field_dict["horizon"] = horizon
@@ -69,36 +58,30 @@
         if historic_rmse_score is not UNSET:
             field_dict["historicRmseScore"] = historic_rmse_score
         if historic_r2_score is not UNSET:
             field_dict["historicR2Score"] = historic_r2_score
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         horizon = d.pop("horizon", UNSET)
 
+        cadence: Union[Unset, SimpleForecastCadence] = UNSET
         _cadence = d.pop("cadence", UNSET)
-        cadence: Union[Unset, SimpleForecastCadence]
-        if isinstance(_cadence,  Unset):
-            cadence = UNSET
-        else:
+        if not isinstance(_cadence,  Unset):
             cadence = SimpleForecastCadence(_cadence)
 
 
 
 
+        index: Union[Unset, datetime.datetime] = UNSET
         _index = d.pop("index", UNSET)
-        index: Union[Unset, datetime.datetime]
-        if isinstance(_index,  Unset):
-            index = UNSET
-        else:
+        if not isinstance(_index,  Unset):
             index = isoparse(_index)
 
 
 
 
         predicted_value = d.pop("predictedValue", UNSET)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simplify_categories_definition.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simplify_categories_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,22 @@
 
 from ..models.simplify_categories_rule import SimplifyCategoriesRule
 
 T = TypeVar("T", bound="SimplifyCategoriesDefinition")
 
 @attr.s(auto_attribs=True)
 class SimplifyCategoriesDefinition:
-    """
-    Attributes:
-        value (str):
-        rules (List[SimplifyCategoriesRule]):
-    """
-
+    """  """
     value: str
     rules: List[SimplifyCategoriesRule]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        value = self.value
+        value =  self.value
         rules = []
         for rules_item_data in self.rules:
             rules_item = rules_item_data.to_dict()
 
             rules.append(rules_item)
 
 
@@ -36,16 +31,14 @@
         field_dict.update({
             "value": value,
             "rules": rules,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         value = d.pop("value")
 
         rules = []
         _rules = d.pop("rules")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simplify_categories_rule.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simplify_categories_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,36 @@
 
 import attr
 
 T = TypeVar("T", bound="SimplifyCategoriesRule")
 
 @attr.s(auto_attribs=True)
 class SimplifyCategoriesRule:
-    """
-    Attributes:
-        matcher (str):
-        enable_regex (bool):
-        enable_case_sensitive (bool):  Default: True.
-    """
-
+    """  """
     matcher: str
     enable_regex: bool = False
     enable_case_sensitive: bool = True
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        matcher = self.matcher
-        enable_regex = self.enable_regex
-        enable_case_sensitive = self.enable_case_sensitive
+        matcher =  self.matcher
+        enable_regex =  self.enable_regex
+        enable_case_sensitive =  self.enable_case_sensitive
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "matcher": matcher,
             "enableRegex": enable_regex,
             "enableCaseSensitive": enable_case_sensitive,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         matcher = d.pop("matcher")
 
         enable_regex = d.pop("enableRegex")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/simplify_categories_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/simplify_categories_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,25 @@
 from ..models.simplify_categories_definition import SimplifyCategoriesDefinition
 from ..models.simplify_categories_step_step_type import SimplifyCategoriesStepStepType
 
 T = TypeVar("T", bound="SimplifyCategoriesStep")
 
 @attr.s(auto_attribs=True)
 class SimplifyCategoriesStep:
-    """
-    Attributes:
-        column (str):
-        new_column_name (str):
-        category_definitions (List[SimplifyCategoriesDefinition]):
-        step_type (SimplifyCategoriesStepStepType):
-    """
-
+    """  """
     column: str
     new_column_name: str
     category_definitions: List[SimplifyCategoriesDefinition]
     step_type: SimplifyCategoriesStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column = self.column
-        new_column_name = self.new_column_name
+        column =  self.column
+        new_column_name =  self.new_column_name
         category_definitions = []
         for category_definitions_item_data in self.category_definitions:
             category_definitions_item = category_definitions_item_data.to_dict()
 
             category_definitions.append(category_definitions_item)
 
 
@@ -46,16 +39,14 @@
             "newColumnName": new_column_name,
             "categoryDefinitions": category_definitions,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         column = d.pop("column")
 
         new_column_name = d.pop("newColumnName")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/split_column_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/split_column_step.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,45 +4,37 @@
 
 from ..models.split_column_step_step_type import SplitColumnStepStepType
 
 T = TypeVar("T", bound="SplitColumnStep")
 
 @attr.s(auto_attribs=True)
 class SplitColumnStep:
-    """
-    Attributes:
-        column (str):
-        split_character (str):
-        step_type (SplitColumnStepStepType):
-    """
-
+    """  """
     column: str
     split_character: str
     step_type: SplitColumnStepStepType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column = self.column
-        split_character = self.split_character
+        column =  self.column
+        split_character =  self.split_character
         step_type = self.step_type.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "column": column,
             "splitCharacter": split_character,
             "stepType": step_type,
         })
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         column = d.pop("column")
 
         split_character = d.pop("splitCharacter")
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/test_list_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/test_list_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 from ..models.test_response import TestResponse
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="TestListResponse")
 
 @attr.s(auto_attribs=True)
 class TestListResponse:
-    """
-    Attributes:
-        tests (Union[Unset, List[TestResponse]]):
-    """
-
+    """  """
     tests: Union[Unset, List[TestResponse]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        tests: Union[Unset, List[Dict[str, Any]]] = UNSET
+        tests: Union[Unset, List[Any]] = UNSET
         if not isinstance(self.tests, Unset):
             tests = []
             for tests_item_data in self.tests:
                 tests_item = tests_item_data.to_dict()
 
                 tests.append(tests_item)
 
@@ -36,16 +32,14 @@
         field_dict.update({
         })
         if tests is not UNSET:
             field_dict["tests"] = tests
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         tests = []
         _tests = d.pop("tests", UNSET)
         for tests_item_data in (_tests or []):
             tests_item = TestResponse.from_dict(tests_item_data)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/transform_text_step.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/transform_text_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,50 +9,39 @@
 from ..models.transform_text_step_step_type import TransformTextStepStepType
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="TransformTextStep")
 
 @attr.s(auto_attribs=True)
 class TransformTextStep:
-    """
-    Attributes:
-        column (str):
-        input_regex (str):
-        if_no_match (TransformTextStepIfNoMatch):
-        step_type (TransformTextStepStepType):
-        ignore_case (Union[Unset, bool]):
-        output_regex (Union[Unset, str]):
-        new_column_name (Union[Unset, str]):
-        replace_existing_column (Union[Unset, TransformTextStepReplaceExistingColumn]):
-    """
-
+    """  """
     column: str
     input_regex: str
     if_no_match: TransformTextStepIfNoMatch
     step_type: TransformTextStepStepType
     ignore_case: Union[Unset, bool] = UNSET
     output_regex: Union[Unset, str] = UNSET
     new_column_name: Union[Unset, str] = UNSET
     replace_existing_column: Union[Unset, TransformTextStepReplaceExistingColumn] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        column = self.column
-        input_regex = self.input_regex
+        column =  self.column
+        input_regex =  self.input_regex
         if_no_match = self.if_no_match.value
 
         step_type = self.step_type.value
 
-        ignore_case = self.ignore_case
-        output_regex = self.output_regex
-        new_column_name = self.new_column_name
-        replace_existing_column: Union[Unset, str] = UNSET
+        ignore_case =  self.ignore_case
+        output_regex =  self.output_regex
+        new_column_name =  self.new_column_name
+        replace_existing_column: Union[Unset, TransformTextStepReplaceExistingColumn] = UNSET
         if not isinstance(self.replace_existing_column, Unset):
-            replace_existing_column = self.replace_existing_column.value
+            replace_existing_column = self.replace_existing_column
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "column": column,
             "inputRegex": input_regex,
@@ -66,16 +55,14 @@
         if new_column_name is not UNSET:
             field_dict["newColumnName"] = new_column_name
         if replace_existing_column is not UNSET:
             field_dict["replaceExistingColumn"] = replace_existing_column
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         column = d.pop("column")
 
         input_regex = d.pop("inputRegex")
 
@@ -91,19 +78,17 @@
 
         ignore_case = d.pop("ignoreCase", UNSET)
 
         output_regex = d.pop("outputRegex", UNSET)
 
         new_column_name = d.pop("newColumnName", UNSET)
 
+        replace_existing_column: Union[Unset, TransformTextStepReplaceExistingColumn] = UNSET
         _replace_existing_column = d.pop("replaceExistingColumn", UNSET)
-        replace_existing_column: Union[Unset, TransformTextStepReplaceExistingColumn]
-        if isinstance(_replace_existing_column,  Unset):
-            replace_existing_column = UNSET
-        else:
+        if not isinstance(_replace_existing_column,  Unset):
             replace_existing_column = TransformTextStepReplaceExistingColumn(_replace_existing_column)
 
 
 
 
         transform_text_step = cls(
             column=column,
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/models/update_deployed_pipeline_api_request.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/models/update_deployed_pipeline_api_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,37 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="UpdateDeployedPipelineApiRequest")
 
 @attr.s(auto_attribs=True)
 class UpdateDeployedPipelineApiRequest:
-    """
-    Attributes:
-        new_pipeline_id (int):
-        notes (Union[Unset, None, str]):
-    """
-
+    """  """
     new_pipeline_id: int
-    notes: Union[Unset, None, str] = UNSET
+    notes: Union[Unset, Optional[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        new_pipeline_id = self.new_pipeline_id
-        notes = self.notes
+        new_pipeline_id =  self.new_pipeline_id
+        notes =  self.notes
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "newPipelineId": new_pipeline_id,
         })
         if notes is not UNSET:
             field_dict["notes"] = notes
 
         return field_dict
 
-
-
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         new_pipeline_id = d.pop("newPipelineId")
 
         notes = d.pop("notes", UNSET)
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/swagger/types.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/swagger/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """ Contains some shared types for properties """
-from typing import BinaryIO, Generic, MutableMapping, Optional, Tuple, TypeVar
+from typing import (
+    BinaryIO,
+    Generic,
+    MutableMapping,
+    Optional,
+    TextIO,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import attr
 
 
 class Unset:
     def __bool__(self) -> bool:
         return False
 
 
 UNSET: Unset = Unset()
 
-FileJsonType = Tuple[Optional[str], BinaryIO, Optional[str]]
-
 
 @attr.s(auto_attribs=True)
 class File:
     """ Contains information for file uploads """
 
-    payload: BinaryIO
+    payload: Union[BinaryIO, TextIO]
     file_name: Optional[str] = None
     mime_type: Optional[str] = None
 
-    def to_tuple(self) -> FileJsonType:
+    def to_tuple(self) -> Tuple[Optional[str], Union[BinaryIO, TextIO], Optional[str]]:
         """ Return a tuple representation that httpx will accept for multipart/form-data """
         return self.file_name, self.payload, self.mime_type
 
 
 T = TypeVar("T")
 
 
@@ -36,8 +43,8 @@
 
     status_code: int
     content: bytes
     headers: MutableMapping[str, str]
     parsed: Optional[T]
 
 
-__all__ = ["File", "Response", "FileJsonType"]
+__all__ = ["File", "Response"]
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/__init__.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_cached_response.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_cached_response.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_polling.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_polling.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     check_not_unset,
     check_response,
 )
 
 
 def wait_for_future_to_succeed(
     client: Client, response: Response[Optional[dto.Future]]
-) -> dto.FutureOutputOfYourRequest:
+) -> dto.FutureOutputofyourrequest:
     status = check_response(response).status
     future_id = check_not_unset(check_response(response).future_id)
 
     while status == dto.Status.IN_PROGRESS:
         sleep(5)
         response = get_future.sync_detailed(client=client, future_id=future_id)
         status = check_response(response).status
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_refreshable_access_token.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_refreshable_access_token.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_swagger_response_utils.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_swagger_response_utils.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry/client/analyze/utils/_token_authenticated_client.py` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry/client/analyze/utils/_token_authenticated_client.py`

 * *Files identical despite different names*

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/PKG-INFO` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindfoundry.client.analyze
-Version: 1.20.4
+Version: 1.9.2
 Summary: Mind Foundry Analyze Python Client
 Home-page: https://www.mindfoundry.ai/platform
 Author: Mind Foundry Ltd
 Author-email: support@mindfoundry.ai
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mindfoundry.client.analyze-1.20.4/src/mindfoundry.client.analyze.egg-info/SOURCES.txt` & `mindfoundry.client.analyze-1.9.2/src/mindfoundry.client.analyze.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,14 @@
 src/mindfoundry/client/analyze/swagger/api/tests/edit_test.py
 src/mindfoundry/client/analyze/swagger/api/tests/get_test.py
 src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_csv_data.py
 src/mindfoundry/client/analyze/swagger/api/tests/get_test_result_parquet_data.py
 src/mindfoundry/client/analyze/swagger/api/tests/get_tests.py
 src/mindfoundry/client/analyze/swagger/api/tests/save_test.py
 src/mindfoundry/client/analyze/swagger/models/__init__.py
-src/mindfoundry/client/analyze/swagger/models/api_column_level.py
-src/mindfoundry/client/analyze/swagger/models/api_column_type.py
 src/mindfoundry/client/analyze/swagger/models/api_history_response.py
 src/mindfoundry/client/analyze/swagger/models/apply_data_prep_steps_request.py
 src/mindfoundry/client/analyze/swagger/models/apply_formula_step.py
 src/mindfoundry/client/analyze/swagger/models/apply_formula_step_step_type.py
 src/mindfoundry/client/analyze/swagger/models/cadence.py
 src/mindfoundry/client/analyze/swagger/models/classification_model_type.py
 src/mindfoundry/client/analyze/swagger/models/classification_scorers.py
@@ -158,18 +156,19 @@
 src/mindfoundry/client/analyze/swagger/models/create_test_request.py
 src/mindfoundry/client/analyze/swagger/models/csv_parse_options.py
 src/mindfoundry/client/analyze/swagger/models/csv_parse_options_file_type.py
 src/mindfoundry/client/analyze/swagger/models/data_partition_method.py
 src/mindfoundry/client/analyze/swagger/models/data_pipeline_create_request.py
 src/mindfoundry/client/analyze/swagger/models/data_pipeline_response.py
 src/mindfoundry/client/analyze/swagger/models/data_pipelines_response.py
+src/mindfoundry/client/analyze/swagger/models/data_prep_step.py
 src/mindfoundry/client/analyze/swagger/models/data_prep_step_response.py
-src/mindfoundry/client/analyze/swagger/models/data_set_column_metadata_response.py
 src/mindfoundry/client/analyze/swagger/models/data_set_response.py
 src/mindfoundry/client/analyze/swagger/models/data_sets_response.py
+src/mindfoundry/client/analyze/swagger/models/data_value.py
 src/mindfoundry/client/analyze/swagger/models/decisioning_decision.py
 src/mindfoundry/client/analyze/swagger/models/decisioning_reward.py
 src/mindfoundry/client/analyze/swagger/models/decisioning_threshold.py
 src/mindfoundry/client/analyze/swagger/models/delete_data_prep_steps_request.py
 src/mindfoundry/client/analyze/swagger/models/deployed_api_client_create_response.py
 src/mindfoundry/client/analyze/swagger/models/deployed_api_client_list_response.py
 src/mindfoundry/client/analyze/swagger/models/deployed_api_client_response.py
@@ -193,15 +192,15 @@
 src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step.py
 src/mindfoundry/client/analyze/swagger/models/fill_missing_value_step_step_type.py
 src/mindfoundry/client/analyze/swagger/models/filter_rows_rule.py
 src/mindfoundry/client/analyze/swagger/models/filter_rows_rule_rule.py
 src/mindfoundry/client/analyze/swagger/models/filter_rows_step.py
 src/mindfoundry/client/analyze/swagger/models/filter_rows_step_step_type.py
 src/mindfoundry/client/analyze/swagger/models/future.py
-src/mindfoundry/client/analyze/swagger/models/future_output_of_your_request.py
+src/mindfoundry/client/analyze/swagger/models/future_outputofyourrequest.py
 src/mindfoundry/client/analyze/swagger/models/group_by_aggregation.py
 src/mindfoundry/client/analyze/swagger/models/group_by_aggregation_rule.py
 src/mindfoundry/client/analyze/swagger/models/group_by_step.py
 src/mindfoundry/client/analyze/swagger/models/group_by_step_step_type.py
 src/mindfoundry/client/analyze/swagger/models/id_response.py
 src/mindfoundry/client/analyze/swagger/models/json_parse_options.py
 src/mindfoundry/client/analyze/swagger/models/json_parse_options_file_type.py
@@ -215,14 +214,15 @@
 src/mindfoundry/client/analyze/swagger/models/model_status.py
 src/mindfoundry/client/analyze/swagger/models/model_validation_method.py
 src/mindfoundry/client/analyze/swagger/models/nlp_language.py
 src/mindfoundry/client/analyze/swagger/models/normalize_text_step.py
 src/mindfoundry/client/analyze/swagger/models/normalize_text_step_rule.py
 src/mindfoundry/client/analyze/swagger/models/normalize_text_step_step_type.py
 src/mindfoundry/client/analyze/swagger/models/null_request.py
+src/mindfoundry/client/analyze/swagger/models/parse_options.py
 src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response.py
 src/mindfoundry/client/analyze/swagger/models/prediction_forecast_response_model_forecasts_item.py
 src/mindfoundry/client/analyze/swagger/models/prediction_list_response.py
 src/mindfoundry/client/analyze/swagger/models/prediction_response.py
 src/mindfoundry/client/analyze/swagger/models/prediction_response_problem_type.py
 src/mindfoundry/client/analyze/swagger/models/prediction_response_task_status.py
 src/mindfoundry/client/analyze/swagger/models/problem_type.py
@@ -249,15 +249,14 @@
 src/mindfoundry/client/analyze/swagger/models/simplify_categories_definition.py
 src/mindfoundry/client/analyze/swagger/models/simplify_categories_rule.py
 src/mindfoundry/client/analyze/swagger/models/simplify_categories_step.py
 src/mindfoundry/client/analyze/swagger/models/simplify_categories_step_step_type.py
 src/mindfoundry/client/analyze/swagger/models/split_column_step.py
 src/mindfoundry/client/analyze/swagger/models/split_column_step_step_type.py
 src/mindfoundry/client/analyze/swagger/models/status.py
-src/mindfoundry/client/analyze/swagger/models/target_distributions.py
 src/mindfoundry/client/analyze/swagger/models/test_list_response.py
 src/mindfoundry/client/analyze/swagger/models/test_response.py
 src/mindfoundry/client/analyze/swagger/models/test_response_problem_type.py
 src/mindfoundry/client/analyze/swagger/models/test_response_task_status.py
 src/mindfoundry/client/analyze/swagger/models/transform_text_step.py
 src/mindfoundry/client/analyze/swagger/models/transform_text_step_if_no_match.py
 src/mindfoundry/client/analyze/swagger/models/transform_text_step_replace_existing_column.py
```

### Comparing `mindfoundry.client.analyze-1.20.4/versioneer.py` & `mindfoundry.client.analyze-1.9.2/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,14 +378,15 @@
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
+            # remember shell=False, so use git.cmd on windows, not just git
             p = subprocess.Popen([c] + args, cwd=cwd, env=env,
                                  stdout=subprocess.PIPE,
                                  stderr=(subprocess.PIPE if hide_stderr
                                          else None))
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
@@ -481,14 +482,15 @@
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
+            # remember shell=False, so use git.cmd on windows, not just git
             p = subprocess.Popen([c] + args, cwd=cwd, env=env,
                                  stdout=subprocess.PIPE,
                                  stderr=(subprocess.PIPE if hide_stderr
                                          else None))
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
```

