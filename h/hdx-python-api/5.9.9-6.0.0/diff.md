# Comparing `tmp/hdx-python-api-5.9.9.tar.gz` & `tmp/hdx-python-api-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-api-5.9.9.tar", last modified: Tue Feb 28 22:08:19 2023, max compression
+gzip compressed data, was "hdx-python-api-6.0.0.tar", last modified: Thu Apr 13 04:41:06 2023, max compression
```

## Comparing `hdx-python-api-5.9.9.tar` & `hdx-python-api-6.0.0.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.110419 hdx-python-api-5.9.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.094419 hdx-python-api-5.9.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.094419 hdx-python-api-5.9.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-02-28 22:08:19.110419 hdx-python-api-5.9.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.094419 hdx-python-api-5.9.9/doc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35530 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-02-28 22:08:19.110419 hdx-python-api-5.9.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.094419 hdx-python-api-5.9.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.094419 hdx-python-api-5.9.9/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.094419 hdx-python-api-5.9.9/src/hdx/api/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-28 22:08:19.000000 hdx-python-api-5.9.9/src/hdx/api/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24827 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/api/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/api/hdx_base_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4541 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/api/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.098419 hdx-python-api-5.9.9/src/hdx/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   110270 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9457 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/date_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/hdx_datasource_topline.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    28494 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/hdxobject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2828 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/indicator_resource_view_template.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    11097 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/organization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24274 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/resource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4532 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7678 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/resource_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15004 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/showcase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9685 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21984 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/data/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.098419 hdx-python-api-5.9.9/src/hdx/facades/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/facades/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3863 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/src/hdx/facades/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.098419 hdx-python-api-5.9.9/src/hdx_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-02-28 22:08:19.000000 hdx-python-api-5.9.9/src/hdx_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-02-28 22:08:19.000000 hdx-python-api-5.9.9/src/hdx_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 22:08:19.000000 hdx-python-api-5.9.9/src/hdx_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-28 22:08:19.000000 hdx-python-api-5.9.9/src/hdx_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-28 22:08:19.000000 hdx-python-api-5.9.9/src/hdx_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 22:08:17.000000 hdx-python-api-5.9.9/src/hdx_python_api.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.094419 hdx-python-api-5.9.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.098419 hdx-python-api-5.9.9/tests/fixtures/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)   169312 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/Tag_Mapping_ChainRuleError.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.102419 hdx-python-api-5.9.9/tests/fixtures/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/empty.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      449 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_base_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_dataset_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_datasource_topline.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_email_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_organization_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      147 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_resource_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_resource_view_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_showcase_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_user_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/hdx_vocabulary_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/project_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/user_agent_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/user_agent_config2.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/user_agent_config3.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/config/user_agent_config_wrong.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    25870 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/dataset_search_results.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.102419 hdx-python-api-5.9.9/tests/fixtures/datastore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23724 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/empty.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.102419 hdx-python-api-5.9.9/tests/fixtures/gen_resource/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      920 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/gen_resource/test_data_no_years.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    13842 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/organization_show_results.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.102419 hdx-python-api-5.9.9/tests/fixtures/qc_from_rows/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/resource_formats.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    14465 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/showcase_all_search_results.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/test_data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/test_data.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.106419 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/
--rw-r--r--   0 runner    (1001) docker     (123)    50900 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   319924 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    92805 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   290790 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   230593 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   216041 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   842238 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    48523 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.106419 hdx-python-api-5.9.9/tests/fixtures/update_logic/
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_logic/update_logic_resources.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/fixtures/update_logic/update_logic_resources_new.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.106419 hdx-python-api-5.9.9/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.106419 hdx-python-api-5.9.9/tests/hdx/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)    34779 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3009 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/api/test_locations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44943 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.110419 hdx-python-api-5.9.9/tests/hdx/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9940 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49148 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    74888 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19570 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_organization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45966 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_resource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19114 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23053 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    63707 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21174 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   116056 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/data/test_vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.110419 hdx-python-api-5.9.9/tests/hdx/facades/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/facades/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3184 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5957 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5651 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/tests/hdx/facades/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:08:19.110419 hdx-python-api-5.9.9/workingexample/
--rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/workingexample/my_code.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/workingexample/my_resource.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/workingexample/my_resource.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-02-28 22:08:02.000000 hdx-python-api-5.9.9/workingexample/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.916793 hdx-python-api-6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.github/workflows/run-python-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.readthedocs.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/doc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42394 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/doc/main.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.916793 hdx-python-api-6.0.0/src/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.924793 hdx-python-api-6.0.0/src/hdx/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx/api/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24827 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/hdx_base_configuration.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4541 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/locations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.924793 hdx-python-api-6.0.0/src/hdx/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   111856 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9457 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/date_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/hdx_datasource_topline.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28494 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/indicator_resource_view_template.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11097 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/organization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24274 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4532 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7678 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/resource_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15004 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/showcase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9685 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21984 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.928794 hdx-python-api-6.0.0/src/hdx/facades/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3863 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.928794 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:41:05.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.928794 hdx-python-api-6.0.0/tests/fixtures/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)   169312 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/empty.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      449 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_base_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_datasource_topline.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_email_configuration.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_organization_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      147 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_view_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_showcase_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_user_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_vocabulary_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/project_configuration.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config2.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config3.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config_wrong.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25870 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/dataset_search_results.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/datastore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23724 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/empty.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/gen_resource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      920 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/test_data_no_years.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13842 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/organization_show_results.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14465 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/showcase_all_search_results.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/test_data.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/test_data.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.940794 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    50900 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   319924 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    92805 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   290790 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   230593 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   216041 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   842238 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48523 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.940794 hdx-python-api-6.0.0/tests/fixtures/update_logic/
+-rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources_new.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.944794 hdx-python-api-6.0.0/tests/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.944794 hdx-python-api-6.0.0/tests/hdx/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34779 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3009 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44943 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/tests/hdx/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9940 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49148 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    75019 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19570 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45966 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19114 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23053 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63707 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21174 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   116056 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/tests/hdx/facades/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3184 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5957 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5651 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/workingexample/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/my_code.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/my_resource.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/my_resource.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/run.py
```

### Comparing `hdx-python-api-5.9.9/.github/workflows/publish.yml` & `hdx-python-api-6.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/.github/workflows/run-python-tests.yml` & `hdx-python-api-6.0.0/.github/workflows/run-python-tests.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/.gitignore` & `hdx-python-api-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/LICENSE` & `hdx-python-api-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/PKG-INFO` & `hdx-python-api-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 5.9.9
+Version: 6.0.0
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Home-page: https://github.com/OCHA-DAP/hdx-python-api
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,API,library,CKAN
 Platform: any
```

### Comparing `hdx-python-api-5.9.9/README.md` & `hdx-python-api-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/doc/main.md` & `hdx-python-api-6.0.0/doc/main.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,18 @@
     -   [Dataset Specific Operations](#dataset-specific-operations)
         -   [Reference Period](#reference-period)
         -   [Expected Update Frequency](#expected-update-frequency)
         -   [Location](#location)
         -   [Tags](#tags)
         -   [Maintainer](#maintainer)
         -   [Organization](#organization)
+        -   [Resource Generation](#resource-generation)
+        -   [QuickCharts Generation](#quickcharts-generation)
     -   [Resource Specific Operations](#resource-specific-operations)
+    -   [Showcase Management](#showcase-management)
     -   [User Management](#user-management)
     -   [Organization Management](#organization-management)
     -   [Vocabulary Management](#vocabulary-management)
 -   [Working Example](#working-example)
 -   [IDMC Example](#idmc-example)
 
 # Information
@@ -44,14 +47,16 @@
 HDX.
 
 The code for the library is [here](https://github.com/OCHA-DAP/hdx-python-api).
 The library has detailed API documentation which can be found in the menu at the top. 
 
 
 ## Breaking Changes
+From 6.0.0, generate_resource_view is renamed to generate_quickcharts
+
 From 5.9.9, get_location_iso3s returns uppercase codes instead of lowercase
 
 From 5.9.8, get_date_of_dataset has become get_reference_period, 
 set_date_of_dataset has become set_reference_period and set_dataset_year_range 
 has become set_reference_period_year_range
 
 From 5.9.7, Python 3.7 no longer supported
@@ -734,14 +739,140 @@
 If you want to set the organization, you do it like this:
 
     dataset.set_organization(ORGANIZATION)
 
 ORGANIZATION is either a string id, dictionary or an Organization
 object.
 
+### Resource generation
+
+There are a range of helpful functions to generate resources. In the following
+examples, RESOURCE DATA takes the form {"name": NAME, "description": 
+DESCRIPTION} and ENCODING is a file encoding like "utf-8".  
+
+A resource can be generated from ROWS which is a list of list, tuple or 
+dictionary. HEADERS is either a row number (rows start counting at 1), or the 
+actual headers defined as a list of strings. If not set, all rows will be 
+treated as containing values:
+
+    dataset.generate_resource_from_rows("FOLDER", "FILENAME", ROWS, 
+                                        RESOURCE DATA, HEADERS, "ENCODING")
+
+A resource for the purpose of driving QuickCharts can be generated by taking 
+ROWS, a list of dictionaries, and producing a cut down subset from it. HXLTAGS 
+are added as the second row after the header. The reduction in rows is 
+performed by only outputting the rows where COLUMN_NAME has a value in 
+QC_IDENTIFIERS. Optionally the columns that are output can be limited by 
+specifying them in HEADERS. 
+
+    dataset.generate_qc_resource_from_rows("FOLDER", "FILENAME", ROWS,
+    RESOURCE DATA, HXLTAGS, "COLUMN_NAME", QC_IDENTIFIERS, HEADERS, "ENCODING")
+
+Building on these basic resource generation methods, there are more powerful 
+ones `generate_resource_from_iterator` and `download_and_generate_resource`. 
+
+A resource can be generated from a given list or tuple: HEADERS and an ITERATOR 
+which can return rows in list, tuple or dictionary form. A mapping from headers 
+to HXL hashtags, HXLTAGS, must be provided along with the FOLDER and FILENAME 
+where the file will be generated for upload to the filestore. The dataset 
+reference period can optionally be set by supplying DATECOL for looking up 
+dates or YEARCOL for looking up years. DATECOl and YEARCOL can be a column name
+or the index of a column. Note that any timezone information is ignored and UTC 
+is assumed. 
+
+Alternatively, DATE_FUNCTION can be supplied to handle any dates
+in a row. It should accept a row and should return None to ignore the row or a
+dictionary which can either be empty if there are no dates in the row or can be
+populated with keys startdate and/or enddate which are of type timezone-aware
+datetime. The lowest start date and highest end date are used to set the 
+reference period and are returned in the results dictionary in keys startdate 
+and enddate.
+
+    dataset.generate_resource_from_iterator(HEADERS, ITERATOR, HXLTAGS, 
+    "FOLDER", "FILENAME", RESOURCE_DATA, DATECOL or YEARCOL or DATE_FUNCTION,
+    QUICKCHARTS, "ENCODING")
+
+If desired, `generate_resource_from_iterator` can generate a separate 
+QuickCharts resource designed to be used in a time series QuickCharts bite 
+provided that the input has #indicator+code, #date and #indicator+value+num. 
+This is achieved by supplying the parameter QUICKCHARTS which activates various 
+QuickCharts related actions depending upon the keys given in the dictionary. 
+The returned dictionary will contain the QuickCharts resource in the key 
+qc_resource. If the keys: hashtag - the HXL hashtag to examine - and values -
+the 3 values to look for in that column - are supplied, then a list of booleans
+indicating which QuickCharts bites should be enabled will be returned in the 
+key bites_disabled in the returned dictionary. For the 3 values, if the key:
+numeric_hashtag is supplied then if that column for a given value contains no
+numbers, then the corresponding bite will be disabled. If the key: cutdown is
+given, if it is 1, then a separate cut down list is created containing only
+columns with HXL hashtags and rows with desired values (if hashtag and values
+are supplied) for the purpose of driving QuickCharts. It is returned in the key
+qcrows in the returned dictionary with the matching headers in qcheaders. If
+cutdown is 2, then a resource is created using the cut down list. If the key
+cutdownhashtags is supplied, then only the provided hashtags are used for
+cutting down otherwise the full list of HXL tags is used.
+
+The QuickCharts resource will be of form similar to below:
+
+    GHO (CODE),ENDYEAR,Numeric
+    #indicator+code,#date+year+end,#indicator+value+num
+    VIOLENCE_HOMICIDERATE,1994,123.4
+    MDG_0000000001,2015,123.4
+
+`download_and_generate_resource` builds on `generate_resource_from_iterator`.
+It uses an DOWNLOADER, an object of class `Download`, `Retrieve` or other class 
+that implements `BaseDownload` to download from URL. Additional arguments in 
+**KWARGS are passed to the `get_tabular_rows` method of the DOWNLOADER.
+
+Optionally, headers can be inserted at specific positions. This is achieved 
+using HEADER_INSERTIONS. If supplied, it is a list of tuples of the form 
+(position, header) to be inserted. A function, ROW_FUNCTION, is called for each 
+row. If supplied, it takes as arguments: headers (prior to any insertions) and 
+row (which will be in dict or list form depending upon the dict_rows argument) 
+and outputs a modified row. 
+
+The rest of the arguments are the same as for 
+`generate_resource_from_iterator`.
+
+    dataset.download_and_generate_resource(DOWNLOADER, "URL", HXLTAGS, 
+    "FOLDER", "FILENAME", RESOURCE_DATA, HEADER_INSERTIONS, ROW_FUNCTION,
+    DATECOL or YEARCOL or DATE_FUNCTION, QUICKCHARTS, **KWARGS)
+
+### QuickCharts Generation
+
+QuickCharts can be generated for datasets using the call below. RESOURCE is a
+a resource id or name, or resource metadata from a Resource object or a 
+dictionary, or the position of the resource in the dataset. It defaults to the
+position 0. PATH points to configuration which if not supplied, defaults to the 
+internal indicators resource view template. You can disable specific bites by 
+providing BITES_DISABLED, a list of 3 bools where True indicates a specific bite 
+is disabled and False indicates leave enabled. 
+
+    datasets.generate_quickcharts(RESOURCE, "PATH", BITES_DISABLED, INDICATORS,
+                                  FIND_REPLACE)
+
+The parameter INDICATORS is only for use with the built-in configuration and is
+a list with 3 dictionaries of form:
+
+        {"code": "MY_INDICATOR_CODE", "title": "MY_INDICATOR_TITLE",
+        "unit": "MY_INDICATOR_UNIT"}. 
+
+Optionally, the following defaults can be overridden in INDICATORS: 
+    
+    {"code_col": "#indicator+code", "value_col": "#indicator+value+num", 
+     "date_col": "#date+year", "date_format": "%Y", "aggregate_col": "null"}.
+
+The built-in configuration assumes data will be of form similar to below:
+
+    GHO (CODE),ENDYEAR,Numeric
+    #indicator+code,#date+year+end,#indicator+value+num
+    VIOLENCE_HOMICIDERATE,1994,123.4
+    MDG_0000000001,2015,123.4
+
+
 ## Resource Specific Operations
 
 You can download a resource using the **download** function eg.
 
     url, path = resource.download("FOLDER_TO_DOWNLOAD_TO")
 
 If you do not supply **FOLDER\_TO\_DOWNLOAD\_TO**, then a temporary folder is used.
@@ -755,16 +886,17 @@
     resource.set_file_to_upload(file_to_upload="PATH_TO_FILE")
 
 There is a getter to read the value back:
 
     file_to_upload = resource.get_file_to_upload()
 
 ## Showcase Management
+
 The **Showcase** class enables you to manage showcases, creating, deleting and updating 
-(as for other HDX objects) according to  your permissions.
+(as for other HDX objects) according to your permissions.
 
 To see the list of datasets a showcase is in, you use the **get\_datasets** function eg.
 
     datasets = showcase.get_datasets()
 
 If you wish to add a dataset to a showcase, you call the **add\_dataset** function, for 
 example:
```

### Comparing `hdx-python-api-5.9.9/pyproject.toml` & `hdx-python-api-6.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/setup.cfg` & `hdx-python-api-6.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -37,24 +37,21 @@
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
 	ckanapi >= 4.7
 	defopt >= 6.4.0
 	email_validator
-	hdx-python-country>=3.4.6
+	hdx-python-country>=3.4.8
 	makefun
 	ndg-httpsclient
 	pyasn1
 	pyOpenSSL
 	quantulum3
 
 [options.packages.find]
 where = src
 
-[bdist_wheel]
-universal = 1
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hdx-python-api-5.9.9/src/hdx/api/configuration.py` & `hdx-python-api-6.0.0/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/api/hdx_base_configuration.yml` & `hdx-python-api-6.0.0/src/hdx/api/hdx_base_configuration.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/api/locations.py` & `hdx-python-api-6.0.0/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/dataset.py` & `hdx-python-api-6.0.0/src/hdx/data/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     List,
     Optional,
     Tuple,
     Union,
 )
 
 from hdx.location.country import Country
+from hdx.utilities.base_downloader import BaseDownload
 from hdx.utilities.dateparse import (
     default_date,
     default_enddate,
     now_utc,
     parse_date,
     parse_date_range,
 )
@@ -2067,21 +2068,28 @@
         self,
         resource: Union["Resource", Dict, str, int] = 0,
         path: Optional[str] = None,
         bites_disabled: Optional[ListTuple[bool]] = None,
         indicators: Optional[ListTuple[Dict]] = None,
         findreplace: Optional[Dict] = None,
     ) -> resource_view.ResourceView:
-        """Create QuickCharts for dataset from configuration saved in resource view. You can disable specific bites
-        by providing bites_disabled, a list of 3 bools where True indicates a specific bite is disabled and False
-        indicates leave enabled. If you supply indicators, then the internal indicators resource view template will be
-        used. The parameter indicators is a list with 3 dictionaries of form:
-        {'code': 'MY_INDICATOR_CODE', 'title': 'MY_INDICATOR_TITLE', 'unit': 'MY_INDICATOR_UNIT'}.
-        Creation of the resource view will be delayed until after the next dataset create
-        or update if a resource id is not yet available.
+        """Create QuickCharts for the given resource in a dataset. If you do
+        not supply a path, then the internal indicators resource view template
+        will be used. You can disable specific bites by providing
+        bites_disabled, a list of 3 bools where True indicates a specific bite
+        is disabled and False indicates leave enabled. The parameter indicators
+        is a list with 3 dictionaries of form:
+        {"code": "MY_INDICATOR_CODE", "title": "MY_INDICATOR_TITLE",
+        "unit": "MY_INDICATOR_UNIT"}. Optionally, the following defaults can be
+        overridden in the parameter indicators: {"code_col": "#indicator+code",
+        "value_col": "#indicator+value+num", "date_col": "#date+year",
+        "date_format": "%Y", "aggregate_col": "null"}.
+
+        Creation of the resource view will be delayed until after the next
+        dataset create or update if a resource id is not yet available.
 
         Args:
             resource (Union[Resource,Dict,str,int]): Either resource id or name, resource metadata from a Resource object or a dictionary or position. Defaults to 0.
             path (Optional[str]): Path to YAML resource view metadata. Defaults to None (config/hdx_resource_view_static.yml or internal template).
             bites_disabled (Optional[ListTuple[bool]]): Which QC bites should be disabled. Defaults to None (all bites enabled).
             indicators (Optional[ListTuple[Dict]]): Indicator codes, QC titles and units for resource view template. Defaults to None (don't use template).
             findreplace (Optional[Dict]): Replacements for anything else in resource view. Defaults to None.
@@ -2113,14 +2121,15 @@
         def replace_string(instr, what, withwhat):
             return instr.replace(what, str(withwhat))
 
         defaults = {
             "code_col": "#indicator+code",
             "value_col": "#indicator+value+num",
             "date_col": "#date+year",
+            "date_format": "%Y",
             "aggregate_col": "null",
         }
 
         def replace_col(hxl_preview_cfg, col_str, ind, col, with_quotes=False):
             if with_quotes:
                 col_str = f'"{col_str}"'
             replace = ind.get(col)
@@ -2162,14 +2171,20 @@
                     hxl_preview_config, "VALUE_COL_1", indicator, "value_col"
                 )
                 hxl_preview_config = replace_col(
                     hxl_preview_config, "DATE_COL_1", indicator, "date_col"
                 )
                 hxl_preview_config = replace_col(
                     hxl_preview_config,
+                    "DATE_FORMAT_1",
+                    indicator,
+                    "date_format",
+                )
+                hxl_preview_config = replace_col(
+                    hxl_preview_config,
                     "AGGREGATE_COL_1",
                     indicator,
                     "aggregate_col",
                     True,
                 )
                 indicators_notexist[0] = False
             if len_indicators > 1 and indicators[1]:
@@ -2195,14 +2210,20 @@
                     hxl_preview_config, "VALUE_COL_2", indicator, "value_col"
                 )
                 hxl_preview_config = replace_col(
                     hxl_preview_config, "DATE_COL_2", indicator, "date_col"
                 )
                 hxl_preview_config = replace_col(
                     hxl_preview_config,
+                    "DATE_FORMAT_2",
+                    indicator,
+                    "date_format",
+                )
+                hxl_preview_config = replace_col(
+                    hxl_preview_config,
                     "AGGREGATE_COL_2",
                     indicator,
                     "aggregate_col",
                     True,
                 )
                 indicators_notexist[1] = False
             if len_indicators > 2 and indicators[2]:
@@ -2228,14 +2249,20 @@
                     hxl_preview_config, "VALUE_COL_3", indicator, "value_col"
                 )
                 hxl_preview_config = replace_col(
                     hxl_preview_config, "DATE_COL_3", indicator, "date_col"
                 )
                 hxl_preview_config = replace_col(
                     hxl_preview_config,
+                    "DATE_FORMAT_3",
+                    indicator,
+                    "date_format",
+                )
+                hxl_preview_config = replace_col(
+                    hxl_preview_config,
                     "AGGREGATE_COL_3",
                     indicator,
                     "aggregate_col",
                     True,
                 )
                 indicators_notexist[2] = False
             if indicators_notexist == [True, True, True]:
@@ -2258,29 +2285,37 @@
         if "resource_id" in resourceview:
             resourceview.create_in_hdx()
             self.preview_resourceview = None
         else:
             self.preview_resourceview = resourceview
         return resourceview
 
-    def generate_resource_view(
+    def generate_quickcharts(
         self,
         resource: Union["Resource", Dict, str, int] = 0,
         path: Optional[str] = None,
         bites_disabled: Optional[ListTuple[bool]] = None,
         indicators: Optional[ListTuple[Dict]] = None,
         findreplace: Optional[Dict] = None,
     ) -> resource_view.ResourceView:
-        """Create QuickCharts for dataset from configuration saved in resource view. You can disable specific bites
-        by providing bites_disabled, a list of 3 bools where True indicates a specific bite is disabled and False
-        indicates leave enabled. If you supply indicators, then the internal indicators resource view template will be
-        used. The parameter indicators is a list with 3 dictionaries of form:
-        {'code': 'MY_INDICATOR_CODE', 'title': 'MY_INDICATOR_TITLE', 'unit': 'MY_INDICATOR_UNIT'}.
-        Creation of the resource view will be delayed until after the next dataset create
-        or update if a resource id is not yet available.
+        """Create QuickCharts for the given resource in a dataset. If you do
+        not supply a path, then the internal indicators resource view template
+        will be used. You can disable specific bites by providing
+        bites_disabled, a list of 3 bools where True indicates a specific bite
+        is disabled and False indicates leave enabled. The parameter indicators
+        is a list with 3 dictionaries of form:
+        {"code": "MY_INDICATOR_CODE", "title": "MY_INDICATOR_TITLE",
+        "unit": "MY_INDICATOR_UNIT"}. Optionally, the following defaults can be
+        overridden in the parameter indicators: {"code_col": "#indicator+code",
+        "value_col": "#indicator+value+num", "date_col": "#date+year",
+        "date_format": "%Y", "aggregate_col": "null"}.
+
+        Creation of the resource view will be delayed until after the next
+        dataset create or update if a resource id is not yet available and will
+        be disabled if there are no valid charts to display.
 
         Args:
             resource (Union[Resource,Dict,str,int]): Either resource id or name, resource metadata from a Resource object or a dictionary or position. Defaults to 0.
             path (Optional[str]): Path to YAML resource view metadata. Defaults to None (config/hdx_resource_view_static.yml or internal template).
             bites_disabled (Optional[ListTuple[bool]]): Which QC bites should be disabled. Defaults to None (all bites enabled).
             indicators (Optional[ListTuple[Dict]]): Indicator codes, QC titles and units for resource view template. Defaults to None (don't use template).
             findreplace (Optional[Dict]): Replacements for anything else in resource view. Defaults to None.
@@ -2338,15 +2373,18 @@
         folder: str,
         filename: str,
         rows: List[ListTupleDict],
         resourcedata: Dict,
         headers: Optional[ListTuple[str]] = None,
         encoding: Optional[str] = None,
     ) -> "Resource":
-        """Write rows to csv and create resource, adding to it the dataset
+        """Write rows to csv and create resource, adding it to the dataset.
+        The headers argument is either a row number (rows start counting at
+        1), or the actual headers defined as a list of strings. If not set, all
+        rows will be treated as containing values.
 
         Args:
             folder (str): Folder to which to write file containing rows
             filename (str): Filename of file to write rows
             rows (List[ListTupleDict]): List of rows in dict or list form
             resourcedata (Dict): Resource data
             headers (Optional[ListTuple[str]]): List of headers. Defaults to None.
@@ -2365,41 +2403,41 @@
 
     def generate_qc_resource_from_rows(
         self,
         folder: str,
         filename: str,
         rows: List[Dict],
         resourcedata: Dict,
-        columnname: str,
         hxltags: Dict[str, str],
-        qc_indicator_codes: ListTuple[str],
+        columnname: str,
+        qc_identifiers: ListTuple[str],
         headers: Optional[ListTuple[str]] = None,
         encoding: Optional[str] = None,
     ) -> Optional["Resource"]:
-        """Generate QuickCharts rows by cutting down input rows by indicator code and
-        optionally restricting to certain columns. Output to csv and create resource,
-        adding to it the dataset.
+        """Generate QuickCharts rows by cutting down input rows by relevant
+        identifiers and optionally restricting to certain columns. Output to
+        csv and create resource, adding it to the dataset.
 
         Args:
             folder (str): Folder to which to write file containing rows
             filename (str): Filename of file to write rows
             rows (List[Dict]): List of rows in dict form
             resourcedata (Dict): Resource data
-            columnname (str): Name of column containing indicator code
             hxltags (Dict[str,str]): Header to HXL hashtag mapping
-            qc_indicator_codes (ListTuple[str]): List of indicator codes to match
+            columnname (str): Name of column containing identifier
+            qc_identifiers (ListTuple[str]): List of ids to match
             headers (Optional[ListTuple[str]]): List of headers to output. Defaults to None (all headers).
             encoding (Optional[str]): Encoding to use. Defaults to None (infer encoding).
 
         Returns:
             Optional[Resource]: The created resource or None
         """
         qc_rows = list()
         for row in rows:
-            if row[columnname] in qc_indicator_codes:
+            if row[columnname] in qc_identifiers:
                 if headers:
                     qcrow = {x: row[x] for x in headers}
                 else:
                     qcrow = row
                 qc_rows.append(qcrow)
         if len(qc_rows) == 0:
             return None
@@ -2423,44 +2461,48 @@
         resourcedata: Dict,
         datecol: Optional[Union[int, str]] = None,
         yearcol: Optional[Union[int, str]] = None,
         date_function: Optional[Callable[[Dict], Optional[Dict]]] = None,
         quickcharts: Optional[Dict] = None,
         encoding: Optional[str] = None,
     ) -> Tuple[bool, Dict]:
-        """Given headers and an iterator, write rows to csv and create resource, adding
-        to it the dataset. The returned dictionary will contain the resource in the key
-        resource, headers in the key headers and list of rows in the key rows.
-
-        The reference period can optionally be set by supplying a column in which the
-        date or year is to be looked up. Note that any timezone information is ignored
-        and UTC assumed. Alternatively, a function can be supplied to handle any dates
-        in a row. It should accept a row and should return None to ignore the row or a
-        dictionary which can either be empty if there are no dates in the row or can be
-        populated with keys startdate and/or enddate which are of type timezone-aware
-        datetime. The lowest start date and highest end date are used to set the date of
-        dataset and are returned in the results dictionary in keys startdate and
-        enddate.
-
-        If the parameter quickcharts is supplied then various QuickCharts related
-        actions will occur depending upon the keys given in the dictionary and the
-        returned dictionary will contain the QuickCharts resource in the key
-        qc_resource. If the keys: hashtag - the HXL hashtag to examine - and values -
-        the 3 values to look for in that column - are supplied, then a list of booleans
-        indicating which QuickCharts bites should be enabled will be returned in the key
-        bites_disabled in the returned dictionary. For the 3 values, if the key:
-        numeric_hashtag is supplied then if that column for a given value contains no
-        numbers, then the corresponding bite will be disabled. If the key: cutdown is
-        given, if it is 1, then a separate cut down list is created containing only
-        columns with HXL hashtags and rows with desired values (if hashtag and values
-        are supplied) for the purpose of driving QuickCharts. It is returned in the key
-        qcrows in the returned dictionary with the matching headers in qcheaders. If
-        cutdown is 2, then a resource is created using the cut down list. If the key
-        cutdownhashtags is supplied, then only the provided hashtags are used for
-        cutting down otherwise the full list of hxl tags is used.
+        """Given headers and an iterator, write rows to csv and create
+        resource, adding to it the dataset. The returned dictionary will
+        contain the resource in the key resource, headers in the key headers
+        and list of rows in the key rows.
+
+        The reference period can optionally be set by supplying a column in
+        which the date or year is to be looked up. Note that any timezone
+        information is ignored and UTC assumed. Alternatively, a function can
+        be supplied to handle any dates in a row. It should accept a row and
+        should return None to ignore the row or a dictionary which can either
+        be empty if there are no dates in the row or can be populated with
+        keys startdate and/or enddate which are of type timezone-aware
+        datetime. The lowest start date and highest end date are used to set
+        the reference period and are returned in the results dictionary in keys
+        startdate and enddate.
+
+        If the parameter quickcharts is supplied then various QuickCharts
+        related actions will occur depending upon the keys given in the
+        dictionary and the returned dictionary will contain the QuickCharts
+        resource in the key qc_resource. If the keys: hashtag - the HXL hashtag
+        to examine - and values - the 3 values to look for in that column - are
+        supplied, then a list of booleans indicating which QuickCharts bites
+        should be enabled will be returned in the key bites_disabled in the
+        returned dictionary. For the 3 values, if the key: numeric_hashtag is
+        supplied then if that column for a given value contains no numbers,
+        then the corresponding bite will be disabled. If the key: cutdown is
+        given, if it is 1, then a separate cut down list is created containing
+        only columns with HXL hashtags and rows with desired values (if hashtag
+        and values are supplied) for the purpose of driving QuickCharts. It is
+        returned in the key qcrows in the returned dictionary with the matching
+        headers in qcheaders. If cutdown is 2, then a resource is created using
+        the cut down list. If the key cutdownhashtags is supplied, then only
+        the provided hashtags are used for cutting down otherwise the full list
+        of HXL tags is used.
 
         Args:
             headers (ListTuple[str]): Headers
             iterator (Iterator[Union[ListTuple,Dict]]): Iterator returning rows
             hxltags (Dict[str,str]): Header to HXL hashtag mapping
             folder (str): Folder to which to write file containing rows
             filename (str): Filename of file to write rows
@@ -2619,68 +2661,73 @@
                         encoding=encoding,
                     )
                     retdict["qc_resource"] = resource
         return True, retdict
 
     def download_and_generate_resource(
         self,
-        downloader: Download,
+        downloader: BaseDownload,
         url: str,
         hxltags: Dict[str, str],
         folder: str,
         filename: str,
         resourcedata: Dict,
         header_insertions: Optional[ListTuple[Tuple[int, str]]] = None,
         row_function: Optional[Callable[[List[str], Dict], Dict]] = None,
         datecol: Optional[str] = None,
         yearcol: Optional[str] = None,
         date_function: Optional[Callable[[Dict], Optional[Dict]]] = None,
         quickcharts: Optional[Dict] = None,
         **kwargs: Any,
     ) -> Tuple[bool, Dict]:
-        """Download url, write rows to csv and create resource, adding to it the
-        dataset. The returned dictionary will contain the resource in the key resource,
-        headers in the key headers and list of rows in the key rows.
-
-        Optionally, headers can be inserted at specific positions. This is achieved
-        using the header_insertions argument. If supplied, it is a list of tuples of the
-        form (position, header) to be inserted. A function is called for each row. If
-        supplied, it takes as arguments: headers (prior to any insertions) and row
-        (which will be in dict or list form depending upon the dict_rows argument) and
-        outputs a modified row.
-
-        The reference period can optionally be set by supplying a column in which the
-        date or year is to be looked up. Note that any timezone information is ignored
-        and UTC assumed. Alternatively, a function can be supplied to handle any dates
-        in a row. It should accept a row and should return None to ignore the row or a
-        dictionary which can either be empty if there are no dates in the row or can be
-        populated with keys startdate and/or enddate which are of type timezone-aware
-        datetime. The lowest start date and highest end date are used to set the date of
-        dataset and are returned in the results dictionary in keys startdate and
-        enddate.
-
-        If the parameter quickcharts is supplied then various QuickCharts related
-        actions will occur depending upon the keys given in the dictionary and the
-        returned dictionary will contain the QuickCharts resource in the key
-        qc_resource. If the keys: hashtag - the HXL hashtag to examine - and values -
-        the 3 values to look for in that column - are supplied, then a list of booleans
-        indicating which QuickCharts bites should be enabled will be returned in the key
-        bites_disabled in the returned dictionary. For the 3 values, if the key:
-        numeric_hashtag is supplied then if that column for a given value contains no
-        numbers, then the corresponding bite will be disabled. If the key: cutdown is
-        given, if it is 1, then a separate cut down list is created containing only
-        columns with HXL hashtags and rows with desired values (if hashtag and values
-        are supplied) for the purpose of driving QuickCharts. It is returned in the key
-        qcrows in the returned dictionary with the matching headers in qcheaders. If
-        cutdown is 2, then a resource is created using the cut down list. If the key
-        cutdownhashtags is supplied, then only the provided hashtags are used for
-        cutting down otherwise the full list of hxl tags is used.
+        """Download url, write rows to csv and create resource, adding to it
+        the dataset. The returned dictionary will contain the resource in the
+        key resource, headers in the key headers and list of rows in the key
+        rows.
+
+        Optionally, headers can be inserted at specific positions. This is
+        achieved using the header_insertions argument. If supplied, it is a
+        list of tuples of the form (position, header) to be inserted. A
+        function is called for each row. If supplied, it takes as arguments:
+        headers (prior to any insertions) and row (which will be in dict or
+        list form depending upon the dict_rows argument) and outputs a modified
+        row.
+
+        The reference period can optionally be set by supplying a column in
+        which the date or year is to be looked up. Note that any timezone
+        information is ignored and UTC assumed. Alternatively, a function can
+        be supplied to handle any dates in a row. It should accept a row and
+        should return None to ignore the row or a dictionary which can either
+        be empty if there are no dates in the row or can be populated with
+        keys startdate and/or enddate which are of type timezone-aware
+        datetime. The lowest start date and highest end date are used to set
+        the reference period and are returned in the results dictionary in keys
+        startdate and enddate.
+
+        If the parameter quickcharts is supplied then various QuickCharts
+        related actions will occur depending upon the keys given in the
+        dictionary and the returned dictionary will contain the QuickCharts
+        resource in the key qc_resource. If the keys: hashtag - the HXL hashtag
+        to examine - and values - the 3 values to look for in that column - are
+        supplied, then a list of booleans indicating which QuickCharts bites
+        should be enabled will be returned in the key bites_disabled in the
+        returned dictionary. For the 3 values, if the key: numeric_hashtag is
+        supplied then if that column for a given value contains no numbers,
+        then the corresponding bite will be disabled. If the key: cutdown is
+        given, if it is 1, then a separate cut down list is created containing
+        only columns with HXL hashtags and rows with desired values (if hashtag
+        and values are supplied) for the purpose of driving QuickCharts. It is
+        returned in the key qcrows in the returned dictionary with the matching
+        headers in qcheaders. If cutdown is 2, then a resource is created using
+        the cut down list. If the key cutdownhashtags is supplied, then only
+        the provided hashtags are used for cutting down otherwise the full list
+        of HXL tags is used.
 
         Args:
-            downloader (Download): Download object
+            downloader (BaseDownload): A Download or Retrieve object
             url (str): URL to download
             hxltags (Dict[str,str]): Header to HXL hashtag mapping
             folder (str): Folder to which to write file containing rows
             filename (str): Filename of file to write rows
             resourcedata (Dict): Resource data
             header_insertions (Optional[ListTuple[Tuple[int,str]]]): List of (position, header) to insert. Defaults to None.
             row_function (Optional[Callable[[List[str],Dict],Dict]]): Function to call for each row. Defaults to None.
```

### Comparing `hdx-python-api-5.9.9/src/hdx/data/dataset_title_helper.py` & `hdx-python-api-6.0.0/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/date_helper.py` & `hdx-python-api-6.0.0/src/hdx/data/date_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/filestore_helper.py` & `hdx-python-api-6.0.0/src/hdx/data/filestore_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/hdxobject.py` & `hdx-python-api-6.0.0/src/hdx/data/hdxobject.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/indicator_resource_view_template.yml` & `hdx-python-api-6.0.0/src/hdx/data/indicator_resource_view_template.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,4 +1,4 @@
 description: ""
 title: "Quick Charts"
 view_type: "hdx_hxl_preview"
-hxl_preview_config: '{"configVersion":5,"bites":[{"tempShowSaveCancelButtons":false,"ingredient":{"aggregateColumn":"AGGREGATE_COL_1","valueColumn":"VALUE_COL_1","aggregateFunction":"sum","dateColumn":"DATE_COL_1","comparisonValueColumn":null,"comparisonOperator":null,"filters":{"filterWith":[{"CODE_COL_1":"CODE_VALUE_1"}]},"description":"DESCRIPTION_VALUE_1"},"type":"timeseries","errorMsg":null,"computedProperties":{"explainedFiltersMap":{"remove empty valued rows":{"filterWith":[{"VALUE_COL_1":"is not empty"}],"filterWithout":[]}},"pieChart":false,"title":"Sum of Value by Year","dataTitle":"UNIT_VALUE_1"},"uiProperties":{"swapAxis":true,"showGrid":true,"color":"#0077ce","sortingByValue1":"DESC","sortingByCategory1":null,"showPoints":true,"internalColorPattern":["#1ebfb3","#0077ce","#f2645a","#9C27B0"],"title":"TITLE_VALUE_1"},"dataProperties":{},"displayCategory":"Timeseries","hashCode":498306664},{"tempShowSaveCancelButtons":false,"ingredient":{"aggregateColumn":"AGGREGATE_COL_2","valueColumn":"VALUE_COL_2","aggregateFunction":"sum","dateColumn":"DATE_COL_2","comparisonValueColumn":null,"comparisonOperator":null,"filters":{"filterWith":[{"CODE_COL_2":"CODE_VALUE_2"}]},"description":"DESCRIPTION_VALUE_2"},"type":"timeseries","errorMsg":null,"computedProperties":{"explainedFiltersMap":{"remove empty valued rows":{"filterWith":[{"VALUE_COL_2":"is not empty"}],"filterWithout":[]}},"pieChart":false,"title":"Sum of Value by Year","dataTitle":"UNIT_VALUE_2"},"uiProperties":{"swapAxis":true,"showGrid":true,"color":"#0077ce","sortingByValue1":"DESC","sortingByCategory1":null,"showPoints":true,"internalColorPattern":["#1ebfb3","#0077ce","#f2645a","#9C27B0"],"title":"TITLE_VALUE_2"},"dataProperties":{},"displayCategory":"Timeseries","hashCode":498306664},{"tempShowSaveCancelButtons":false,"ingredient":{"aggregateColumn":"AGGREGATE_COL_3","valueColumn":"VALUE_COL_3","aggregateFunction":"sum","dateColumn":"DATE_COL_3","comparisonValueColumn":null,"comparisonOperator":null,"filters":{"filterWith":[{"CODE_COL_3":"CODE_VALUE_3"}]},"description":"DESCRIPTION_VALUE_3"},"type":"timeseries","errorMsg":null,"computedProperties":{"explainedFiltersMap":{"remove empty valued rows":{"filterWith":[{"VALUE_COL_3":"is not empty"}],"filterWithout":[]}},"pieChart":false,"title":"Sum of Value by Year","dataTitle":"UNIT_VALUE_3"},"uiProperties":{"swapAxis":true,"showGrid":true,"color":"#0077ce","sortingByValue1":"DESC","sortingByCategory1":null,"showPoints":true,"internalColorPattern":["#1ebfb3","#0077ce","#f2645a","#9C27B0"],"title":"TITLE_VALUE_3"},"dataProperties":{},"displayCategory":"Timeseries","hashCode":498306664}],"recipeUrl":"https://raw.githubusercontent.com/mcarans/hxl-recipes/dev/recipes/historic-values-filtered/recipe.json"}'
+hxl_preview_config: '{"configVersion":5,"bites":[{"tempShowSaveCancelButtons":false,"ingredient":{"aggregateColumn":"AGGREGATE_COL_1","valueColumn":"VALUE_COL_1","aggregateFunction":"sum","dateColumn":"DATE_COL_1","comparisonValueColumn":null,"comparisonOperator":null,"filters":{"filterWith":[{"CODE_COL_1":"CODE_VALUE_1"}]},"description":"DESCRIPTION_VALUE_1"},"type":"timeseries","errorMsg":null,"computedProperties":{"explainedFiltersMap":{"remove empty valued rows":{"filterWith":[{"VALUE_COL_1":"is not empty"}],"filterWithout":[]}},"pieChart":false,"title":"Sum of Value by Year","dataTitle":"UNIT_VALUE_1"},"uiProperties":{"swapAxis":true,"showGrid":true,"color":"#0077ce","sortingByValue1":"DESC","sortingByCategory1":null,"showPoints":true,"internalColorPattern":["#1ebfb3","#0077ce","#f2645a","#9C27B0"],"title":"TITLE_VALUE_1","dateFormat":"DATE_FORMAT_1"},"dataProperties":{},"displayCategory":"Timeseries","hashCode":498306664},{"tempShowSaveCancelButtons":false,"ingredient":{"aggregateColumn":"AGGREGATE_COL_2","valueColumn":"VALUE_COL_2","aggregateFunction":"sum","dateColumn":"DATE_COL_2","comparisonValueColumn":null,"comparisonOperator":null,"filters":{"filterWith":[{"CODE_COL_2":"CODE_VALUE_2"}]},"description":"DESCRIPTION_VALUE_2"},"type":"timeseries","errorMsg":null,"computedProperties":{"explainedFiltersMap":{"remove empty valued rows":{"filterWith":[{"VALUE_COL_2":"is not empty"}],"filterWithout":[]}},"pieChart":false,"title":"Sum of Value by Year","dataTitle":"UNIT_VALUE_2"},"uiProperties":{"swapAxis":true,"showGrid":true,"color":"#0077ce","sortingByValue1":"DESC","sortingByCategory1":null,"showPoints":true,"internalColorPattern":["#1ebfb3","#0077ce","#f2645a","#9C27B0"],"title":"TITLE_VALUE_2","dateFormat":"DATE_FORMAT_2"},"dataProperties":{},"displayCategory":"Timeseries","hashCode":498306664},{"tempShowSaveCancelButtons":false,"ingredient":{"aggregateColumn":"AGGREGATE_COL_3","valueColumn":"VALUE_COL_3","aggregateFunction":"sum","dateColumn":"DATE_COL_3","comparisonValueColumn":null,"comparisonOperator":null,"filters":{"filterWith":[{"CODE_COL_3":"CODE_VALUE_3"}]},"description":"DESCRIPTION_VALUE_3"},"type":"timeseries","errorMsg":null,"computedProperties":{"explainedFiltersMap":{"remove empty valued rows":{"filterWith":[{"VALUE_COL_3":"is not empty"}],"filterWithout":[]}},"pieChart":false,"title":"Sum of Value by Year","dataTitle":"UNIT_VALUE_3"},"uiProperties":{"swapAxis":true,"showGrid":true,"color":"#0077ce","sortingByValue1":"DESC","sortingByCategory1":null,"showPoints":true,"internalColorPattern":["#1ebfb3","#0077ce","#f2645a","#9C27B0"],"title":"TITLE_VALUE_3","dateFormat":"DATE_FORMAT_3"},"dataProperties":{},"displayCategory":"Timeseries","hashCode":498306664}],"recipeUrl":"https://raw.githubusercontent.com/mcarans/hxl-recipes/dev/recipes/historic-values-filtered/recipe.json"}'
```

### Comparing `hdx-python-api-5.9.9/src/hdx/data/organization.py` & `hdx-python-api-6.0.0/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/resource.py` & `hdx-python-api-6.0.0/src/hdx/data/resource.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/resource_matcher.py` & `hdx-python-api-6.0.0/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/resource_view.py` & `hdx-python-api-6.0.0/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/showcase.py` & `hdx-python-api-6.0.0/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/user.py` & `hdx-python-api-6.0.0/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/data/vocabulary.py` & `hdx-python-api-6.0.0/src/hdx/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/facades/infer_arguments.py` & `hdx-python-api-6.0.0/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/facades/keyword_arguments.py` & `hdx-python-api-6.0.0/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx/facades/simple.py` & `hdx-python-api-6.0.0/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/src/hdx_python_api.egg-info/PKG-INFO` & `hdx-python-api-6.0.0/src/hdx_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 5.9.9
+Version: 6.0.0
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Home-page: https://github.com/OCHA-DAP/hdx-python-api
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,API,library,CKAN
 Platform: any
```

### Comparing `hdx-python-api-5.9.9/src/hdx_python_api.egg-info/SOURCES.txt` & `hdx-python-api-6.0.0/src/hdx_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/Accepted_Tags.csv` & `hdx-python-api-6.0.0/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/Tag_Mapping.csv` & `hdx-python-api-6.0.0/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/config/hdx_dataset_static.json` & `hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/config/hdx_dataset_static.yml` & `hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/config/hdx_datasource_topline.json` & `hdx-python-api-6.0.0/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/config/hdx_resource_view_static.yml` & `hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_view_static.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/dataset_search_results.yml` & `hdx-python-api-6.0.0/tests/fixtures/dataset_search_results.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx-python-api-6.0.0/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx-python-api-6.0.0/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx-python-api-6.0.0/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx-python-api-6.0.0/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/organization_show_results.yml` & `hdx-python-api-6.0.0/tests/fixtures/organization_show_results.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/resource_formats.json` & `hdx-python-api-6.0.0/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/showcase_all_search_results.yml` & `hdx-python-api-6.0.0/tests/fixtures/showcase_all_search_results.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/test_data.csv` & `hdx-python-api-6.0.0/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/test_data.zip` & `hdx-python-api-6.0.0/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_logic/update_logic_resources.yml` & `hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/fixtures/update_logic/update_logic_resources_new.yml` & `hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources_new.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/api/test_configuration.py` & `hdx-python-api-6.0.0/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/api/test_locations.py` & `hdx-python-api-6.0.0/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/conftest.py` & `hdx-python-api-6.0.0/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/__init__.py` & `hdx-python-api-6.0.0/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_dataset_core.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_dataset_core.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_dataset_noncore.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_dataset_noncore.py`

 * *Files 1% similar despite different names*

```diff
@@ -723,39 +723,39 @@
         self, configuration, vocabulary_update, static_resource_view_yaml
     ):
         datasetdata = copy.deepcopy(dataset_data)
         resourcesdata = copy.deepcopy(resources_data)
         datasetdata["resources"] = resourcesdata
         dataset = Dataset(datasetdata)
         assert "dataset_preview" not in dataset
-        resourceview = dataset.generate_resource_view(
+        resourceview = dataset.generate_quickcharts(
             path=static_resource_view_yaml
         )
         hxl_preview_config = json.loads(resourceview["hxl_preview_config"])
         assert resourceview["id"] == "c06b5a0d-1d41-4a74-a196-41c251c76023"
         assert hxl_preview_config["bites"][0]["title"] == "Sum of fatalities"
         assert (
             hxl_preview_config["bites"][1]["title"]
             == "Sum of fatalities grouped by admin1"
         )
         assert (
             hxl_preview_config["bites"][2]["title"]
             == "Sum of fatalities grouped by admin2"
         )
-        resourceview = dataset.generate_resource_view(
+        resourceview = dataset.generate_quickcharts(
             path=static_resource_view_yaml, bites_disabled=[False, True, False]
         )
         hxl_preview_config = json.loads(resourceview["hxl_preview_config"])
         assert resourceview["id"] == "c06b5a0d-1d41-4a74-a196-41c251c76023"
         assert hxl_preview_config["bites"][0]["title"] == "Sum of fatalities"
         assert (
             hxl_preview_config["bites"][1]["title"]
             == "Sum of fatalities grouped by admin2"
         )
-        resourceview = dataset.generate_resource_view(
+        resourceview = dataset.generate_quickcharts(
             path=static_resource_view_yaml, bites_disabled=[True, True, True]
         )
         assert resourceview is None
         indicators = [
             {
                 "code": "1",
                 "title": "My1",
@@ -769,17 +769,18 @@
                 "aggregate_col": "Agg2",
             },
             {
                 "code": "3",
                 "title": "My3",
                 "description": "This is my three!",
                 "date_col": "dt3",
+                "date_format": "%b %Y",
             },
         ]
-        resourceview = dataset.generate_resource_view(indicators=indicators)
+        resourceview = dataset.generate_quickcharts(indicators=indicators)
         hxl_preview_config = json.loads(resourceview["hxl_preview_config"])
         assert resourceview["id"] == "c06b5a0d-1d41-4a74-a196-41c251c76023"
         assert (
             hxl_preview_config["bites"][0]["ingredient"]["filters"][
                 "filterWith"
             ][0]["#indicator+code"]
             == "1"
@@ -825,15 +826,19 @@
             hxl_preview_config["bites"][2]["ingredient"]["dateColumn"] == "dt3"
         )
         assert hxl_preview_config["bites"][2]["uiProperties"]["title"] == "My3"
         assert (
             hxl_preview_config["bites"][2]["computedProperties"]["dataTitle"]
             == ""
         )
-        resourceview = dataset.generate_resource_view(
+        assert (
+            hxl_preview_config["bites"][2]["uiProperties"]["dateFormat"]
+            == "%b %Y"
+        )
+        resourceview = dataset.generate_quickcharts(
             indicators=indicators,
             findreplace={
                 "#indicator+code": "#item+code",
                 "#indicator+value+num": "#value",
             },
         )
         hxl_preview_config = json.loads(resourceview["hxl_preview_config"])
@@ -844,34 +849,33 @@
             ][0]["#item+code"]
             == "1"
         )
         assert (
             hxl_preview_config["bites"][0]["ingredient"]["valueColumn"]
             == "#value"
         )
-        assert dataset.generate_resource_view(indicators=[]) is None
+        assert dataset.generate_quickcharts(indicators=[]) is None
         assert (
-            dataset.generate_resource_view(indicators=[None, None, None])
-            is None
+            dataset.generate_quickcharts(indicators=[None, None, None]) is None
         )
         assert (
-            dataset.generate_resource_view(
+            dataset.generate_quickcharts(
                 resource="123", path=static_resource_view_yaml
             )
             is None
         )
         del dataset.get_resources()[0]["id"]
-        resourceview = dataset.generate_resource_view(
+        resourceview = dataset.generate_quickcharts(
             path=static_resource_view_yaml
         )
         assert "id" not in resourceview
         assert "resource_id" not in resourceview
         assert resourceview["resource_name"] == "Resource1"
         with pytest.raises(IOError):
-            dataset.generate_resource_view()
+            dataset.generate_quickcharts()
 
     def test_remove_dates_from_title(self):
         dataset = Dataset()
         with pytest.raises(HDXError):
             dataset.remove_dates_from_title()
         assert "title" not in dataset
         title = "Title with no dates"
@@ -966,16 +970,16 @@
                 columnname = "EVENT_ID_CNTY"
                 qc_indicator_codes = ["1416RTA", "XXXXRTA", "2231RTA"]
                 resource = dataset.generate_qc_resource_from_rows(
                     folder,
                     qc_filename,
                     rows,
                     resourcedata,
-                    columnname,
                     TestDatasetNoncore.hxltags,
+                    columnname,
                     qc_indicator_codes,
                 )
                 assert resource == {
                     "name": "Conflict Data for Algeria",
                     "description": "Conflict data with HXL tags",
                     "format": "csv",
                     "resource_type": "file.upload",
@@ -987,31 +991,31 @@
                 )
                 qc_filename = "qc_conflict_data_alg_one_col.csv"
                 dataset.generate_qc_resource_from_rows(
                     folder,
                     qc_filename,
                     rows,
                     resourcedata,
-                    columnname,
                     TestDatasetNoncore.hxltags,
+                    columnname,
                     qc_indicator_codes,
                     headers=[columnname],
                 )
                 assert_files_same(
                     join("tests", "fixtures", "qc_from_rows", qc_filename),
                     join(folder, qc_filename),
                 )
                 rows = list()
                 resource = dataset.generate_qc_resource_from_rows(
                     folder,
                     qc_filename,
                     rows,
                     resourcedata,
-                    columnname,
                     TestDatasetNoncore.hxltags,
+                    columnname,
                     qc_indicator_codes,
                 )
                 assert resource is None
 
     def test_download_and_generate_resource(self, configuration):
         with temp_dir("test") as folder:
             filename = "conflict_data_alg.csv"
```

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_dataset_title_helper.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_organization.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_resource.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_resource.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_resource_view.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_showcase.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_update_dataset_resources.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_update_dataset_resources.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_update_logic.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_user.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/data/test_vocabulary.py` & `hdx-python-api-6.0.0/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/facades/__init__.py` & `hdx-python-api-6.0.0/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/facades/test_infer_arguments.py` & `hdx-python-api-6.0.0/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/facades/test_keyword_arguments.py` & `hdx-python-api-6.0.0/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/tests/hdx/facades/test_simple.py` & `hdx-python-api-6.0.0/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-5.9.9/workingexample/my_resource.xlsx` & `hdx-python-api-6.0.0/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

