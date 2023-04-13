# Comparing `tmp/awswrangler-3.0.0rc2.tar.gz` & `tmp/awswrangler-3.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awswrangler-3.0.0rc2.tar", max compression
+gzip compressed data, was "awswrangler-3.0.0rc3.tar", max compression
```

## Comparing `awswrangler-3.0.0rc2.tar` & `awswrangler-3.0.0rc3.tar`

### file list

```diff
@@ -1,113 +1,125 @@
--rw-r--r--   0        0        0    10142 2022-08-02 16:44:38.861100 awswrangler-3.0.0rc2/LICENSE.txt
--rw-r--r--   0        0        0       92 2022-09-01 20:50:36.683640 awswrangler-3.0.0rc2/NOTICE.txt
--rw-r--r--   0        0        0    20733 2022-11-07 15:13:39.446063 awswrangler-3.0.0rc2/README.md
--rw-r--r--   0        0        0    17494 2022-08-02 16:44:38.861401 awswrangler-3.0.0rc2/THIRD_PARTY.txt
--rw-r--r--   0        0        0     1269 2022-11-01 16:19:08.118764 awswrangler-3.0.0rc2/awswrangler/__init__.py
--rw-r--r--   0        0        0      279 2022-11-07 15:13:39.447133 awswrangler-3.0.0rc2/awswrangler/__metadata__.py
--rw-r--r--   0        0        0     3898 2022-11-01 16:19:08.119696 awswrangler-3.0.0rc2/awswrangler/_arrow.py
--rw-r--r--   0        0        0    21070 2022-11-01 16:19:08.120850 awswrangler-3.0.0rc2/awswrangler/_config.py
--rw-r--r--   0        0        0    30852 2022-11-01 16:19:08.122191 awswrangler-3.0.0rc2/awswrangler/_data_types.py
--rw-r--r--   0        0        0    11543 2022-11-01 16:19:08.122685 awswrangler-3.0.0rc2/awswrangler/_databases.py
--rw-r--r--   0        0        0     4695 2022-11-01 16:19:08.123248 awswrangler-3.0.0rc2/awswrangler/_distributed.py
--rw-r--r--   0        0        0     6165 2022-11-01 16:19:08.123466 awswrangler-3.0.0rc2/awswrangler/_sql_formatter.py
--rw-r--r--   0        0        0     1655 2022-11-01 16:19:08.123857 awswrangler-3.0.0rc2/awswrangler/_threading.py
--rw-r--r--   0        0        0    17073 2022-11-01 16:19:08.124775 awswrangler-3.0.0rc2/awswrangler/_utils.py
--rw-r--r--   0        0        0     1038 2022-10-24 19:41:03.913126 awswrangler-3.0.0rc2/awswrangler/athena/__init__.py
--rw-r--r--   0        0        0     9086 2022-09-01 20:50:36.701144 awswrangler-3.0.0rc2/awswrangler/athena/_cache.py
--rw-r--r--   0        0        0    54824 2022-11-07 15:13:39.447917 awswrangler-3.0.0rc2/awswrangler/athena/_read.py
--rw-r--r--   0        0        0    49018 2022-11-01 16:19:08.126659 awswrangler-3.0.0rc2/awswrangler/athena/_utils.py
--rw-r--r--   0        0        0     2414 2022-08-02 16:44:38.862836 awswrangler-3.0.0rc2/awswrangler/catalog/__init__.py
--rw-r--r--   0        0        0    14124 2022-08-02 16:44:38.863006 awswrangler-3.0.0rc2/awswrangler/catalog/_add.py
--rw-r--r--   0        0        0    50606 2022-09-28 16:01:56.861248 awswrangler-3.0.0rc2/awswrangler/catalog/_create.py
--rw-r--r--   0        0        0    11272 2022-08-02 16:44:38.863251 awswrangler-3.0.0rc2/awswrangler/catalog/_definitions.py
--rw-r--r--   0        0        0     8318 2022-08-22 18:40:46.328287 awswrangler-3.0.0rc2/awswrangler/catalog/_delete.py
--rw-r--r--   0        0        0    36271 2022-08-22 18:40:46.329025 awswrangler-3.0.0rc2/awswrangler/catalog/_get.py
--rw-r--r--   0        0        0    11110 2022-09-01 20:50:36.707612 awswrangler-3.0.0rc2/awswrangler/catalog/_utils.py
--rw-r--r--   0        0        0     1199 2022-08-02 16:44:38.863657 awswrangler-3.0.0rc2/awswrangler/chime.py
--rw-r--r--   0        0        0     8326 2022-08-22 18:40:46.329577 awswrangler-3.0.0rc2/awswrangler/cloudwatch.py
--rw-r--r--   0        0        0      141 2022-08-02 16:44:38.863831 awswrangler-3.0.0rc2/awswrangler/data_api/__init__.py
--rw-r--r--   0        0        0     2829 2022-08-02 16:44:38.863903 awswrangler-3.0.0rc2/awswrangler/data_api/connector.py
--rw-r--r--   0        0        0     5715 2022-08-22 16:56:27.686982 awswrangler-3.0.0rc2/awswrangler/data_api/rds.py
--rw-r--r--   0        0        0     9561 2022-09-21 22:18:08.121983 awswrangler-3.0.0rc2/awswrangler/data_api/redshift.py
--rw-r--r--   0        0        0       26 2022-11-01 16:19:08.126820 awswrangler-3.0.0rc2/awswrangler/distributed/__init__.py
--rw-r--r--   0        0        0      237 2022-11-01 16:19:08.127265 awswrangler-3.0.0rc2/awswrangler/distributed/ray/__init__.py
--rw-r--r--   0        0        0     5563 2022-11-04 17:41:02.111626 awswrangler-3.0.0rc2/awswrangler/distributed/ray/_core.py
--rw-r--r--   0        0        0      931 2022-11-04 17:41:02.112379 awswrangler-3.0.0rc2/awswrangler/distributed/ray/_core.pyi
--rw-r--r--   0        0        0      563 2022-11-01 16:19:08.127844 awswrangler-3.0.0rc2/awswrangler/distributed/ray/_pool.py
--rw-r--r--   0        0        0     3027 2022-11-04 20:31:38.531026 awswrangler-3.0.0rc2/awswrangler/distributed/ray/_register.py
--rw-r--r--   0        0        0      749 2022-11-01 16:19:08.128486 awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/__init__.py
--rw-r--r--   0        0        0     2166 2022-11-01 16:19:08.128987 awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
--rw-r--r--   0        0        0    18780 2022-11-04 17:41:02.113499 awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
--rw-r--r--   0        0        0     5490 2022-11-04 17:41:02.114082 awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
--rw-r--r--   0        0        0     5840 2022-11-04 17:41:02.114691 awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
--rw-r--r--   0        0        0      135 2022-11-01 16:19:08.130370 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/__init__.py
--rw-r--r--   0        0        0     2430 2022-11-01 16:19:08.130616 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/_core.py
--rw-r--r--   0        0        0      850 2022-11-04 17:41:02.115294 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/_data_types.py
--rw-r--r--   0        0        0     2909 2022-11-04 17:41:02.115932 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/_utils.py
--rw-r--r--   0        0        0       27 2022-11-01 16:19:08.131491 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/__init__.py
--rw-r--r--   0        0        0     1405 2022-11-01 16:19:08.131798 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_read_parquet.py
--rw-r--r--   0        0        0     4043 2022-11-01 16:19:08.132235 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_read_text.py
--rw-r--r--   0        0        0     7201 2022-11-04 17:41:02.116493 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_write_dataset.py
--rw-r--r--   0        0        0     3099 2022-11-01 16:19:08.132821 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_write_parquet.py
--rw-r--r--   0        0        0     5448 2022-11-01 16:19:08.133236 awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_write_text.py
--rw-r--r--   0        0        0      385 2022-08-02 16:44:38.864155 awswrangler-3.0.0rc2/awswrangler/dynamodb/__init__.py
--rw-r--r--   0        0        0     1530 2022-08-22 18:40:46.331964 awswrangler-3.0.0rc2/awswrangler/dynamodb/_delete.py
--rw-r--r--   0        0        0     4910 2022-08-22 18:40:46.332356 awswrangler-3.0.0rc2/awswrangler/dynamodb/_read.py
--rw-r--r--   0        0        0     1813 2022-08-22 18:40:46.332730 awswrangler-3.0.0rc2/awswrangler/dynamodb/_utils.py
--rw-r--r--   0        0        0     5341 2022-09-01 20:50:36.708266 awswrangler-3.0.0rc2/awswrangler/dynamodb/_write.py
--rw-r--r--   0        0        0    42178 2022-09-01 20:50:36.708870 awswrangler-3.0.0rc2/awswrangler/emr.py
--rw-r--r--   0        0        0     2239 2022-08-02 16:44:38.864695 awswrangler-3.0.0rc2/awswrangler/exceptions.py
--rw-r--r--   0        0        0      682 2022-08-02 16:44:38.864788 awswrangler-3.0.0rc2/awswrangler/lakeformation/__init__.py
--rw-r--r--   0        0        0    10599 2022-11-01 16:19:08.133695 awswrangler-3.0.0rc2/awswrangler/lakeformation/_read.py
--rw-r--r--   0        0        0    13287 2022-11-03 13:55:05.614930 awswrangler-3.0.0rc2/awswrangler/lakeformation/_utils.py
--rw-r--r--   0        0        0    17156 2022-08-22 16:56:27.690137 awswrangler-3.0.0rc2/awswrangler/mysql.py
--rw-r--r--   0        0        0      482 2022-08-02 16:44:38.865162 awswrangler-3.0.0rc2/awswrangler/neptune/__init__.py
--rw-r--r--   0        0        0     3739 2022-08-02 16:44:38.865229 awswrangler-3.0.0rc2/awswrangler/neptune/_utils.py
--rw-r--r--   0        0        0     9459 2022-08-22 16:56:27.691117 awswrangler-3.0.0rc2/awswrangler/neptune/client.py
--rw-r--r--   0        0        0     2326 2022-08-02 16:44:38.865371 awswrangler-3.0.0rc2/awswrangler/neptune/gremlin_parser.py
--rw-r--r--   0        0        0    15719 2022-09-01 20:50:36.709488 awswrangler-3.0.0rc2/awswrangler/neptune/neptune.py
--rw-r--r--   0        0        0      458 2022-08-02 16:44:38.865568 awswrangler-3.0.0rc2/awswrangler/opensearch/__init__.py
--rw-r--r--   0        0        0     5867 2022-08-02 16:44:38.865650 awswrangler-3.0.0rc2/awswrangler/opensearch/_read.py
--rw-r--r--   0        0        0     3921 2022-09-21 22:18:08.124538 awswrangler-3.0.0rc2/awswrangler/opensearch/_utils.py
--rw-r--r--   0        0        0    20535 2022-08-22 18:40:46.334379 awswrangler-3.0.0rc2/awswrangler/opensearch/_write.py
--rw-r--r--   0        0        0    16590 2022-11-01 16:19:08.134458 awswrangler-3.0.0rc2/awswrangler/oracle.py
--rw-r--r--   0        0        0    15819 2022-08-22 16:56:27.697813 awswrangler-3.0.0rc2/awswrangler/postgresql.py
--rw-r--r--   0        0        0       27 2022-08-02 16:44:38.866284 awswrangler-3.0.0rc2/awswrangler/py.typed
--rw-r--r--   0        0        0     2219 2022-08-02 16:44:38.866388 awswrangler-3.0.0rc2/awswrangler/quicksight/__init__.py
--rw-r--r--   0        0        0     1931 2022-08-02 16:44:38.866482 awswrangler-3.0.0rc2/awswrangler/quicksight/_cancel.py
--rw-r--r--   0        0        0    15571 2022-09-21 22:12:59.297774 awswrangler-3.0.0rc2/awswrangler/quicksight/_create.py
--rw-r--r--   0        0        0    11088 2022-08-02 16:44:38.866665 awswrangler-3.0.0rc2/awswrangler/quicksight/_delete.py
--rw-r--r--   0        0        0     8698 2022-08-02 16:44:38.866743 awswrangler-3.0.0rc2/awswrangler/quicksight/_describe.py
--rw-r--r--   0        0        0    23793 2022-08-02 16:44:38.866827 awswrangler-3.0.0rc2/awswrangler/quicksight/_get_list.py
--rw-r--r--   0        0        0     1908 2022-08-02 16:44:38.866908 awswrangler-3.0.0rc2/awswrangler/quicksight/_utils.py
--rw-r--r--   0        0        0    66775 2022-11-03 13:55:05.615950 awswrangler-3.0.0rc2/awswrangler/redshift.py
--rw-r--r--   0        0        0     1690 2022-10-11 16:56:41.224551 awswrangler-3.0.0rc2/awswrangler/s3/__init__.py
--rw-r--r--   0        0        0     9819 2022-08-02 16:44:38.867327 awswrangler-3.0.0rc2/awswrangler/s3/_copy.py
--rw-r--r--   0        0        0     5161 2022-11-01 16:19:08.135857 awswrangler-3.0.0rc2/awswrangler/s3/_delete.py
--rw-r--r--   0        0        0    10473 2022-11-04 20:31:38.531945 awswrangler-3.0.0rc2/awswrangler/s3/_describe.py
--rw-r--r--   0        0        0     2713 2022-08-02 16:44:38.867698 awswrangler-3.0.0rc2/awswrangler/s3/_download.py
--rw-r--r--   0        0        0    23403 2022-11-01 16:19:08.136441 awswrangler-3.0.0rc2/awswrangler/s3/_fs.py
--rw-r--r--   0        0        0    14499 2022-09-06 20:46:03.829201 awswrangler-3.0.0rc2/awswrangler/s3/_list.py
--rw-r--r--   0        0        0     2638 2022-08-22 16:56:27.700453 awswrangler-3.0.0rc2/awswrangler/s3/_list.pyi
--rw-r--r--   0        0        0     5874 2022-09-21 22:12:59.298836 awswrangler-3.0.0rc2/awswrangler/s3/_merge_upsert_table.py
--rw-r--r--   0        0        0     5933 2022-11-04 20:31:38.533026 awswrangler-3.0.0rc2/awswrangler/s3/_read.py
--rw-r--r--   0        0        0     3231 2022-09-01 20:50:36.713521 awswrangler-3.0.0rc2/awswrangler/s3/_read_excel.py
--rw-r--r--   0        0        0    35037 2022-11-07 15:13:39.448610 awswrangler-3.0.0rc2/awswrangler/s3/_read_parquet.py
--rw-r--r--   0        0        0    26790 2022-11-07 15:13:39.449178 awswrangler-3.0.0rc2/awswrangler/s3/_read_text.py
--rw-r--r--   0        0        0     4121 2022-11-01 16:19:08.139549 awswrangler-3.0.0rc2/awswrangler/s3/_read_text_core.py
--rw-r--r--   0        0        0    11194 2022-11-01 16:19:08.140194 awswrangler-3.0.0rc2/awswrangler/s3/_select.py
--rw-r--r--   0        0        0     2538 2022-08-02 16:44:38.868843 awswrangler-3.0.0rc2/awswrangler/s3/_upload.py
--rw-r--r--   0        0        0     6254 2022-11-01 16:19:08.140785 awswrangler-3.0.0rc2/awswrangler/s3/_wait.py
--rw-r--r--   0        0        0     4286 2022-11-01 16:19:08.141255 awswrangler-3.0.0rc2/awswrangler/s3/_write.py
--rw-r--r--   0        0        0     2234 2022-11-01 16:19:08.141566 awswrangler-3.0.0rc2/awswrangler/s3/_write_concurrent.py
--rw-r--r--   0        0        0    12310 2022-11-03 13:55:05.616660 awswrangler-3.0.0rc2/awswrangler/s3/_write_dataset.py
--rw-r--r--   0        0        0     3162 2022-09-01 20:50:36.715461 awswrangler-3.0.0rc2/awswrangler/s3/_write_excel.py
--rw-r--r--   0        0        0    40603 2022-11-07 15:13:39.449742 awswrangler-3.0.0rc2/awswrangler/s3/_write_parquet.py
--rw-r--r--   0        0        0    46340 2022-11-07 15:13:39.450220 awswrangler-3.0.0rc2/awswrangler/s3/_write_text.py
--rw-r--r--   0        0        0     2146 2022-08-02 16:44:38.869642 awswrangler-3.0.0rc2/awswrangler/secretsmanager.py
--rw-r--r--   0        0        0    15948 2022-09-01 20:50:36.717118 awswrangler-3.0.0rc2/awswrangler/sqlserver.py
--rw-r--r--   0        0        0     2025 2022-08-02 16:44:38.869785 awswrangler-3.0.0rc2/awswrangler/sts.py
--rw-r--r--   0        0        0    20507 2022-11-01 16:19:08.144249 awswrangler-3.0.0rc2/awswrangler/timestream.py
--rw-r--r--   0        0        0     3142 2022-11-07 15:13:39.452059 awswrangler-3.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    22746 1970-01-01 00:00:00.000000 awswrangler-3.0.0rc2/setup.py
--rw-r--r--   0        0        0    22685 1970-01-01 00:00:00.000000 awswrangler-3.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    10142 2021-01-13 17:42:05.000000 awswrangler-3.0.0rc3/LICENSE.txt
+-rw-r--r--   0        0        0       92 2022-09-07 12:05:27.255553 awswrangler-3.0.0rc3/NOTICE.txt
+-rw-r--r--   0        0        0    21748 2023-03-09 12:07:46.432839 awswrangler-3.0.0rc3/README.md
+-rw-r--r--   0        0        0    17494 2021-01-13 17:42:05.000000 awswrangler-3.0.0rc3/THIRD_PARTY.txt
+-rw-r--r--   0        0        0     1405 2023-03-08 12:15:27.591147 awswrangler-3.0.0rc3/awswrangler/__init__.py
+-rw-r--r--   0        0        0      279 2023-03-09 12:07:49.987326 awswrangler-3.0.0rc3/awswrangler/__metadata__.py
+-rw-r--r--   0        0        0     3909 2023-03-08 12:15:27.591821 awswrangler-3.0.0rc3/awswrangler/_arrow.py
+-rw-r--r--   0        0        0    26860 2023-03-08 12:15:27.592854 awswrangler-3.0.0rc3/awswrangler/_config.py
+-rw-r--r--   0        0        0    31114 2023-03-08 12:15:27.594375 awswrangler-3.0.0rc3/awswrangler/_data_types.py
+-rw-r--r--   0        0        0    12621 2023-03-08 15:59:02.540573 awswrangler-3.0.0rc3/awswrangler/_databases.py
+-rw-r--r--   0        0        0     5271 2023-03-08 12:15:27.595561 awswrangler-3.0.0rc3/awswrangler/_distributed.py
+-rw-r--r--   0        0        0     6211 2023-03-08 12:15:27.595743 awswrangler-3.0.0rc3/awswrangler/_sql_formatter.py
+-rw-r--r--   0        0        0     1657 2023-03-08 12:15:27.595951 awswrangler-3.0.0rc3/awswrangler/_threading.py
+-rw-r--r--   0        0        0    27386 2023-03-08 15:59:02.541259 awswrangler-3.0.0rc3/awswrangler/_utils.py
+-rw-r--r--   0        0        0     1700 2023-02-28 14:45:26.197772 awswrangler-3.0.0rc3/awswrangler/annotations.py
+-rw-r--r--   0        0        0     1038 2023-02-06 14:01:33.949479 awswrangler-3.0.0rc3/awswrangler/athena/__init__.py
+-rw-r--r--   0        0        0     9301 2023-03-08 12:15:27.597366 awswrangler-3.0.0rc3/awswrangler/athena/_cache.py
+-rw-r--r--   0        0        0    65007 2023-03-09 12:07:51.643380 awswrangler-3.0.0rc3/awswrangler/athena/_read.py
+-rw-r--r--   0        0        0    52218 2023-03-09 12:05:44.014718 awswrangler-3.0.0rc3/awswrangler/athena/_utils.py
+-rw-r--r--   0        0        0     2414 2023-02-06 14:01:33.952737 awswrangler-3.0.0rc3/awswrangler/catalog/__init__.py
+-rw-r--r--   0        0        0    14077 2023-03-08 12:15:27.600887 awswrangler-3.0.0rc3/awswrangler/catalog/_add.py
+-rw-r--r--   0        0        0    49119 2023-03-08 12:15:27.601768 awswrangler-3.0.0rc3/awswrangler/catalog/_create.py
+-rw-r--r--   0        0        0    11466 2023-03-08 12:15:27.602150 awswrangler-3.0.0rc3/awswrangler/catalog/_definitions.py
+-rw-r--r--   0        0        0     8178 2023-03-08 12:15:27.602755 awswrangler-3.0.0rc3/awswrangler/catalog/_delete.py
+-rw-r--r--   0        0        0    36005 2023-03-08 15:59:02.542310 awswrangler-3.0.0rc3/awswrangler/catalog/_get.py
+-rw-r--r--   0        0        0    11221 2023-03-08 15:59:02.543175 awswrangler-3.0.0rc3/awswrangler/catalog/_utils.py
+-rw-r--r--   0        0        0     1199 2022-10-08 10:37:42.800465 awswrangler-3.0.0rc3/awswrangler/chime.py
+-rw-r--r--   0        0        0    16587 2023-03-08 15:59:02.543878 awswrangler-3.0.0rc3/awswrangler/cloudwatch.py
+-rw-r--r--   0        0        0      141 2022-10-08 10:37:42.802168 awswrangler-3.0.0rc3/awswrangler/data_api/__init__.py
+-rw-r--r--   0        0        0     2829 2023-03-08 15:59:02.545717 awswrangler-3.0.0rc3/awswrangler/data_api/_connector.py
+-rw-r--r--   0        0        0     5711 2023-03-08 15:59:02.546277 awswrangler-3.0.0rc3/awswrangler/data_api/rds.py
+-rw-r--r--   0        0        0     9535 2023-03-08 15:59:02.548007 awswrangler-3.0.0rc3/awswrangler/data_api/redshift.py
+-rw-r--r--   0        0        0      377 2023-02-06 14:01:33.956385 awswrangler-3.0.0rc3/awswrangler/data_quality/__init__.py
+-rw-r--r--   0        0        0    13575 2023-03-08 15:59:02.548811 awswrangler-3.0.0rc3/awswrangler/data_quality/_create.py
+-rw-r--r--   0        0        0     1392 2023-03-08 15:59:02.549405 awswrangler-3.0.0rc3/awswrangler/data_quality/_get.py
+-rw-r--r--   0        0        0     6531 2023-03-08 15:59:02.549879 awswrangler-3.0.0rc3/awswrangler/data_quality/_utils.py
+-rw-r--r--   0        0        0       26 2023-03-08 12:15:27.608654 awswrangler-3.0.0rc3/awswrangler/distributed/__init__.py
+-rw-r--r--   0        0        0      237 2023-03-08 12:15:27.608904 awswrangler-3.0.0rc3/awswrangler/distributed/ray/__init__.py
+-rw-r--r--   0        0        0     6256 2023-03-08 12:15:27.609095 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.py
+-rw-r--r--   0        0        0      931 2023-03-08 12:15:27.609264 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.pyi
+-rw-r--r--   0        0        0      691 2023-03-08 12:15:27.609747 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_pool.py
+-rw-r--r--   0        0        0     3794 2023-03-08 15:59:02.550452 awswrangler-3.0.0rc3/awswrangler/distributed/ray/_register.py
+-rw-r--r--   0        0        0     1013 2023-03-08 12:15:27.611382 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/__init__.py
+-rw-r--r--   0        0        0     2191 2023-03-08 12:15:27.611592 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py
+-rw-r--r--   0        0        0     1273 2023-03-08 12:15:27.611744 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_json_datasource.py
+-rw-r--r--   0        0        0     3323 2023-03-08 12:15:27.612380 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_parquet_base_datasource.py
+-rw-r--r--   0        0        0    18550 2023-03-08 12:15:27.613073 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py
+-rw-r--r--   0        0        0     5880 2023-03-08 12:15:27.614125 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py
+-rw-r--r--   0        0        0     5896 2023-03-08 12:15:27.614332 awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_text_datasource.py
+-rw-r--r--   0        0        0      135 2023-03-08 12:15:27.614858 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/__init__.py
+-rw-r--r--   0        0        0     2524 2023-03-08 12:15:27.615045 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_core.py
+-rw-r--r--   0        0        0      929 2023-03-08 12:15:27.615199 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_data_types.py
+-rw-r--r--   0        0        0     4116 2023-03-08 15:59:02.551878 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_utils.py
+-rw-r--r--   0        0        0       27 2023-03-08 12:15:27.615513 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/__init__.py
+-rw-r--r--   0        0        0     1861 2023-03-08 12:15:27.616193 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_read_parquet.py
+-rw-r--r--   0        0        0     5507 2023-03-08 12:15:27.617730 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_read_text.py
+-rw-r--r--   0        0        0     7368 2023-03-08 12:15:27.617987 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_dataset.py
+-rw-r--r--   0        0        0     3065 2023-03-08 12:15:27.618180 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_parquet.py
+-rw-r--r--   0        0        0     5500 2023-03-08 12:15:27.619168 awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_text.py
+-rw-r--r--   0        0        0       21 2023-03-08 12:15:27.619453 awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/__init__.py
+-rw-r--r--   0        0        0     2413 2023-03-08 12:15:27.620925 awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/_list.py
+-rw-r--r--   0        0        0      948 2023-03-08 12:15:27.621309 awswrangler-3.0.0rc3/awswrangler/distributed/ray/s3/_read_parquet.py
+-rw-r--r--   0        0        0      484 2023-01-26 20:57:05.678884 awswrangler-3.0.0rc3/awswrangler/dynamodb/__init__.py
+-rw-r--r--   0        0        0     1530 2023-02-03 14:21:04.504277 awswrangler-3.0.0rc3/awswrangler/dynamodb/_delete.py
+-rw-r--r--   0        0        0    24682 2023-03-08 15:59:02.552497 awswrangler-3.0.0rc3/awswrangler/dynamodb/_read.py
+-rw-r--r--   0        0        0     6951 2023-03-08 12:15:27.623772 awswrangler-3.0.0rc3/awswrangler/dynamodb/_utils.py
+-rw-r--r--   0        0        0     5367 2023-03-08 15:59:02.553390 awswrangler-3.0.0rc3/awswrangler/dynamodb/_write.py
+-rw-r--r--   0        0        0    43346 2023-03-08 12:15:27.625778 awswrangler-3.0.0rc3/awswrangler/emr.py
+-rw-r--r--   0        0        0     2610 2023-03-08 12:15:27.626512 awswrangler-3.0.0rc3/awswrangler/exceptions.py
+-rw-r--r--   0        0        0      682 2023-02-06 14:01:33.970611 awswrangler-3.0.0rc3/awswrangler/lakeformation/__init__.py
+-rw-r--r--   0        0        0    10914 2023-03-08 12:15:27.627707 awswrangler-3.0.0rc3/awswrangler/lakeformation/_read.py
+-rw-r--r--   0        0        0    13144 2023-03-08 12:15:27.629036 awswrangler-3.0.0rc3/awswrangler/lakeformation/_utils.py
+-rw-r--r--   0        0        0    20092 2023-03-08 15:59:02.554140 awswrangler-3.0.0rc3/awswrangler/mysql.py
+-rw-r--r--   0        0        0      484 2023-03-08 12:15:27.630640 awswrangler-3.0.0rc3/awswrangler/neptune/__init__.py
+-rw-r--r--   0        0        0     9648 2023-03-08 12:15:27.631252 awswrangler-3.0.0rc3/awswrangler/neptune/_client.py
+-rw-r--r--   0        0        0      923 2023-03-08 12:15:27.631448 awswrangler-3.0.0rc3/awswrangler/neptune/_gremlin_init.py
+-rw-r--r--   0        0        0     2685 2023-03-08 12:15:27.631634 awswrangler-3.0.0rc3/awswrangler/neptune/_gremlin_parser.py
+-rw-r--r--   0        0        0    15665 2023-03-08 15:59:02.555007 awswrangler-3.0.0rc3/awswrangler/neptune/_neptune.py
+-rw-r--r--   0        0        0     3736 2023-03-08 15:59:02.555454 awswrangler-3.0.0rc3/awswrangler/neptune/_utils.py
+-rw-r--r--   0        0        0      502 2023-02-06 14:01:33.975500 awswrangler-3.0.0rc3/awswrangler/opensearch/__init__.py
+-rw-r--r--   0        0        0     6470 2023-03-08 15:59:02.555999 awswrangler-3.0.0rc3/awswrangler/opensearch/_read.py
+-rw-r--r--   0        0        0    13684 2023-03-08 12:15:27.633906 awswrangler-3.0.0rc3/awswrangler/opensearch/_utils.py
+-rw-r--r--   0        0        0    21497 2023-03-08 15:59:02.557225 awswrangler-3.0.0rc3/awswrangler/opensearch/_write.py
+-rw-r--r--   0        0        0    18538 2023-03-08 15:59:02.557830 awswrangler-3.0.0rc3/awswrangler/oracle.py
+-rw-r--r--   0        0        0    18557 2023-03-08 15:59:02.558527 awswrangler-3.0.0rc3/awswrangler/postgresql.py
+-rw-r--r--   0        0        0       27 2022-10-08 10:37:42.809867 awswrangler-3.0.0rc3/awswrangler/py.typed
+-rw-r--r--   0        0        0     2219 2023-02-06 14:01:33.981133 awswrangler-3.0.0rc3/awswrangler/quicksight/__init__.py
+-rw-r--r--   0        0        0     1906 2023-03-08 12:15:27.637078 awswrangler-3.0.0rc3/awswrangler/quicksight/_cancel.py
+-rw-r--r--   0        0        0    15485 2023-03-08 12:15:27.637832 awswrangler-3.0.0rc3/awswrangler/quicksight/_create.py
+-rw-r--r--   0        0        0    11710 2023-03-08 12:15:27.638684 awswrangler-3.0.0rc3/awswrangler/quicksight/_delete.py
+-rw-r--r--   0        0        0     8659 2023-03-08 12:15:27.639397 awswrangler-3.0.0rc3/awswrangler/quicksight/_describe.py
+-rw-r--r--   0        0        0    23655 2023-03-08 12:15:27.640237 awswrangler-3.0.0rc3/awswrangler/quicksight/_get_list.py
+-rw-r--r--   0        0        0     1929 2023-03-08 12:15:27.640749 awswrangler-3.0.0rc3/awswrangler/quicksight/_utils.py
+-rw-r--r--   0        0        0    71162 2023-03-09 12:05:44.015919 awswrangler-3.0.0rc3/awswrangler/redshift.py
+-rw-r--r--   0        0        0     1704 2023-03-08 12:15:27.644244 awswrangler-3.0.0rc3/awswrangler/s3/__init__.py
+-rw-r--r--   0        0        0    10654 2023-03-08 12:15:27.646030 awswrangler-3.0.0rc3/awswrangler/s3/_copy.py
+-rw-r--r--   0        0        0     5305 2023-03-08 12:15:27.647330 awswrangler-3.0.0rc3/awswrangler/s3/_delete.py
+-rw-r--r--   0        0        0     9346 2023-03-08 12:15:27.648395 awswrangler-3.0.0rc3/awswrangler/s3/_describe.py
+-rw-r--r--   0        0        0     2633 2023-01-26 18:51:25.209062 awswrangler-3.0.0rc3/awswrangler/s3/_download.py
+-rw-r--r--   0        0        0    23119 2023-03-08 12:15:27.649704 awswrangler-3.0.0rc3/awswrangler/s3/_fs.py
+-rw-r--r--   0        0        0    15630 2023-03-08 12:15:27.650507 awswrangler-3.0.0rc3/awswrangler/s3/_list.py
+-rw-r--r--   0        0        0     3970 2023-03-08 12:15:27.651659 awswrangler-3.0.0rc3/awswrangler/s3/_list.pyi
+-rw-r--r--   0        0        0     5342 2023-03-08 12:15:27.651979 awswrangler-3.0.0rc3/awswrangler/s3/_read.py
+-rw-r--r--   0        0        0     3345 2023-03-08 12:15:27.652310 awswrangler-3.0.0rc3/awswrangler/s3/_read_deltalake.py
+-rw-r--r--   0        0        0     3265 2023-03-08 12:15:27.652733 awswrangler-3.0.0rc3/awswrangler/s3/_read_excel.py
+-rw-r--r--   0        0        0    43247 2023-03-09 12:07:53.865219 awswrangler-3.0.0rc3/awswrangler/s3/_read_parquet.py
+-rw-r--r--   0        0        0    33704 2023-03-09 12:07:56.102213 awswrangler-3.0.0rc3/awswrangler/s3/_read_text.py
+-rw-r--r--   0        0        0     4108 2023-03-08 12:15:27.655668 awswrangler-3.0.0rc3/awswrangler/s3/_read_text_core.py
+-rw-r--r--   0        0        0    11642 2023-03-08 12:15:27.656418 awswrangler-3.0.0rc3/awswrangler/s3/_select.py
+-rw-r--r--   0        0        0     2465 2023-03-08 12:15:27.656776 awswrangler-3.0.0rc3/awswrangler/s3/_upload.py
+-rw-r--r--   0        0        0     6584 2023-03-08 12:15:27.658242 awswrangler-3.0.0rc3/awswrangler/s3/_wait.py
+-rw-r--r--   0        0        0     4298 2023-03-08 12:15:27.658568 awswrangler-3.0.0rc3/awswrangler/s3/_write.py
+-rw-r--r--   0        0        0     1840 2023-03-08 12:15:27.658883 awswrangler-3.0.0rc3/awswrangler/s3/_write_concurrent.py
+-rw-r--r--   0        0        0    12676 2023-03-08 12:15:27.659239 awswrangler-3.0.0rc3/awswrangler/s3/_write_dataset.py
+-rw-r--r--   0        0        0     3196 2023-03-08 12:15:27.659541 awswrangler-3.0.0rc3/awswrangler/s3/_write_excel.py
+-rw-r--r--   0        0        0    43164 2023-03-09 12:07:57.600534 awswrangler-3.0.0rc3/awswrangler/s3/_write_parquet.py
+-rw-r--r--   0        0        0    48770 2023-03-09 12:07:58.910296 awswrangler-3.0.0rc3/awswrangler/s3/_write_text.py
+-rw-r--r--   0        0        0     2018 2023-03-08 12:15:27.662297 awswrangler-3.0.0rc3/awswrangler/secretsmanager.py
+-rw-r--r--   0        0        0    17879 2023-03-08 15:59:02.559864 awswrangler-3.0.0rc3/awswrangler/sqlserver.py
+-rw-r--r--   0        0        0     1853 2023-03-08 12:15:27.665913 awswrangler-3.0.0rc3/awswrangler/sts.py
+-rw-r--r--   0        0        0    28314 2023-03-08 15:59:02.560527 awswrangler-3.0.0rc3/awswrangler/timestream.py
+-rw-r--r--   0        0        0     8209 2023-03-08 12:15:27.667551 awswrangler-3.0.0rc3/awswrangler/typing.py
+-rw-r--r--   0        0        0     4454 2023-03-09 12:07:41.676456 awswrangler-3.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    24090 1970-01-01 00:00:00.000000 awswrangler-3.0.0rc3/setup.py
+-rw-r--r--   0        0        0    24270 1970-01-01 00:00:00.000000 awswrangler-3.0.0rc3/PKG-INFO
```

### Comparing `awswrangler-3.0.0rc2/LICENSE.txt` & `awswrangler-3.0.0rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/README.md` & `awswrangler-3.0.0rc3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/release-3.0.0rc2-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/release-3.0.0rc3-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Coverage](https://img.shields.io/badge/coverage-91%25-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
 
 | Source | Downloads | Installation Command |
 |--------|-----------|----------------------|
 | **[PyPi](https://pypi.org/project/awswrangler/)**  | [![PyPI Downloads](https://pepy.tech/badge/awswrangler)](https://pypi.org/project/awswrangler/) | `pip install awswrangler` |
 | **[Conda](https://anaconda.org/conda-forge/awswrangler)** | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/awswrangler.svg)](https://anaconda.org/conda-forge/awswrangler) | `conda install -c conda-forge awswrangler` |
 
-> ⚠️ **For platforms without PyArrow 3 support (e.g. [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr-cluster), [Glue PySpark Job](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs), MWAA):**<br>
-➡️ `pip install pyarrow==2 awswrangler`
+> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>
+➡️`pip install 'awswrangler[redshift]'`
 
 Powered By [<img src="https://arrow.apache.org/img/arrow.png" width="200">](https://arrow.apache.org/powered_by/)
 
 ## Table of contents
 
 - [Quick Start](#quick-start)
 - [At Scale](#at-scale)
@@ -41,16 +41,16 @@
 - [Logging](#logging)
 - [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-pandas)
 
 ## Quick Start
 
 Installation command: `pip install awswrangler`
 
-> ⚠️ **For platforms without PyArrow 3 support (e.g. [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr-cluster), [Glue PySpark Job](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs), MWAA):**<br>
-➡️`pip install pyarrow==2 awswrangler`
+> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>
+➡️`pip install 'awswrangler[redshift]'`
 
 ```py3
 import awswrangler as wr
 import pandas as pd
 from datetime import datetime
 
 df = pd.DataFrame({"id": [1, 2], "value": ["foo", "boo"]})
@@ -94,60 +94,75 @@
 SELECT time, measure_value::double, my_dimension
 FROM "sampleDB"."sampleTable" ORDER BY time DESC LIMIT 3
 """)
 
 ```
 
 ## At scale
-AWS SDK for pandas can also run your workflows at scale by leveraging [modin](https://modin.readthedocs.io/en/stable/) and [ray](https://www.ray.io/). Both projects aim to speed up data workloads (pandas workloads in particular in the case of modin) by distributing processing over a cluster of workers.
+AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
+
+The quickest way to get started is to use AWS Glue with Ray. Read our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/) to learn about it, then head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/release-3.0.0/tutorials) to discover even more features.
 
 ### Installation
 ```
-pip install "awswrangler[modin,ray]==3.0.0rc2"
+pip install "awswrangler[modin,ray]==3.0.0rc3"
 ```
 
 As a result existing scripts can run on significantly larger datasets with no code rewrite. Supported APIs are parallelized across cores on a single machine or across multiple nodes on a cluster in the cloud.
 
 ### Supported APIs
 
 <p align="center">
 
-| Service     | API                                                           | Implementation |
-|-------------------|:------------------------------------------------------------------------------------:|:---------------:|
-|  `S3`    | `read_parquet`                                               | ✅ |
-|    | `read_csv`                                               | ✅ |
-|    | `read_json`                                               | ✅ |
-|    | `read_fwf`                                               | ✅ |
-|    | `to_parquet`                                               | ✅ |
-|    | `to_csv`                                               | ✅ |
-|    | `to_json`                                               | ✅ |
-|    | `select_query`                                               | ✅ |
-|    | `delete`                                               | ✅ |
-|    | `copy`                                               | ✅ |
-|    | `wait`                                               | ✅ |
-|  `Redshift`    | `copy`                                               | ✅ |
-|    | `unload`                                               | ✅ |
-|  `Athena`    | `read_sql_query`                                               | ✅ |
-|  `LakeFormation`    | `read_sql_query`                                               | ✅ |
-|  `Timestream`    | `write`                                               | ✅ |
+| Service         | API                      | Implementation |
+|-----------------|--------------------------|:--------------:|
+| `S3`            | `read_parquet`           |       ✅        |
+|                 | `read_parquet_metadata`  |       ✅        |
+|                 | `read_parquet_table`     |       ✅        |
+|                 | `read_csv`               |       ✅        |
+|                 | `read_json`              |       ✅        |
+|                 | `read_fwf`               |       ✅        |
+|                 | `to_parquet`             |       ✅        |
+|                 | `to_csv`                 |       ✅        |
+|                 | `to_json`                |       ✅        |
+|                 | `select_query`           |       ✅        |
+|                 | `store_parquet_metadata` |       ✅        |
+|                 | `delete_objects`         |       ✅        |
+|                 | `describe_objects`       |       ✅        |
+|                 | `size_objects`           |       ✅        |
+|                 | `wait_objects_exist`     |       ✅        |
+|                 | `wait_objects_not_exist` |       ✅        |
+|                 | `merge_datasets`         |       ✅        |
+|                 | `copy_objects`           |       ✅        |
+| `Redshift`      | `copy`                   |       ✅        |
+|                 | `unload`                 |       ✅        |
+| `Athena`        | `read_sql_query`         |       ✅        |
+|                 | `read_sql_table`         |       ✅        |
+|                 | `describe_table`         |       ✅        |
+|                 | `get_query_results`      |       ✅        |
+|                 | `show_create_table`      |       ✅        |
+| `DynamoDB`      | `read_items`             |       ✅        |
+| `LakeFormation` | `read_sql_query`         |       ✅        |
+|                 | `read_sql_table`         |       ✅        |
+| `Timestream`    | `write`                  |       ✅        |
 </p>
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/what.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#from-source)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/what.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#from-source)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -174,39 +189,42 @@
   - [027 - Amazon Timestream 2](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/027%20-%20Amazon%20Timestream%202.ipynb)
   - [028 - Amazon DynamoDB](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/028%20-%20DynamoDB.ipynb)
   - [029 - S3 Select](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/029%20-%20S3%20Select.ipynb)
   - [030 - Data Api](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/030%20-%20Data%20Api.ipynb)
   - [031 - OpenSearch](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/031%20-%20OpenSearch.ipynb)
   - [032 - Lake Formation Governed Tables](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/032%20-%20Lake%20Formation%20Governed%20Tables.ipynb)
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
-  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0rc2/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
-  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0rc2/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#opensearch)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#global-configurations)
+  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
+  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
+  - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
+  - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
+  - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#opensearch)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#global-configurations)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

### Comparing `awswrangler-3.0.0rc2/THIRD_PARTY.txt` & `awswrangler-3.0.0rc3/THIRD_PARTY.txt`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/__init__.py` & `awswrangler-3.0.0rc3/awswrangler/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from awswrangler import (  # noqa
     athena,
     catalog,
     chime,
     cloudwatch,
     data_api,
+    data_quality,
     dynamodb,
     emr,
     exceptions,
     lakeformation,
     mysql,
     neptune,
     opensearch,
@@ -25,28 +26,30 @@
     quicksight,
     redshift,
     s3,
     secretsmanager,
     sqlserver,
     sts,
     timestream,
+    typing,
 )
 from awswrangler.__metadata__ import __description__, __license__, __title__, __version__  # noqa
 from awswrangler._config import config  # noqa
-from awswrangler._distributed import engine, memory_format  # noqa
+from awswrangler._distributed import EngineEnum, MemoryFormatEnum, engine, memory_format  # noqa
 
 engine.initialize()
 
 __all__ = [
     "athena",
     "catalog",
     "chime",
     "cloudwatch",
     "emr",
     "data_api",
+    "data_quality",
     "dynamodb",
     "exceptions",
     "opensearch",
     "oracle",
     "quicksight",
     "s3",
     "sts",
@@ -57,15 +60,18 @@
     "postgresql",
     "secretsmanager",
     "sqlserver",
     "config",
     "engine",
     "memory_format",
     "timestream",
+    "typing",
     "__description__",
     "__license__",
     "__title__",
     "__version__",
+    "EngineEnum",
+    "MemoryFormatEnum",
 ]
 
 
 _logging.getLogger("awswrangler").addHandler(_logging.NullHandler())
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/_arrow.py` & `awswrangler-3.0.0rc3/awswrangler/_arrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 def _extract_partitions_from_path(path_root: str, path: str) -> Dict[str, str]:
     path_root = path_root if path_root.endswith("/") else f"{path_root}/"
     if path_root not in path:
         raise Exception(f"Object {path} is not under the root path ({path_root}).")
     path_wo_filename: str = path.rpartition("/")[0] + "/"
     path_wo_prefix: str = path_wo_filename.replace(f"{path_root}/", "")
-    dirs: Tuple[str, ...] = tuple(x for x in path_wo_prefix.split("/") if (x != "") and (x.count("=") == 1))
+    dirs: Tuple[str, ...] = tuple(x for x in path_wo_prefix.split("/") if (x != "") and (x.count("=") > 0))
     if not dirs:
         return {}
-    values_tups = cast(Tuple[Tuple[str, str]], tuple(tuple(x.split("=")[:2]) for x in dirs))
+    values_tups = cast(Tuple[Tuple[str, str]], tuple(tuple(x.split("=", maxsplit=1)[:2]) for x in dirs))
     values_dics: Dict[str, str] = dict(values_tups)
     return values_dics
 
 
 def _add_table_partitions(
     table: pa.Table,
     path: str,
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/_config.py` & `awswrangler-3.0.0rc3/awswrangler/_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,91 @@
 """Configuration file for AWS SDK for pandas."""
 
 import inspect
 import logging
 import os
-from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Type, Union, cast
+from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Type, TypeVar, Union, cast
 
 import botocore.config
 import pandas as pd
 
 from awswrangler import exceptions
+from awswrangler.typing import AthenaCacheSettings
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-_ConfigValueType = Union[str, bool, int, botocore.config.Config, None]
+_ConfigValueType = Union[str, bool, int, float, botocore.config.Config, dict]
 
 
 class _ConfigArg(NamedTuple):
-    dtype: Type[Union[str, bool, int, botocore.config.Config]]
+    dtype: Type[_ConfigValueType]
     nullable: bool
     enforced: bool = False
     loaded: bool = False
     default: Optional[_ConfigValueType] = None
+    parent_parameter_key: Optional[str] = None
+    is_parent: bool = False
 
 
 # Please, also add any new argument as a property in the _Config class
 _CONFIG_ARGS: Dict[str, _ConfigArg] = {
     "catalog_id": _ConfigArg(dtype=str, nullable=True),
     "concurrent_partitioning": _ConfigArg(dtype=bool, nullable=False),
     "ctas_approach": _ConfigArg(dtype=bool, nullable=False),
     "database": _ConfigArg(dtype=str, nullable=True),
-    "max_cache_query_inspections": _ConfigArg(dtype=int, nullable=False),
-    "max_cache_seconds": _ConfigArg(dtype=int, nullable=False),
-    "max_remote_cache_entries": _ConfigArg(dtype=int, nullable=False),
-    "max_local_cache_entries": _ConfigArg(dtype=int, nullable=False),
+    "athena_cache_settings": _ConfigArg(dtype=dict, nullable=False, is_parent=True, loaded=True),
+    "max_cache_query_inspections": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
+    "max_cache_seconds": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
+    "max_remote_cache_entries": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
+    "max_local_cache_entries": _ConfigArg(dtype=int, nullable=False, parent_parameter_key="athena_cache_settings"),
+    "athena_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
+    "cloudwatch_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
+    "lakeformation_query_wait_polling_delay": _ConfigArg(dtype=float, nullable=False),
     "s3_block_size": _ConfigArg(dtype=int, nullable=False, enforced=True),
     "workgroup": _ConfigArg(dtype=str, nullable=False, enforced=True),
     "chunksize": _ConfigArg(dtype=int, nullable=False, enforced=True),
+    "suppress_warnings": _ConfigArg(dtype=bool, nullable=False, default=False, loaded=True),
     # Endpoints URLs
     "s3_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "athena_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "sts_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "glue_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "redshift_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "kms_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "emr_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "lakeformation_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "dynamodb_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     "secretsmanager_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
-    "timestream_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
+    "timestream_query_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
+    "timestream_write_endpoint_url": _ConfigArg(dtype=str, nullable=True, enforced=True, loaded=True),
     # Botocore config
     "botocore_config": _ConfigArg(dtype=botocore.config.Config, nullable=True),
     "verify": _ConfigArg(dtype=str, nullable=True, loaded=True),
     # Distributed
     "address": _ConfigArg(dtype=str, nullable=True),
     "redis_password": _ConfigArg(dtype=str, nullable=True),
     "ignore_reinit_error": _ConfigArg(dtype=bool, nullable=True),
     "include_dashboard": _ConfigArg(dtype=bool, nullable=True),
+    "configure_logging": _ConfigArg(dtype=bool, nullable=True),
     "log_to_driver": _ConfigArg(dtype=bool, nullable=True),
+    "logging_level": _ConfigArg(dtype=int, nullable=True),
     "object_store_memory": _ConfigArg(dtype=int, nullable=True),
     "cpu_count": _ConfigArg(dtype=int, nullable=True),
     "gpu_count": _ConfigArg(dtype=int, nullable=True),
 }
 
 
 class _Config:  # pylint: disable=too-many-instance-attributes,too-many-public-methods
     """AWS Wrangler's Configuration class."""
 
     def __init__(self) -> None:
-        self._loaded_values: Dict[str, _ConfigValueType] = {}
-        name: str
+        self._loaded_values: Dict[str, Optional[_ConfigValueType]] = {}
+        self.botocore_config = None
+
         for name in _CONFIG_ARGS:
             self._load_config(name=name)
 
     def reset(self, item: Optional[str] = None) -> None:
         """Reset one or all (if None is received) configuration values.
 
         Parameters
@@ -111,82 +123,118 @@
         --------
         >>> import awswrangler as wr
         >>> wr.config.to_pandas()
 
         """
         args: List[Dict[str, Any]] = []
         for k, v in _CONFIG_ARGS.items():
+            if v.is_parent:
+                continue
+
             arg: Dict[str, Any] = {
                 "name": k,
-                "Env. Variable": f"WR_{k.upper()}",
+                "Env.Variable": f"WR_{k.upper()}",
                 "type": v.dtype,
                 "nullable": v.nullable,
                 "enforced": v.enforced,
+                "parent_parameter_name": v.parent_parameter_key,
             }
             if k in self._loaded_values:
                 arg["configured"] = True
                 arg["value"] = self._loaded_values[k]
             else:
                 arg["configured"] = False
                 arg["value"] = None
             args.append(arg)
         return pd.DataFrame(args)
 
-    def _load_config(self, name: str) -> bool:
-        loaded_config: bool = False
+    def _load_config(self, name: str) -> None:
+        if _CONFIG_ARGS[name].is_parent:
+            if self._loaded_values.get(name) is None:
+                self._set_config_value(key=name, value={})
+            return
+
         if _CONFIG_ARGS[name].loaded:
             self._set_config_value(key=name, value=_CONFIG_ARGS[name].default)
-            loaded_config = True
+
         env_var: Optional[str] = os.getenv(f"WR_{name.upper()}")
         if env_var is not None:
             self._set_config_value(key=name, value=env_var)
-            loaded_config = True
-        return loaded_config
 
     def _set_config_value(self, key: str, value: Any) -> None:
         if key not in _CONFIG_ARGS:
             raise exceptions.InvalidArgumentValue(
                 f"{key} is not a valid configuration. Please use: {list(_CONFIG_ARGS.keys())}"
             )
-        value_casted: _ConfigValueType = self._apply_type(
-            name=key, value=value, dtype=_CONFIG_ARGS[key].dtype, nullable=_CONFIG_ARGS[key].nullable
+        value_casted: Optional[_ConfigValueType] = self._apply_type(
+            name=key,
+            value=value,
+            dtype=_CONFIG_ARGS[key].dtype,
+            nullable=_CONFIG_ARGS[key].nullable,
         )
-        self._loaded_values[key] = value_casted
 
-    def __getitem__(self, item: str) -> _ConfigValueType:
-        if item not in self._loaded_values:
+        parent_key = _CONFIG_ARGS[key].parent_parameter_key
+        if parent_key:
+            self._loaded_values[parent_key][key] = value_casted  # type: ignore[index]
+        else:
+            self._loaded_values[key] = value_casted
+
+    def __getitem__(self, item: str) -> Optional[_ConfigValueType]:
+        if issubclass(_CONFIG_ARGS[item].dtype, dict):
+            return self._loaded_values[item]
+
+        loaded_values: Dict[str, Optional[_ConfigValueType]]
+        parent_key = _CONFIG_ARGS[item].parent_parameter_key
+        if parent_key:
+            loaded_values = self[parent_key]  # type: ignore[assignment]
+        else:
+            loaded_values = self._loaded_values
+
+        if item not in loaded_values:
             raise AttributeError(f"{item} not configured yet.")
-        return self._loaded_values[item]
+
+        return loaded_values[item]
 
     def _reset_item(self, item: str) -> None:
-        if item in self._loaded_values:
-            if _CONFIG_ARGS[item].loaded:
-                self._loaded_values[item] = _CONFIG_ARGS[item].default
+        config_arg = _CONFIG_ARGS[item]
+        loaded_values: Dict[str, Optional[_ConfigValueType]]
+
+        if config_arg.parent_parameter_key:
+            loaded_values = self[config_arg.parent_parameter_key]  # type: ignore[assignment]
+        else:
+            loaded_values = self._loaded_values
+
+        if item in loaded_values:
+            if config_arg.is_parent:
+                loaded_values[item] = {}
+            elif config_arg.loaded:
+                loaded_values[item] = config_arg.default
             else:
-                del self._loaded_values[item]
+                del loaded_values[item]
+
         self._load_config(name=item)
 
     def _repr_html_(self) -> Any:
         return self.to_pandas().to_html()
 
     @staticmethod
-    def _apply_type(name: str, value: Any, dtype: Type[Union[str, bool, int]], nullable: bool) -> _ConfigValueType:
+    def _apply_type(name: str, value: Any, dtype: Type[_ConfigValueType], nullable: bool) -> Optional[_ConfigValueType]:
         if _Config._is_null(value=value):
             if nullable is True:
                 return None
             raise exceptions.InvalidArgumentValue(
                 f"{name} configuration does not accept a null value. Please pass {dtype}."
             )
         try:
             return dtype(value) if isinstance(value, dtype) is False else value
         except ValueError as ex:
             raise exceptions.InvalidConfiguration(f"Config {name} must receive a {dtype} value.") from ex
 
     @staticmethod
-    def _is_null(value: _ConfigValueType) -> bool:
+    def _is_null(value: Optional[_ConfigValueType]) -> bool:
         if value is None:
             return True
         if isinstance(value, str) is True:
             value = cast(str, value)
             if value.lower() in ("none", "null", "nil"):
                 return True
         return False
@@ -224,14 +272,19 @@
         return cast(Optional[str], self["database"])
 
     @database.setter
     def database(self, value: Optional[str]) -> None:
         self._set_config_value(key="database", value=value)
 
     @property
+    def athena_cache_settings(self) -> AthenaCacheSettings:
+        """Property athena_cache_settings."""
+        return cast(AthenaCacheSettings, self["athena_cache_settings"])
+
+    @property
     def max_cache_query_inspections(self) -> int:
         """Property max_cache_query_inspections."""
         return cast(int, self["max_cache_query_inspections"])
 
     @max_cache_query_inspections.setter
     def max_cache_query_inspections(self, value: int) -> None:
         self._set_config_value(key="max_cache_query_inspections", value=value)
@@ -271,14 +324,41 @@
         return cast(int, self["max_remote_cache_entries"])
 
     @max_remote_cache_entries.setter
     def max_remote_cache_entries(self, value: int) -> None:
         self._set_config_value(key="max_remote_cache_entries", value=value)
 
     @property
+    def athena_query_wait_polling_delay(self) -> float:
+        """Property athena_query_wait_polling_delay."""
+        return cast(float, self["athena_query_wait_polling_delay"])
+
+    @athena_query_wait_polling_delay.setter
+    def athena_query_wait_polling_delay(self, value: float) -> None:
+        self._set_config_value(key="athena_query_wait_polling_delay", value=value)
+
+    @property
+    def cloudwatch_query_wait_polling_delay(self) -> float:
+        """Property cloudwatch_query_wait_polling_delay."""
+        return cast(float, self["cloudwatch_query_wait_polling_delay"])
+
+    @cloudwatch_query_wait_polling_delay.setter
+    def cloudwatch_query_wait_polling_delay(self, value: float) -> None:
+        self._set_config_value(key="cloudwatch_query_wait_polling_delay", value=value)
+
+    @property
+    def lakeformation_query_wait_polling_delay(self) -> float:
+        """Property lakeformation_query_wait_polling_delay."""
+        return cast(float, self["lakeformation_query_wait_polling_delay"])
+
+    @lakeformation_query_wait_polling_delay.setter
+    def lakeformation_query_wait_polling_delay(self, value: float) -> None:
+        self._set_config_value(key="lakeformation_query_wait_polling_delay", value=value)
+
+    @property
     def s3_block_size(self) -> int:
         """Property s3_block_size."""
         return cast(int, self["s3_block_size"])
 
     @s3_block_size.setter
     def s3_block_size(self, value: int) -> None:
         self._set_config_value(key="s3_block_size", value=value)
@@ -298,14 +378,23 @@
         return cast(int, self["chunksize"])
 
     @chunksize.setter
     def chunksize(self, value: int) -> None:
         self._set_config_value(key="chunksize", value=value)
 
     @property
+    def suppress_warnings(self) -> bool:
+        """Property suppress_warnings."""
+        return cast(bool, self["suppress_warnings"])
+
+    @suppress_warnings.setter
+    def suppress_warnings(self, value: bool) -> None:
+        self._set_config_value(key="suppress_warnings", value=value)
+
+    @property
     def s3_endpoint_url(self) -> Optional[str]:
         """Property s3_endpoint_url."""
         return cast(Optional[str], self["s3_endpoint_url"])
 
     @s3_endpoint_url.setter
     def s3_endpoint_url(self, value: Optional[str]) -> None:
         self._set_config_value(key="s3_endpoint_url", value=value)
@@ -388,24 +477,43 @@
         return cast(Optional[str], self["secretsmanager_endpoint_url"])
 
     @secretsmanager_endpoint_url.setter
     def secretsmanager_endpoint_url(self, value: Optional[str]) -> None:
         self._set_config_value(key="secretsmanager_endpoint_url", value=value)
 
     @property
-    def timestream_endpoint_url(self) -> Optional[str]:
-        """Property timestream_endpoint_url."""
-        return cast(Optional[str], self["timestream_endpoint_url"])
+    def timestream_query_endpoint_url(self) -> Optional[str]:
+        """
+        Property timestream_query_endpoint_url.
+
+        Before setting this endpoint, consult the documentation for DescribeEndpoints.
+        https://docs.aws.amazon.com/timestream/latest/developerguide/API_DescribeEndpoints.html
+        """
+        return cast(Optional[str], self["timestream_query_endpoint_url"])
+
+    @timestream_query_endpoint_url.setter
+    def timestream_query_endpoint_url(self, value: Optional[str]) -> None:
+        self._set_config_value(key="timestream_query_endpoint_url", value=value)
+
+    @property
+    def timestream_write_endpoint_url(self) -> Optional[str]:
+        """
+        Property timestream_write_endpoint_url.
 
-    @timestream_endpoint_url.setter
-    def timestream_endpoint_url(self, value: Optional[str]) -> None:
-        self._set_config_value(key="timestream_endpoint_url", value=value)
+        Before setting this endpoint, consult the documentation for DescribeEndpoints.
+        https://docs.aws.amazon.com/timestream/latest/developerguide/API_DescribeEndpoints.html
+        """
+        return cast(Optional[str], self["timestream_write_endpoint_url"])
+
+    @timestream_write_endpoint_url.setter
+    def timestream_write_endpoint_url(self, value: Optional[str]) -> None:
+        self._set_config_value(key="timestream_write_endpoint_url", value=value)
 
     @property
-    def botocore_config(self) -> botocore.config.Config:
+    def botocore_config(self) -> Optional[botocore.config.Config]:
         """Property botocore_config."""
         return cast(Optional[botocore.config.Config], self["botocore_config"])
 
     @botocore_config.setter
     def botocore_config(self, value: Optional[botocore.config.Config]) -> None:
         self._set_config_value(key="botocore_config", value=value)
 
@@ -451,23 +559,41 @@
         return cast(Optional[str], self["redis_password"])
 
     @redis_password.setter
     def redis_password(self, value: Optional[str]) -> None:
         self._set_config_value(key="redis_password", value=value)
 
     @property
+    def configure_logging(self) -> Optional[bool]:
+        """Property configure_logging."""
+        return cast(Optional[bool], self["configure_logging"])
+
+    @configure_logging.setter
+    def configure_logging(self, value: Optional[bool]) -> None:
+        self._set_config_value(key="configure_logging", value=value)
+
+    @property
     def log_to_driver(self) -> Optional[bool]:
         """Property log_to_driver."""
         return cast(Optional[bool], self["log_to_driver"])
 
     @log_to_driver.setter
     def log_to_driver(self, value: Optional[bool]) -> None:
         self._set_config_value(key="log_to_driver", value=value)
 
     @property
+    def logging_level(self) -> int:
+        """Property logging_level."""
+        return cast(int, self["logging_level"])
+
+    @logging_level.setter
+    def logging_level(self, value: int) -> None:
+        self._set_config_value(key="logging_level", value=value)
+
+    @property
     def object_store_memory(self) -> int:
         """Property object_store_memory."""
         return cast(int, self["object_store_memory"])
 
     @object_store_memory.setter
     def object_store_memory(self, value: int) -> None:
         self._set_config_value(key="object_store_memory", value=value)
@@ -515,40 +641,58 @@
         "021%20-%20Global%20Configurations.ipynb>`_"
         " for details.\n"
     )
     insertion: str = header + args_block + footer + "\n\n"
     return _insert_str(text=doc, token="\n    Parameters", insert=insertion)
 
 
-def apply_configs(function: Callable[..., Any]) -> Callable[..., Any]:
+def _assign_args_value(args: Dict[str, Any], name: str, value: Any) -> None:
+    if _CONFIG_ARGS[name].is_parent:
+        if name not in args:
+            args[name] = {}
+
+        nested_args = cast(Dict[str, Any], value)
+        for nested_arg_name, nested_arg_value in nested_args.items():
+            _assign_args_value(args[name], nested_arg_name, nested_arg_value)
+        return
+
+    if name not in args:
+        _logger.debug("Applying default config argument %s with value %s.", name, value)
+        args[name] = value
+
+    elif _CONFIG_ARGS[name].enforced is True:
+        _logger.debug("Applying ENFORCED config argument %s with value %s.", name, value)
+        args[name] = value
+
+
+FunctionType = TypeVar("FunctionType", bound=Callable[..., Any])
+
+
+def apply_configs(function: FunctionType) -> FunctionType:
     """Decorate some function with configs."""
     signature = inspect.signature(function)
     args_names: Tuple[str, ...] = tuple(signature.parameters.keys())
     available_configs: Tuple[str, ...] = tuple(x for x in _CONFIG_ARGS if x in args_names)
 
     def wrapper(*args_raw: Any, **kwargs: Any) -> Any:
         args: Dict[str, Any] = signature.bind_partial(*args_raw, **kwargs).arguments
         for name in available_configs:
             if hasattr(config, name) is True:
-                value: _ConfigValueType = config[name]
-                if name not in args:
-                    _logger.debug("Applying default config argument %s with value %s.", name, value)
-                    args[name] = value
-                elif _CONFIG_ARGS[name].enforced is True:
-                    _logger.debug("Applying ENFORCED config argument %s with value %s.", name, value)
-                    args[name] = value
+                value = config[name]
+                _assign_args_value(args, name, value)
+
         for name, param in signature.parameters.items():
             if param.kind == param.VAR_KEYWORD and name in args:
                 if isinstance(args[name], dict) is False:
                     raise RuntimeError(f"Argument {name} ({args[name]}) is a non dictionary keyword argument.")
                 keywords: Dict[str, Any] = args[name]
                 del args[name]
                 args = {**args, **keywords}
         return function(**args)
 
     wrapper.__doc__ = _inject_config_doc(doc=function.__doc__, available_configs=available_configs)
     wrapper.__name__ = function.__name__
     wrapper.__setattr__("__signature__", signature)  # pylint: disable=no-member
-    return wrapper
+    return wrapper  # type: ignore[return-value]
 
 
 config: _Config = _Config()
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/_data_types.py` & `awswrangler-3.0.0rc3/awswrangler/_data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     if pa.types.is_decimal(dtype):
         return f"decimal({dtype.precision},{dtype.scale})"
     if pa.types.is_list(dtype):
         return f"array<{pyarrow2athena(dtype=dtype.value_type)}>"
     if pa.types.is_struct(dtype):
         return f"struct<{','.join([f'{f.name}:{pyarrow2athena(dtype=f.type)}' for f in dtype])}>"
     if pa.types.is_map(dtype):
-        return f"map<{pyarrow2athena(dtype=dtype.key_type)}, {pyarrow2athena(dtype=dtype.item_type)}>"
+        return f"map<{pyarrow2athena(dtype=dtype.key_type)},{pyarrow2athena(dtype=dtype.item_type)}>"
     if dtype == pa.null():
         if ignore_null:
             return ""
         raise exceptions.UndetectedType("We can not infer the data type from an entire null object column")
     raise exceptions.UnsupportedType(f"Unsupported Pyarrow type: {dtype}")
 
 
@@ -85,14 +85,16 @@
         return "BOOL"
     if pa.types.is_string(dtype):
         return string_type
     if pa.types.is_timestamp(dtype):
         return "TIMESTAMP"
     if pa.types.is_date(dtype):
         return "DATE"
+    if pa.types.is_time(dtype):
+        return "TIME"
     if pa.types.is_decimal(dtype):
         return f"DECIMAL({dtype.precision},{dtype.scale})"
     if pa.types.is_dictionary(dtype):
         return pyarrow2redshift(dtype=dtype.value_type, string_type=string_type)
     if pa.types.is_list(dtype) or pa.types.is_struct(dtype) or pa.types.is_map(dtype):
         return "SUPER"
     raise exceptions.UnsupportedType(f"Unsupported Redshift type: {dtype}")
@@ -260,14 +262,20 @@
         return "DOUBLE"
     if pa.types.is_float64(dtype):
         return "DOUBLE"
     if pa.types.is_boolean(dtype):
         return "BOOLEAN"
     if pa.types.is_string(dtype):
         return "VARCHAR"
+    if pa.types.is_date(dtype):
+        return "DATE"
+    if pa.types.is_time(dtype):
+        return "TIME"
+    if pa.types.is_timestamp(dtype):
+        return "TIMESTAMP"
     raise exceptions.UnsupportedType(f"Unsupported Amazon Timestream measure type: {dtype}")
 
 
 def _split_fields(s: str) -> Iterator[str]:
     counter: int = 0
     last: int = 0
     for i, x in enumerate(s):
@@ -307,15 +315,15 @@
         return pa.int64()
     if dtype in ("float", "real"):
         return pa.float32()
     if dtype == "double":
         return pa.float64()
     if dtype == "boolean":
         return pa.bool_()
-    if (dtype == "string") or dtype.startswith("char") or dtype.startswith("varchar"):
+    if (dtype in ("string", "uuid")) or dtype.startswith("char") or dtype.startswith("varchar"):
         return pa.string()
     if dtype == "timestamp":
         return pa.timestamp(unit="ns")
     if dtype == "date":
         return pa.date32()
     if dtype in ("binary" or "varbinary"):
         return pa.binary()
@@ -579,15 +587,15 @@
     raise ex
 
 
 def process_not_inferred_array(ex: pa.ArrowInvalid, values: Any) -> pa.Array:
     """Infer `pyarrow.array` from PyArrow inference exception."""
     dtype = process_not_inferred_dtype(ex=ex)
     if dtype == pa.string():
-        array: pa.Array = pa.array(obj=[str(x) for x in values], type=dtype, safe=True)
+        array: pa.Array = pa.array(obj=[str(x) if x is not None else None for x in values], type=dtype, safe=True)
     else:
         raise ex
     return array
 
 
 def athena_types_from_pandas(
     df: pd.DataFrame, index: bool, dtype: Optional[Dict[str, str]] = None, index_left: bool = False
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/_databases.py` & `awswrangler-3.0.0rc3/awswrangler/_databases.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Databases Utilities."""
 
 import importlib.util
 import logging
 import ssl
-from typing import Any, Dict, Generator, Iterator, List, NamedTuple, Optional, Tuple, Union, cast
+from typing import Any, Dict, Generator, Iterator, List, NamedTuple, Optional, Tuple, Union, cast, overload
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 
 from awswrangler import _data_types, _utils, exceptions, oracle, secretsmanager
 from awswrangler.catalog import get_connection
@@ -26,17 +26,17 @@
     host: str
     port: int
     database: str
     ssl_context: Optional[ssl.SSLContext]
 
 
 def _get_dbname(cluster_id: str, boto3_session: Optional[boto3.Session] = None) -> str:
-    client_redshift: boto3.client = _utils.client(service_name="redshift", session=boto3_session)
-    res: Dict[str, Any] = client_redshift.describe_clusters(ClusterIdentifier=cluster_id)["Clusters"][0]
-    return cast(str, res["DBName"])
+    client_redshift = _utils.client(service_name="redshift", session=boto3_session)
+    res = client_redshift.describe_clusters(ClusterIdentifier=cluster_id)["Clusters"][0]
+    return res["DBName"]
 
 
 def _get_connection_attributes_from_catalog(
     connection: str, catalog_id: Optional[str], dbname: Optional[str], boto3_session: Optional[boto3.Session]
 ) -> ConnectionAttributes:
     details: Dict[str, Any] = get_connection(name=connection, catalog_id=catalog_id, boto3_session=boto3_session)[
         "ConnectionProperties"
@@ -48,18 +48,18 @@
     port, database = details["JDBC_CONNECTION_URL"].split(":")[-1].split(database_sep)
     ssl_context: Optional[ssl.SSLContext] = None
     if details.get("JDBC_ENFORCE_SSL") == "true":
         ssl_cert_path: Optional[str] = details.get("CUSTOM_JDBC_CERT")
         ssl_cadata: Optional[str] = None
         if ssl_cert_path:
             bucket_name, key_path = _utils.parse_path(ssl_cert_path)
-            client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
+            client_s3 = _utils.client(service_name="s3", session=boto3_session)
             try:
                 ssl_cadata = client_s3.get_object(Bucket=bucket_name, Key=key_path)["Body"].read().decode("utf-8")
-            except client_s3.exception.NoSuchKey:
+            except client_s3.exceptions.NoSuchKey:
                 raise exceptions.NoFilesFound(  # pylint: disable=raise-missing-from
                     f"No CA certificate found at {ssl_cert_path}."
                 )
         ssl_context = ssl.create_default_context(cadata=ssl_cadata)
 
     return ConnectionAttributes(
         kind=details["JDBC_CONNECTION_URL"].split(":")[1].lower(),
@@ -238,14 +238,58 @@
             index=index_col,
             dtype=dtype,
             safe=safe,
             timestamp_as_object=timestamp_as_object,
         )
 
 
+@overload
+def read_sql_query(
+    sql: str,
+    con: Any,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: Any,
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: Any,
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
 def read_sql_query(
     sql: str,
     con: Any,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/_distributed.py` & `awswrangler-3.0.0rc3/awswrangler/_distributed.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # pylint: disable=import-outside-toplevel
 
 import importlib.util
 from collections import defaultdict
 from enum import Enum, unique
 from functools import wraps
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, TypeVar
 
 
 @unique
 class EngineEnum(Enum):
     """Execution engine enum."""
 
     RAY = "ray"
@@ -21,100 +21,114 @@
 class MemoryFormatEnum(Enum):
     """Memory format enum."""
 
     MODIN = "modin"
     PANDAS = "pandas"
 
 
+FunctionType = TypeVar("FunctionType", bound=Callable[..., Any])
+
+
 class Engine:
     """Execution engine configuration class."""
 
-    _enum: Optional[Enum] = None
+    _engine: Optional[EngineEnum] = None
+    _initialized_engine: Optional[EngineEnum] = None
     _registry: Dict[str, Dict[str, Callable[..., Any]]] = defaultdict(dict)
 
     @classmethod
-    def get_installed(cls) -> Enum:
+    def get_installed(cls) -> EngineEnum:
         """Get the installed distribution engine.
 
         This is the engine that can be imported.
 
         Returns
         -------
         EngineEnum
             The distribution engine installed.
         """
         if importlib.util.find_spec("ray"):
             return EngineEnum.RAY
         return EngineEnum.PYTHON
 
     @classmethod
-    def get(cls) -> Enum:
+    def get(cls) -> EngineEnum:
         """Get the configured distribution engine.
 
         This is the engine currently configured. If None, the installed engine is returned.
 
         Returns
         -------
         str
             The distribution engine configured.
         """
-        return cls._enum if cls._enum else cls.get_installed()
+        return cls._engine if cls._engine else cls.get_installed()
 
     @classmethod
     def set(cls, name: str) -> None:
         """Set the distribution engine."""
-        cls._enum = EngineEnum._member_map_[name.upper()]  # pylint: disable=protected-access,no-member
+        cls._engine = EngineEnum._member_map_[  # type: ignore[assignment]  # pylint: disable=protected-access,no-member
+            name.upper()
+        ]
 
     @classmethod
-    def dispatch_func(cls, source_func: Callable[..., Any], value: Optional[Any] = None) -> Callable[..., Any]:
+    def dispatch_func(cls, source_func: FunctionType, value: Optional[Any] = None) -> FunctionType:
         """Dispatch a func based on value or the distribution engine and the source function."""
         try:
-            return cls._registry[value or cls.get().value][source_func.__name__]
+            return cls._registry[value or cls.get().value][source_func.__name__]  # type: ignore[return-value]
         except KeyError:
             return getattr(source_func, "_source_func", source_func)
 
     @classmethod
     def register_func(cls, source_func: Callable[..., Any], destination_func: Callable[..., Any]) -> Callable[..., Any]:
         """Register a func based on the distribution engine and source function."""
         cls._registry[cls.get().value][source_func.__name__] = destination_func
         return destination_func
 
     @classmethod
-    def dispatch_on_engine(cls, func: Callable[..., Any]) -> Callable[..., Any]:
+    def dispatch_on_engine(cls, func: FunctionType) -> FunctionType:
         """Dispatch on engine function decorator."""
 
         @wraps(func)
         def wrapper(*args: Any, **kw: Dict[str, Any]) -> Any:
             return cls.dispatch_func(func)(*args, **kw)
 
         # Save the original function
-        wrapper._source_func = func  # type: ignore  # pylint: disable=protected-access
-        return wrapper
+        wrapper._source_func = func  # type: ignore[attr-defined]  # pylint: disable=protected-access
+        return wrapper  # type: ignore[return-value]
 
     @classmethod
     def register(cls, name: Optional[str] = None) -> None:
         """Register the distribution engine dispatch methods."""
-        engine_name = cls.get_installed().value if not name else name
+        engine_name = name or cls.get_installed().value
         cls.set(engine_name)
         cls._registry.clear()
 
         if engine_name == EngineEnum.RAY.value:
             from awswrangler.distributed.ray._register import register_ray
 
             register_ray()
 
     @classmethod
     def initialize(cls, name: Optional[str] = None) -> None:
         """Initialize the distribution engine."""
-        engine_name = cls.get_installed().value if not name else name
+        engine_name = name or cls.get_installed().value
         if engine_name == EngineEnum.RAY.value:
             from awswrangler.distributed.ray import initialize_ray
 
             initialize_ray()
         cls.register(engine_name)
+        cls._initialized_engine = cls.get()
+
+    @classmethod
+    def is_initialized(cls, name: Optional[str] = None) -> bool:
+        """Check if the distribution engine is initialized."""
+        engine_name = name or cls.get_installed().value
+
+        return False if not cls._initialized_engine else cls._initialized_engine.value == engine_name
 
 
 class MemoryFormat:
     """Memory format configuration class."""
 
     _enum: Optional[Enum] = None
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/_sql_formatter.py` & `awswrangler-3.0.0rc3/awswrangler/_sql_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,31 +125,31 @@
             if not isinstance(key, key_type):
                 raise TypeError("All Map key elements must be the same type.")
 
         map_values = list(self.data.values())
         return f"MAP(ARRAY [{', '.join(map(str, map_keys))}], ARRAY [{', '.join(map(str, map_values))}])"
 
 
-_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore
+_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore[valid-type]
     bool: _BooleanType,
     str: _StringType,
     int: _IntegerType,
     datetime.datetime: _TimestampType,
     datetime.date: _DateType,
     decimal.Decimal: _DecimalType,
     float: _FloatType,
 }
 
-_ARRAY_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore
+_ARRAY_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore[valid-type]
     list: _ArrayType,
     tuple: _ArrayType,
     set: _ArrayType,
 }
 
-_MAP_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore
+_MAP_FORMATS: Dict[Type[Any], Type[_AbstractType[_PythonType]]] = {  # type: ignore[valid-type]
     dict: _MapType,
 }
 
 
 def _create_abstract_type(
     data: _PythonType,
     engine: _EngineType,
@@ -196,15 +196,15 @@
 
 def _process_sql_params(sql: str, params: Optional[Dict[str, Any]], engine: _EngineType = _EngineType.PRESTO) -> str:
     if params is None:
         params = {}
 
     processed_params = _format_parameters(params, engine=engine)
 
-    def replace(match: re.Match) -> str:  # type: ignore
+    def replace(match: re.Match) -> str:  # type: ignore[type-arg]
         key = match.group(1)
 
         if key not in processed_params:
             # do not replace anything if the parameter is not provided
             return str(match.group(0))
 
         return str(processed_params[key])
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/_utils.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,448 +1,419 @@
-"""Internal (private) Utilities Module."""
+"""Amazon S3 List Module (PRIVATE)."""
 
-import copy
-import itertools
+import datetime
+import fnmatch
 import logging
-import math
-import os
-import random
-import time
-from concurrent.futures import FIRST_COMPLETED, Future, wait
-from typing import Any, Callable, Dict, Generator, List, Optional, Sequence, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Sequence, Union
 
 import boto3
-import botocore.config
-import numpy as np
-import pandas as pd
-import pyarrow as pa
-
-from awswrangler import _config, exceptions
-from awswrangler.__metadata__ import __version__
-from awswrangler._arrow import _table_to_df
-from awswrangler._config import apply_configs
-from awswrangler._distributed import engine
-
-_logger: logging.Logger = logging.getLogger(__name__)
-
-Boto3PrimitivesType = Dict[str, Optional[str]]
+import botocore.exceptions
 
+from awswrangler import _utils, exceptions
+from awswrangler._distributed import engine
+from awswrangler.s3 import _fs
 
-def ensure_session(session: Union[None, boto3.Session, Boto3PrimitivesType] = None) -> boto3.Session:
-    """Ensure that a valid boto3.Session will be returned."""
-    if isinstance(session, dict):  # Primitives received
-        return boto3_from_primitives(primitives=session)
-    if session is not None:
-        return session
-    # Ensure the boto3's default session is used so that its parameters can be
-    # set via boto3.setup_default_session()
-    if boto3.DEFAULT_SESSION is not None:
-        return boto3.DEFAULT_SESSION
-    return boto3.Session()
-
-
-def boto3_to_primitives(boto3_session: Optional[boto3.Session] = None) -> Boto3PrimitivesType:
-    """Convert Boto3 Session to Python primitives."""
-    _boto3_session: boto3.Session = ensure_session(session=boto3_session)
-    credentials = _boto3_session.get_credentials()
-    return {
-        "aws_access_key_id": getattr(credentials, "access_key", None),
-        "aws_secret_access_key": getattr(credentials, "secret_key", None),
-        "aws_session_token": getattr(credentials, "token", None),
-        "region_name": _boto3_session.region_name,
-        "profile_name": _boto3_session.profile_name,
-    }
-
-
-def boto3_from_primitives(primitives: Optional[Boto3PrimitivesType] = None) -> boto3.Session:
-    """Convert Python primitives to Boto3 Session."""
-    if primitives is None:
-        return ensure_session()
-    _primitives: Boto3PrimitivesType = copy.deepcopy(primitives)
-    profile_name: Optional[str] = _primitives.get("profile_name", None)
-    _primitives["profile_name"] = None if profile_name in (None, "default") else profile_name
-    args: Dict[str, str] = {k: v for k, v in _primitives.items() if v is not None}
-    return boto3.Session(**args)
-
-
-def default_botocore_config() -> botocore.config.Config:
-    """Botocore configuration."""
-    retries_config: Dict[str, Union[str, int]] = {
-        "max_attempts": int(os.getenv("AWS_MAX_ATTEMPTS", "5")),
-    }
-    mode: Optional[str] = os.getenv("AWS_RETRY_MODE")
-    if mode:
-        retries_config["mode"] = mode
-    return botocore.config.Config(
-        retries=retries_config,
-        connect_timeout=10,
-        max_pool_connections=10,
-        user_agent_extra=f"awswrangler/{__version__}",
-    )
-
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
 
-def _get_endpoint_url(service_name: str) -> Optional[str]:
-    endpoint_url: Optional[str] = None
-    if service_name == "s3" and _config.config.s3_endpoint_url is not None:
-        endpoint_url = _config.config.s3_endpoint_url
-    elif service_name == "athena" and _config.config.athena_endpoint_url is not None:
-        endpoint_url = _config.config.athena_endpoint_url
-    elif service_name == "sts" and _config.config.sts_endpoint_url is not None:
-        endpoint_url = _config.config.sts_endpoint_url
-    elif service_name == "glue" and _config.config.glue_endpoint_url is not None:
-        endpoint_url = _config.config.glue_endpoint_url
-    elif service_name == "redshift" and _config.config.redshift_endpoint_url is not None:
-        endpoint_url = _config.config.redshift_endpoint_url
-    elif service_name == "kms" and _config.config.kms_endpoint_url is not None:
-        endpoint_url = _config.config.kms_endpoint_url
-    elif service_name == "emr" and _config.config.emr_endpoint_url is not None:
-        endpoint_url = _config.config.emr_endpoint_url
-    elif service_name == "lakeformation" and _config.config.lakeformation_endpoint_url is not None:
-        endpoint_url = _config.config.lakeformation_endpoint_url
-    elif service_name == "dynamodb" and _config.config.dynamodb_endpoint_url is not None:
-        endpoint_url = _config.config.dynamodb_endpoint_url
-    elif service_name == "secretsmanager" and _config.config.secretsmanager_endpoint_url is not None:
-        endpoint_url = _config.config.secretsmanager_endpoint_url
-    elif service_name == "timestream" and _config.config.timestream_endpoint_url is not None:
-        endpoint_url = _config.config.timestream_endpoint_url
-    return endpoint_url
-
-
-@apply_configs
-def client(
-    service_name: str,
-    session: Optional[boto3.Session] = None,
-    botocore_config: Optional[botocore.config.Config] = None,
-    verify: Optional[Union[str, bool]] = None,
-) -> boto3.client:
-    """Create a valid boto3.client."""
-    endpoint_url: Optional[str] = _get_endpoint_url(service_name=service_name)
-    return ensure_session(session=session).client(
-        service_name=service_name,
-        endpoint_url=endpoint_url,
-        use_ssl=True,
-        config=botocore_config or default_botocore_config(),
-        verify=verify or _config.config.verify,
-    )
+_logger: logging.Logger = logging.getLogger(__name__)
 
 
-@apply_configs
-def resource(
-    service_name: str,
-    session: Optional[boto3.Session] = None,
-    botocore_config: Optional[botocore.config.Config] = None,
-    verify: Optional[Union[str, bool]] = None,
-) -> boto3.resource:
-    """Create a valid boto3.resource."""
-    endpoint_url: Optional[str] = _get_endpoint_url(service_name=service_name)
-    return ensure_session(session=session).resource(
-        service_name=service_name,
-        endpoint_url=endpoint_url,
-        use_ssl=True,
-        verify=verify,
-        config=default_botocore_config() if botocore_config is None else botocore_config,
+def _path2list(
+    path: Union[str, Sequence[str]],
+    s3_client: "S3Client",
+    s3_additional_kwargs: Optional[Dict[str, Any]],
+    last_modified_begin: Optional[datetime.datetime] = None,
+    last_modified_end: Optional[datetime.datetime] = None,
+    suffix: Union[str, List[str], None] = None,
+    ignore_suffix: Union[str, List[str], None] = None,
+    ignore_empty: bool = False,
+) -> List[str]:
+    """Convert Amazon S3 path to list of objects."""
+    _suffix: Optional[List[str]] = [suffix] if isinstance(suffix, str) else suffix
+    _ignore_suffix: Optional[List[str]] = [ignore_suffix] if isinstance(ignore_suffix, str) else ignore_suffix
+    if isinstance(path, str):  # prefix
+        paths: List[str] = [
+            path
+            for paths in _list_objects(
+                path=path,
+                s3_client=s3_client,
+                suffix=_suffix,
+                ignore_suffix=_ignore_suffix,
+                last_modified_begin=last_modified_begin,
+                last_modified_end=last_modified_end,
+                ignore_empty=ignore_empty,
+                s3_additional_kwargs=s3_additional_kwargs,
+            )
+            for path in paths
+        ]
+    elif isinstance(path, list):
+        if last_modified_begin or last_modified_end:
+            raise exceptions.InvalidArgumentCombination(
+                "Specify a list of files or (last_modified_begin and last_modified_end)"
+            )
+        paths = path if _suffix is None else [x for x in path if x.endswith(tuple(_suffix))]
+        paths = path if _ignore_suffix is None else [x for x in paths if x.endswith(tuple(_ignore_suffix)) is False]
+    else:
+        raise exceptions.InvalidArgumentType(f"{type(path)} is not a valid path type. Please, use str or List[str].")
+    return paths
+
+
+def _validate_datetimes(
+    last_modified_begin: Optional[datetime.datetime] = None, last_modified_end: Optional[datetime.datetime] = None
+) -> None:
+    if (last_modified_begin is not None) and (last_modified_begin.tzinfo is None):
+        raise exceptions.InvalidArgumentValue("Timezone is not defined for last_modified_begin.")
+    if (last_modified_end is not None) and (last_modified_end.tzinfo is None):
+        raise exceptions.InvalidArgumentValue("Timezone is not defined for last_modified_end.")
+    if (last_modified_begin is not None) and (last_modified_end is not None):
+        if last_modified_begin > last_modified_end:
+            raise exceptions.InvalidArgumentValue("last_modified_begin is bigger than last_modified_end.")
+
+
+def _prefix_cleanup(prefix: str) -> str:
+    for n, c in enumerate(prefix):
+        if c in ["*", "?", "["]:
+            return prefix[:n]
+    return prefix
+
+
+def _list_objects(
+    path: str,
+    s3_client: "S3Client",
+    delimiter: Optional[str] = None,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    suffix: Union[str, List[str], None] = None,
+    ignore_suffix: Union[str, List[str], None] = None,
+    last_modified_begin: Optional[datetime.datetime] = None,
+    last_modified_end: Optional[datetime.datetime] = None,
+    ignore_empty: bool = False,
+) -> Iterator[List[str]]:
+    suffix: Union[List[str], None] = [suffix] if isinstance(suffix, str) else suffix
+    ignore_suffix: Union[List[str], None] = [ignore_suffix] if isinstance(ignore_suffix, str) else ignore_suffix
+    _validate_datetimes(last_modified_begin=last_modified_begin, last_modified_end=last_modified_end)
+    bucket, pattern = _utils.parse_path(path=path)
+    prefix: str = _prefix_cleanup(prefix=pattern)
+
+    return _list_objects_paginate(
+        bucket=bucket,
+        pattern=pattern,
+        prefix=prefix,
+        s3_client=s3_client,
+        delimiter=delimiter,
+        suffix=suffix,
+        ignore_suffix=ignore_suffix,
+        last_modified_begin=last_modified_begin,
+        last_modified_end=last_modified_end,
+        ignore_empty=ignore_empty,
+        s3_additional_kwargs=s3_additional_kwargs,
     )
 
 
-def parse_path(path: str) -> Tuple[str, str]:
-    """Split a full S3 path in bucket and key strings.
-
-    's3://bucket/key' -> ('bucket', 'key')
+@engine.dispatch_on_engine
+def _list_objects_paginate(  # pylint: disable=too-many-branches
+    bucket: str,
+    pattern: str,
+    prefix: str,
+    s3_client: "S3Client",
+    delimiter: Optional[str],
+    s3_additional_kwargs: Optional[Dict[str, Any]],
+    suffix: Union[List[str], None],
+    ignore_suffix: Union[List[str], None],
+    last_modified_begin: Optional[datetime.datetime],
+    last_modified_end: Optional[datetime.datetime],
+    ignore_empty: bool,
+) -> Iterator[List[str]]:
+    default_pagination: Dict[str, int] = {"PageSize": 1000}
+    extra_kwargs: Dict[str, Any] = {"PaginationConfig": default_pagination}
+    if s3_additional_kwargs:
+        extra_kwargs = _fs.get_botocore_valid_kwargs(
+            function_name="list_objects_v2", s3_additional_kwargs=s3_additional_kwargs
+        )
+        extra_kwargs["PaginationConfig"] = (
+            s3_additional_kwargs["PaginationConfig"]
+            if "PaginationConfig" in s3_additional_kwargs
+            else default_pagination
+        )
+    paginator = s3_client.get_paginator("list_objects_v2")
+    args: Dict[str, Any] = {"Bucket": bucket, "Prefix": prefix, **extra_kwargs}
+    if delimiter is not None:
+        args["Delimiter"] = delimiter
+    _logger.debug("args: %s", args)
+    response_iterator = paginator.paginate(**args)
+    paths: List[str] = []
+
+    for page in response_iterator:  # pylint: disable=too-many-nested-blocks
+        if delimiter is None:
+            contents = page.get("Contents")
+            if contents is not None:
+                for content in contents:
+                    key: str = content["Key"]
+                    if ignore_empty and content.get("Size", 0) == 0:
+                        _logger.debug("Skipping empty file: %s", f"s3://{bucket}/{key}")
+                    elif (content is not None) and ("Key" in content):
+                        if (suffix is None) or key.endswith(tuple(suffix)):
+                            if last_modified_begin is not None:
+                                if content["LastModified"] < last_modified_begin:
+                                    continue
+                            if last_modified_end is not None:
+                                if content["LastModified"] > last_modified_end:
+                                    continue
+                            paths.append(f"s3://{bucket}/{key}")
+        else:
+            prefixes = page.get("CommonPrefixes")
+            if prefixes is not None:
+                for pfx in prefixes:
+                    if (pfx is not None) and ("Prefix" in pfx):
+                        key = pfx["Prefix"]
+                        paths.append(f"s3://{bucket}/{key}")
+
+        if prefix != pattern:
+            paths = fnmatch.filter(paths, f"s3://{bucket}/{pattern}")
+
+        if ignore_suffix is not None:
+            paths = [p for p in paths if p.endswith(tuple(ignore_suffix)) is False]
+
+        if paths:
+            yield paths
+        paths = []
+
+
+def does_object_exist(
+    path: str,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    boto3_session: Optional[boto3.Session] = None,
+    version_id: Optional[str] = None,
+) -> bool:
+    """Check if object exists on S3.
 
     Parameters
     ----------
-    path : str
+    path: str
         S3 path (e.g. s3://bucket/key).
+    s3_additional_kwargs : Optional[Dict[str, Any]]
+        Forwarded to botocore requests.
+        e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
+    version_id: str, optional
+        Specific version of the object that should exist.
 
     Returns
     -------
-    Tuple[str, str]
-        Tuple of bucket and key strings
+    bool
+        True if exists, False otherwise.
 
     Examples
     --------
-    >>> from awswrangler._utils import parse_path
-    >>> bucket, key = parse_path('s3://bucket/key')
+    Using the default boto3 session
 
-    >>> from awswrangler._utils import parse_path
-    >>> bucket, key = parse_path('s3://arn:aws:s3:<awsregion>:<awsaccount>:accesspoint/<ap_name>/<key>')
-    """
-    if path.startswith("s3://") is False:
-        raise exceptions.InvalidArgumentValue(f"'{path}' is not a valid path. It MUST start with 's3://'")
-    parts = path.replace("s3://", "").replace(":accesspoint/", ":accesspoint:").split("/", 1)
-    bucket: str = parts[0]
-    if "/" in bucket:
-        raise exceptions.InvalidArgumentValue(f"'{bucket}' is not a valid bucket name.")
-    key: str = ""
-    if len(parts) == 2:
-        key = key if parts[1] is None else parts[1]
-    return bucket, key
+    >>> import awswrangler as wr
+    >>> wr.s3.does_object_exist('s3://bucket/key_real')
+    True
+    >>> wr.s3.does_object_exist('s3://bucket/key_unreal')
+    False
+
+    Using a custom boto3 session
+
+    >>> import boto3
+    >>> import awswrangler as wr
+    >>> wr.s3.does_object_exist('s3://bucket/key_real', boto3_session=boto3.Session())
+    True
+    >>> wr.s3.does_object_exist('s3://bucket/key_unreal', boto3_session=boto3.Session())
+    False
 
+    """
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
+    bucket: str
+    key: str
+    bucket, key = _utils.parse_path(path=path)
+    if s3_additional_kwargs:
+        extra_kwargs: Dict[str, Any] = _fs.get_botocore_valid_kwargs(
+            function_name="head_object", s3_additional_kwargs=s3_additional_kwargs
+        )
+    else:
+        extra_kwargs = {}
+    try:
+        if version_id:
+            extra_kwargs["VersionId"] = version_id
+        s3_client.head_object(Bucket=bucket, Key=key, **extra_kwargs)
+        return True
+    except botocore.exceptions.ClientError as ex:
+        if ex.response["ResponseMetadata"]["HTTPStatusCode"] == 404:
+            return False
+        raise ex
+
+
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
+def list_directories(
+    path: str,
+    chunked: bool = False,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    boto3_session: Optional[boto3.Session] = None,
+) -> Union[List[str], Iterator[List[str]]]:
+    """List Amazon S3 objects from a prefix.
 
-def ensure_cpu_count(use_threads: Union[bool, int] = True) -> int:
-    """Get the number of cpu cores to be used.
-
-    Note
-    ----
-    In case of `use_threads=True` the number of threads that could be spawned will be get from os.cpu_count().
+    This function accepts Unix shell-style wildcards in the path argument.
+    * (matches everything), ? (matches any single character),
+    [seq] (matches any character in seq), [!seq] (matches any character not in seq).
+    If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
+    you can use `glob.escape(path)` before passing the path to this function.
 
     Parameters
     ----------
-    use_threads : Union[bool, int]
-            True to enable multi-core utilization, False to disable.
-            If given an int will simply return the input value.
+    path : str
+        S3 path (e.g. s3://bucket/prefix).
+    chunked: bool
+        If True returns iterator, and a single list otherwise. False by default.
+    s3_additional_kwargs : Optional[Dict[str, Any]]
+        Forwarded to botocore requests.
+        e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
-    int
-        Number of cpu cores to be used.
+    Union[List[str], Iterator[List[str]]]
+        List of objects paths.
 
     Examples
     --------
-    >>> from awswrangler._utils import ensure_cpu_count
-    >>> ensure_cpu_count(use_threads=True)
-    4
-    >>> ensure_cpu_count(use_threads=False)
-    1
+    Using the default boto3 session
+
+    >>> import awswrangler as wr
+    >>> wr.s3.list_directories('s3://bucket/prefix/')
+    ['s3://bucket/prefix/dir0/', 's3://bucket/prefix/dir1/', 's3://bucket/prefix/dir2/']
+
+    Using a custom boto3 session
+
+    >>> import boto3
+    >>> import awswrangler as wr
+    >>> wr.s3.list_directories('s3://bucket/prefix/', boto3_session=boto3.Session())
+    ['s3://bucket/prefix/dir0/', 's3://bucket/prefix/dir1/', 's3://bucket/prefix/dir2/']
 
     """
-    if type(use_threads) == int:  # pylint: disable=unidiomatic-typecheck
-        if use_threads < 1:
-            return 1
-        return use_threads
-    cpus: int = 1
-    if use_threads is True:
-        cpu_cnt: Optional[int] = os.cpu_count()
-        if cpu_cnt is not None:
-            cpus = cpu_cnt if cpu_cnt > cpus else cpus
-    return cpus
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
+    result_iterator = _list_objects(
+        path=path,
+        delimiter="/",
+        s3_client=s3_client,
+        s3_additional_kwargs=s3_additional_kwargs,
+    )
+    if chunked:
+        return result_iterator
+    return [path for paths in result_iterator for path in paths]
+
+
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
+def list_objects(
+    path: str,
+    suffix: Union[str, List[str], None] = None,
+    ignore_suffix: Union[str, List[str], None] = None,
+    last_modified_begin: Optional[datetime.datetime] = None,
+    last_modified_end: Optional[datetime.datetime] = None,
+    ignore_empty: bool = False,
+    chunked: bool = False,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    boto3_session: Optional[boto3.Session] = None,
+) -> Union[List[str], Iterator[List[str]]]:
+    """List Amazon S3 objects from a prefix.
 
+    This function accepts Unix shell-style wildcards in the path argument.
+    * (matches everything), ? (matches any single character),
+    [seq] (matches any character in seq), [!seq] (matches any character not in seq).
+    If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
+    you can use `glob.escape(path)` before passing the path to this function.
 
-def chunkify(lst: List[Any], num_chunks: int = 1, max_length: Optional[int] = None) -> List[List[Any]]:
-    """Split a list in a List of List (chunks) with even sizes.
+    Note
+    ----
+    The filter by last_modified begin last_modified end is applied after list all S3 files
 
     Parameters
     ----------
-    lst: List
-        List of anything to be splitted.
-    num_chunks: int, optional
-        Maximum number of chunks.
-    max_length: int, optional
-        Max length of each chunk. Has priority over num_chunks.
+    path : str
+        S3 path (e.g. s3://bucket/prefix).
+    suffix: Union[str, List[str], None]
+        Suffix or List of suffixes for filtering S3 keys.
+    ignore_suffix: Union[str, List[str], None]
+        Suffix or List of suffixes for S3 keys to be ignored.
+    last_modified_begin
+        Filter the s3 files by the Last modified date of the object.
+        The filter is applied only after list all s3 files.
+    last_modified_end: datetime, optional
+        Filter the s3 files by the Last modified date of the object.
+        The filter is applied only after list all s3 files.
+    ignore_empty: bool
+        Ignore files with 0 bytes.
+    chunked: bool
+        If True returns iterator, and a single list otherwise. False by default.
+    s3_additional_kwargs : Optional[Dict[str, Any]]
+        Forwarded to botocore requests.
+        e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
-    List[List[Any]]
-        List of List (chunks) with even sizes.
+    Union[List[str], Iterator[List[str]]]
+        List of objects paths.
 
     Examples
     --------
-    >>> from awswrangler._utils import chunkify
-    >>> chunkify(list(range(13)), num_chunks=3)
-    [[0, 1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12]]
-    >>> chunkify(list(range(13)), max_length=4)
-    [[0, 1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]]
-
-    """
-    if not lst:
-        return []
-    n: int = num_chunks if max_length is None else int(math.ceil((float(len(lst)) / float(max_length))))
-    np_chunks = np.array_split(lst, n)  # type: ignore
-    return [arr.tolist() for arr in np_chunks if len(arr) > 0]
-
-
-def empty_generator() -> Generator[None, None, None]:
-    """Empty Generator."""
-    yield from ()
-
+    Using the default boto3 session
 
-def get_directory(path: str) -> str:
-    """Extract directory path."""
-    return path.rsplit(sep="/", maxsplit=1)[0] + "/"
+    >>> import awswrangler as wr
+    >>> wr.s3.list_objects('s3://bucket/prefix')
+    ['s3://bucket/prefix0', 's3://bucket/prefix1', 's3://bucket/prefix2']
+
+    Using a custom boto3 session
+
+    >>> import boto3
+    >>> import awswrangler as wr
+    >>> wr.s3.list_objects('s3://bucket/prefix', boto3_session=boto3.Session())
+    ['s3://bucket/prefix0', 's3://bucket/prefix1', 's3://bucket/prefix2']
 
-
-def get_region_from_subnet(subnet_id: str, boto3_session: Optional[boto3.Session] = None) -> str:
-    """Extract region from Subnet ID."""
-    session: boto3.Session = ensure_session(session=boto3_session)
-    client_ec2: boto3.client = client(service_name="ec2", session=session)
-    return cast(str, client_ec2.describe_subnets(SubnetIds=[subnet_id])["Subnets"][0]["AvailabilityZone"][:-1])
-
-
-def get_region_from_session(boto3_session: Optional[boto3.Session] = None, default_region: Optional[str] = None) -> str:
-    """Extract region from session."""
-    session: boto3.Session = ensure_session(session=boto3_session)
-    region: Optional[str] = session.region_name
-    if region is not None:
-        return region
-    if default_region is not None:
-        return default_region
-    raise exceptions.InvalidArgument("There is no region_name defined on boto3, please configure it.")
-
-
-def get_credentials_from_session(
-    boto3_session: Optional[boto3.Session] = None,
-) -> botocore.credentials.ReadOnlyCredentials:
-    """Get AWS credentials from boto3 session."""
-    session: boto3.Session = ensure_session(session=boto3_session)
-    credentials: botocore.credentials.Credentials = session.get_credentials()
-    frozen_credentials: botocore.credentials.ReadOnlyCredentials = credentials.get_frozen_credentials()
-    return frozen_credentials
-
-
-def list_sampling(lst: List[Any], sampling: float) -> List[Any]:
-    """Random List sampling."""
-    if sampling == 1.0:
-        return lst
-    if sampling > 1.0 or sampling <= 0.0:
-        raise exceptions.InvalidArgumentValue(f"Argument <sampling> must be [0.0 < value <= 1.0]. {sampling} received.")
-    _len: int = len(lst)
-    if _len == 0:
-        return []
-    num_samples: int = int(round(_len * sampling))
-    num_samples = _len if num_samples > _len else num_samples
-    num_samples = 1 if num_samples < 1 else num_samples
-    _logger.debug("_len: %s", _len)
-    _logger.debug("sampling: %s", sampling)
-    _logger.debug("num_samples: %s", num_samples)
-    random_lst: List[Any] = random.sample(population=lst, k=num_samples)
-    random_lst.sort()
-    return random_lst
-
-
-def ensure_df_is_mutable(df: pd.DataFrame) -> pd.DataFrame:
-    """Ensure that all columns has the writeable flag True."""
-    for column in df.columns.to_list():
-        if hasattr(df[column].values, "flags") is True:
-            if df[column].values.flags.writeable is False:
-                s: pd.Series = df[column]
-                df[column] = None
-                df[column] = s
-    return df
-
-
-def check_duplicated_columns(df: pd.DataFrame) -> Any:
-    """Raise an exception if there are duplicated columns names."""
-    duplicated: List[str] = df.loc[:, df.columns.duplicated()].columns.to_list()
-    if duplicated:
-        raise exceptions.InvalidDataFrame(
-            f"There are duplicated column names in your DataFrame: {duplicated}. "
-            f"Note that your columns may have been sanitized and it can be the cause of "
-            f"the duplicity."
-        )
-
-
-def try_it(
-    f: Callable[..., Any],
-    ex: Any,
-    ex_code: Optional[str] = None,
-    base: float = 1.0,
-    max_num_tries: int = 3,
-    **kwargs: Any,
-) -> Any:
-    """Run function with decorrelated Jitter.
-
-    Reference: https://aws.amazon.com/blogs/architecture/exponential-backoff-and-jitter/
     """
-    delay: float = base
-    for i in range(max_num_tries):
-        try:
-            return f(**kwargs)
-        except ex as exception:
-            if ex_code is not None and hasattr(exception, "response"):
-                if exception.response["Error"]["Code"] != ex_code:
-                    raise
-            if i == (max_num_tries - 1):
-                raise
-            delay = random.uniform(base, delay * 3)
-            _logger.error("Retrying %s | Fail number %s/%s | Exception: %s", f, i + 1, max_num_tries, exception)
-            time.sleep(delay)
-    raise RuntimeError()
-
-
-def get_even_chunks_sizes(total_size: int, chunk_size: int, upper_bound: bool) -> Tuple[int, ...]:
-    """Calculate even chunks sizes (Best effort)."""
-    round_func: Callable[[float], float] = math.ceil if upper_bound is True else math.floor
-    num_chunks: int = int(round_func(float(total_size) / float(chunk_size)))
-    num_chunks = 1 if num_chunks < 1 else num_chunks
-    base_size: int = int(total_size / num_chunks)
-    rest: int = total_size % num_chunks
-    sizes: List[int] = list(itertools.repeat(base_size, num_chunks))
-    for i in range(rest):
-        i_cycled: int = i % len(sizes)
-        sizes[i_cycled] += 1
-    return tuple(sizes)
-
-
-def get_running_futures(seq: Sequence[Future]) -> Tuple[Future, ...]:  # type: ignore
-    """Filter only running futures."""
-    return tuple(f for f in seq if f.running())
-
-
-def wait_any_future_available(seq: Sequence[Future]) -> None:  # type: ignore
-    """Wait until any future became available."""
-    wait(fs=seq, timeout=None, return_when=FIRST_COMPLETED)
-
-
-def block_waiting_available_thread(seq: Sequence[Future], max_workers: int) -> None:  # type: ignore
-    """Block until any thread became available."""
-    running: Tuple[Future, ...] = get_running_futures(seq=seq)  # type: ignore
-    while len(running) >= max_workers:
-        wait_any_future_available(seq=running)
-        running = get_running_futures(seq=running)
-
-
-def check_schema_changes(columns_types: Dict[str, str], table_input: Optional[Dict[str, Any]], mode: str) -> None:
-    """Check schema changes."""
-    if (table_input is not None) and (mode in ("append", "overwrite_partitions")):
-        catalog_cols: Dict[str, str] = {x["Name"]: x["Type"] for x in table_input["StorageDescriptor"]["Columns"]}
-        for c, t in columns_types.items():
-            if c not in catalog_cols:
-                raise exceptions.InvalidArgumentValue(
-                    f"Schema change detected: New column {c} with type {t}. "
-                    "Please pass schema_evolution=True to allow new columns "
-                    "behaviour."
-                )
-            if t != catalog_cols[c]:  # Data type change detected!
-                raise exceptions.InvalidArgumentValue(
-                    f"Schema change detected: Data type change on column {c} "
-                    f"(Old type: {catalog_cols[c]} / New type {t})."
-                )
-
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
+    # On top of user provided ignore_suffix input, add "/"
+    ignore_suffix_acc = set("/")
+    if isinstance(ignore_suffix, str):
+        ignore_suffix_acc.add(ignore_suffix)
+    elif isinstance(ignore_suffix, list):
+        ignore_suffix_acc.update(ignore_suffix)
+
+    result_iterator = _list_objects(
+        path=path,
+        suffix=suffix,
+        ignore_suffix=list(ignore_suffix_acc),
+        last_modified_begin=last_modified_begin,
+        last_modified_end=last_modified_end,
+        ignore_empty=ignore_empty,
+        s3_client=s3_client,
+        s3_additional_kwargs=s3_additional_kwargs,
+    )
+    if chunked:
+        return result_iterator
+    return [path for paths in result_iterator for path in paths]
 
-@engine.dispatch_on_engine
-def split_pandas_frame(df: pd.DataFrame, splits: int) -> List[pd.DataFrame]:
-    """Split a DataFrame into n chunks."""
-    return [sub_df for sub_df in np.array_split(df, splits) if not sub_df.empty]  # type: ignore
 
+def list_buckets(boto3_session: Optional[boto3.Session] = None) -> List[str]:
+    """List Amazon S3 buckets.
 
-@engine.dispatch_on_engine
-def table_refs_to_df(tables: List[pa.Table], kwargs: Dict[str, Any]) -> pd.DataFrame:  # type: ignore
-    """Build Pandas dataframe from list of PyArrow tables."""
-    return _table_to_df(pa.concat_tables(tables, promote=True), kwargs=kwargs)
+    Parameters
+    ----------
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 session to use, default to None.
 
+    Returns
+    -------
+    List[str]
+        List of bucket names.
 
-@engine.dispatch_on_engine
-def is_pandas_frame(obj: Any) -> bool:
-    """Check if the passed objected is a Pandas DataFrame."""
-    return isinstance(obj, pd.DataFrame)
-
-
-def list_to_arrow_table(
-    mapping: List[Dict[str, Any]],
-    schema: Optional[pa.Schema] = None,
-    metadata: Optional[Dict[str, Any]] = None,
-) -> pa.Table:
-    """Construct a PyArrow Table from list of dictionaries."""
-    arrays = []
-    if not schema:
-        names = []
-        if mapping:
-            names = list(mapping[0].keys())
-        for n in names:
-            v = [row[n] if n in row else None for row in mapping]
-            arrays.append(v)
-        return pa.Table.from_arrays(arrays, names, metadata=metadata)
-    for n in schema.names:
-        v = [row[n] if n in row else None for row in mapping]
-        arrays.append(v)
-    # Will raise if metadata is not None
-    return pa.Table.from_arrays(arrays, schema=schema, metadata=metadata)
+    """
+    client_s3 = _utils.client(service_name="s3", session=boto3_session)
+    buckets = client_s3.list_buckets()["Buckets"]
+    return [bucket["Name"] for bucket in buckets]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/athena/__init__.py` & `awswrangler-3.0.0rc3/awswrangler/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/athena/_cache.py` & `awswrangler-3.0.0rc3/awswrangler/athena/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Cache Module for Amazon Athena."""
 import datetime
 import logging
 import re
 from heapq import heappop, heappush
-from typing import Any, Dict, List, Match, NamedTuple, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Match, NamedTuple, Optional, Tuple, Union
 
 import boto3
 
 from awswrangler import _utils
 
+if TYPE_CHECKING:
+    from mypy_boto3_athena.type_defs import QueryExecutionTypeDef
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 class _CacheInfo(NamedTuple):
     has_valid_cache: bool
     file_format: Optional[str] = None
     query_execution_id: Optional[str] = None
@@ -125,44 +128,44 @@
 
 def _get_last_query_infos(
     max_remote_cache_entries: int,
     boto3_session: Optional[boto3.Session] = None,
     workgroup: Optional[str] = None,
 ) -> List[Dict[str, Any]]:
     """Return an iterator of `query_execution_info`s run by the workgroup in Athena."""
-    client_athena: boto3.client = _utils.client(service_name="athena", session=boto3_session)
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
     page_size = 50
     args: Dict[str, Union[str, Dict[str, int]]] = {
         "PaginationConfig": {"MaxItems": max_remote_cache_entries, "PageSize": page_size}
     }
     if workgroup is not None:
         args["WorkGroup"] = workgroup
     paginator = client_athena.get_paginator("list_query_executions")
-    uncached_ids = []
-    for page in paginator.paginate(**args):
+    uncached_ids: List[str] = []
+    for page in paginator.paginate(**args):  # type: ignore[arg-type]
         _logger.debug("paginating Athena's queries history...")
         query_execution_id_list: List[str] = page["QueryExecutionIds"]
         for query_execution_id in query_execution_id_list:
             if query_execution_id not in _cache_manager:
                 uncached_ids.append(query_execution_id)
     if uncached_ids:
-        new_execution_data = []
+        new_execution_data: List[QueryExecutionTypeDef] = []
         for i in range(0, len(uncached_ids), page_size):
             new_execution_data.extend(
-                client_athena.batch_get_query_execution(QueryExecutionIds=uncached_ids[i : i + page_size]).get(
-                    "QueryExecutions"
-                )
+                client_athena.batch_get_query_execution(  # type: ignore[arg-type]
+                    QueryExecutionIds=uncached_ids[i : i + page_size],
+                ).get("QueryExecutions")
             )
-        _cache_manager.update_cache(new_execution_data)
+        _cache_manager.update_cache(new_execution_data)  # type: ignore[arg-type]
     return _cache_manager.sorted_successful_generator()
 
 
 def _check_for_cached_results(
     sql: str,
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     workgroup: Optional[str],
     max_cache_seconds: int,
     max_cache_query_inspections: int,
     max_remote_cache_entries: int,
 ) -> _CacheInfo:
     """
     Check whether `sql` has been run before, within the `max_cache_seconds` window, by the `workgroup`.
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/athena/_read.py` & `awswrangler-3.0.0rc3/awswrangler/athena/_read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Amazon Athena Module gathering all read_sql_* function."""
 
+# pylint: disable=too-many-lines
 import csv
 import logging
 import sys
 import uuid
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterator, List, Literal, Optional, Union, cast, overload
 
 import boto3
 import botocore.exceptions
 import pandas as pd
 
-from awswrangler import _utils, catalog, exceptions, s3
+from awswrangler import _utils, catalog, exceptions, s3, typing
 from awswrangler._config import apply_configs
 from awswrangler._data_types import cast_pandas_with_athena_types
 from awswrangler._sql_formatter import _process_sql_params
 from awswrangler.athena._utils import (
+    _QUERY_WAIT_POLLING_DELAY,
     _apply_query_metadata,
     _empty_dataframe_response,
     _get_query_metadata,
     _get_s3_output,
     _get_workgroup_config,
     _QueryMetadata,
     _start_query_execution,
@@ -30,15 +32,15 @@
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _extract_ctas_manifest_paths(path: str, boto3_session: Optional[boto3.Session] = None) -> List[str]:
     """Get the list of paths of the generated files."""
     bucket_name, key_path = _utils.parse_path(path)
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
+    client_s3 = _utils.client(service_name="s3", session=boto3_session)
     body: bytes = client_s3.get_object(Bucket=bucket_name, Key=key_path)["Body"].read()
     return [x for x in body.decode("utf-8").split("\n") if x != ""]
 
 
 def _fix_csv_types_generator(
     dfs: Iterator[pd.DataFrame], parse_dates: List[str], binaries: List[str]
 ) -> Iterator[pd.DataFrame]:
@@ -66,15 +68,15 @@
     return df
 
 
 def _delete_after_iterate(
     dfs: Iterator[pd.DataFrame],
     paths: List[str],
     use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, str]],
 ) -> Iterator[pd.DataFrame]:
     for df in dfs:
         yield df
     s3.delete_objects(
         path=paths, use_threads=use_threads, boto3_session=boto3_session, s3_additional_kwargs=s3_additional_kwargs
     )
@@ -82,15 +84,15 @@
 
 def _fetch_parquet_result(
     query_metadata: _QueryMetadata,
     keep_files: bool,
     categories: Optional[List[str]],
     chunksize: Optional[int],
     use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     temp_table_fqn: Optional[str] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ret: Union[pd.DataFrame, Iterator[pd.DataFrame]]
     chunked: Union[bool, int] = False if chunksize is None else chunksize
     _logger.debug("chunked: %s", chunked)
@@ -103,14 +105,17 @@
     paths: List[str] = _extract_ctas_manifest_paths(path=manifest_path, boto3_session=boto3_session)
     if not paths:
         if not temp_table_fqn:
             raise exceptions.EmptyDataFrame("Query would return untyped, empty dataframe.")
 
         database, temp_table_name = map(lambda x: x.replace('"', ""), temp_table_fqn.split("."))
         dtype_dict = catalog.get_table_types(database=database, table=temp_table_name, boto3_session=boto3_session)
+        if dtype_dict is None:
+            raise exceptions.ResourceDoesNotExist(f"Temp table {temp_table_fqn} not found.")
+
         df = pd.DataFrame(columns=list(dtype_dict.keys()))
         df = cast_pandas_with_athena_types(df=df, dtype=dtype_dict)
         df = _apply_query_metadata(df=df, query_metadata=query_metadata)
 
         if chunked:
             return (df,)
 
@@ -124,14 +129,15 @@
     ret = s3.read_parquet(
         path=paths,
         use_threads=use_threads,
         boto3_session=boto3_session,
         chunked=chunked,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
+
     if chunked is False:
         ret = _apply_query_metadata(df=ret, query_metadata=query_metadata)
     else:
         ret = _add_query_metadata_generator(dfs=ret, query_metadata=query_metadata)
     paths_delete: List[str] = paths + [manifest_path, metadata_path]
     _logger.debug("type(ret): %s", type(ret))
     if chunked is False:
@@ -155,15 +161,15 @@
 
 
 def _fetch_csv_result(
     query_metadata: _QueryMetadata,
     keep_files: bool,
     chunksize: Optional[int],
     use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     _chunksize: Optional[int] = chunksize if isinstance(chunksize, int) else None
     _logger.debug("_chunksize: %s", _chunksize)
     if query_metadata.output_location is None or query_metadata.output_location.endswith(".csv") is False:
         chunked = _chunksize is not None
         return _empty_dataframe_response(chunked, query_metadata)
@@ -209,28 +215,30 @@
 
 
 def _resolve_query_with_cache(
     cache_info: _CacheInfo,
     categories: Optional[List[str]],
     chunksize: Optional[Union[int, bool]],
     use_threads: Union[bool, int],
+    athena_query_wait_polling_delay: float,
     session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, Any]],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Fetch cached data and return it as a pandas DataFrame (or list of DataFrames)."""
     _logger.debug("cache_info:\n%s", cache_info)
     if cache_info.query_execution_id is None:
         raise RuntimeError("Trying to resolve with cache but w/o any query execution ID.")
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=cache_info.query_execution_id,
         boto3_session=session,
         categories=categories,
         query_execution_payload=cache_info.query_execution_payload,
         metadata_cache_manager=_cache_manager,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
     if cache_info.file_format == "parquet":
         return _fetch_parquet_result(
             query_metadata=query_metadata,
             keep_files=True,
             categories=categories,
             chunksize=chunksize,
@@ -260,36 +268,40 @@
     chunksize: Union[int, bool, None],
     categories: Optional[List[str]],
     encryption: Optional[str],
     workgroup: Optional[str],
     kms_key: Optional[str],
     alt_database: Optional[str],
     name: Optional[str],
-    ctas_bucketing_info: Optional[Tuple[List[str], int]],
+    ctas_bucketing_info: Optional[typing.BucketingInfoTuple],
+    ctas_write_compression: Optional[str],
+    athena_query_wait_polling_delay: float,
     use_threads: Union[bool, int],
     s3_additional_kwargs: Optional[Dict[str, Any]],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     ctas_query_info: Dict[str, Union[str, _QueryMetadata]] = create_ctas_table(
         sql=sql,
         database=database,
         ctas_table=name,
         ctas_database=alt_database,
         bucketing_info=ctas_bucketing_info,
         data_source=data_source,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
+        write_compression=ctas_write_compression,
         kms_key=kms_key,
         wait=True,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         boto3_session=boto3_session,
     )
     fully_qualified_name: str = f'"{ctas_query_info["ctas_database"]}"."{ctas_query_info["ctas_table"]}"'
-    ctas_query_metadata: _QueryMetadata = ctas_query_info["ctas_query_metadata"]  # type: ignore
+    ctas_query_metadata = cast(_QueryMetadata, ctas_query_info["ctas_query_metadata"])
     _logger.debug("ctas_query_metadata: %s", ctas_query_metadata)
     return _fetch_parquet_result(
         query_metadata=ctas_query_metadata,
         keep_files=keep_files,
         categories=categories,
         chunksize=chunksize,
         use_threads=use_threads,
@@ -312,16 +324,17 @@
     keep_files: bool,
     chunksize: Union[int, bool, None],
     categories: Optional[List[str]],
     encryption: Optional[str],
     kms_key: Optional[str],
     workgroup: Optional[str],
     use_threads: Union[bool, int],
+    athena_query_wait_polling_delay: float,
     s3_additional_kwargs: Optional[Dict[str, Any]],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     query_metadata = _unload(
         sql=sql,
         path=s3_output,
         file_format=file_format,
         compression=compression,
@@ -329,14 +342,15 @@
         partitioned_by=partitioned_by,
         workgroup=workgroup,
         database=database,
         encryption=encryption,
         kms_key=kms_key,
         boto3_session=boto3_session,
         data_source=data_source,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
     if file_format == "PARQUET":
         return _fetch_parquet_result(
             query_metadata=query_metadata,
             keep_files=keep_files,
             categories=categories,
             chunksize=chunksize,
@@ -356,16 +370,17 @@
     keep_files: bool,
     chunksize: Union[int, bool, None],
     categories: Optional[List[str]],
     encryption: Optional[str],
     workgroup: Optional[str],
     kms_key: Optional[str],
     use_threads: Union[bool, int],
+    athena_query_wait_polling_delay: float,
     s3_additional_kwargs: Optional[Dict[str, Any]],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
     s3_output = _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=boto3_session)
     s3_output = s3_output[:-1] if s3_output[-1] == "/" else s3_output
     _logger.debug("sql: %s", sql)
     query_id: str = _start_query_execution(
         sql=sql,
@@ -380,14 +395,15 @@
     )
     _logger.debug("query_id: %s", query_id)
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=query_id,
         boto3_session=boto3_session,
         categories=categories,
         metadata_cache_manager=_cache_manager,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
     return _fetch_csv_result(
         query_metadata=query_metadata,
         keep_files=keep_files,
         chunksize=chunksize,
         use_threads=use_threads,
         boto3_session=boto3_session,
@@ -398,28 +414,30 @@
 def _resolve_query_without_cache(
     # pylint: disable=too-many-branches,too-many-locals,too-many-return-statements,too-many-statements
     sql: str,
     database: str,
     data_source: Optional[str],
     ctas_approach: bool,
     unload_approach: bool,
-    unload_parameters: Optional[Dict[str, Any]],
+    unload_parameters: Optional[typing.AthenaUNLOADSettings],
     categories: Optional[List[str]],
     chunksize: Union[int, bool, None],
     s3_output: Optional[str],
     workgroup: Optional[str],
     encryption: Optional[str],
     kms_key: Optional[str],
     keep_files: bool,
     ctas_database: Optional[str],
     ctas_temp_table_name: Optional[str],
-    ctas_bucketing_info: Optional[Tuple[List[str], int]],
+    ctas_bucketing_info: Optional[typing.BucketingInfoTuple],
+    ctas_write_compression: Optional[str],
+    athena_query_wait_polling_delay: float,
     use_threads: Union[bool, int],
     s3_additional_kwargs: Optional[Dict[str, Any]],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """
     Execute a query in Athena and returns results as DataFrame, back to `read_sql_query`.
 
     Usually called by `read_sql_query` when using cache is not possible.
     """
@@ -439,14 +457,16 @@
                 categories=categories,
                 encryption=encryption,
                 workgroup=workgroup,
                 kms_key=kms_key,
                 alt_database=ctas_database,
                 name=name,
                 ctas_bucketing_info=ctas_bucketing_info,
+                ctas_write_compression=ctas_write_compression,
+                athena_query_wait_polling_delay=athena_query_wait_polling_delay,
                 use_threads=use_threads,
                 s3_additional_kwargs=s3_additional_kwargs,
                 boto3_session=boto3_session,
                 pyarrow_additional_kwargs=pyarrow_additional_kwargs,
             )
         finally:
             catalog.delete_table_if_exists(database=ctas_database or database, table=name, boto3_session=boto3_session)
@@ -465,14 +485,15 @@
             keep_files=keep_files,
             chunksize=chunksize,
             categories=categories,
             encryption=encryption,
             kms_key=kms_key,
             workgroup=workgroup,
             use_threads=use_threads,
+            athena_query_wait_polling_delay=athena_query_wait_polling_delay,
             s3_additional_kwargs=s3_additional_kwargs,
             boto3_session=boto3_session,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
         )
     return _resolve_query_without_cache_regular(
         sql=sql,
         database=database,
@@ -481,14 +502,15 @@
         keep_files=keep_files,
         chunksize=chunksize,
         categories=categories,
         encryption=encryption,
         workgroup=workgroup,
         kms_key=kms_key,
         use_threads=use_threads,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
     )
 
 
 def _unload(
     sql: str,
@@ -497,16 +519,17 @@
     compression: Optional[str],
     field_delimiter: Optional[str],
     partitioned_by: Optional[List[str]],
     workgroup: Optional[str],
     database: Optional[str],
     encryption: Optional[str],
     kms_key: Optional[str],
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     data_source: Optional[str],
+    athena_query_wait_polling_delay: float,
 ) -> _QueryMetadata:
     wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
     s3_output: str = _get_s3_output(s3_output=path, wg_config=wg_config, boto3_session=boto3_session)
     s3_output = s3_output[:-1] if s3_output[-1] == "/" else s3_output
     # Athena does not enforce a Query Result Location for UNLOAD. Thus, the workgroup output location
     # is only used if no path is supplied.
     if not path:
@@ -533,24 +556,25 @@
             s3_output=s3_output,
             encryption=encryption,
             kms_key=kms_key,
             boto3_session=boto3_session,
         )
     except botocore.exceptions.ClientError as ex:
         msg: str = str(ex)
-        error: Dict[str, Any] = ex.response["Error"]
+        error = ex.response["Error"]
         if error["Code"] == "InvalidRequestException":
             raise exceptions.InvalidArgumentValue(f"Exception parsing query. Root error message: {msg}")
         raise ex
     _logger.debug("query_id: %s", query_id)
     try:
         query_metadata: _QueryMetadata = _get_query_metadata(
             query_execution_id=query_id,
             boto3_session=boto3_session,
             metadata_cache_manager=_cache_manager,
+            athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         )
     except exceptions.QueryFailed as ex:
         msg = str(ex)
         if "Column name" in msg and "specified more than once" in msg:
             raise exceptions.InvalidArgumentValue(
                 f"Please, define distinct names for your columns. Root error message: {msg}"
             )
@@ -563,23 +587,82 @@
                 "Please, don't leave undefined columns types in your query. You can cast to ensure it. "
                 "(E.g. 'SELECT CAST(NULL AS INTEGER) AS MY_COL, ...')"
             )
         raise ex
     return query_metadata
 
 
+@overload
+def get_query_results(
+    query_execution_id: str,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Union[None, Literal[False]] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def get_query_results(
+    query_execution_id: str,
+    *,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Literal[True],
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def get_query_results(
+    query_execution_id: str,
+    *,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: bool,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@overload
+def get_query_results(
+    query_execution_id: str,
+    *,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: int,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
 @apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def get_query_results(
     query_execution_id: str,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     categories: Optional[List[str]] = None,
     chunksize: Optional[Union[int, bool]] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Get AWS Athena SQL query results as a Pandas DataFrame.
 
     Parameters
     ----------
     query_execution_id : str
         SQL query's execution_id on AWS Athena.
@@ -596,21 +679,19 @@
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
         If an `INTEGER` is passed awswrangler will iterate on the data by number of rows igual the received INTEGER.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     pyarrow_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to the ParquetFile class or converting an Arrow table to Pandas, currently only an
-        "coerce_int96_timestamp_unit" or "timestamp_as_object" argument will be considered. If reading parquet
-        files where you cannot convert a timestamp to pandas Timestamp[ns] consider setting timestamp_as_object=True,
-        to allow for timestamp units larger than "ns". If reading parquet data that still uses INT96 (like Athena
-        outputs) you can use coerce_int96_timestamp_unit to specify what timestamp unit to encode INT96 to (by default
-        this is "ns", if you know the output parquet came from a system that encodes timestamp to a particular unit
-        then set this to that same unit e.g. coerce_int96_timestamp_unit="ms").
+        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
+        Valid values include "split_blocks", "self_destruct", "ignore_metadata".
+        e.g. pyarrow_additional_kwargs={'split_blocks': True}.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
 
     Returns
     -------
     Union[pd.DataFrame, Iterator[pd.DataFrame]]
         Pandas DataFrame or Generator of Pandas DataFrames if chunksize is passed.
 
     Examples
@@ -622,19 +703,18 @@
 
     """
     query_metadata: _QueryMetadata = _get_query_metadata(
         query_execution_id=query_execution_id,
         boto3_session=boto3_session,
         categories=categories,
         metadata_cache_manager=_cache_manager,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
-    client_athena: boto3.client = _utils.client(service_name="athena", session=boto3_session)
-    query_info: Dict[str, Any] = client_athena.get_query_execution(QueryExecutionId=query_execution_id)[
-        "QueryExecution"
-    ]
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
+    query_info = client_athena.get_query_execution(QueryExecutionId=query_execution_id)["QueryExecution"]
     statement_type: Optional[str] = query_info.get("StatementType")
     if (statement_type == "DDL" and query_info["Query"].startswith("CREATE TABLE")) or (
         statement_type == "DML" and query_info["Query"].startswith("UNLOAD")
     ):
         return _fetch_parquet_result(
             query_metadata=query_metadata,
             keep_files=True,
@@ -653,51 +733,189 @@
             use_threads=use_threads,
             boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
         )
     raise exceptions.UndetectedType(f"""Unable to get results for: {query_info["Query"]}.""")
 
 
-@apply_configs
+@overload
+def read_sql_query(  # pylint: disable=too-many-arguments
+    sql: str,
+    database: str,
+    ctas_approach: bool = ...,
+    unload_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Union[None, Literal[False]] = ...,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    database: str,
+    *,
+    ctas_approach: bool = ...,
+    unload_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Literal[True],
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
 def read_sql_query(
     sql: str,
     database: str,
+    *,
+    ctas_approach: bool = ...,
+    unload_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: bool,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    database: str,
+    *,
+    ctas_approach: bool = ...,
+    unload_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: int,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    database: str,
+    *,
+    ctas_approach: bool = ...,
+    unload_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Optional[Union[int, bool]],
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
+def read_sql_query(  # pylint: disable=too-many-arguments,too-many-locals
+    sql: str,
+    database: str,
     ctas_approach: bool = True,
     unload_approach: bool = False,
-    unload_parameters: Optional[Dict[str, Any]] = None,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = None,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = None,
     categories: Optional[List[str]] = None,
     chunksize: Optional[Union[int, bool]] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     keep_files: bool = True,
-    ctas_database: Optional[str] = None,
-    ctas_temp_table_name: Optional[str] = None,
-    ctas_bucketing_info: Optional[Tuple[List[str], int]] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
-    max_cache_seconds: int = 0,
-    max_cache_query_inspections: int = 50,
-    max_remote_cache_entries: int = 50,
-    max_local_cache_entries: int = 100,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
     data_source: Optional[str] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     params: Optional[Dict[str, Any]] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Execute any SQL query on AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
     **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
@@ -753,15 +971,15 @@
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -777,20 +995,21 @@
     ----
     `chunksize` argument (Memory Friendly) (i.e batching):
 
     Return an Iterable of DataFrames instead of a regular DataFrame.
 
     There are two batching strategies:
 
-    - If **chunksize=True**, a new DataFrame will be returned for each file in the query result.
+    - If **chunksize=True**, depending on the size of the data, one or more data frames are returned per file in the query result.
+      Unlike **chunksize=INTEGER**, rows from different files are not mixed in the resulting data frames.
 
-    - If **chunksize=INTEGER**, awswrangler will iterate on the data by number of rows igual the received INTEGER.
+    - If **chunksize=INTEGER**, awswrangler iterates on the data by number of rows equal to the received INTEGER.
 
     `P.S.` `chunksize=True` is faster and uses less memory while `chunksize=INTEGER` is more precise
-    in number of rows for each Dataframe.
+    in number of rows for each data frame.
 
     `P.P.S.` If `ctas_approach=False` and `chunksize=True`, you will always receive an iterator with a
     single DataFrame because regular Athena queries only produces a single output file.
 
     Note
     ----
     In case of `use_threads=True` the number of threads
@@ -806,15 +1025,17 @@
         (e.g. `database.table`).
     ctas_approach: bool
         Wraps the query using a CTAS, and read the resulted parquet data on S3.
         If false, read the regular CSV on S3.
     unload_approach: bool
         Wraps the query using UNLOAD, and read the results from S3.
         Only PARQUET format is supported.
-    unload_parameters : Optional[Dict[str, Any]]
+    ctas_parameters: typing.AthenaCTASSettings, optional
+        Params of the CTAS such as database, temp_table_name, bucketing_info, and compression.
+    unload_parameters : typing.AthenaUNLOADSettings, optional
         Params of the UNLOAD such as format, compression, field_delimiter, and partitioned_by.
     categories: List[str], optional
         List of columns names that should be returned as pandas.Categorical.
         Recommended for memory restricted environments.
     chunksize : Union[int, bool], optional
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
@@ -825,68 +1046,43 @@
         Athena workgroup.
     encryption : str, optional
         Valid values: [None, 'SSE_S3', 'SSE_KMS']. Notice: 'CSE_KMS' is not supported.
     kms_key : str, optional
         For SSE-KMS, this is the KMS key ARN or ID.
     keep_files : bool
         Whether staging files produced by Athena are retained. 'True' by default.
-    ctas_database : str, optional
-        The name of the alternative database where the CTAS temporary table is stored.
-        If None, the default `database` is used.
-    ctas_temp_table_name : str, optional
-        The name of the temporary table and also the directory name on S3 where the CTAS result is stored.
-        If None, it will use the follow random pattern: `f"temp_table_{uuid.uuid4().hex()}"`.
-        On S3 this directory will be under under the pattern: `f"{s3_output}/{ctas_temp_table_name}/"`.
-    ctas_bucketing_info: Tuple[List[str], int], optional
-        Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
-        second element.
-        Only `str`, `int` and `bool` are supported as column data types for bucketing.
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    max_cache_seconds : int
-        awswrangler can look up in Athena's history if this query has been run before.
-        If so, and its completion time is less than `max_cache_seconds` before now, awswrangler
-        skips query execution and just returns the same results as last time.
+    athena_cache_settings: typing.AthenaCacheSettings, optional
+        Params of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
+        max_remote_cache_entries, and max_local_cache_entries.
+        AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaCacheSettings or as a regular Python dict.
         If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
         `keep_files` and `ctas_temp_table_name` params.
         If reading cached data fails for any reason, execution falls back to the usual query run path.
-    max_cache_query_inspections : int
-        Max number of queries that will be inspected from the history to try to find some result to reuse.
-        The bigger the number of inspection, the bigger will be the latency for not cached queries.
-        Only takes effect if max_cache_seconds > 0.
-    max_remote_cache_entries : int
-        Max number of queries that will be retrieved from AWS for cache inspection.
-        The bigger the number of inspection, the bigger will be the latency for not cached queries.
-        Only takes effect if max_cache_seconds > 0 and default value is 50.
-    max_local_cache_entries : int
-        Max number of queries for which metadata will be cached locally. This will reduce the latency and also
-        enables keeping more than `max_remote_cache_entries` available for the cache. This value should not be
-        smaller than max_remote_cache_entries.
-        Only takes effect if max_cache_seconds > 0 and default value is 100.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
     params: Dict[str, any], optional
         Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
         The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
         `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     pyarrow_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to the ParquetFile class or converting an Arrow table to Pandas, currently only an
-        "coerce_int96_timestamp_unit" or "timestamp_as_object" argument will be considered. If reading parquet
-        files where you cannot convert a timestamp to pandas Timestamp[ns] consider setting timestamp_as_object=True,
-        to allow for timestamp units larger than "ns". If reading parquet data that still uses INT96 (like Athena
-        outputs) you can use coerce_int96_timestamp_unit to specify what timestamp unit to encode INT96 to (by default
-        this is "ns", if you know the output parquet came from a system that encodes timestamp to a particular unit
-        then set this to that same unit e.g. coerce_int96_timestamp_unit="ms").
+        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
+        Valid values include "split_blocks", "self_destruct", "ignore_metadata".
+        e.g. pyarrow_additional_kwargs={'split_blocks': True}.
 
     Returns
     -------
     Union[pd.DataFrame, Iterator[pd.DataFrame]]
         Pandas DataFrame or Generator of Pandas DataFrames if chunksize is passed.
 
     Examples
@@ -897,60 +1093,82 @@
 
     >>> import awswrangler as wr
     >>> df = wr.athena.read_sql_query(
     ...     sql="SELECT * FROM my_table WHERE name=:name AND city=:city",
     ...     params={"name": "filtered_name", "city": "filtered_city"}
     ... )
 
+    >>> import awswrangler as wr
+    >>> df = wr.athena.read_sql_query(
+    ...     sql="...",
+    ...     database="...",
+    ...     athena_cache_settings={
+    ...          "max_cache_seconds": 90,
+    ...     },
+    ... )
+
     """
     if ctas_approach and data_source not in (None, "AwsDataCatalog"):
         raise exceptions.InvalidArgumentCombination(
             "Queries with ctas_approach=True (default) does not support "
             "data_source values different than None and 'AwsDataCatalog'. "
             "Please check the related tutorial for more details "
             "(https://github.com/aws/aws-sdk-pandas/blob/main/"
             "tutorials/006%20-%20Amazon%20Athena.ipynb)"
         )
     if ctas_approach and unload_approach:
         raise exceptions.InvalidArgumentCombination("Only one of ctas_approach=True or unload_approach=True is allowed")
     if unload_parameters and unload_parameters.get("file_format") not in (None, "PARQUET"):
         raise exceptions.InvalidArgumentCombination("Only PARQUET file format is supported if unload_approach=True")
     chunksize = sys.maxsize if ctas_approach is False and chunksize is True else chunksize
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
+
+    athena_cache_settings = athena_cache_settings if athena_cache_settings else {}
+    max_cache_seconds = athena_cache_settings.get("max_cache_seconds", 0)
+    max_cache_query_inspections = athena_cache_settings.get("max_cache_query_inspections", 50)
+    max_remote_cache_entries = athena_cache_settings.get("max_remote_cache_entries", 50)
+    max_local_cache_entries = athena_cache_settings.get("max_local_cache_entries", 100)
 
     # Substitute query parameters
     sql = _process_sql_params(sql, params)
 
     max_remote_cache_entries = min(max_remote_cache_entries, max_local_cache_entries)
 
     _cache_manager.max_cache_size = max_local_cache_entries
     cache_info: _CacheInfo = _check_for_cached_results(
         sql=sql,
-        boto3_session=session,
+        boto3_session=boto3_session,
         workgroup=workgroup,
         max_cache_seconds=max_cache_seconds,
         max_cache_query_inspections=max_cache_query_inspections,
         max_remote_cache_entries=max_remote_cache_entries,
     )
     _logger.debug("cache_info:\n%s", cache_info)
     if cache_info.has_valid_cache is True:
         _logger.debug("Valid cache found. Retrieving...")
         try:
             return _resolve_query_with_cache(
                 cache_info=cache_info,
                 categories=categories,
                 chunksize=chunksize,
                 use_threads=use_threads,
-                session=session,
+                session=boto3_session,
+                athena_query_wait_polling_delay=athena_query_wait_polling_delay,
                 s3_additional_kwargs=s3_additional_kwargs,
                 pyarrow_additional_kwargs=pyarrow_additional_kwargs,
             )
         except Exception as e:  # pylint: disable=broad-except
             _logger.error(e)  # if there is anything wrong with the cache, just fallback to the usual path
             _logger.debug("Corrupted cache. Continuing to execute query...")
+
+    ctas_parameters = ctas_parameters if ctas_parameters else {}
+    ctas_database = ctas_parameters.get("database")
+    ctas_temp_table_name = ctas_parameters.get("temp_table_name")
+    ctas_bucketing_info = ctas_parameters.get("bucketing_info")
+    ctas_write_compression = ctas_parameters.get("compression")
+
     return _resolve_query_without_cache(
         sql=sql,
         database=database,
         data_source=data_source,
         ctas_approach=ctas_approach,
         unload_approach=unload_approach,
         unload_parameters=unload_parameters,
@@ -960,60 +1178,190 @@
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
         keep_files=keep_files,
         ctas_database=ctas_database,
         ctas_temp_table_name=ctas_temp_table_name,
         ctas_bucketing_info=ctas_bucketing_info,
+        ctas_write_compression=ctas_write_compression,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=session,
+        boto3_session=boto3_session,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
 
 
+@overload
+def read_sql_table(
+    table: str,
+    database: str,
+    *,
+    unload_approach: bool = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    ctas_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Union[None, Literal[False]] = ...,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    database: str,
+    *,
+    unload_approach: bool = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    ctas_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Literal[True],
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    database: str,
+    *,
+    unload_approach: bool = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    ctas_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: bool,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    database: str,
+    *,
+    unload_approach: bool = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    ctas_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: int,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    database: str,
+    *,
+    unload_approach: bool = ...,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = ...,
+    ctas_approach: bool = ...,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = ...,
+    categories: Optional[List[str]] = ...,
+    chunksize: Optional[Union[int, bool]],
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    keep_files: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    data_source: Optional[str] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
 @apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
 def read_sql_table(
     table: str,
     database: str,
-    ctas_approach: bool = True,
     unload_approach: bool = False,
-    unload_parameters: Optional[Dict[str, Any]] = None,
+    unload_parameters: Optional[typing.AthenaUNLOADSettings] = None,
+    ctas_approach: bool = True,
+    ctas_parameters: Optional[typing.AthenaCTASSettings] = None,
     categories: Optional[List[str]] = None,
     chunksize: Optional[Union[int, bool]] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     keep_files: bool = True,
-    ctas_database: Optional[str] = None,
-    ctas_temp_table_name: Optional[str] = None,
-    ctas_bucketing_info: Optional[Tuple[List[str], int]] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
-    max_cache_seconds: int = 0,
-    max_cache_query_inspections: int = 50,
-    max_remote_cache_entries: int = 50,
-    max_local_cache_entries: int = 100,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
     data_source: Optional[str] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Extract the full table AWS Athena and return the results as a Pandas DataFrame.
 
     **Related tutorial:**
 
-    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    - `Amazon Athena <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
       tutorials/006%20-%20Amazon%20Athena.html>`_
-    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    - `Athena Cache <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
       tutorials/019%20-%20Athena%20Cache.html>`_
-    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    - `Global Configurations <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
       tutorials/021%20-%20Global%20Configurations.html>`_
 
-    **There are two approaches to be defined through ctas_approach parameter:**
+    **There are three approaches available through ctas_approach and unload_approach parameters:**
 
     **1** - ctas_approach=True (Default):
 
     Wrap the query with a CTAS and then reads the table data as parquet directly from s3.
 
     PROS:
 
@@ -1023,39 +1371,58 @@
     CONS:
 
     - Requires create/delete table permissions on Glue.
     - Does not support timestamp with time zone
     - Does not support columns with repeated names.
     - Does not support columns with undefined data types.
     - A temporary table will be created and then deleted immediately.
+    - Does not support custom data_source/catalog_id.
 
-    **2** - ctas_approach=False:
+    **2** - unload_approach=True and ctas_approach=False:
+
+    Does an UNLOAD query on Athena and parse the Parquet result on s3.
+
+    PROS:
+
+    - Faster for mid and big result sizes.
+    - Can handle some level of nested types.
+    - Does not modify Glue Data Catalog
+
+    CONS:
+
+    - Output S3 path must be empty.
+    - Does not support timestamp with time zone.
+    - Does not support columns with repeated names.
+    - Does not support columns with undefined data types.
+
+    **3** - ctas_approach=False:
 
     Does a regular query on Athena and parse the regular CSV result on s3.
 
     PROS:
 
     - Faster for small result sizes (less latency).
     - Does not require create/delete table permissions on Glue
     - Supports timestamp with time zone.
+    - Support custom data_source/catalog_id.
 
     CONS:
 
     - Slower for big results (But stills faster than other libraries that uses the regular Athena's API)
     - Does not handle nested types at all.
 
     Note
     ----
     The resulting DataFrame (or every DataFrame in the returned Iterator for chunked queries) have a
     `query_metadata` attribute, which brings the query result metadata returned by
     `Boto3/Athena <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services
     /athena.html#Athena.Client.get_query_execution>`_ .
 
     For a practical example check out the
-    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/
+    `related tutorial <https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/
     tutorials/024%20-%20Athena%20Query%20Metadata.html>`_!
 
 
     Note
     ----
     Valid encryption modes: [None, 'SSE_S3', 'SSE_KMS'].
 
@@ -1071,22 +1438,23 @@
     ----
     `chunksize` argument (Memory Friendly) (i.e batching):
 
     Return an Iterable of DataFrames instead of a regular DataFrame.
 
     There are two batching strategies:
 
-    - If **chunksize=True**, a new DataFrame will be returned for each file in the query result.
+    - If **chunksize=True**, depending on the size of the data, one or more data frames are returned per file in the query result.
+      Unlike **chunksize=INTEGER**, rows from different files are not mixed in the resulting data frames.
 
-    - If **chunksize=INTEGER**, awswrangler will iterate on the data by number of rows igual the received INTEGER.
+    - If **chunksize=INTEGER**, awswrangler iterates on the data by number of rows equal to the received INTEGER.
 
     `P.S.` `chunksize=True` is faster and uses less memory while `chunksize=INTEGER` is more precise
-    in number of rows for each Dataframe.
+    in number of rows for each data frame.
 
-    `P.P.S.` If `ctas_approach=False` and `chunksize=True`, you will always receive an interador with a
+    `P.P.S.` If `ctas_approach=False` and `chunksize=True`, you will always receive an iterator with a
     single DataFrame because regular Athena queries only produces a single output file.
 
     Note
     ----
     In case of `use_threads=True` the number of threads
     that will be spawned will be gotten from os.cpu_count().
 
@@ -1098,15 +1466,17 @@
         AWS Glue/Athena database name.
     ctas_approach: bool
         Wraps the query using a CTAS, and read the resulted parquet data on S3.
         If false, read the regular CSV on S3.
     unload_approach: bool
         Wraps the query using UNLOAD, and read the results from S3.
         Only PARQUET format is supported.
-    unload_parameters : Optional[Dict[str, Any]]
+    ctas_parameters: typing.AthenaCTASSettings, optional
+        Params of the CTAS such as database, temp_table_name, bucketing_info, and compression.
+    unload_parameters : typing.AthenaUNLOADSettings, optional
         Params of the UNLOAD such as format, compression, field_delimiter, and partitioned_by.
     categories: List[str], optional
         List of columns names that should be returned as pandas.Categorical.
         Recommended for memory restricted environments.
     chunksize : Union[int, bool], optional
         If passed will split the data in a Iterable of DataFrames (Memory friendly).
         If `True` awswrangler iterates on the data by files in the most efficient way without guarantee of chunksize.
@@ -1117,102 +1487,70 @@
         Athena workgroup.
     encryption : str, optional
         Valid values: [None, 'SSE_S3', 'SSE_KMS']. Notice: 'CSE_KMS' is not supported.
     kms_key : str, optional
         For SSE-KMS, this is the KMS key ARN or ID.
     keep_files : bool
         Should awswrangler delete or keep the staging files produced by Athena?
-    ctas_database : str, optional
-        The name of the alternative database where the CTAS temporary table is stored.
-        If None, the default `database` is used.
-    ctas_temp_table_name : str, optional
-        The name of the temporary table and also the directory name on S3 where the CTAS result is stored.
-        If None, it will use the follow random pattern: `f"temp_table_{uuid.uuid4().hex}"`.
-        On S3 this directory will be under under the pattern: `f"{s3_output}/{ctas_temp_table_name}/"`.
-    ctas_bucketing_info: Tuple[List[str], int], optional
-        Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
-        second element.
-        Only `str`, `int` and `bool` are supported as column data types for bucketing.
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    max_cache_seconds: int
-        awswrangler can look up in Athena's history if this table has been read before.
-        If so, and its completion time is less than `max_cache_seconds` before now, awswrangler
-        skips query execution and just returns the same results as last time.
+    athena_cache_settings: typing.AthenaCacheSettings, optional
+        Params of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
+        max_remote_cache_entries, and max_local_cache_entries.
+        AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaCacheSettings or as a regular Python dict.
         If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
         `keep_files` and `ctas_temp_table_name` params.
         If reading cached data fails for any reason, execution falls back to the usual query run path.
-    max_cache_query_inspections : int
-        Max number of queries that will be inspected from the history to try to find some result to reuse.
-        The bigger the number of inspection, the bigger will be the latency for not cached queries.
-        Only takes effect if max_cache_seconds > 0.
-    max_remote_cache_entries : int
-        Max number of queries that will be retrieved from AWS for cache inspection.
-        The bigger the number of inspection, the bigger will be the latency for not cached queries.
-        Only takes effect if max_cache_seconds > 0 and default value is 50.
-    max_local_cache_entries : int
-        Max number of queries for which metadata will be cached locally. This will reduce the latency and also
-        enables keeping more than `max_remote_cache_entries` available for the cache. This value should not be
-        smaller than max_remote_cache_entries.
-        Only takes effect if max_cache_seconds > 0 and default value is 100.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     pyarrow_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to the ParquetFile class or converting an Arrow table to Pandas, currently only an
-        "coerce_int96_timestamp_unit" or "timestamp_as_object" argument will be considered. If
-        reading parquet fileswhere you cannot convert a timestamp to pandas Timestamp[ns] consider
-        setting timestamp_as_object=True, to allow for timestamp units > NS. If reading parquet data that
-        still uses INT96 (like Athena outputs) you can use coerce_int96_timestamp_unit to specify what
-        timestamp unit to encode INT96 to (by default this is "ns", if you know the output parquet came from
-        a system that encodes timestamp to a particular unit then set this to that same unit e.g.
-        coerce_int96_timestamp_unit="ms").
+        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
+        Valid values include "split_blocks", "self_destruct", "ignore_metadata".
+        e.g. pyarrow_additional_kwargs={'split_blocks': True}.
 
     Returns
     -------
     Union[pd.DataFrame, Iterator[pd.DataFrame]]
         Pandas DataFrame or Generator of Pandas DataFrames if chunksize is passed.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df = wr.athena.read_sql_table(table="...", database="...")
     >>> scanned_bytes = df.query_metadata["Statistics"]["DataScannedInBytes"]
 
     """
     table = catalog.sanitize_table_name(table=table)
+
     return read_sql_query(
         sql=f'SELECT * FROM "{table}"',
         database=database,
-        data_source=data_source,
         ctas_approach=ctas_approach,
         unload_approach=unload_approach,
+        ctas_parameters=ctas_parameters,
         unload_parameters=unload_parameters,
         categories=categories,
         chunksize=chunksize,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
         keep_files=keep_files,
-        ctas_database=ctas_database,
-        ctas_temp_table_name=ctas_temp_table_name,
-        ctas_bucketing_info=ctas_bucketing_info,
         use_threads=use_threads,
         boto3_session=boto3_session,
-        max_cache_seconds=max_cache_seconds,
-        max_cache_query_inspections=max_cache_query_inspections,
-        max_remote_cache_entries=max_remote_cache_entries,
-        max_local_cache_entries=max_local_cache_entries,
+        athena_cache_settings=athena_cache_settings,
+        data_source=data_source,
         s3_additional_kwargs=s3_additional_kwargs,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
 
 
 @apply_configs
 def unload(
@@ -1225,14 +1563,15 @@
     partitioned_by: Optional[List[str]] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     data_source: Optional[str] = None,
     params: Optional[Dict[str, Any]] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
 ) -> _QueryMetadata:
     """Write query results from a SELECT statement to the specified data format using UNLOAD.
 
     https://docs.aws.amazon.com/athena/latest/ug/unload.html
 
     Parameters
     ----------
@@ -1264,14 +1603,16 @@
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
     params: Dict[str, any], optional
         Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
         The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
         `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
 
     Returns
     -------
     _QueryMetadata
         Query metadata including query execution id, dtypes, manifest & output location.
 
     Examples
@@ -1279,26 +1620,25 @@
     >>> import awswrangler as wr
     >>> res = wr.athena.unload(
     ...     sql="SELECT * FROM my_table WHERE name=:name AND city=:city",
     ...     params={"name": "filtered_name", "city": "filtered_city"}
     ... )
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-
     # Substitute query parameters
     sql = _process_sql_params(sql, params)
 
     return _unload(
         sql=sql,
         path=path,
         file_format=file_format,
         compression=compression,
         field_delimiter=field_delimiter,
         partitioned_by=partitioned_by,
         workgroup=workgroup,
         database=database,
         encryption=encryption,
         kms_key=kms_key,
-        boto3_session=session,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
+        boto3_session=boto3_session,
         data_source=data_source,
     )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/athena/_utils.py` & `awswrangler-3.0.0rc3/awswrangler/athena/_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,29 +4,46 @@
 import json
 import logging
 import pprint
 import time
 import uuid
 import warnings
 from decimal import Decimal
-from typing import Any, Dict, Generator, List, NamedTuple, Optional, Tuple, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Generator,
+    List,
+    Literal,
+    NamedTuple,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    cast,
+    overload,
+)
 
 import boto3
 import botocore.exceptions
 import pandas as pd
 
-from awswrangler import _data_types, _utils, catalog, exceptions, s3, sts
+from awswrangler import _data_types, _utils, catalog, exceptions, s3, sts, typing
 from awswrangler._config import apply_configs
-from awswrangler._sql_formatter import _EngineType, _format_parameters
+from awswrangler._sql_formatter import _process_sql_params
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 
 from ._cache import _cache_manager, _CacheInfo, _check_for_cached_results, _LocalMetadataCacheManager
 
+if TYPE_CHECKING:
+    from mypy_boto3_glue.type_defs import ColumnTypeDef
+
 _QUERY_FINAL_STATES: List[str] = ["FAILED", "SUCCEEDED", "CANCELLED"]
-_QUERY_WAIT_POLLING_DELAY: float = 0.25  # SECONDS
+_QUERY_WAIT_POLLING_DELAY: float = 1.0  # SECONDS
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 class _QueryMetadata(NamedTuple):
     execution_id: str
     dtype: Dict[str, str]
@@ -42,15 +59,17 @@
 class _WorkGroupConfig(NamedTuple):
     enforced: bool
     s3_output: Optional[str]
     encryption: Optional[str]
     kms_key: Optional[str]
 
 
-def _get_s3_output(s3_output: Optional[str], wg_config: _WorkGroupConfig, boto3_session: boto3.Session) -> str:
+def _get_s3_output(
+    s3_output: Optional[str], wg_config: _WorkGroupConfig, boto3_session: Optional[boto3.Session] = None
+) -> str:
     if wg_config.enforced and wg_config.s3_output is not None:
         return wg_config.s3_output
     if s3_output is not None:
         return s3_output
     if wg_config.s3_output is not None:
         return wg_config.s3_output
     return create_athena_bucket(boto3_session=boto3_session)
@@ -64,19 +83,18 @@
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     args: Dict[str, Any] = {"QueryString": sql}
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
 
     # s3_output
     args["ResultConfiguration"] = {
-        "OutputLocation": _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=session)
+        "OutputLocation": _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=boto3_session)
     }
 
     # encryption
     if wg_config.enforced is True:
         if wg_config.encryption is not None:
             args["ResultConfiguration"]["EncryptionConfiguration"] = {"EncryptionOption": wg_config.encryption}
             if wg_config.kms_key is not None:
@@ -93,27 +111,27 @@
         if data_source is not None:
             args["QueryExecutionContext"]["Catalog"] = data_source
 
     # workgroup
     if workgroup is not None:
         args["WorkGroup"] = workgroup
 
-    client_athena: boto3.client = _utils.client(service_name="athena", session=session)
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
     _logger.debug("args: \n%s", pprint.pformat(args))
-    response: Dict[str, Any] = _utils.try_it(
+    response = _utils.try_it(
         f=client_athena.start_query_execution,
         ex=botocore.exceptions.ClientError,
         ex_code="ThrottlingException",
         max_num_tries=5,
         **args,
     )
-    return cast(str, response["QueryExecutionId"])
+    return response["QueryExecutionId"]
 
 
-def _get_workgroup_config(session: boto3.Session, workgroup: Optional[str] = None) -> _WorkGroupConfig:
+def _get_workgroup_config(session: Optional[boto3.Session] = None, workgroup: Optional[str] = None) -> _WorkGroupConfig:
     enforced: bool
     wg_s3_output: Optional[str]
     wg_encryption: Optional[str]
     wg_kms_key: Optional[str]
 
     enforced, wg_s3_output, wg_encryption, wg_kms_key = False, None, None, None
     if workgroup is not None:
@@ -131,15 +149,15 @@
     _logger.debug("wg_config:\n%s", wg_config)
     return wg_config
 
 
 def _fetch_txt_result(
     query_metadata: _QueryMetadata,
     keep_files: bool,
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, str]],
 ) -> pd.DataFrame:
     if query_metadata.output_location is None or query_metadata.output_location.endswith(".txt") is False:
         return pd.DataFrame()
     path: str = query_metadata.output_location
     _logger.debug("Start TXT reading from %s", path)
     df = s3.read_csv(
@@ -182,27 +200,32 @@
             target_df_dict["Partition"].append(False)
             target_df_dict["Comment"].append(origin_df_dict["comment"][index].strip())
     return pd.DataFrame(data=target_df_dict)
 
 
 def _get_query_metadata(  # pylint: disable=too-many-statements
     query_execution_id: str,
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session] = None,
     categories: Optional[List[str]] = None,
     query_execution_payload: Optional[Dict[str, Any]] = None,
     metadata_cache_manager: Optional[_LocalMetadataCacheManager] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
 ) -> _QueryMetadata:
     """Get query metadata."""
     if (query_execution_payload is not None) and (query_execution_payload["Status"]["State"] in _QUERY_FINAL_STATES):
         if query_execution_payload["Status"]["State"] != "SUCCEEDED":
             reason: str = query_execution_payload["Status"]["StateChangeReason"]
             raise exceptions.QueryFailed(f"Query error: {reason}")
         _query_execution_payload: Dict[str, Any] = query_execution_payload
     else:
-        _query_execution_payload = wait_query(query_execution_id=query_execution_id, boto3_session=boto3_session)
+        _query_execution_payload = wait_query(
+            query_execution_id=query_execution_id,
+            boto3_session=boto3_session,
+            athena_query_wait_polling_delay=athena_query_wait_polling_delay,
+        )
     cols_types: Dict[str, str] = get_query_columns_types(
         query_execution_id=query_execution_id, boto3_session=boto3_session
     )
     _logger.debug("cols_types: %s", cols_types)
     dtype: Dict[str, str] = {}
     parse_timestamps: List[str] = []
     parse_dates: List[str] = []
@@ -284,18 +307,16 @@
         Boto3 Session. If none, the default boto3 session is used.
 
     Returns
     -------
     str
         The named query statement string
     """
-    client_athena: boto3.client = _utils.client(
-        service_name="athena", session=_utils.ensure_session(session=boto3_session)
-    )
-    return client_athena.get_named_query(NamedQueryId=named_query_id)["NamedQuery"]["QueryString"]  # type: ignore
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
+    return client_athena.get_named_query(NamedQueryId=named_query_id)["NamedQuery"]["QueryString"]
 
 
 def get_query_columns_types(query_execution_id: str, boto3_session: Optional[boto3.Session] = None) -> Dict[str, str]:
     """Get the data type of all columns queried.
 
     https://docs.aws.amazon.com/athena/latest/ug/data-types.html
 
@@ -314,19 +335,17 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.athena.get_query_columns_types('query-execution-id')
     {'col0': 'int', 'col1': 'double'}
 
     """
-    client_athena: boto3.client = _utils.client(
-        service_name="athena", session=_utils.ensure_session(session=boto3_session)
-    )
-    response: Dict[str, Any] = client_athena.get_query_results(QueryExecutionId=query_execution_id, MaxResults=1)
-    col_info: List[Dict[str, str]] = response["ResultSet"]["ResultSetMetadata"]["ColumnInfo"]
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
+    response = client_athena.get_query_results(QueryExecutionId=query_execution_id, MaxResults=1)
+    col_info = response["ResultSet"]["ResultSetMetadata"]["ColumnInfo"]
     return dict(
         (c["Name"], f"{c['Type']}({c['Precision']},{c.get('Scale', 0)})")
         if c["Type"] in ["decimal"]
         else (c["Name"], c["Type"])
         for c in col_info
     )
 
@@ -347,47 +366,99 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.athena.create_athena_bucket()
     's3://aws-athena-query-results-ACCOUNT-REGION/'
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    account_id: str = sts.get_account_id(boto3_session=session)
-    region_name: str = str(session.region_name).lower()
+    account_id: str = sts.get_account_id(boto3_session=boto3_session)
+    region_name: str = _utils.get_region_from_session(boto3_session=boto3_session).lower()
     bucket_name = f"aws-athena-query-results-{account_id}-{region_name}"
     path = f"s3://{bucket_name}/"
-    resource = _utils.resource(service_name="s3", session=session)
-    bucket = resource.Bucket(bucket_name)
+    client_s3 = _utils.client(service_name="s3", session=boto3_session)
     args = {} if region_name == "us-east-1" else {"CreateBucketConfiguration": {"LocationConstraint": region_name}}
     try:
-        bucket.create(**args)
-    except resource.meta.client.exceptions.BucketAlreadyOwnedByYou as err:
+        client_s3.create_bucket(Bucket=bucket_name, **args)  # type: ignore[arg-type]
+    except (client_s3.exceptions.BucketAlreadyExists, client_s3.exceptions.BucketAlreadyOwnedByYou) as err:
         _logger.debug("Bucket %s already exists.", err.response["Error"]["BucketName"])
     except botocore.exceptions.ClientError as err:
         if err.response["Error"]["Code"] == "OperationAborted":
             _logger.debug("A conflicting conditional operation is currently in progress against this resource.")
-    bucket.wait_until_exists()
+    client_s3.get_waiter("bucket_exists").wait(Bucket=bucket_name)
     return path
 
 
+@overload
+def start_query_execution(
+    sql: str,
+    database: Optional[str] = ...,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    data_source: Optional[str] = ...,
+    wait: Literal[False] = ...,
+) -> str:
+    ...
+
+
+@overload
+def start_query_execution(
+    sql: str,
+    *,
+    database: Optional[str] = ...,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    data_source: Optional[str] = ...,
+    wait: Literal[True],
+) -> Dict[str, Any]:
+    ...
+
+
+@overload
+def start_query_execution(
+    sql: str,
+    *,
+    database: Optional[str] = ...,
+    s3_output: Optional[str] = ...,
+    workgroup: Optional[str] = ...,
+    encryption: Optional[str] = ...,
+    kms_key: Optional[str] = ...,
+    params: Optional[Dict[str, Any]] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = ...,
+    athena_query_wait_polling_delay: float = ...,
+    data_source: Optional[str] = ...,
+    wait: bool,
+) -> Union[str, Dict[str, Any]]:
+    ...
+
+
 @apply_configs
 def start_query_execution(
     sql: str,
     database: Optional[str] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     params: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
-    max_cache_seconds: int = 0,
-    max_cache_query_inspections: int = 50,
-    max_remote_cache_entries: int = 50,
-    max_local_cache_entries: int = 100,
+    athena_cache_settings: Optional[typing.AthenaCacheSettings] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     data_source: Optional[str] = None,
     wait: bool = False,
 ) -> Union[str, Dict[str, Any]]:
     """Start a SQL Query against AWS Athena.
 
     Note
     ----
@@ -410,33 +481,24 @@
         For SSE-KMS and CSE-KMS , this is the KMS key ARN or ID.
     params: Dict[str, any], optional
         Dict of parameters that will be used for constructing the SQL query. Only named parameters are supported.
         The dict needs to contain the information in the form {'name': 'value'} and the SQL query needs to contain
         `:name`. Note that for varchar columns and similar, you must surround the value in single quotes.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    max_cache_seconds: int
-        awswrangler can look up in Athena's history if this query has been run before.
-        If so, and its completion time is less than `max_cache_seconds` before now, awswrangler
-        skips query execution and just returns the same results as last time.
-        If cached results are valid, awswrangler ignores the `s3_output`, `encryption` and `kms_key` params.
+    athena_cache_settings: typing.AthenaCacheSettings, optional
+        Params of the Athena cache settings such as max_cache_seconds, max_cache_query_inspections,
+        max_remote_cache_entries, and max_local_cache_entries.
+        AthenaCacheSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaCacheSettings or as a regular Python dict.
+        If cached results are valid, awswrangler ignores the `ctas_approach`, `s3_output`, `encryption`, `kms_key`,
+        `keep_files` and `ctas_temp_table_name` params.
         If reading cached data fails for any reason, execution falls back to the usual query run path.
-    max_cache_query_inspections : int
-        Max number of queries that will be inspected from the history to try to find some result to reuse.
-        The bigger the number of inspection, the bigger will be the latency for not cached queries.
-        Only takes effect if max_cache_seconds > 0.
-    max_remote_cache_entries : int
-        Max number of queries that will be retrieved from AWS for cache inspection.
-        The bigger the number of inspection, the bigger will be the latency for not cached queries.
-        Only takes effect if max_cache_seconds > 0 and default value is 50.
-    max_local_cache_entries : int
-        Max number of queries for which metadata will be cached locally. This will reduce the latency and also
-        enables keeping more than `max_remote_cache_entries` available for the cache. This value should not be
-        smaller than max_remote_cache_entries.
-        Only takes effect if max_cache_seconds > 0 and default value is 100.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
     data_source : str, optional
         Data Source / Catalog name. If None, 'AwsDataCatalog' will be used by default.
     wait : bool, default False
         Indicates whether to wait for the query to finish and return a dictionary with the query execution response.
 
     Returns
     -------
@@ -452,63 +514,71 @@
 
     Querying into another data source (PostgreSQL, Redshift, etc)
 
     >>> import awswrangler as wr
     >>> query_exec_id = wr.athena.start_query_execution(sql='...', database='...', data_source='...')
 
     """
-    if params is None:
-        params = {}
-    params = _format_parameters(params, engine=_EngineType.PRESTO)
-    for key, value in params.items():
-        sql = sql.replace(f":{key}", str(value))
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
+    sql = _process_sql_params(sql, params)
+
+    athena_cache_settings = athena_cache_settings if athena_cache_settings else {}
+    max_cache_seconds = athena_cache_settings.get("max_cache_seconds", 0)
+    max_cache_query_inspections = athena_cache_settings.get("max_cache_query_inspections", 50)
+    max_remote_cache_entries = athena_cache_settings.get("max_remote_cache_entries", 50)
+    max_local_cache_entries = athena_cache_settings.get("max_local_cache_entries", 100)
 
     max_remote_cache_entries = min(max_remote_cache_entries, max_local_cache_entries)
 
     _cache_manager.max_cache_size = max_local_cache_entries
     cache_info: _CacheInfo = _check_for_cached_results(
         sql=sql,
-        boto3_session=session,
+        boto3_session=boto3_session,
         workgroup=workgroup,
         max_cache_seconds=max_cache_seconds,
         max_cache_query_inspections=max_cache_query_inspections,
         max_remote_cache_entries=max_remote_cache_entries,
     )
+    _logger.debug("cache_info:\n%s", cache_info)
 
     if cache_info.has_valid_cache and cache_info.query_execution_id is not None:
         query_execution_id = cache_info.query_execution_id
+        _logger.debug("Valid cache found. Retrieving...")
     else:
-        wg_config: _WorkGroupConfig = _get_workgroup_config(session=session, workgroup=workgroup)
+        wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
         query_execution_id = _start_query_execution(
             sql=sql,
             wg_config=wg_config,
             database=database,
             data_source=data_source,
             s3_output=s3_output,
             workgroup=workgroup,
             encryption=encryption,
             kms_key=kms_key,
-            boto3_session=session,
+            boto3_session=boto3_session,
         )
     if wait:
-        return wait_query(query_execution_id=query_execution_id, boto3_session=session)
+        return wait_query(
+            query_execution_id=query_execution_id,
+            boto3_session=boto3_session,
+            athena_query_wait_polling_delay=athena_query_wait_polling_delay,
+        )
 
     return query_execution_id
 
 
 @apply_configs
 def repair_table(
     table: str,
     database: Optional[str] = None,
     data_source: Optional[str] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     """Run the Hive's metastore consistency check: 'MSCK REPAIR TABLE table;'.
 
     Recovers partitions and data associated with partitions.
     Use this statement when you add partitions to the catalog.
     It is possible it will take some time to add all partitions.
@@ -532,14 +602,16 @@
         AWS S3 path.
     workgroup : str, optional
         Athena workgroup.
     encryption : str, optional
         None, 'SSE_S3', 'SSE_KMS', 'CSE_KMS'.
     kms_key : str, optional
         For SSE-KMS and CSE-KMS , this is the KMS key ARN or ID.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     str
         Query final state ('SUCCEEDED', 'FAILED', 'CANCELLED').
@@ -549,37 +621,44 @@
     >>> import awswrangler as wr
     >>> query_final_state = wr.athena.repair_table(table='...', database='...')
 
     """
     query = f"MSCK REPAIR TABLE `{table}`;"
     if (database is not None) and (not database.startswith("`")):
         database = f"`{database}`"
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     query_id = start_query_execution(
         sql=query,
         database=database,
         data_source=data_source,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
-        boto3_session=session,
+        boto3_session=boto3_session,
+    )
+    response: Dict[str, Any] = wait_query(
+        query_execution_id=query_id,
+        boto3_session=boto3_session,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
     )
-    response: Dict[str, Any] = wait_query(query_execution_id=query_id, boto3_session=session)
     return cast(str, response["Status"]["State"])
 
 
 @apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def describe_table(
     table: str,
     database: Optional[str] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> pd.DataFrame:
     """Show the list of columns, including partition columns: 'DESCRIBE table;'.
 
     Shows the list of columns, including partition columns, for the named column.
     The result of this function will be equal to `wr.catalog.table`.
@@ -599,14 +678,16 @@
         AWS S3 path.
     workgroup : str, optional
         Athena workgroup.
     encryption : str, optional
         None, 'SSE_S3', 'SSE_KMS', 'CSE_KMS'.
     kms_key : str, optional
         For SSE-KMS and CSE-KMS , this is the KMS key ARN or ID.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
@@ -619,61 +700,68 @@
     >>> import awswrangler as wr
     >>> df_table = wr.athena.describe_table(table='my_table', database='default')
 
     """
     query = f"DESCRIBE `{table}`;"
     if (database is not None) and (not database.startswith("`")):
         database = f"`{database}`"
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     query_id = start_query_execution(
         sql=query,
         database=database,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
-        boto3_session=session,
+        boto3_session=boto3_session,
+    )
+    query_metadata: _QueryMetadata = _get_query_metadata(
+        query_execution_id=query_id,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
+        boto3_session=boto3_session,
     )
-    query_metadata: _QueryMetadata = _get_query_metadata(query_execution_id=query_id, boto3_session=session)
     raw_result = _fetch_txt_result(
-        query_metadata=query_metadata, keep_files=True, boto3_session=session, s3_additional_kwargs=s3_additional_kwargs
+        query_metadata=query_metadata,
+        keep_files=True,
+        boto3_session=boto3_session,
+        s3_additional_kwargs=s3_additional_kwargs,
     )
     return _parse_describe_table(raw_result)
 
 
 @apply_configs
 def create_ctas_table(  # pylint: disable=too-many-locals
     sql: str,
-    database: str,
+    database: Optional[str] = None,
     ctas_table: Optional[str] = None,
     ctas_database: Optional[str] = None,
     s3_output: Optional[str] = None,
     storage_format: Optional[str] = None,
     write_compression: Optional[str] = None,
     partitioning_info: Optional[List[str]] = None,
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     field_delimiter: Optional[str] = None,
     schema_only: bool = False,
     workgroup: Optional[str] = None,
     data_source: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
     categories: Optional[List[str]] = None,
     wait: bool = False,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Dict[str, Union[str, _QueryMetadata]]:
     """Create a new table populated with the results of a SELECT query.
 
     https://docs.aws.amazon.com/athena/latest/ug/create-table-as.html
 
     Parameters
     ----------
     sql : str
         SELECT SQL query.
-    database : str
+    database : Optional[str], optional
         The name of the database where the original table is stored.
     ctas_table : Optional[str], optional
         The name of the CTAS table.
         If None, a name with a random string is used.
     ctas_database : Optional[str], optional
         The name of the alternative database where the CTAS table should be stored.
         If None, `database` is used, that is the CTAS table is stored in the same database as the original table.
@@ -705,14 +793,16 @@
     kms_key : str, optional
         For SSE-KMS, this is the KMS key ARN or ID.
     categories: List[str], optional
         List of columns names that should be returned as pandas.Categorical.
         Recommended for memory restricted environments.
     wait : bool, default False
         Whether to wait for the query to finish and return a dictionary with the Query metadata.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
     boto3_session : Optional[boto3.Session], optional
         Boto3 Session. The default boto3 session is used if boto3_session is None.
 
     Returns
     -------
     Dict[str, Union[str, _QueryMetadata]]
         A dictionary with the the CTAS database and table names.
@@ -752,14 +842,18 @@
     ...     partitioning_info=["par0", "par1"],
     ...     wait=True,
     ... )
 
     """
     ctas_table = catalog.sanitize_table_name(ctas_table) if ctas_table else f"temp_table_{uuid.uuid4().hex}"
     ctas_database = ctas_database if ctas_database else database
+
+    if ctas_database is None:
+        raise exceptions.InvalidArgumentCombination("Either ctas_database or database must be defined.")
+
     fully_qualified_name = f'"{ctas_database}"."{ctas_table}"'
 
     wg_config: _WorkGroupConfig = _get_workgroup_config(session=boto3_session, workgroup=workgroup)
     s3_output = _get_s3_output(s3_output=s3_output, wg_config=wg_config, boto3_session=boto3_session)
     s3_output = s3_output[:-1] if s3_output[-1] == "/" else s3_output
     # If the workgroup enforces an external location, then it overrides the user supplied argument
     external_location_str: str = (
@@ -804,15 +898,15 @@
             s3_output=s3_output,
             workgroup=workgroup,
             encryption=encryption,
             kms_key=kms_key,
             boto3_session=boto3_session,
         )
     except botocore.exceptions.ClientError as ex:
-        error: Dict[str, Any] = ex.response["Error"]
+        error = ex.response["Error"]
         if error["Code"] == "InvalidRequestException" and "Exception parsing query" in error["Message"]:
             raise exceptions.InvalidCtasApproachQuery(
                 f"It is not possible to wrap this query into a CTAS statement. Root error message: {error['Message']}"
             )
         if error["Code"] == "InvalidRequestException" and "extraneous input" in error["Message"]:
             raise exceptions.InvalidCtasApproachQuery(
                 f"It is not possible to wrap this query into a CTAS statement. Root error message: {error['Message']}"
@@ -823,14 +917,15 @@
     if wait:
         try:
             response["ctas_query_metadata"] = _get_query_metadata(
                 query_execution_id=query_execution_id,
                 boto3_session=boto3_session,
                 categories=categories,
                 metadata_cache_manager=_cache_manager,
+                athena_query_wait_polling_delay=athena_query_wait_polling_delay,
             )
         except exceptions.QueryFailed as ex:
             msg: str = str(ex)
             if "Column name" in msg and "specified more than once" in msg:
                 raise exceptions.InvalidCtasApproachQuery(
                     f"Please, define distinct names for your columns. Root error message: {msg}"
                 )
@@ -846,21 +941,25 @@
             raise ex
     else:
         response["ctas_query_id"] = query_execution_id
     return response
 
 
 @apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def show_create_table(
     table: str,
     database: Optional[str] = None,
     s3_output: Optional[str] = None,
     workgroup: Optional[str] = None,
     encryption: Optional[str] = None,
     kms_key: Optional[str] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
     """Generate the query that created it: 'SHOW CREATE TABLE table;'.
 
     Analyzes an existing table named table_name to generate the query that created it.
 
@@ -879,14 +978,16 @@
         AWS S3 path.
     workgroup : str, optional
         Athena workgroup.
     encryption : str, optional
         None, 'SSE_S3', 'SSE_KMS', 'CSE_KMS'.
     kms_key : str, optional
         For SSE-KMS and CSE-KMS , this is the KMS key ARN or ID.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
@@ -899,27 +1000,33 @@
     >>> import awswrangler as wr
     >>> df_table = wr.athena.show_create_table(table='my_table', database='default')
 
     """
     query = f"SHOW CREATE TABLE `{table}`;"
     if (database is not None) and (not database.startswith("`")):
         database = f"`{database}`"
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     query_id = start_query_execution(
         sql=query,
         database=database,
         s3_output=s3_output,
         workgroup=workgroup,
         encryption=encryption,
         kms_key=kms_key,
-        boto3_session=session,
+        boto3_session=boto3_session,
+    )
+    query_metadata: _QueryMetadata = _get_query_metadata(
+        query_execution_id=query_id,
+        athena_query_wait_polling_delay=athena_query_wait_polling_delay,
+        boto3_session=boto3_session,
     )
-    query_metadata: _QueryMetadata = _get_query_metadata(query_execution_id=query_id, boto3_session=session)
     raw_result = _fetch_txt_result(
-        query_metadata=query_metadata, keep_files=True, boto3_session=session, s3_additional_kwargs=s3_additional_kwargs
+        query_metadata=query_metadata,
+        keep_files=True,
+        boto3_session=boto3_session,
+        s3_additional_kwargs=s3_additional_kwargs,
     )
     return cast(str, raw_result.createtab_stmt.str.strip().str.cat(sep=" "))
 
 
 @apply_configs
 def generate_create_query(
     table: str,
@@ -958,15 +1065,15 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> view_create_query: str = wr.athena.generate_create_query(table='my_view', database='default')
 
     """
 
-    def parse_columns(columns_description: List[Dict[str, str]]) -> str:
+    def parse_columns(columns_description: Sequence["ColumnTypeDef"]) -> str:
         columns_str: List[str] = []
         for column in columns_description:
             column_str = f"  `{column['Name']}` {column['Type']}"
             if "Comment" in column:
                 column_str += f" COMMENT '{column['Comment']}'"
             columns_str.append(column_str)
         return ", \n".join(columns_str)
@@ -976,16 +1083,16 @@
         for key, value in parameters.items():
             if key == "EXTERNAL":
                 continue
             property_key_value = f"  '{key}'='{value}'"
             properties_str.append(property_key_value)
         return ", \n".join(properties_str)
 
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    table_detail: Dict[str, Any] = client_glue.get_table(
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
+    table_detail = client_glue.get_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(
                 transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database, Name=table
             ),
         )
     )["Table"]
@@ -1033,15 +1140,15 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> res = wr.athena.get_work_group(workgroup='workgroup_name')
 
     """
-    client_athena: boto3.client = _utils.client(service_name="athena", session=boto3_session)
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
     return cast(
         Dict[str, Any],
         _utils.try_it(
             f=client_athena.get_work_group,
             ex=botocore.exceptions.ClientError,
             ex_code="ThrottlingException",
             max_num_tries=5,
@@ -1069,45 +1176,51 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.athena.stop_query_execution(query_execution_id='query-execution-id')
 
     """
-    client_athena: boto3.client = _utils.client(service_name="athena", session=boto3_session)
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
     client_athena.stop_query_execution(QueryExecutionId=query_execution_id)
 
 
-def wait_query(query_execution_id: str, boto3_session: Optional[boto3.Session] = None) -> Dict[str, Any]:
+@apply_configs
+def wait_query(
+    query_execution_id: str,
+    boto3_session: Optional[boto3.Session] = None,
+    athena_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
+) -> Dict[str, Any]:
     """Wait for the query end.
 
     Parameters
     ----------
     query_execution_id : str
         Athena query execution ID.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
+    athena_query_wait_polling_delay: float, default: 0.25 seconds
+        Interval in seconds for how often the function will check if the Athena query has completed.
 
     Returns
     -------
     Dict[str, Any]
         Dictionary with the get_query_execution response.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> res = wr.athena.wait_query(query_execution_id='query-execution-id')
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    response: Dict[str, Any] = get_query_execution(query_execution_id=query_execution_id, boto3_session=session)
+    response: Dict[str, Any] = get_query_execution(query_execution_id=query_execution_id, boto3_session=boto3_session)
     state: str = response["Status"]["State"]
     while state not in _QUERY_FINAL_STATES:
-        time.sleep(_QUERY_WAIT_POLLING_DELAY)
-        response = get_query_execution(query_execution_id=query_execution_id, boto3_session=session)
+        time.sleep(athena_query_wait_polling_delay)
+        response = get_query_execution(query_execution_id=query_execution_id, boto3_session=boto3_session)
         state = response["Status"]["State"]
     _logger.debug("state: %s", state)
     _logger.debug("StateChangeReason: %s", response["Status"].get("StateChangeReason"))
     if state == "FAILED":
         raise exceptions.QueryFailed(response["Status"].get("StateChangeReason"))
     if state == "CANCELLED":
         raise exceptions.QueryCancelled(response["Status"].get("StateChangeReason"))
@@ -1133,16 +1246,16 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> res = wr.athena.get_query_execution(query_execution_id='query-execution-id')
 
     """
-    client_athena: boto3.client = _utils.client(service_name="athena", session=boto3_session)
-    response: Dict[str, Any] = _utils.try_it(
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
+    response = _utils.try_it(
         f=client_athena.get_query_execution,
         ex=botocore.exceptions.ClientError,
         ex_code="ThrottlingException",
         max_num_tries=5,
         QueryExecutionId=query_execution_id,
     )
     return cast(Dict[str, Any], response["QueryExecution"])
@@ -1178,17 +1291,17 @@
     --------
     >>> import awswrangler as wr
     >>> query_executions_df, unprocessed_query_executions_df = wr.athena.get_query_executions(
             query_execution_ids=['query-execution-id','query-execution-id1']
         )
     """
     chunked_size: int = 50
-    query_executions: List[Dict[str, Any]] = []
-    unprocessed_query_execution: List[Dict[str, str]] = []
-    client_athena: boto3.client = _utils.client(service_name="athena", session=boto3_session)
+    query_executions = []
+    unprocessed_query_execution = []
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
     for i in range(0, len(query_execution_ids), chunked_size):
         response = client_athena.batch_get_query_execution(QueryExecutionIds=query_execution_ids[i : i + chunked_size])
         query_executions += response["QueryExecutions"]
         unprocessed_query_execution += response["UnprocessedQueryExecutionIds"]
     if unprocessed_query_execution and not return_unprocessed:
         _logger.warning(
             "Some of query execution ids are unable to be processed."
@@ -1219,20 +1332,20 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> res = wr.athena.list_query_executions(workgroup='workgroup-name')
 
     """
-    client_athena: boto3.client = _utils.client(service_name="athena", session=boto3_session)
+    client_athena = _utils.client(service_name="athena", session=boto3_session)
     kwargs: Dict[str, Any] = {"base": 1}
     if workgroup:
         kwargs["WorkGroup"] = workgroup
     query_list: List[str] = []
-    response: Dict[str, Any] = _utils.try_it(
+    response = _utils.try_it(
         f=client_athena.list_query_executions,
         ex=botocore.exceptions.ClientError,
         ex_code="ThrottlingException",
         max_num_tries=5,
         **kwargs,
     )
     query_list += response["QueryExecutionIds"]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/catalog/__init__.py` & `awswrangler-3.0.0rc3/awswrangler/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/catalog/_add.py` & `awswrangler-3.0.0rc3/awswrangler/catalog/_add.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """AWS Glue Catalog Delete Module."""
 
 import logging
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 import boto3
 
-from awswrangler import _utils, exceptions
+from awswrangler import _utils, exceptions, typing
 from awswrangler._config import apply_configs
 from awswrangler.catalog._definitions import (
     _check_column_type,
     _csv_partition_definition,
     _json_partition_definition,
     _parquet_partition_definition,
     _update_table_definition,
@@ -23,17 +23,17 @@
     database: str,
     table: str,
     boto3_session: Optional[boto3.Session],
     inputs: List[Dict[str, Any]],
     catalog_id: Optional[str] = None,
 ) -> None:
     chunks: List[List[Dict[str, Any]]] = _utils.chunkify(lst=inputs, max_length=100)
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     for chunk in chunks:  # pylint: disable=too-many-nested-blocks
-        res: Dict[str, Any] = client_glue.batch_create_partition(
+        res = client_glue.batch_create_partition(
             **_catalog_id(catalog_id=catalog_id, DatabaseName=database, TableName=table, PartitionInputList=chunk)
         )
         if ("Errors" in res) and res["Errors"]:
             for error in res["Errors"]:
                 if "ErrorDetail" in error:
                     if "ErrorCode" in error["ErrorDetail"]:
                         if error["ErrorDetail"]["ErrorCode"] != "AlreadyExistsException":
@@ -41,15 +41,15 @@
 
 
 @apply_configs
 def add_csv_partitions(
     database: str,
     table: str,
     partitions_values: Dict[str, List[str]],
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     catalog_id: Optional[str] = None,
     compression: Optional[str] = None,
     sep: str = ",",
     serde_library: Optional[str] = None,
     serde_parameters: Optional[Dict[str, str]] = None,
     boto3_session: Optional[boto3.Session] = None,
     columns_types: Optional[Dict[str, str]] = None,
@@ -131,15 +131,15 @@
 
 
 @apply_configs
 def add_json_partitions(
     database: str,
     table: str,
     partitions_values: Dict[str, List[str]],
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     catalog_id: Optional[str] = None,
     compression: Optional[str] = None,
     serde_library: Optional[str] = None,
     serde_parameters: Optional[Dict[str, str]] = None,
     boto3_session: Optional[boto3.Session] = None,
     columns_types: Optional[Dict[str, str]] = None,
     partitions_parameters: Optional[Dict[str, str]] = None,
@@ -217,15 +217,15 @@
 
 
 @apply_configs
 def add_parquet_partitions(
     database: str,
     table: str,
     partitions_values: Dict[str, List[str]],
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     catalog_id: Optional[str] = None,
     compression: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     columns_types: Optional[Dict[str, str]] = None,
     partitions_parameters: Optional[Dict[str, str]] = None,
 ) -> None:
     """Add partitions (metadata) to a Parquet Table in the AWS Glue Catalog.
@@ -339,16 +339,16 @@
     ...     database='my_db',
     ...     table='my_table',
     ...     column_name='my_col',
     ...     column_type='int'
     ... )
     """
     if _check_column_type(column_type):
-        client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-        table_res: Dict[str, Any] = client_glue.get_table(
+        client_glue = _utils.client(service_name="glue", session=boto3_session)
+        table_res = client_glue.get_table(
             **_catalog_id(
                 catalog_id=catalog_id,
                 **_transaction_id(transaction_id=transaction_id, DatabaseName=database, Name=table),
             )
         )
         table_input: Dict[str, Any] = _update_table_definition(table_res)
         table_input["StorageDescriptor"]["Columns"].append(
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/catalog/_create.py` & `awswrangler-3.0.0rc3/awswrangler/catalog/_create.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """AWS Glue Catalog Module."""
 
 import logging
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 import boto3
 
-from awswrangler import _utils, exceptions
+from awswrangler import _utils, exceptions, typing
 from awswrangler._config import apply_configs
 from awswrangler.catalog._definitions import _csv_table_definition, _json_table_definition, _parquet_table_definition
 from awswrangler.catalog._delete import delete_all_partitions, delete_table_if_exists
 from awswrangler.catalog._get import _get_table_input
 from awswrangler.catalog._utils import _catalog_id, _transaction_id, sanitize_column_name, sanitize_table_name
 
+if TYPE_CHECKING:
+    from mypy_boto3_glue import GlueClient
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _update_if_necessary(dic: Dict[str, str], key: str, value: Optional[str], mode: str) -> str:
     if value is not None:
         if key not in dic or dic[key] != value:
             dic[key] = value
@@ -31,54 +34,49 @@
     parameters: Optional[Dict[str, str]],
     mode: str,
     catalog_versioning: bool,
     boto3_session: Optional[boto3.Session],
     table_input: Dict[str, Any],
     table_type: Optional[str],
     table_exist: bool,
-    projection_enabled: bool,
     partitions_types: Optional[Dict[str, str]],
     columns_comments: Optional[Dict[str, str]],
     transaction_id: Optional[str],
-    projection_types: Optional[Dict[str, str]],
-    projection_ranges: Optional[Dict[str, str]],
-    projection_values: Optional[Dict[str, str]],
-    projection_intervals: Optional[Dict[str, str]],
-    projection_digits: Optional[Dict[str, str]],
-    projection_formats: Optional[Dict[str, str]],
-    projection_storage_location_template: Optional[str],
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings],
     catalog_id: Optional[str],
 ) -> None:
     # Description
     mode = _update_if_necessary(dic=table_input, key="Description", value=description, mode=mode)
 
     if "Parameters" not in table_input:
         table_input["Parameters"] = {}
 
     # Parameters
     parameters = parameters if parameters else {}
     for k, v in parameters.items():
         mode = _update_if_necessary(dic=table_input["Parameters"], key=k, value=v, mode=mode)
 
     # Projection
-    if projection_enabled is True:
+    projection_params = athena_partition_projection_settings if athena_partition_projection_settings else {}
+    if athena_partition_projection_settings:
         table_input["Parameters"]["projection.enabled"] = "true"
         partitions_types = partitions_types if partitions_types else {}
-        projection_types = projection_types if projection_types else {}
-        projection_ranges = projection_ranges if projection_ranges else {}
-        projection_values = projection_values if projection_values else {}
-        projection_intervals = projection_intervals if projection_intervals else {}
-        projection_digits = projection_digits if projection_digits else {}
-        projection_formats = projection_formats if projection_formats else {}
+        projection_types = projection_params.get("projection_types", {})
+        projection_ranges = projection_params.get("projection_ranges", {})
+        projection_values = projection_params.get("projection_values", {})
+        projection_intervals = projection_params.get("projection_intervals", {})
+        projection_digits = projection_params.get("projection_digits", {})
+        projection_formats = projection_params.get("projection_formats", {})
         projection_types = {sanitize_column_name(k): v for k, v in projection_types.items()}
         projection_ranges = {sanitize_column_name(k): v for k, v in projection_ranges.items()}
         projection_values = {sanitize_column_name(k): v for k, v in projection_values.items()}
         projection_intervals = {sanitize_column_name(k): v for k, v in projection_intervals.items()}
         projection_digits = {sanitize_column_name(k): v for k, v in projection_digits.items()}
         projection_formats = {sanitize_column_name(k): v for k, v in projection_formats.items()}
+        projection_storage_location_template = projection_params.get("projection_storage_location_template")
         for k, v in projection_types.items():
             dtype: Optional[str] = partitions_types.get(k)
             if dtype is None and projection_storage_location_template is None:
                 raise exceptions.InvalidArgumentCombination(
                     f"Column {k} appears as projected column but not as partitioned column."
                 )
             if dtype == "date":
@@ -125,16 +123,15 @@
         for par in table_input["PartitionKeys"]:
             name = par["Name"]
             if name in columns_comments:
                 mode = _update_if_necessary(dic=par, key="Comment", value=columns_comments[name], mode=mode)
 
     _logger.debug("table_input: %s", table_input)
 
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_glue: boto3.client = _utils.client(service_name="glue", session=session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     skip_archive: bool = not catalog_versioning
     if mode not in ("overwrite", "append", "overwrite_partitions", "update"):
         raise exceptions.InvalidArgument(
             f"{mode} is not a valid mode. It must be 'overwrite', 'append' or 'overwrite_partitions'."
         )
     args: Dict[str, Any] = _catalog_id(
         catalog_id=catalog_id,
@@ -145,15 +142,17 @@
         ),
     )
     if table_exist:
         _logger.debug("Updating table (%s)...", mode)
         args["SkipArchive"] = skip_archive
         if mode == "overwrite":
             if table_type != "GOVERNED":
-                delete_all_partitions(table=table, database=database, catalog_id=catalog_id, boto3_session=session)
+                delete_all_partitions(
+                    table=table, database=database, catalog_id=catalog_id, boto3_session=boto3_session
+                )
             client_glue.update_table(**args)
         elif mode == "update":
             client_glue.update_table(**args)
     else:
         try:
             _logger.debug("Creating table (%s)...", mode)
             client_glue.create_table(**args)
@@ -170,15 +169,15 @@
                     transaction_id=transaction_id,
                     boto3_session=boto3_session,
                 )
     _logger.debug("Leaving table as is (%s)...", mode)
 
 
 def _overwrite_table(
-    client_glue: boto3.client,
+    client_glue: "GlueClient",
     catalog_id: Optional[str],
     database: str,
     table: str,
     table_input: Dict[str, Any],
     transaction_id: Optional[str],
     boto3_session: boto3.Session,
 ) -> None:
@@ -234,15 +233,15 @@
     transaction_id: Optional[str],
     catalog_versioning: bool,
     catalog_id: Optional[str],
     table_input: Dict[str, Any],
     boto3_session: Optional[boto3.Session],
 ) -> Dict[str, str]:
     table_input["Parameters"] = parameters
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     skip_archive: bool = not catalog_versioning
     client_glue.update_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(
                 transaction_id=transaction_id, DatabaseName=database, TableInput=table_input, SkipArchive=skip_archive
             ),
@@ -254,31 +253,24 @@
 def _create_parquet_table(
     database: str,
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Optional[Dict[str, str]],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     catalog_id: Optional[str],
     compression: Optional[str],
     description: Optional[str],
     parameters: Optional[Dict[str, str]],
     columns_comments: Optional[Dict[str, str]],
     mode: str,
     catalog_versioning: bool,
-    projection_enabled: bool,
     transaction_id: Optional[str],
-    projection_types: Optional[Dict[str, str]],
-    projection_ranges: Optional[Dict[str, str]],
-    projection_values: Optional[Dict[str, str]],
-    projection_intervals: Optional[Dict[str, str]],
-    projection_digits: Optional[Dict[str, str]],
-    projection_formats: Optional[Dict[str, str]],
-    projection_storage_location_template: Optional[str],
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings],
     boto3_session: Optional[boto3.Session],
     catalog_table_input: Optional[Dict[str, Any]],
 ) -> None:
     table = sanitize_table_name(table=table)
     partitions_types = {} if partitions_types is None else partitions_types
     _logger.debug("catalog_table_input: %s", catalog_table_input)
     table_input: Dict[str, Any]
@@ -316,55 +308,41 @@
         catalog_versioning=catalog_versioning,
         boto3_session=boto3_session,
         table_input=table_input,
         table_type=table_type,
         table_exist=table_exist,
         partitions_types=partitions_types,
         transaction_id=transaction_id,
-        projection_enabled=projection_enabled,
-        projection_types=projection_types,
-        projection_ranges=projection_ranges,
-        projection_values=projection_values,
-        projection_intervals=projection_intervals,
-        projection_digits=projection_digits,
-        projection_formats=projection_formats,
-        projection_storage_location_template=projection_storage_location_template,
+        athena_partition_projection_settings=athena_partition_projection_settings,
         catalog_id=catalog_id,
     )
 
 
 def _create_csv_table(  # pylint: disable=too-many-arguments,too-many-locals
     database: str,
     table: str,
     path: Optional[str],
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Optional[Dict[str, str]],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     description: Optional[str],
     compression: Optional[str],
     parameters: Optional[Dict[str, str]],
     columns_comments: Optional[Dict[str, str]],
     mode: str,
     transaction_id: Optional[str],
     catalog_versioning: bool,
     schema_evolution: bool,
     sep: str,
     skip_header_line_count: Optional[int],
     serde_library: Optional[str],
     serde_parameters: Optional[Dict[str, str]],
     boto3_session: Optional[boto3.Session],
-    projection_enabled: bool,
-    projection_types: Optional[Dict[str, str]],
-    projection_ranges: Optional[Dict[str, str]],
-    projection_values: Optional[Dict[str, str]],
-    projection_intervals: Optional[Dict[str, str]],
-    projection_digits: Optional[Dict[str, str]],
-    projection_formats: Optional[Dict[str, str]],
-    projection_storage_location_template: Optional[str],
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings],
     catalog_table_input: Optional[Dict[str, Any]],
     catalog_id: Optional[str],
 ) -> None:
     table = sanitize_table_name(table=table)
     partitions_types = {} if partitions_types is None else partitions_types
     _logger.debug("catalog_table_input: %s", catalog_table_input)
     table_input: Dict[str, Any]
@@ -398,53 +376,39 @@
         catalog_versioning=catalog_versioning,
         boto3_session=boto3_session,
         table_input=table_input,
         table_type=table_type,
         table_exist=table_exist,
         partitions_types=partitions_types,
         transaction_id=transaction_id,
-        projection_enabled=projection_enabled,
-        projection_types=projection_types,
-        projection_ranges=projection_ranges,
-        projection_values=projection_values,
-        projection_intervals=projection_intervals,
-        projection_digits=projection_digits,
-        projection_formats=projection_formats,
-        projection_storage_location_template=projection_storage_location_template,
+        athena_partition_projection_settings=athena_partition_projection_settings,
         catalog_id=catalog_id,
     )
 
 
 def _create_json_table(  # pylint: disable=too-many-arguments
     database: str,
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Optional[Dict[str, str]],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     description: Optional[str],
     compression: Optional[str],
     parameters: Optional[Dict[str, str]],
     columns_comments: Optional[Dict[str, str]],
     mode: str,
     catalog_versioning: bool,
     schema_evolution: bool,
     transaction_id: Optional[str],
     serde_library: Optional[str],
     serde_parameters: Optional[Dict[str, str]],
     boto3_session: Optional[boto3.Session],
-    projection_enabled: bool,
-    projection_types: Optional[Dict[str, str]],
-    projection_ranges: Optional[Dict[str, str]],
-    projection_values: Optional[Dict[str, str]],
-    projection_intervals: Optional[Dict[str, str]],
-    projection_digits: Optional[Dict[str, str]],
-    projection_formats: Optional[Dict[str, str]],
-    projection_storage_location_template: Optional[str],
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings],
     catalog_table_input: Optional[Dict[str, Any]],
     catalog_id: Optional[str],
 ) -> None:
     table = sanitize_table_name(table=table)
     partitions_types = {} if partitions_types is None else partitions_types
     _logger.debug("catalog_table_input: %s", catalog_table_input)
     table_input: Dict[str, Any]
@@ -476,22 +440,15 @@
         catalog_versioning=catalog_versioning,
         transaction_id=transaction_id,
         boto3_session=boto3_session,
         table_input=table_input,
         table_type=table_type,
         table_exist=table_exist,
         partitions_types=partitions_types,
-        projection_enabled=projection_enabled,
-        projection_types=projection_types,
-        projection_ranges=projection_ranges,
-        projection_values=projection_values,
-        projection_intervals=projection_intervals,
-        projection_digits=projection_digits,
-        projection_formats=projection_formats,
-        projection_storage_location_template=projection_storage_location_template,
+        athena_partition_projection_settings=athena_partition_projection_settings,
         catalog_id=catalog_id,
     )
 
 
 @apply_configs
 def upsert_table_parameters(
     parameters: Dict[str, str],
@@ -532,24 +489,27 @@
     >>> import awswrangler as wr
     >>> pars = wr.catalog.upsert_table_parameters(
     ...     parameters={"source": "mysql", "destination":  "datalake"},
     ...     database="...",
     ...     table="...")
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     table_input: Optional[Dict[str, str]] = _get_table_input(
-        database=database, table=table, boto3_session=session, transaction_id=transaction_id, catalog_id=catalog_id
+        database=database,
+        table=table,
+        boto3_session=boto3_session,
+        transaction_id=transaction_id,
+        catalog_id=catalog_id,
     )
     if table_input is None:
         raise exceptions.InvalidArgumentValue(f"Table {database}.{table} does not exist.")
     return _upsert_table_parameters(
         parameters=parameters,
         database=database,
-        boto3_session=session,
+        boto3_session=boto3_session,
         transaction_id=transaction_id,
         catalog_id=catalog_id,
         table_input=table_input,
         catalog_versioning=catalog_versioning,
     )
 
 
@@ -593,27 +553,30 @@
     >>> import awswrangler as wr
     >>> pars = wr.catalog.overwrite_table_parameters(
     ...     parameters={"source": "mysql", "destination":  "datalake"},
     ...     database="...",
     ...     table="...")
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     table_input: Optional[Dict[str, Any]] = _get_table_input(
-        database=database, table=table, transaction_id=transaction_id, catalog_id=catalog_id, boto3_session=session
+        database=database,
+        table=table,
+        transaction_id=transaction_id,
+        catalog_id=catalog_id,
+        boto3_session=boto3_session,
     )
     if table_input is None:
         raise exceptions.InvalidTable(f"Table {table} does not exist on database {database}.")
     return _overwrite_table_parameters(
         parameters=parameters,
         database=database,
         catalog_id=catalog_id,
         transaction_id=transaction_id,
         table_input=table_input,
-        boto3_session=session,
+        boto3_session=boto3_session,
         catalog_versioning=catalog_versioning,
     )
 
 
 @apply_configs
 def create_database(
     name: str,
@@ -647,15 +610,15 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.catalog.create_database(
     ...     name='awswrangler_test'
     ... )
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     args: Dict[str, str] = {"Name": name}
     if description is not None:
         args["Description"] = description
 
     try:
         r = client_glue.get_database(**_catalog_id(catalog_id=catalog_id, Name=name))
         if not exist_ok:
@@ -670,31 +633,24 @@
 def create_parquet_table(
     database: str,
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str] = None,
     partitions_types: Optional[Dict[str, str]] = None,
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     catalog_id: Optional[str] = None,
     compression: Optional[str] = None,
     description: Optional[str] = None,
     parameters: Optional[Dict[str, str]] = None,
     columns_comments: Optional[Dict[str, str]] = None,
     mode: str = "overwrite",
     catalog_versioning: bool = False,
     transaction_id: Optional[str] = None,
-    projection_enabled: bool = False,
-    projection_types: Optional[Dict[str, str]] = None,
-    projection_ranges: Optional[Dict[str, str]] = None,
-    projection_values: Optional[Dict[str, str]] = None,
-    projection_intervals: Optional[Dict[str, str]] = None,
-    projection_digits: Optional[Dict[str, str]] = None,
-    projection_formats: Optional[Dict[str, str]] = None,
-    projection_storage_location_template: Optional[str] = None,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> None:
     """Create a Parquet Table (Metadata Only) in the AWS Glue Catalog.
 
     'https://docs.aws.amazon.com/athena/latest/ug/data-types.html'
 
     Parameters
@@ -728,46 +684,64 @@
         Columns names and the related comments (e.g. {'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}).
     mode: str
         'overwrite' to recreate any possible existing table or 'append' to keep any possible existing table.
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     transaction_id: str, optional
         The ID of the transaction (i.e. used with GOVERNED tables).
-    projection_enabled : bool
-        Enable Partition Projection on Athena (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html)
-    projection_types : Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections types.
-        Valid types: "enum", "integer", "date", "injected"
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
-    projection_ranges: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections ranges.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
-    projection_values: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections values.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
-    projection_intervals: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections intervals.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '5'})
-    projection_digits: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections digits.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '2'})
-    projection_formats: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections formats.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
-    projection_storage_location_template: Optional[str]
-        Value which is allows Athena to properly map partition values if the S3 file locations do not follow
-        a typical `.../column=value/...` pattern.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
-        (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
@@ -784,17 +758,20 @@
     ...     compression='snappy',
     ...     description='My own table!',
     ...     parameters={'source': 'postgresql'},
     ...     columns_comments={'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}
     ... )
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     catalog_table_input: Optional[Dict[str, Any]] = _get_table_input(
-        database=database, table=table, boto3_session=session, transaction_id=transaction_id, catalog_id=catalog_id
+        database=database,
+        table=table,
+        boto3_session=boto3_session,
+        transaction_id=transaction_id,
+        catalog_id=catalog_id,
     )
     _create_parquet_table(
         database=database,
         table=table,
         path=path,
         columns_types=columns_types,
         table_type=table_type,
@@ -804,63 +781,54 @@
         compression=compression,
         description=description,
         parameters=parameters,
         columns_comments=columns_comments,
         mode=mode,
         catalog_versioning=catalog_versioning,
         transaction_id=transaction_id,
-        projection_enabled=projection_enabled,
-        projection_types=projection_types,
-        projection_ranges=projection_ranges,
-        projection_values=projection_values,
-        projection_intervals=projection_intervals,
-        projection_digits=projection_digits,
-        projection_formats=projection_formats,
-        projection_storage_location_template=projection_storage_location_template,
+        athena_partition_projection_settings=athena_partition_projection_settings,
         boto3_session=boto3_session,
         catalog_table_input=catalog_table_input,
     )
 
 
 @apply_configs
 def create_csv_table(  # pylint: disable=too-many-arguments,too-many-locals
     database: str,
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str] = None,
     partitions_types: Optional[Dict[str, str]] = None,
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     compression: Optional[str] = None,
     description: Optional[str] = None,
     parameters: Optional[Dict[str, str]] = None,
     columns_comments: Optional[Dict[str, str]] = None,
     mode: str = "overwrite",
     catalog_versioning: bool = False,
     schema_evolution: bool = False,
     sep: str = ",",
     skip_header_line_count: Optional[int] = None,
     serde_library: Optional[str] = None,
     serde_parameters: Optional[Dict[str, str]] = None,
     transaction_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
-    projection_enabled: bool = False,
-    projection_types: Optional[Dict[str, str]] = None,
-    projection_ranges: Optional[Dict[str, str]] = None,
-    projection_values: Optional[Dict[str, str]] = None,
-    projection_intervals: Optional[Dict[str, str]] = None,
-    projection_digits: Optional[Dict[str, str]] = None,
-    projection_formats: Optional[Dict[str, str]] = None,
-    projection_storage_location_template: Optional[str] = None,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
     catalog_id: Optional[str] = None,
 ) -> None:
     r"""Create a CSV Table (Metadata Only) in the AWS Glue Catalog.
 
     'https://docs.aws.amazon.com/athena/latest/ug/data-types.html'
 
+    Note
+    ----
+    Athena requires the columns in the underlying CSV files in S3 to be in the same order
+    as the columns in the Glue data catalog.
+
     Parameters
     ----------
     database : str
         Database name.
     table : str
         Table name.
     path : str
@@ -901,46 +869,64 @@
         as a string.
         If no library is provided the default is `org.apache.hadoop.hive.serde2.lazy.LazySimpleSerDe`.
     serde_parameters : Optional[str]
         Dictionary of initialization parameters for the SerDe.
         The default is `{"field.delim": sep, "escape.delim": "\\"}`.
     transaction_id: str, optional
         The ID of the transaction (i.e. used with GOVERNED tables).
-    projection_enabled : bool
-        Enable Partition Projection on Athena (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html)
-    projection_types : Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections types.
-        Valid types: "enum", "integer", "date", "injected"
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
-    projection_ranges: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections ranges.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
-    projection_values: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections values.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
-    projection_intervals: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections intervals.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '5'})
-    projection_digits: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections digits.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '2'})
-    projection_formats: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections formats.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
-    projection_storage_location_template: Optional[str]
-        Value which is allows Athena to properly map partition values if the S3 file locations do not follow
-        a typical `.../column=value/...` pattern.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
-        (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     catalog_id : str, optional
         The ID of the Data Catalog from which to retrieve Databases.
         If none is provided, the AWS account ID is used by default.
 
     Returns
@@ -960,17 +946,20 @@
     ...     compression='gzip',
     ...     description='My own table!',
     ...     parameters={'source': 'postgresql'},
     ...     columns_comments={'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}
     ... )
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     catalog_table_input: Optional[Dict[str, Any]] = _get_table_input(
-        database=database, table=table, boto3_session=session, transaction_id=transaction_id, catalog_id=catalog_id
+        database=database,
+        table=table,
+        boto3_session=boto3_session,
+        transaction_id=transaction_id,
+        catalog_id=catalog_id,
     )
     _create_csv_table(
         database=database,
         table=table,
         path=path,
         columns_types=columns_types,
         table_type=table_type,
@@ -981,22 +970,15 @@
         description=description,
         parameters=parameters,
         columns_comments=columns_comments,
         mode=mode,
         catalog_versioning=catalog_versioning,
         transaction_id=transaction_id,
         schema_evolution=schema_evolution,
-        projection_enabled=projection_enabled,
-        projection_types=projection_types,
-        projection_ranges=projection_ranges,
-        projection_values=projection_values,
-        projection_intervals=projection_intervals,
-        projection_digits=projection_digits,
-        projection_formats=projection_formats,
-        projection_storage_location_template=projection_storage_location_template,
+        athena_partition_projection_settings=athena_partition_projection_settings,
         boto3_session=boto3_session,
         catalog_table_input=catalog_table_input,
         sep=sep,
         skip_header_line_count=skip_header_line_count,
         serde_library=serde_library,
         serde_parameters=serde_parameters,
     )
@@ -1006,34 +988,27 @@
 def create_json_table(  # pylint: disable=too-many-arguments
     database: str,
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str] = None,
     partitions_types: Optional[Dict[str, str]] = None,
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[typing.BucketingInfoTuple] = None,
     compression: Optional[str] = None,
     description: Optional[str] = None,
     parameters: Optional[Dict[str, str]] = None,
     columns_comments: Optional[Dict[str, str]] = None,
     mode: str = "overwrite",
     catalog_versioning: bool = False,
     schema_evolution: bool = False,
     serde_library: Optional[str] = None,
     serde_parameters: Optional[Dict[str, str]] = None,
     transaction_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
-    projection_enabled: bool = False,
-    projection_types: Optional[Dict[str, str]] = None,
-    projection_ranges: Optional[Dict[str, str]] = None,
-    projection_values: Optional[Dict[str, str]] = None,
-    projection_intervals: Optional[Dict[str, str]] = None,
-    projection_digits: Optional[Dict[str, str]] = None,
-    projection_formats: Optional[Dict[str, str]] = None,
-    projection_storage_location_template: Optional[str] = None,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
     catalog_id: Optional[str] = None,
 ) -> None:
     r"""Create a JSON Table (Metadata Only) in the AWS Glue Catalog.
 
     'https://docs.aws.amazon.com/athena/latest/ug/data-types.html'
 
     Parameters
@@ -1076,46 +1051,64 @@
         as a string.
         If no library is provided the default is `org.openx.data.jsonserde.JsonSerDe`.
     serde_parameters : Optional[str]
         Dictionary of initialization parameters for the SerDe.
         The default is `{"field.delim": sep, "escape.delim": "\\"}`.
     transaction_id: str, optional
         The ID of the transaction (i.e. used with GOVERNED tables).
-    projection_enabled : bool
-        Enable Partition Projection on Athena (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html)
-    projection_types : Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections types.
-        Valid types: "enum", "integer", "date", "injected"
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
-    projection_ranges: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections ranges.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
-    projection_values: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections values.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
-    projection_intervals: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections intervals.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '5'})
-    projection_digits: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections digits.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '2'})
-    projection_formats: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections formats.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
-    projection_storage_location_template: Optional[str]
-        Value which is allows Athena to properly map partition values if the S3 file locations do not follow
-        a typical `.../column=value/...` pattern.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
-        (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     catalog_id : str, optional
         The ID of the Data Catalog from which to retrieve Databases.
         If none is provided, the AWS account ID is used by default.
 
     Returns
@@ -1134,17 +1127,16 @@
     ...     partitions_types={'col2': 'date'},
     ...     description='My very own JSON table!',
     ...     parameters={'source': 'postgresql'},
     ...     columns_comments={'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}
     ... )
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     catalog_table_input: Optional[Dict[str, Any]] = _get_table_input(
-        database=database, table=table, boto3_session=session, catalog_id=catalog_id
+        database=database, table=table, boto3_session=boto3_session, catalog_id=catalog_id
     )
     _create_json_table(
         database=database,
         table=table,
         path=path,
         columns_types=columns_types,
         table_type=table_type,
@@ -1155,20 +1147,13 @@
         description=description,
         parameters=parameters,
         columns_comments=columns_comments,
         mode=mode,
         catalog_versioning=catalog_versioning,
         transaction_id=transaction_id,
         schema_evolution=schema_evolution,
-        projection_enabled=projection_enabled,
-        projection_types=projection_types,
-        projection_ranges=projection_ranges,
-        projection_values=projection_values,
-        projection_intervals=projection_intervals,
-        projection_digits=projection_digits,
-        projection_formats=projection_formats,
-        projection_storage_location_template=projection_storage_location_template,
+        athena_partition_projection_settings=athena_partition_projection_settings,
         boto3_session=boto3_session,
         catalog_table_input=catalog_table_input,
         serde_library=serde_library,
         serde_parameters=serde_parameters,
     )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/catalog/_definitions.py` & `awswrangler-3.0.0rc3/awswrangler/catalog/_definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """AWS Glue Catalog Delete Module."""
 
 import logging
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
+
+from awswrangler import typing
+
+if TYPE_CHECKING:
+    from mypy_boto3_glue.type_defs import GetTableResponseTypeDef
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 _LEGAL_COLUMN_TYPES = [
     "array",
     "bigint",
     "binary",
@@ -29,15 +34,15 @@
 
 def _parquet_table_definition(
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Dict[str, str],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     compression: Optional[str],
 ) -> Dict[str, Any]:
     compressed: bool = compression is not None
     return {
         "Name": table,
         "PartitionKeys": [{"Name": cname, "Type": dtype} for cname, dtype in partitions_types.items()],
         "TableType": "EXTERNAL_TABLE" if table_type is None else table_type,
@@ -65,15 +70,15 @@
         },
     }
 
 
 def _parquet_partition_definition(
     location: str,
     values: List[str],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     compression: Optional[str],
     columns_types: Optional[Dict[str, str]],
     partitions_parameters: Optional[Dict[str, str]],
 ) -> Dict[str, Any]:
     compressed: bool = compression is not None
     definition: Dict[str, Any] = {
         "StorageDescriptor": {
@@ -101,15 +106,15 @@
 
 def _csv_table_definition(
     table: str,
     path: Optional[str],
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Dict[str, str],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     compression: Optional[str],
     sep: str,
     skip_header_line_count: Optional[int],
     serde_library: Optional[str],
     serde_parameters: Optional[Dict[str, str]],
 ) -> Dict[str, Any]:
     compressed: bool = compression is not None
@@ -149,15 +154,15 @@
         },
     }
 
 
 def _csv_partition_definition(
     location: str,
     values: List[str],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     compression: Optional[str],
     sep: str,
     serde_library: Optional[str],
     serde_parameters: Optional[Dict[str, str]],
     columns_types: Optional[Dict[str, str]],
     partitions_parameters: Optional[Dict[str, str]],
 ) -> Dict[str, Any]:
@@ -191,15 +196,15 @@
 
 def _json_table_definition(
     table: str,
     path: str,
     columns_types: Dict[str, str],
     table_type: Optional[str],
     partitions_types: Dict[str, str],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     compression: Optional[str],
     serde_library: Optional[str],
     serde_parameters: Optional[Dict[str, str]],
 ) -> Dict[str, Any]:
     compressed: bool = compression is not None
     parameters: Dict[str, str] = {
         "classification": "json",
@@ -230,15 +235,15 @@
         },
     }
 
 
 def _json_partition_definition(
     location: str,
     values: List[str],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     compression: Optional[str],
     serde_library: Optional[str],
     serde_parameters: Optional[Dict[str, str]],
     columns_types: Optional[Dict[str, str]],
     partitions_parameters: Optional[Dict[str, str]],
 ) -> Dict[str, Any]:
     compressed: bool = compression is not None
@@ -269,15 +274,15 @@
 
 def _check_column_type(column_type: str) -> bool:
     if column_type not in _LEGAL_COLUMN_TYPES:
         raise ValueError(f"{column_type} is not a legal data type.")
     return True
 
 
-def _update_table_definition(current_definition: Dict[str, Any]) -> Dict[str, Any]:
+def _update_table_definition(current_definition: "GetTableResponseTypeDef") -> Dict[str, Any]:
     definition: Dict[str, Any] = {}
     keep_keys = [
         "Name",
         "Description",
         "Owner",
         "LastAccessTime",
         "LastAnalyzedTime",
@@ -288,9 +293,9 @@
         "ViewExpandedText",
         "TableType",
         "Parameters",
         "TargetTable",
     ]
     for key in current_definition["Table"]:
         if key in keep_keys:
-            definition[key] = current_definition["Table"][key]
+            definition[key] = current_definition["Table"][key]  # type: ignore[literal-required]
     return definition
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/catalog/_delete.py` & `awswrangler-3.0.0rc3/awswrangler/catalog/_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.catalog.delete_database(
     ...     name='awswrangler_test'
     ... )
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     client_glue.delete_database(**_catalog_id(Name=name, catalog_id=catalog_id))
 
 
 @apply_configs
 def delete_table_if_exists(
     database: str,
     table: str,
@@ -78,15 +78,15 @@
     >>> import awswrangler as wr
     >>> wr.catalog.delete_table_if_exists(database='default', table='my_table')  # deleted
     True
     >>> wr.catalog.delete_table_if_exists(database='default', table='my_table')  # Nothing to be deleted
     False
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     try:
         client_glue.delete_table(
             **_catalog_id(
                 **_transaction_id(
                     transaction_id=transaction_id, DatabaseName=database, Name=table, catalog_id=catalog_id
                 )
             )
@@ -131,15 +131,15 @@
     >>> import awswrangler as wr
     >>> wr.catalog.delete_partitions(
     ...     table='my_table',
     ...     database='awswrangler_test',
     ...     partitions_values=[['2020', '10', '25'], ['2020', '11', '16'], ['2020', '12', '19']]
     ... )
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     chunks: List[List[List[str]]] = _utils.chunkify(lst=partitions_values, max_length=25)
     for chunk in chunks:
         client_glue.batch_delete_partition(
             **_catalog_id(
                 catalog_id=catalog_id,
                 DatabaseName=database,
                 TableName=table,
@@ -175,18 +175,17 @@
     --------
     >>> import awswrangler as wr
     >>> partitions = wr.catalog.delete_all_partitions(
     ...     table='my_table',
     ...     database='awswrangler_test',
     ... )
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     _logger.debug("Fetching existing partitions...")
     partitions_values: List[List[str]] = list(
-        _get_partitions(database=database, table=table, boto3_session=session, catalog_id=catalog_id).values()
+        _get_partitions(database=database, table=table, boto3_session=boto3_session, catalog_id=catalog_id).values()
     )
     _logger.debug("Number of old partitions: %s", len(partitions_values))
     _logger.debug("Deleting existing partitions...")
     delete_partitions(
         table=table,
         database=database,
         catalog_id=catalog_id,
@@ -233,16 +232,16 @@
     >>> import awswrangler as wr
     >>> wr.catalog.delete_column(
     ...     database='my_db',
     ...     table='my_table',
     ...     column_name='my_col',
     ... )
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    table_res: Dict[str, Any] = client_glue.get_table(
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
+    table_res = client_glue.get_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(transaction_id=transaction_id, DatabaseName=database, Name=table),
         )
     )
     table_input: Dict[str, Any] = _update_table_definition(table_res)
     table_input["StorageDescriptor"]["Columns"] = [
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/catalog/_get.py` & `awswrangler-3.0.0rc3/awswrangler/catalog/_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """AWS Glue Catalog Get Module."""
 # pylint: disable=redefined-outer-name
 
 import base64
 import itertools
 import logging
-from typing import Any, Dict, Iterator, List, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Union, cast
 
 import boto3
 import botocore.exceptions
 import pandas as pd
 
 from awswrangler import _utils, exceptions
 from awswrangler._config import apply_configs
 from awswrangler.catalog._utils import _catalog_id, _extract_dtypes_from_table_details, _transaction_id
 
+if TYPE_CHECKING:
+    from mypy_boto3_glue.type_defs import GetPartitionsResponseTypeDef
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _get_table_input(
     database: str,
     table: str,
     boto3_session: Optional[boto3.Session],
     transaction_id: Optional[str] = None,
     catalog_id: Optional[str] = None,
 ) -> Optional[Dict[str, Any]]:
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client("glue", session=boto3_session)
     args: Dict[str, Any] = _catalog_id(
         catalog_id=catalog_id, **_transaction_id(transaction_id=transaction_id, DatabaseName=database, Name=table)
     )
     try:
-        response: Dict[str, Any] = client_glue.get_table(**args)
+        response = client_glue.get_table(**args)
     except client_glue.exceptions.EntityNotFoundException:
         return None
     table_input: Dict[str, Any] = {}
     for k, v in response["Table"].items():
         if k in [
             "Name",
             "Description",
@@ -49,15 +52,17 @@
             "Parameters",
             "TargetTable",
         ]:
             table_input[k] = v
     return table_input
 
 
-def _append_partitions(partitions_values: Dict[str, List[str]], response: Dict[str, Any]) -> Optional[str]:
+def _append_partitions(
+    partitions_values: Dict[str, List[str]], response: "GetPartitionsResponseTypeDef"
+) -> Optional[str]:
     _logger.debug("response: %s", response)
     token: Optional[str] = response.get("NextToken", None)
     if (response is not None) and ("Partitions" in response):
         for partition in response["Partitions"]:
             location: Optional[str] = partition["StorageDescriptor"].get("Location")
             if location is not None:
                 values: List[str] = partition["Values"]
@@ -70,15 +75,15 @@
 def _get_partitions(
     database: str,
     table: str,
     expression: Optional[str] = None,
     catalog_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Dict[str, List[str]]:
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client("glue", session=boto3_session)
 
     args: Dict[str, Any] = _catalog_id(
         catalog_id=catalog_id,
         DatabaseName=database,
         TableName=table,
         MaxResults=1_000,
         Segment={"SegmentNumber": 0, "TotalSegments": 1},
@@ -86,15 +91,15 @@
     )
     if expression is not None:
         args["Expression"] = expression
 
     partitions_values: Dict[str, List[str]] = {}
     _logger.debug("Starting pagination...")
 
-    response: Dict[str, Any] = client_glue.get_partitions(**args)
+    response = client_glue.get_partitions(**args)
     token: Optional[str] = _append_partitions(partitions_values=partitions_values, response=response)
     while token is not None:
         args["NextToken"] = response["NextToken"]
         response = client_glue.get_partitions(**args)
         token = _append_partitions(partitions_values=partitions_values, response=response)
 
     _logger.debug("Pagination done.")
@@ -141,17 +146,17 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.catalog.get_table_types(database='default', table='my_table')
     {'col0': 'int', 'col1': double}
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     try:
-        response: Dict[str, Any] = client_glue.get_table(
+        response = client_glue.get_table(
             **_catalog_id(
                 catalog_id=catalog_id,
                 **_transaction_id(
                     transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database, Name=table
                 ),
             )
         )
@@ -180,20 +185,20 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> dbs = wr.catalog.get_databases()
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client("glue", session=boto3_session)
     paginator = client_glue.get_paginator("get_databases")
     response_iterator = paginator.paginate(**_catalog_id(catalog_id=catalog_id))
     for page in response_iterator:
         for db in page["DatabaseList"]:
-            yield db
+            yield cast(Dict[str, Any], db)
 
 
 @apply_configs
 def databases(
     limit: int = 100, catalog_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
 ) -> pd.DataFrame:
     """Get a Pandas DataFrame with all listed databases.
@@ -215,15 +220,15 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df_dbs = wr.catalog.databases()
 
     """
-    database_iter: Iterator[Dict[str, Any]] = get_databases(catalog_id=catalog_id, boto3_session=boto3_session)
+    database_iter = get_databases(catalog_id=catalog_id, boto3_session=boto3_session)
     dbs = itertools.islice(database_iter, limit)
     df_dict: Dict[str, List[str]] = {"Database": [], "Description": []}
     for db in dbs:
         df_dict["Database"].append(db["Name"])
         df_dict["Description"].append(db.get("Description", ""))
     return pd.DataFrame(data=df_dict)
 
@@ -238,15 +243,15 @@
     name_suffix: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Iterator[Dict[str, Any]]:
     """Get an iterator of tables.
 
     Note
     ----
-    Please, does not filter using name_contains and name_prefix/name_suffix at the same time.
+    Please, do not filter using name_contains and name_prefix/name_suffix at the same time.
     Only name_prefix and name_suffix can be combined together.
 
     Parameters
     ----------
     catalog_id : str, optional
         The ID of the Data Catalog from which to retrieve Databases.
         If none is provided, the AWS account ID is used by default.
@@ -270,20 +275,20 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> tables = wr.catalog.get_tables()
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     paginator = client_glue.get_paginator("get_tables")
     args: Dict[str, str] = {}
     if (name_prefix is not None) and (name_suffix is not None) and (name_contains is not None):
         raise exceptions.InvalidArgumentCombination(
-            "Please, does not filter using name_contains and "
+            "Please, do not filter using name_contains and "
             "name_prefix/name_suffix at the same time. Only "
             "name_prefix and name_suffix can be combined together."
         )
     if (name_prefix is not None) and (name_suffix is not None):
         args["Expression"] = f"{name_prefix}*{name_suffix}"
     elif name_contains is not None:
         args["Expression"] = f"*{name_contains}*"
@@ -299,15 +304,15 @@
         args["DatabaseName"] = db
         response_iterator = paginator.paginate(
             **_catalog_id(catalog_id=catalog_id, **_transaction_id(transaction_id=transaction_id, **args))
         )
         try:
             for page in response_iterator:
                 for tbl in page["TableList"]:
-                    yield tbl
+                    yield cast(Dict[str, Any], tbl)
         except client_glue.exceptions.EntityNotFoundException:
             continue
 
 
 @apply_configs
 def tables(
     limit: int = 100,
@@ -433,24 +438,24 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df_tables = wr.catalog.search_tables(text='my_property')
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client("glue", session=boto3_session)
     args: Dict[str, Any] = _catalog_id(catalog_id=catalog_id, SearchText=text)
-    response: Dict[str, Any] = client_glue.search_tables(**args)
+    response = client_glue.search_tables(**args)
     for tbl in response["TableList"]:
-        yield tbl
+        yield cast(Dict[str, Any], tbl)
     while "NextToken" in response:
         args["NextToken"] = response["NextToken"]
         response = client_glue.search_tables(**args)
         for tbl in response["TableList"]:
-            yield tbl
+            yield cast(Dict[str, Any], tbl)
 
 
 @apply_configs
 def table(
     database: str,
     table: str,
     transaction_id: Optional[str] = None,
@@ -488,15 +493,15 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> df_table = wr.catalog.table(database='default', table='my_table')
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     tbl = client_glue.get_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(
                 transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database, Name=table
             ),
         )
@@ -563,25 +568,25 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.catalog.get_table_location(database='default', table='my_table')
     's3://bucket/prefix/'
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    res: Dict[str, Any] = client_glue.get_table(
+    client_glue = _utils.client("glue", session=boto3_session)
+    res = client_glue.get_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(
                 transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database, Name=table
             ),
         )
     )
     try:
-        return cast(str, res["Table"]["StorageDescriptor"]["Location"])
+        return res["Table"]["StorageDescriptor"]["Location"]
     except KeyError as ex:
         raise exceptions.InvalidTable(f"{database}.{table}") from ex
 
 
 def get_connection(
     name: str, catalog_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
 ) -> Dict[str, Any]:
@@ -605,15 +610,15 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> res = wr.catalog.get_connection(name='my_connection')
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client("glue", session=boto3_session)
 
     res = _utils.try_it(
         f=client_glue.get_connection,
         ex=botocore.exceptions.ClientError,
         ex_code="ThrottlingException",
         max_num_tries=3,
         **_catalog_id(catalog_id=catalog_id, Name=name, HidePassword=False),
@@ -876,16 +881,16 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> pars = wr.catalog.get_table_parameters(database="...", table="...")
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    response: Dict[str, Any] = client_glue.get_table(
+    client_glue = _utils.client("glue", session=boto3_session)
+    response = client_glue.get_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(
                 transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database, Name=table
             ),
         )
     )
@@ -931,16 +936,16 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> desc = wr.catalog.get_table_description(database="...", table="...")
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    response: Dict[str, Any] = client_glue.get_table(
+    client_glue = _utils.client("glue", session=boto3_session)
+    response = client_glue.get_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(
                 transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database, Name=table
             ),
         )
     )
@@ -987,29 +992,29 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> pars = wr.catalog.get_columns_comments(database="...", table="...")
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    response: Dict[str, Any] = client_glue.get_table(
+    client_glue = _utils.client("glue", session=boto3_session)
+    response = client_glue.get_table(
         **_catalog_id(
             catalog_id=catalog_id,
             **_transaction_id(
                 transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database, Name=table
             ),
         )
     )
     comments: Dict[str, str] = {}
     for c in response["Table"]["StorageDescriptor"]["Columns"]:
-        comments[c["Name"]] = c.get("Comment")
+        comments[c["Name"]] = c["Comment"]
     if "PartitionKeys" in response["Table"]:
         for p in response["Table"]["PartitionKeys"]:
-            comments[p["Name"]] = p.get("Comment")
+            comments[p["Name"]] = p["Comment"]
     return comments
 
 
 @apply_configs
 def get_table_versions(
     database: str, table: str, catalog_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
 ) -> List[Dict[str, Any]]:
@@ -1035,21 +1040,21 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> tables_versions = wr.catalog.get_table_versions(database="...", table="...")
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client("glue", session=boto3_session)
     paginator = client_glue.get_paginator("get_table_versions")
     versions: List[Dict[str, Any]] = []
     response_iterator = paginator.paginate(**_catalog_id(DatabaseName=database, TableName=table, catalog_id=catalog_id))
     for page in response_iterator:
         for tbl in page["TableVersions"]:
-            versions.append(tbl)
+            versions.append(cast(Dict[str, Any], tbl))
     return versions
 
 
 @apply_configs
 def get_table_number_of_versions(
     database: str, table: str, catalog_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
 ) -> int:
@@ -1074,14 +1079,14 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> num = wr.catalog.get_table_number_of_versions(database="...", table="...")
 
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     paginator = client_glue.get_paginator("get_table_versions")
     count: int = 0
     response_iterator = paginator.paginate(**_catalog_id(DatabaseName=database, TableName=table, catalog_id=catalog_id))
     for page in response_iterator:
         count += len(page["TableVersions"])
     return count
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/catalog/_utils.py` & `awswrangler-3.0.0rc3/awswrangler/catalog/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Utilities Module for AWS Glue Catalog."""
 import logging
 import re
 import unicodedata
 import warnings
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 import boto3
 import pandas as pd
 
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._config import apply_configs
 
+if TYPE_CHECKING:
+    from mypy_boto3_glue.type_defs import GetTableResponseTypeDef
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _catalog_id(catalog_id: Optional[str] = None, **kwargs: Any) -> Dict[str, Any]:
     if catalog_id is not None:
         kwargs["CatalogId"] = catalog_id
     return kwargs
@@ -35,15 +38,15 @@
 
 
 def _sanitize_name(name: str) -> str:
     name = "".join(c for c in unicodedata.normalize("NFD", name) if unicodedata.category(c) != "Mn")  # strip accents
     return re.sub("[^A-Za-z0-9_]+", "_", name).lower()  # Replacing non alphanumeric characters by underscore
 
 
-def _extract_dtypes_from_table_details(response: Dict[str, Any]) -> Dict[str, str]:
+def _extract_dtypes_from_table_details(response: "GetTableResponseTypeDef") -> Dict[str, str]:
     dtypes: Dict[str, str] = {}
     for col in response["Table"]["StorageDescriptor"]["Columns"]:
         dtypes[col["Name"]] = col["Type"]
     if "PartitionKeys" in response["Table"]:
         for par in response["Table"]["PartitionKeys"]:
             dtypes[par["Name"]] = par["Type"]
     return dtypes
@@ -79,15 +82,15 @@
         True if exists, otherwise False.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.catalog.does_table_exist(database='default', table='my_table')
     """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
+    client_glue = _utils.client(service_name="glue", session=boto3_session)
     try:
         client_glue.get_table(
             **_catalog_id(
                 catalog_id=catalog_id,
                 **_transaction_id(transaction_id=transaction_id, DatabaseName=database, Name=table),
             )
         )
@@ -208,15 +211,15 @@
     >>> df_normalized_rename = wr.catalog.sanitize_dataframe_columns_names(
             df=pd.DataFrame({"A": [1, 2], "a": [3, 4], "a_1": [4, 6]}), handle_duplicate_columns="rename"
         )
 
     """
     df.columns = [sanitize_column_name(x) for x in df.columns]
     df.index.names = [None if x is None else sanitize_column_name(x) for x in df.index.names]
-    if df.columns.duplicated().any():  # type: ignore
+    if df.columns.duplicated().any():  # type: ignore[attr-defined]
         if handle_duplicate_columns == "warn":
             warnings.warn(
                 "Duplicate columns were detected, consider using `handle_duplicate_columns='[drop|rename]'`",
                 UserWarning,
             )
         elif handle_duplicate_columns == "drop":
             df = drop_duplicated_columns(df)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/chime.py` & `awswrangler-3.0.0rc3/awswrangler/chime.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/cloudwatch.py` & `awswrangler-3.0.0rc3/awswrangler/quicksight/_describe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,249 @@
-"""CloudWatch Logs module."""
+"""Amazon QuickSight Describe Module."""
 
-import datetime
 import logging
-import time
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, Dict, Optional, cast
 
 import boto3
-import pandas as pd
 
-from awswrangler import _utils, exceptions
+from awswrangler import _utils, exceptions, sts
+from awswrangler.quicksight._get_list import get_dashboard_id, get_data_source_id, get_dataset_id
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
-_QUERY_WAIT_POLLING_DELAY: float = 0.2  # SECONDS
 
-
-def _validate_args(
-    start_timestamp: int,
-    end_timestamp: int,
-) -> None:
-    if start_timestamp < 0:
-        raise exceptions.InvalidArgument("`start_time` cannot be a negative value.")
-    if start_timestamp >= end_timestamp:
-        raise exceptions.InvalidArgumentCombination("`start_time` must be inferior to `end_time`.")
-
-
-def start_query(
-    query: str,
-    log_group_names: List[str],
-    start_time: datetime.datetime = datetime.datetime(year=1970, month=1, day=1, tzinfo=datetime.timezone.utc),
-    end_time: datetime.datetime = datetime.datetime.utcnow(),
-    limit: Optional[int] = None,
+def describe_dashboard(
+    name: Optional[str] = None,
+    dashboard_id: Optional[str] = None,
+    account_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
-) -> str:
-    """Run a query against AWS CloudWatchLogs Insights.
+) -> Dict[str, Any]:
+    """Describe a QuickSight dashboard by name or ID.
 
-    https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html
+    Note
+    ----
+    You must pass a not None ``name`` or ``dashboard_id`` argument.
 
     Parameters
     ----------
-    query : str
-        The query string.
-    log_group_names : str
-        The list of log groups to be queried. You can include up to 20 log groups.
-    start_time : datetime.datetime
-        The beginning of the time range to query.
-    end_time : datetime.datetime
-        The end of the time range to query.
-    limit : Optional[int]
-        The maximum number of log events to return in the query.
+    name : str, optional
+        Dashboard name.
+    dashboard_id : str, optional
+        Dashboard ID.
+    account_id : str, optional
+        If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
-    str
-        Query ID.
+    Dict[str, Any]
+        Dashboad Description.
 
     Examples
     --------
     >>> import awswrangler as wr
-    >>> query_id = wr.cloudwatch.start_query(
-    ...     log_group_names=["loggroup"],
-    ...     query="fields @timestamp, @message | sort @timestamp desc | limit 5",
-    ... )
-
+    >>> description = wr.quicksight.describe_dashboard(name="my-dashboard")
     """
-    _logger.debug("log_group_names: %s", log_group_names)
-    start_timestamp: int = int(1000 * start_time.timestamp())
-    end_timestamp: int = int(1000 * end_time.timestamp())
-    _logger.debug("start_timestamp: %s", start_timestamp)
-    _logger.debug("end_timestamp: %s", end_timestamp)
-    _validate_args(start_timestamp=start_timestamp, end_timestamp=end_timestamp)
-    args: Dict[str, Any] = {
-        "logGroupNames": log_group_names,
-        "startTime": start_timestamp,
-        "endTime": end_timestamp,
-        "queryString": query,
-    }
-    if limit is not None:
-        args["limit"] = limit
-    client_logs: boto3.client = _utils.client(service_name="logs", session=boto3_session)
-    response: Dict[str, Any] = client_logs.start_query(**args)
-    return cast(str, response["queryId"])
+    if (name is None) and (dashboard_id is None):
+        raise exceptions.InvalidArgument("You must pass a not None name or dashboard_id argument.")
+    if account_id is None:
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    if (dashboard_id is None) and (name is not None):
+        dashboard_id = get_dashboard_id(name=name, account_id=account_id, boto3_session=boto3_session)
+
+    client = _utils.client(service_name="quicksight", session=boto3_session)
+    dashboard_id = cast(str, dashboard_id)
+
+    response = client.describe_dashboard(AwsAccountId=account_id, DashboardId=dashboard_id)
+    return response["Dashboard"]  # type: ignore[return-value]
+
+
+def describe_data_source(
+    name: Optional[str] = None,
+    data_source_id: Optional[str] = None,
+    account_id: Optional[str] = None,
+    boto3_session: Optional[boto3.Session] = None,
+) -> Dict[str, Any]:
+    """Describe a QuickSight data source by name or ID.
 
+    Note
+    ----
+    You must pass a not None ``name`` or ``data_source_id`` argument.
 
-def wait_query(query_id: str, boto3_session: Optional[boto3.Session] = None) -> Dict[str, Any]:
-    """Wait query ends.
+    Parameters
+    ----------
+    name : str, optional
+        Data source name.
+    data_source_id : str, optional
+        Data source ID.
+    account_id : str, optional
+        If None, the account ID will be inferred from your boto3 session.
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
-    https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html
+    Returns
+    -------
+    Dict[str, Any]
+        Data source Description.
+
+    Examples
+    --------
+    >>> import awswrangler as wr
+    >>> description = wr.quicksight.describe_data_source("...")
+    """
+    if (name is None) and (data_source_id is None):
+        raise exceptions.InvalidArgument("You must pass a not None name or data_source_id argument.")
+    if account_id is None:
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    if (data_source_id is None) and (name is not None):
+        data_source_id = get_data_source_id(name=name, account_id=account_id, boto3_session=boto3_session)
+
+    client = _utils.client(service_name="quicksight", session=boto3_session)
+    data_source_id = cast(str, data_source_id)
+
+    response = client.describe_data_source(AwsAccountId=account_id, DataSourceId=data_source_id)
+    return response["DataSource"]  # type: ignore[return-value]
+
+
+def describe_data_source_permissions(
+    name: Optional[str] = None,
+    data_source_id: Optional[str] = None,
+    account_id: Optional[str] = None,
+    boto3_session: Optional[boto3.Session] = None,
+) -> Dict[str, Any]:
+    """Describe a QuickSight data source permissions by name or ID.
+
+    Note
+    ----
+    You must pass a not None ``name`` or ``data_source_id`` argument.
 
     Parameters
     ----------
-    query_id : str
-        Query ID.
+    name : str, optional
+        Data source name.
+    data_source_id : str, optional
+        Data source ID.
+    account_id : str, optional
+        If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     Dict[str, Any]
-        Query result payload.
+        Data source Permissions Description.
 
     Examples
     --------
     >>> import awswrangler as wr
-    >>> query_id = wr.cloudwatch.start_query(
-    ...     log_group_names=["loggroup"],
-    ...     query="fields @timestamp, @message | sort @timestamp desc | limit 5",
-    ... )
-    ... response = wr.cloudwatch.wait_query(query_id=query_id)
-
+    >>> description = wr.quicksight.describe_data_source_permissions("my-data-source")
     """
-    final_states: List[str] = ["Complete", "Failed", "Cancelled"]
-    client_logs: boto3.client = _utils.client(service_name="logs", session=boto3_session)
-    response: Dict[str, Any] = client_logs.get_query_results(queryId=query_id)
-    status: str = response["status"]
-    while status not in final_states:
-        time.sleep(_QUERY_WAIT_POLLING_DELAY)
-        response = client_logs.get_query_results(queryId=query_id)
-        status = response["status"]
-    _logger.debug("status: %s", status)
-    if status == "Failed":
-        raise exceptions.QueryFailed(f"query ID: {query_id}")
-    if status == "Cancelled":
-        raise exceptions.QueryCancelled(f"query ID: {query_id}")
-    return response
-
-
-def run_query(
-    query: str,
-    log_group_names: List[str],
-    start_time: datetime.datetime = datetime.datetime(year=1970, month=1, day=1, tzinfo=datetime.timezone.utc),
-    end_time: datetime.datetime = datetime.datetime.utcnow(),
-    limit: Optional[int] = None,
+    if (name is None) and (data_source_id is None):
+        raise exceptions.InvalidArgument("You must pass a not None name or data_source_id argument.")
+    if account_id is None:
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    if (data_source_id is None) and (name is not None):
+        data_source_id = get_data_source_id(name=name, account_id=account_id, boto3_session=boto3_session)
+
+    client = _utils.client(service_name="quicksight", session=boto3_session)
+    data_source_id = cast(str, data_source_id)
+
+    response = client.describe_data_source_permissions(AwsAccountId=account_id, DataSourceId=data_source_id)
+    return response["Permissions"]  # type: ignore[return-value]
+
+
+def describe_dataset(
+    name: Optional[str] = None,
+    dataset_id: Optional[str] = None,
+    account_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
-) -> List[List[Dict[str, str]]]:
-    """Run a query against AWS CloudWatchLogs Insights and wait the results.
+) -> Dict[str, Any]:
+    """Describe a QuickSight dataset by name or ID.
 
-    https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html
+    Note
+    ----
+    You must pass a not None ``name`` or ``dataset_id`` argument.
 
     Parameters
     ----------
-    query : str
-        The query string.
-    log_group_names : str
-        The list of log groups to be queried. You can include up to 20 log groups.
-    start_time : datetime.datetime
-        The beginning of the time range to query.
-    end_time : datetime.datetime
-        The end of the time range to query.
-    limit : Optional[int]
-        The maximum number of log events to return in the query.
+    name : str, optional
+        Dataset name.
+    dataset_id : str, optional
+        Dataset ID.
+    account_id : str, optional
+        If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
-    List[List[Dict[str, str]]]
-        Result.
+    Dict[str, Any]
+        Dataset Description.
 
     Examples
     --------
     >>> import awswrangler as wr
-    >>> result = wr.cloudwatch.run_query(
-    ...     log_group_names=["loggroup"],
-    ...     query="fields @timestamp, @message | sort @timestamp desc | limit 5",
-    ... )
-
+    >>> description = wr.quicksight.describe_dataset("my-dataset")
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    query_id: str = start_query(
-        query=query,
-        log_group_names=log_group_names,
-        start_time=start_time,
-        end_time=end_time,
-        limit=limit,
-        boto3_session=session,
-    )
-    response: Dict[str, Any] = wait_query(query_id=query_id, boto3_session=session)
-    return cast(List[List[Dict[str, str]]], response["results"])
-
-
-def read_logs(
-    query: str,
-    log_group_names: List[str],
-    start_time: datetime.datetime = datetime.datetime(year=1970, month=1, day=1, tzinfo=datetime.timezone.utc),
-    end_time: datetime.datetime = datetime.datetime.utcnow(),
-    limit: Optional[int] = None,
+    if (name is None) and (dataset_id is None):
+        raise exceptions.InvalidArgument("You must pass a not None name or dataset_id argument.")
+    if account_id is None:
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    if (dataset_id is None) and (name is not None):
+        dataset_id = get_dataset_id(name=name, account_id=account_id, boto3_session=boto3_session)
+
+    client = _utils.client(service_name="quicksight", session=boto3_session)
+    dataset_id = cast(str, dataset_id)
+
+    response = client.describe_data_set(AwsAccountId=account_id, DataSetId=dataset_id)
+    return response["DataSet"]  # type: ignore[return-value]
+
+
+def describe_ingestion(
+    ingestion_id: str,
+    dataset_name: Optional[str] = None,
+    dataset_id: Optional[str] = None,
+    account_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
-) -> pd.DataFrame:
-    """Run a query against AWS CloudWatchLogs Insights and convert the results to Pandas DataFrame.
+) -> Dict[str, Any]:
+    """Describe a QuickSight ingestion by ID.
 
-    https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/CWL_QuerySyntax.html
+    Note
+    ----
+    You must pass a not None value for ``dataset_name`` or ``dataset_id`` argument.
 
     Parameters
     ----------
-    query : str
-        The query string.
-    log_group_names : str
-        The list of log groups to be queried. You can include up to 20 log groups.
-    start_time : datetime.datetime
-        The beginning of the time range to query.
-    end_time : datetime.datetime
-        The end of the time range to query.
-    limit : Optional[int]
-        The maximum number of log events to return in the query.
+    ingestion_id : str
+        Ingestion ID.
+    dataset_name : str, optional
+        Dataset name.
+    dataset_id : str, optional
+        Dataset ID.
+    account_id : str, optional
+        If None, the account ID will be inferred from your boto3 session.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
-    pandas.DataFrame
-        Result as a Pandas DataFrame.
+    Dict[str, Any]
+        Ingestion Description.
 
     Examples
     --------
     >>> import awswrangler as wr
-    >>> df = wr.cloudwatch.read_logs(
-    ...     log_group_names=["loggroup"],
-    ...     query="fields @timestamp, @message | sort @timestamp desc | limit 5",
-    ... )
-
+    >>> description = wr.quicksight.describe_dataset(ingestion_id="...", dataset_name="...")
     """
-    results: List[List[Dict[str, str]]] = run_query(
-        query=query,
-        log_group_names=log_group_names,
-        start_time=start_time,
-        end_time=end_time,
-        limit=limit,
-        boto3_session=boto3_session,
-    )
-    pre_df: List[Dict[str, str]] = []
-    for row in results:
-        new_row: Dict[str, str] = {}
-        for col in row:
-            if col["field"].startswith("@"):
-                col_name = col["field"].replace("@", "", 1)
-            else:
-                col_name = col["field"]
-            new_row[col_name] = col["value"]
-        pre_df.append(new_row)
-    df: pd.DataFrame = pd.DataFrame(pre_df, dtype="string")
-    if "timestamp" in df.columns:
-        df["timestamp"] = pd.to_datetime(df["timestamp"])
-    return df
+    if (dataset_name is None) and (dataset_id is None):
+        raise exceptions.InvalidArgument("You must pass a not None name or dataset_id argument.")
+    if account_id is None:
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    if (dataset_id is None) and (dataset_name is not None):
+        dataset_id = get_dataset_id(name=dataset_name, account_id=account_id, boto3_session=boto3_session)
+
+    client = _utils.client(service_name="quicksight", session=boto3_session)
+    dataset_id = cast(str, dataset_id)
+
+    response = client.describe_ingestion(IngestionId=ingestion_id, AwsAccountId=account_id, DataSetId=dataset_id)
+    return response["Ingestion"]  # type: ignore[return-value]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/data_api/connector.py` & `awswrangler-3.0.0rc3/awswrangler/data_api/_connector.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/data_api/rds.py` & `awswrangler-3.0.0rc3/awswrangler/data_api/rds.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import uuid
 from typing import Any, Dict, List, Optional
 
 import boto3
 import pandas as pd
 
 from awswrangler import _utils
-from awswrangler.data_api import connector
+from awswrangler.data_api import _connector
 
 
-class RdsDataApi(connector.DataApiConnector):
+class RdsDataApi(_connector.DataApiConnector):
     """Provides access to the RDS Data API.
 
     Parameters
     ----------
     resource_arn: str
         ARN for the RDS resource.
     database: str
@@ -41,16 +41,16 @@
         backoff: float = 1.0,
         retries: int = 30,
         boto3_session: Optional[boto3.Session] = None,
     ) -> None:
         self.resource_arn = resource_arn
         self.database = database
         self.secret_arn = secret_arn
-        self.wait_config = connector.WaitConfig(sleep, backoff, retries)
-        self.client: boto3.client = _utils.client(service_name="rds-data", session=boto3_session)
+        self.wait_config = _connector.WaitConfig(sleep, backoff, retries)
+        self.client = _utils.client(service_name="rds-data", session=boto3_session)
         self.results: Dict[str, Dict[str, Any]] = {}
         logger: logging.Logger = logging.getLogger(__name__)
         super().__init__(self.client, logger)
 
     def _execute_statement(self, sql: str, database: Optional[str] = None) -> str:
         if database is None:
             database = self.database
@@ -84,15 +84,15 @@
                 )
                 time.sleep(sleep)
                 total_tries += 1
                 sleep *= self.wait_config.backoff
 
         if response is None:
             self.logger.exception("Maximum BadRequestException retries reached for query %s", sql)
-            raise last_exception  # type: ignore
+            raise last_exception  # type: ignore[misc]
 
         request_id: str = uuid.uuid4().hex
         self.results[request_id] = response
         return request_id
 
     def _get_statement_result(self, request_id: str) -> pd.DataFrame:
         try:
@@ -102,15 +102,15 @@
 
         if "records" not in result:
             return pd.DataFrame()
 
         rows: List[List[Any]] = []
         for record in result["records"]:
             row: List[Any] = [
-                connector.DataApiConnector._get_column_value(column)  # pylint: disable=protected-access
+                _connector.DataApiConnector._get_column_value(column)  # pylint: disable=protected-access
                 for column in record
             ]
             rows.append(row)
 
         column_names: List[str] = [column["name"] for column in result["columnMetadata"]]
         dataframe = pd.DataFrame(rows, columns=column_names)
         return dataframe
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/data_api/redshift.py` & `awswrangler-3.0.0rc3/awswrangler/data_api/redshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import time
 from typing import Any, Dict, List, Optional
 
 import boto3
 import pandas as pd
 
 from awswrangler import _utils
-from awswrangler.data_api import connector
+from awswrangler.data_api import _connector
 
 
-class RedshiftDataApi(connector.DataApiConnector):
+class RedshiftDataApi(_connector.DataApiConnector):
     """Provides access to a Redshift cluster via the Data API.
 
     Note
     ----
     When connecting to a standard Redshift cluster, `cluster_id` is used.
     When connecting to Redshift Serverless, `workgroup_name` is used. These two arguments are mutually exclusive.
 
@@ -53,15 +53,15 @@
         boto3_session: Optional[boto3.Session] = None,
     ) -> None:
         self.cluster_id = cluster_id
         self.database = database
         self.workgroup_name = workgroup_name
         self.secret_arn = secret_arn
         self.db_user = db_user
-        self.client: boto3.client = _utils.client(service_name="redshift-data", session=boto3_session)
+        self.client = _utils.client(service_name="redshift-data", session=boto3_session)
         self.waiter = RedshiftDataApiWaiter(self.client, sleep, backoff, retries)
         logger: logging.Logger = logging.getLogger(__name__)
         super().__init__(self.client, logger)
 
     def _validate_redshift_target(self) -> None:
         if self.database == "":
             raise ValueError("`database` must be set for connection")
@@ -86,15 +86,15 @@
 
         if self.cluster_id:
             redshift_target = {"ClusterIdentifier": self.cluster_id}
         elif self.workgroup_name:
             redshift_target = {"WorkgroupName": self.workgroup_name}
 
         self.logger.debug("Executing %s", sql)
-        response: Dict[str, Any] = self.client.execute_statement(
+        response = self.client.execute_statement(
             **redshift_target,
             Database=database,
             Sql=sql,
             **credentials,
         )
         return str(response["Id"])
 
@@ -110,15 +110,15 @@
 
         rows: List[List[Any]] = []
         column_metadata: List[Dict[str, str]]
         for response in response_iterator:
             column_metadata = response["ColumnMetadata"]
             for record in response["Records"]:
                 row: List[Any] = [
-                    connector.DataApiConnector._get_column_value(column)  # pylint: disable=protected-access
+                    _connector.DataApiConnector._get_column_value(column)  # pylint: disable=protected-access
                     for column in record
                 ]
                 rows.append(row)
 
         column_names: List[str] = [column["name"] for column in column_metadata]
         dataframe = pd.DataFrame(rows, columns=column_names)
         return dataframe
@@ -137,15 +137,15 @@
         Factor by which to increase the sleep between tries.
     retries: int
         Maximum number of tries.
     """
 
     def __init__(self, client: Any, sleep: float, backoff: float, retries: int) -> None:
         self.client = client
-        self.wait_config = connector.WaitConfig(sleep, backoff, retries)
+        self.wait_config = _connector.WaitConfig(sleep, backoff, retries)
         self.logger: logging.Logger = logging.getLogger(__name__)
 
     def wait(self, request_id: str) -> bool:
         """Wait for the `describe_statement` function of self.client to return a completed status.
 
         Parameters
         ----------
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/_core.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,26 +14,31 @@
 
 
 class RayLogger:
     """Create discrete Logger instance for Ray Tasks."""
 
     def __init__(
         self,
-        log_level: int = logging.DEBUG,
+        logging_level: int = logging.INFO,
         format: str = "%(asctime)s::%(levelname)-2s::%(name)s::%(message)s",  # pylint: disable=redefined-builtin
         datefmt: str = "%Y-%m-%d %H:%M:%S",
     ):
-        logging.basicConfig(level=log_level, format=format, datefmt=datefmt)
+        logging.basicConfig(level=logging_level, format=format, datefmt=datefmt)
 
     def get_logger(self, name: Union[str, Any] = None) -> Optional[logging.Logger]:
         """Return logger object."""
         return logging.getLogger(name)
 
 
-def ray_logger(function: Callable[..., Any]) -> Callable[..., Any]:
+@apply_configs
+def ray_logger(
+    function: Callable[..., Any],
+    configure_logging: bool = True,
+    logging_level: int = logging.INFO,
+) -> Callable[..., Any]:
     """
     Decorate callable to add RayLogger.
 
     Parameters
     ----------
     function : Callable[..., Any]
         Callable as input to decorator.
@@ -41,15 +46,16 @@
     Returns
     -------
     Callable[..., Any]
     """
 
     @wraps(function)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
-        RayLogger().get_logger(name=function.__name__)
+        if configure_logging:
+            RayLogger(logging_level=logging_level).get_logger(name=function.__name__)
         return function(*args, **kwargs)
 
     return wrapper
 
 
 def ray_remote(**options: Any) -> Callable[..., Any]:
     """
@@ -82,15 +88,15 @@
         function = getattr(function, "_source_func", function)
 
         @wraps(function)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
             remote_fn = ray.remote(ray_logger(function))
             if options:
                 remote_fn = remote_fn.options(**options)
-            return remote_fn.remote(*args, **kwargs)  # type: ignore
+            return remote_fn.remote(*args, **kwargs)
 
         return wrapper
 
     return remote_decorator
 
 
 def ray_get(futures: Union["ray.ObjectRef[Any]", List["ray.ObjectRef[Any]"]]) -> Any:
@@ -103,25 +109,27 @@
         List of Ray futures
 
     Returns
     -------
     List[Any]
     """
     if engine.get() == EngineEnum.RAY:
-        return ray.get(futures)
+        return ray.get(futures)  # type: ignore[attr-defined]
     return futures
 
 
 @apply_configs
 def initialize_ray(
     address: Optional[str] = None,
     redis_password: Optional[str] = None,
     ignore_reinit_error: bool = True,
     include_dashboard: Optional[bool] = False,
+    configure_logging: bool = True,
     log_to_driver: bool = False,
+    logging_level: int = logging.INFO,
     object_store_memory: Optional[int] = None,
     cpu_count: Optional[int] = None,
     gpu_count: Optional[int] = None,
 ) -> None:
     """
     Connect to an existing Ray cluster or start one and connect to it.
 
@@ -131,16 +139,20 @@
         Address of the Ray cluster to connect to, by default None
     redis_password : Optional[str]
         Password to the Redis cluster, by default None
     ignore_reinit_error : bool
         If true, Ray suppress errors from calling ray.init() twice, by default True
     include_dashboard : Optional[bool]
         Boolean flag indicating whether or not to start the Ray dashboard, by default False
+    configure_logging : Optional[bool]
+        Boolean flag indicating whether or not to enable logging, by default True
     log_to_driver : bool
         Boolean flag to enable routing of all worker logs to the driver, by default False
+    logging_level : int
+        Logging level, defaults to logging.INFO. Ignored unless "configure_logging" is True
     object_store_memory : Optional[int]
         The amount of memory (in bytes) to start the object store with, by default None
     cpu_count : Optional[int]
         Number of CPUs to assign to each raylet, by default None
     gpu_count : Optional[int]
         Number of GPUs to assign to each raylet, by default None
     """
@@ -153,27 +165,31 @@
 
         if address:
             _logger.info("Connecting to a Ray cluster at: %s", address)
             ray.init(
                 address=address,
                 include_dashboard=include_dashboard,
                 ignore_reinit_error=ignore_reinit_error,
+                configure_logging=configure_logging,
                 log_to_driver=log_to_driver,
+                logging_level=logging_level,
             )
         else:
             ray_runtime_env_vars = [
                 "__MODIN_AUTOIMPORT_PANDAS__",
             ]
 
             ray_init_kwargs = {
                 "num_cpus": cpu_count,
                 "num_gpus": gpu_count,
                 "include_dashboard": include_dashboard,
                 "ignore_reinit_error": ignore_reinit_error,
+                "configure_logging": configure_logging,
                 "log_to_driver": log_to_driver,
+                "logging_level": logging_level,
                 "object_store_memory": object_store_memory,
                 "_redis_password": redis_password,
                 "_memory": object_store_memory,
                 "runtime_env": {
                     "env_vars": {var: os.environ.get(var) for var in ray_runtime_env_vars if os.environ.get(var)}
                 },
             }
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/_core.pyi` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/_core.pyi`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/_pool.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/_pool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Ray Threading Module (PRIVATE)."""
 
 import itertools
 import logging
-from typing import Any, Callable, List
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, TypeVar
 
-import boto3
+if TYPE_CHECKING:
+    from botocore.client import BaseClient
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
+MapOutputType = TypeVar("MapOutputType")
+
 
 class _RayPoolExecutor:
     def __init__(self) -> None:
         pass
 
-    def map(self, func: Callable[..., Any], _: boto3.Session, *args: Any) -> List[Any]:
+    def map(self, func: Callable[..., MapOutputType], _: Optional["BaseClient"], *args: Any) -> List[MapOutputType]:
         """Map func and return ray futures."""
         _logger.debug("Ray map: %s", func)
-        # Discard boto3.Session object & return futures
+        # Discard boto3 client
         return list(func(*arg) for arg in zip(itertools.repeat(None), *args))
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/_register.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/_register.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,63 @@
 """Ray and Modin registered methods (PRIVATE)."""
 # pylint: disable=import-outside-toplevel
 from awswrangler._data_types import pyarrow_types_from_pandas
 from awswrangler._distributed import MemoryFormatEnum, engine, memory_format
-from awswrangler._utils import is_pandas_frame, split_pandas_frame, table_refs_to_df
+from awswrangler._utils import copy_df_shallow, is_pandas_frame, split_pandas_frame, table_refs_to_df
 from awswrangler.distributed.ray import ray_remote
+from awswrangler.distributed.ray.s3._list import _list_objects_s3fs
+from awswrangler.distributed.ray.s3._read_parquet import _read_parquet_metadata_file_distributed
+from awswrangler.dynamodb._read import _read_scan
 from awswrangler.lakeformation._read import _get_work_unit_results
+from awswrangler.s3._copy import _copy_objects
 from awswrangler.s3._delete import _delete_objects
+from awswrangler.s3._describe import _describe_object
+from awswrangler.s3._list import _list_objects_paginate
 from awswrangler.s3._read_parquet import _read_parquet, _read_parquet_metadata_file
 from awswrangler.s3._read_text import _read_text
 from awswrangler.s3._select import _select_object_content, _select_query
 from awswrangler.s3._wait import _wait_object_batch
 from awswrangler.s3._write_dataset import _to_buckets, _to_partitions
 from awswrangler.s3._write_parquet import _to_parquet
 from awswrangler.s3._write_text import _to_text
 from awswrangler.timestream import _write_batch, _write_df
 
 
 def register_ray() -> None:
     """Register dispatched Ray and Modin (on Ray) methods."""
     for func in [
         _get_work_unit_results,
+        _copy_objects,
+        _describe_object,
         _delete_objects,
-        _read_parquet_metadata_file,
+        _read_scan,
         _select_query,
         _select_object_content,
         _wait_object_batch,
     ]:
         # Schedule for maximum concurrency
         engine.register_func(func, ray_remote(scheduling_strategy="SPREAD")(func))
 
     for func in [
         _write_batch,
         _write_df,
     ]:
         engine.register_func(func, ray_remote()(func))
 
+    for o_f, d_f in {
+        _list_objects_paginate: _list_objects_s3fs,
+        _read_parquet_metadata_file: ray_remote()(_read_parquet_metadata_file_distributed),
+    }.items():
+        engine.register_func(o_f, d_f)  # type: ignore[arg-type]
+
     if memory_format.get() == MemoryFormatEnum.MODIN:
         from awswrangler.distributed.ray.modin._data_types import pyarrow_types_from_pandas_distributed
         from awswrangler.distributed.ray.modin._utils import (
             _arrow_refs_to_df,
+            _copy_modin_df_shallow,
             _is_pandas_or_modin_frame,
             _split_modin_frame,
         )
         from awswrangler.distributed.ray.modin.s3._read_parquet import _read_parquet_distributed
         from awswrangler.distributed.ray.modin.s3._read_text import _read_text_distributed
         from awswrangler.distributed.ray.modin.s3._write_dataset import (
             _to_buckets_distributed,
@@ -55,12 +70,13 @@
             pyarrow_types_from_pandas: pyarrow_types_from_pandas_distributed,
             _read_parquet: _read_parquet_distributed,
             _read_text: _read_text_distributed,
             _to_buckets: _to_buckets_distributed,
             _to_parquet: _to_parquet_distributed,
             _to_partitions: _to_partitions_distributed,
             _to_text: _to_text_distributed,
+            copy_df_shallow: _copy_modin_df_shallow,
             is_pandas_frame: _is_pandas_or_modin_frame,
             split_pandas_frame: _split_modin_frame,
             table_refs_to_df: _arrow_refs_to_df,
         }.items():
-            engine.register_func(o_f, d_f)  # type: ignore
+            engine.register_func(o_f, d_f)  # type: ignore[arg-type]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/__init__.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 """Ray Datasources Module."""
 
 from awswrangler.distributed.ray.datasources.arrow_csv_datasource import ArrowCSVDatasource
+from awswrangler.distributed.ray.datasources.arrow_json_datasource import ArrowJSONDatasource
+from awswrangler.distributed.ray.datasources.arrow_parquet_base_datasource import ArrowParquetBaseDatasource
 from awswrangler.distributed.ray.datasources.arrow_parquet_datasource import ArrowParquetDatasource
 from awswrangler.distributed.ray.datasources.pandas_file_based_datasource import UserProvidedKeyBlockWritePathProvider
 from awswrangler.distributed.ray.datasources.pandas_text_datasource import (
     PandasCSVDataSource,
     PandasFWFDataSource,
     PandasJSONDatasource,
     PandasTextDatasource,
 )
 
 __all__ = [
     "ArrowCSVDatasource",
+    "ArrowJSONDatasource",
+    "ArrowParquetBaseDatasource",
     "ArrowParquetDatasource",
     "PandasCSVDataSource",
     "PandasFWFDataSource",
     "PandasJSONDatasource",
     "PandasTextDatasource",
     "UserProvidedKeyBlockWritePathProvider",
 ]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_csv_datasource.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class ArrowCSVDatasource(PandasFileBasedDatasource):  # pylint: disable=abstract-method
     """CSV datasource, for reading and writing CSV files using PyArrow."""
 
     _FILE_EXTENSION = "csv"
 
-    def _read_stream(  # type: ignore  # pylint: disable=arguments-differ
+    def _read_stream(  # type: ignore[override]  # pylint: disable=arguments-differ
         self,
         f: pa.NativeFile,
         path: str,
         path_root: str,
         dataset: bool,
         **reader_args: Any,
     ) -> Iterator[pa.Table]:
@@ -52,17 +52,17 @@
                     )
 
                 yield table
 
             except StopIteration:
                 return
 
-    def _write_block(  # type: ignore  # pylint: disable=arguments-differ
+    def _write_block(  # type: ignore[override]  # pylint: disable=arguments-differ
         self,
         f: pa.NativeFile,
         block: BlockAccessor[Any],
-        **writer_args,
+        **writer_args: Any,
     ) -> None:
         write_options_dict = writer_args.get("write_options", {})
         write_options = csv.WriteOptions(**write_options_dict)
 
         csv.write_csv(block.to_arrow(), f, write_options)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/arrow_parquet_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 
 # fs required to implicitly trigger S3 subsystem initialization
 import pyarrow.fs  # noqa: F401 pylint: disable=unused-import
 import ray
 from pyarrow.dataset import ParquetFileFragment
 from pyarrow.lib import Schema
 from ray import cloudpickle
+from ray.data._internal.output_buffer import BlockOutputBuffer
 from ray.data.block import Block, BlockAccessor
 from ray.data.context import DatasetContext
-from ray.data.dataset import BlockOutputBuffer  # type: ignore
 from ray.data.datasource import Reader, ReadTask
 from ray.data.datasource.file_based_datasource import _resolve_paths_and_filesystem
-from ray.data.datasource.file_meta_provider import _handle_read_os_error  # type: ignore
-from ray.data.datasource.file_meta_provider import DefaultParquetMetadataProvider, ParquetMetadataProvider
+from ray.data.datasource.file_meta_provider import (
+    DefaultParquetMetadataProvider,
+    ParquetMetadataProvider,
+    _handle_read_os_error,
+)
 
 from awswrangler._arrow import _add_table_partitions, _df_to_table
 from awswrangler.distributed.ray import ray_remote
-from awswrangler.distributed.ray.datasources.pandas_file_based_datasource import PandasFileBasedDatasource
+from awswrangler.distributed.ray.datasources.arrow_parquet_base_datasource import ArrowParquetBaseDatasource
 from awswrangler.s3._write import _COMPRESSION_2_EXT
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 # The number of rows to read per batch. This is sized to generate 10MiB batches
 # for rows about 1KiB in size.
 PARQUET_READER_ROW_BATCH_SIZE = 100000
@@ -65,31 +68,29 @@
 PARQUET_ENCODING_RATIO_ESTIMATE_MAX_NUM_SAMPLES = 10
 
 # The number of rows to read from each file for sampling. Try to keep it low to avoid
 # reading too much data into memory.
 PARQUET_ENCODING_RATIO_ESTIMATE_NUM_ROWS = 5
 
 
-class ArrowParquetDatasource(PandasFileBasedDatasource):  # pylint: disable=abstract-method
+class ArrowParquetDatasource(ArrowParquetBaseDatasource):  # pylint: disable=abstract-method
     """(AWS SDK for pandas) Parquet datasource, for reading and writing Parquet files.
 
     The following are the changes to the original Ray implementation:
     1. Added handling of additional parameters `dtype`, `index`, `compression` and added the ability
        to pass through additional `pyarrow_additional_kwargs` and `s3_additional_kwargs` for writes.
     3. Added `dataset` and `path_root` parameters to allow user to control loading partitions
        relative to the root S3 prefix.
     """
 
-    _FILE_EXTENSION = "parquet"
-
     def create_reader(self, **kwargs: Dict[str, Any]) -> Reader[Any]:
         """Return a Reader for the given read arguments."""
-        return _ArrowParquetDatasourceReader(**kwargs)  # type: ignore
+        return _ArrowParquetDatasourceReader(**kwargs)  # type: ignore[arg-type]
 
-    def _write_block(  # type: ignore  # pylint: disable=arguments-differ, arguments-renamed, unused-argument
+    def _write_block(  # type: ignore[override]  # pylint: disable=arguments-differ, arguments-renamed, unused-argument
         self,
         f: "pyarrow.NativeFile",
         block: BlockAccessor[Any],
         pandas_kwargs: Optional[Dict[str, Any]],
         **writer_args: Any,
     ) -> None:
         """Write a block to S3."""
@@ -106,23 +107,23 @@
             f,
             compression=compression,
             **pyarrow_additional_kwargs,
         )
 
     def _get_file_suffix(self, file_format: str, compression: Optional[str]) -> str:
         if compression is not None:
-            return f"{_COMPRESSION_2_EXT.get(compression)[1:]}.{file_format}"  # type: ignore
+            return f"{_COMPRESSION_2_EXT.get(compression)[1:]}.{file_format}"  # type: ignore[index]
         return file_format
 
 
 # TODO(ekl) this is a workaround for a pyarrow serialization bug, where serializing a
 # raw pyarrow file fragment causes S3 network calls.
 class _SerializedPiece:
     def __init__(self, frag: ParquetFileFragment):
-        self._data = cloudpickle.dumps(  # type: ignore
+        self._data = cloudpickle.dumps(  # type: ignore[attr-defined]
             (frag.format, frag.path, frag.filesystem, frag.partition_expression)
         )
 
     def deserialize(self) -> ParquetFileFragment:
         """Implicitly trigger S3 subsystem initialization by importing pyarrow.fs."""
         import pyarrow.fs  # noqa: F401 pylint: disable=unused-import
 
@@ -177,15 +178,15 @@
                 # at slightly different time
                 min_interval = 1 + random.random()
             # exponential backoff at
             # 1, 2, 4, 8, 16, 32, 64
             time.sleep(min_interval)
             min_interval = min_interval * 2
             final_exception = e
-    raise final_exception  # type: ignore
+    raise final_exception  # type: ignore[misc]
 
 
 class _ArrowParquetDatasourceReader(Reader[Any]):  # pylint: disable=too-many-instance-attributes
     def __init__(
         self,
         paths: Union[str, List[str]],
         filesystem: Optional["pyarrow.fs.FileSystem"] = None,
@@ -212,15 +213,15 @@
         if columns:
             schema = pa.schema([schema.field(column) for column in columns], schema.metadata)
 
         if _block_udf is not None:
             # Try to infer dataset schema by passing dummy table through UDF.
             dummy_table = schema.empty_table()
             try:
-                inferred_schema = _block_udf(dummy_table).schema  # type: ignore
+                inferred_schema = _block_udf(dummy_table).schema  # type: ignore[union-attr]
                 inferred_schema = inferred_schema.with_metadata(schema.metadata)
             except Exception:  # pylint: disable=broad-except
                 _logger.debug(
                     "Failed to infer schema of dataset by passing dummy table "
                     "through UDF due to the following exception:",
                     exc_info=True,
                 )
@@ -244,15 +245,15 @@
     def estimate_inmemory_data_size(self) -> Optional[int]:
         """Estimate data size."""
         total_size: int = 0
         for file_metadata in self._metadata:
             for row_group_idx in range(file_metadata.num_row_groups):
                 row_group_metadata = file_metadata.row_group(row_group_idx)
                 total_size += row_group_metadata.total_byte_size
-        return total_size * self._encoding_ratio  # type: ignore
+        return total_size * self._encoding_ratio  # type: ignore[return-value]
 
     def get_read_tasks(self, parallelism: int) -> List[ReadTask]:
         """Override the base class FileBasedDatasource.get_read_tasks().
 
         Required in order to leverage pyarrow's ParquetDataset abstraction,
         which simplifies partitioning logic. We still use
         FileBasedDatasource's write side (do_write), however.
@@ -278,15 +279,15 @@
                 pieces=pieces,
                 prefetched_metadata=metadata,
             )
             if meta.size_bytes is not None:
                 meta.size_bytes = int(meta.size_bytes * self._encoding_ratio)
             read_tasks.append(
                 ReadTask(
-                    lambda p=serialized_pieces: _read_pieces(  # type: ignore
+                    lambda p=serialized_pieces: _read_pieces(  # type: ignore[misc]
                         block_udf,
                         reader_args,
                         columns,
                         schema,
                         p,
                     ),
                     meta,
@@ -329,32 +330,27 @@
         sample_ratios = ray.get(futures)
         ratio = np.mean(sample_ratios)
 
         sampling_duration = time.perf_counter() - start_time
         if sampling_duration > 5:
             _logger.info("Parquet input size estimation took %s seconds.", round(sampling_duration, 2))
         _logger.debug("Estimated Parquet encoding ratio from sampling is %s.", ratio)
-        return max(ratio, PARQUET_ENCODING_RATIO_ESTIMATE_LOWER_BOUND)  # type: ignore
+        return max(ratio, PARQUET_ENCODING_RATIO_ESTIMATE_LOWER_BOUND)  # type: ignore[no-any-return]
 
 
 # (AWS SDK for pandas) The following are the changes to the original ray implementation:
 # 1. Use _add_table_partitions to add partition columns. The behavior is controlled by Pandas SDK
 #    native `dataset` parameter. The partitions are loaded relative to the `path_root` prefix.
 def _read_pieces(
     block_udf: Optional[Callable[[Block[Any]], Block[Any]]],
     reader_args: Any,
     columns: Optional[List[str]],
     schema: Optional[Union[type, "pyarrow.lib.Schema"]],
     serialized_pieces: List[_SerializedPiece],
 ) -> Iterator["pyarrow.Table"]:
-    # This import is necessary to load the tensor extension type.
-    from ray.data.extensions.tensor_extension import (  # type: ignore # noqa: F401, E501 # pylint: disable=import-outside-toplevel, unused-import
-        ArrowTensorType,
-    )
-
     # Deserialize after loading the filesystem class.
     pieces: List[ParquetFileFragment] = _deserialize_pieces_with_retry(serialized_pieces)
 
     # Ensure that we're reading at least one dataset fragment.
     assert len(pieces) > 0
 
     import pyarrow as pa  # pylint: disable=import-outside-toplevel
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_file_based_datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         super().__init__()
 
         self._write_paths: List[str] = []
 
     def _read_file(self, f: pyarrow.NativeFile, path: str, **reader_args: Any) -> pd.DataFrame:
         raise NotImplementedError()
 
-    def do_write(  # type: ignore  # pylint: disable=arguments-differ
+    def do_write(  # type: ignore[override]  # pylint: disable=arguments-differ
         self,
         blocks: List[ObjectRef[pd.DataFrame]],
         metadata: List[BlockMetadata],
         path: str,
         dataset_uuid: str,
         filesystem: Optional[pyarrow.fs.FileSystem] = None,
         try_create_dir: bool = True,
@@ -80,16 +80,14 @@
         if pandas_kwargs is None:
             pandas_kwargs = {}
 
         if not compression:
             compression = pandas_kwargs.get("compression")
 
         def write_block(write_path: str, block: pd.DataFrame) -> str:
-            _logger.debug("Writing %s file.", write_path)
-
             if _block_udf is not None:
                 block = _block_udf(block)
 
             with open_s3_object(
                 path=write_path,
                 mode=mode,
                 use_threads=False,
@@ -133,22 +131,27 @@
         f: "pyarrow.NativeFile",
         block: BlockAccessor[Any],
         writer_args_fn: Callable[[], Dict[str, Any]] = lambda: {},
         **writer_args: Any,
     ) -> None:
         raise NotImplementedError("Subclasses of PandasFileBasedDatasource must implement _write_block().")
 
+    # Note: this callback function is called once by the main thread after
+    # [all write tasks complete](https://github.com/ray-project/ray/blob/ray-2.3.0/python/ray/data/dataset.py#L2716)
+    # and is meant to be used for singular actions like
+    # [committing a transaction](https://docs.ray.io/en/latest/data/api/doc/ray.data.Datasource.html).
+    # As deceptive as it may look, there is no race condition here.
     def on_write_complete(self, write_results: List[Any], **_: Any) -> None:
-        """Execute callback on write complete."""
+        """Execute callback after all write tasks complete."""
         _logger.debug("Write complete %s.", write_results)
 
         # Collect and return all write task paths
         self._write_paths.extend(write_results)
 
     def on_write_failed(self, write_results: List[ObjectRef[Any]], error: Exception, **_: Any) -> None:
-        """Execute callback on write failed."""
+        """Execute callback after write tasks fail."""
         _logger.debug("Write failed %s.", write_results)
         raise error
 
     def get_write_paths(self) -> List[str]:
         """Return S3 paths of where the results have been written."""
         return self._write_paths
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/datasources/pandas_text_datasource.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/datasources/pandas_text_datasource.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,21 +29,21 @@
         super().__init__()
 
         self.read_text_func = read_text_func
         self.write_text_func = write_text_func
 
         self._write_paths: List[str] = []
 
-    def _read_stream(  # type: ignore  # pylint: disable=arguments-differ
+    def _read_stream(  # type: ignore[override]  # pylint: disable=arguments-differ
         self,
         f: pyarrow.NativeFile,  # Refactor reader to use wr.open_s3_object
         path: str,
         path_root: str,
         dataset: bool,
-        version_ids: Dict[str, Optional[str]],
+        version_ids: Optional[Dict[str, str]],
         s3_additional_kwargs: Optional[Dict[str, str]],
         pandas_kwargs: Optional[Dict[str, Any]],
         **reader_args: Any,
     ) -> Iterator[pd.DataFrame]:
         read_text_func = self.read_text_func
 
         if not s3_additional_kwargs:
@@ -55,58 +55,58 @@
         s3_path = f"s3://{path}"
         yield from _read_text_chunked(
             path=s3_path,
             chunksize=READER_ROW_BATCH_SIZE,
             parser_func=read_text_func,
             path_root=path_root,
             dataset=dataset,
-            boto3_session=None,
+            s3_client=None,
             pandas_kwargs=pandas_kwargs,
             s3_additional_kwargs=s3_additional_kwargs,
             use_threads=False,
-            version_id=version_ids.get(s3_path),
+            version_id=version_ids.get(s3_path) if version_ids else None,
         )
 
     def _read_file(self, f: pyarrow.NativeFile, path: str, **reader_args: Any) -> pd.DataFrame:
         raise NotImplementedError()
 
-    def _write_block(  # type: ignore  # pylint: disable=arguments-differ, arguments-renamed
+    def _write_block(  # type: ignore[override]  # pylint: disable=arguments-differ, arguments-renamed
         self,
         f: io.TextIOWrapper,
         block: BlockAccessor[Any],
         pandas_kwargs: Optional[Dict[str, Any]],
         **writer_args: Any,
     ) -> None:
         write_text_func = self.write_text_func
 
         if not pandas_kwargs:
             pandas_kwargs = {}
 
-        write_text_func(block.to_pandas(), f, **pandas_kwargs)  # type: ignore
+        write_text_func(block.to_pandas(), f, **pandas_kwargs)  # type: ignore[misc]
 
 
 class PandasCSVDataSource(PandasTextDatasource):  # pylint: disable=abstract-method
     """Pandas CSV datasource, for reading and writing CSV files using Pandas."""
 
     _FILE_EXTENSION = "csv"
 
     def __init__(self) -> None:
         super().__init__(pd.read_csv, pd.DataFrame.to_csv)
 
-    def _read_stream(  # type: ignore
+    def _read_stream(  # type: ignore[override]
         self,
         f: pyarrow.NativeFile,
         path: str,
         path_root: str,
         dataset: bool,
-        version_ids: Dict[str, Optional[str]],
+        version_ids: Optional[Dict[str, str]],
         s3_additional_kwargs: Optional[Dict[str, str]],
         pandas_kwargs: Dict[str, Any],
         **reader_args: Any,
-    ) -> Iterator[pd.DataFrame]:  # type: ignore
+    ) -> Iterator[pd.DataFrame]:
         pandas_header_arg = pandas_kwargs.get("header", "infer")
         pandas_names_arg = pandas_kwargs.get("names", None)
 
         if pandas_header_arg is None and not pandas_names_arg:
             raise exceptions.InvalidArgumentCombination(
                 "Distributed read_csv cannot read CSV files without header, or a `names` parameter."
             )
@@ -136,25 +136,25 @@
     """Pandas JSON datasource, for reading and writing JSON files using Pandas."""
 
     _FILE_EXTENSION = "json"
 
     def __init__(self) -> None:
         super().__init__(pd.read_json, pd.DataFrame.to_json)
 
-    def _read_stream(  # type: ignore
+    def _read_stream(  # type: ignore[override]
         self,
         f: pyarrow.NativeFile,
         path: str,
         path_root: str,
         dataset: bool,
-        version_ids: Dict[str, Optional[str]],
+        version_ids: Optional[Dict[str, str]],
         s3_additional_kwargs: Optional[Dict[str, str]],
         pandas_kwargs: Dict[str, Any],
         **reader_args: Any,
-    ) -> Iterator[pd.DataFrame]:  # type: ignore
+    ) -> Iterator[pd.DataFrame]:
         read_text_func = self.read_text_func
 
         pandas_lines = pandas_kwargs.get("lines", False)
         if pandas_lines:
             yield from super()._read_stream(
                 f,
                 path,
@@ -168,12 +168,12 @@
         else:
             s3_path = f"s3://{path}"
             yield _read_text_file(
                 path=s3_path,
                 parser_func=read_text_func,
                 path_root=path_root,
                 dataset=dataset,
-                boto3_session=None,
+                s3_client=None,
                 pandas_kwargs=pandas_kwargs,
                 s3_additional_kwargs=s3_additional_kwargs,
-                version_id=version_ids.get(s3_path),
+                version_id=version_ids.get(s3_path) if version_ids else None,
             )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/_core.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Modin on Ray Core module (PRIVATE)."""
 # pylint: disable=import-outside-toplevel
 import logging
 from functools import wraps
-from typing import Any, Callable, Optional
+from typing import Any, Callable, Optional, TypeVar
 
 import numpy as np
 import pandas as pd
 from modin.distributed.dataframe.pandas import from_partitions, unwrap_partitions
 from modin.pandas import DataFrame as ModinDataFrame
 
 _logger: logging.Logger = logging.getLogger(__name__)
@@ -26,15 +26,18 @@
     bool
     """
     # Unwrap partitions as they are currently stored (axis=None)
     partitions_shape = np.array(unwrap_partitions(df)).shape
     return partitions_shape[1] == 1
 
 
-def modin_repartition(function: Callable[..., Any]) -> Callable[..., Any]:
+FunctionType = TypeVar("FunctionType", bound=Callable[..., Any])
+
+
+def modin_repartition(function: FunctionType) -> FunctionType:
     """
     Decorate callable to repartition Modin data frame.
 
     By default, repartition along row (axis=0) axis.
     This avoids a situation where columns are split along multiple blocks.
 
     Parameters
@@ -68,8 +71,8 @@
                     "each partition can be processed independently."
                 )
                 axis = 0
             if axis is not None:
                 df = from_partitions(unwrap_partitions(df, axis=axis), axis=axis, row_lengths=row_lengths)
         return function(df, *args, **kwargs)
 
-    return wrapper
+    return wrapper  # type: ignore[return-value]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/_data_types.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/_data_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Internal (private) Data Types Module."""
 from typing import Dict, List, Optional
 
 import modin.pandas as pd
 import pyarrow as pa
-import ray
 
 from awswrangler._data_types import pyarrow_types_from_pandas
 from awswrangler.distributed.ray import ray_get, ray_remote
+from awswrangler.distributed.ray.modin._utils import _ray_dataset_from_df
 
 
 def pyarrow_types_from_pandas_distributed(
     df: pd.DataFrame, index: bool, ignore_cols: Optional[List[str]] = None, index_left: bool = False
 ) -> Dict[str, pa.DataType]:
     """Extract the related Pyarrow data types from a pandas DataFrame."""
     func = ray_remote()(pyarrow_types_from_pandas)
-    first_block_object_ref = ray.data.from_modin(df).get_internal_block_refs()[0]
-    return ray_get(  # type: ignore
+    first_block_object_ref = _ray_dataset_from_df(df).get_internal_block_refs()[0]
+    return ray_get(  # type: ignore[no-any-return]
         func(
             df=first_block_object_ref,
             index=index,
             ignore_cols=ignore_cols,
             index_left=index_left,
         )
     )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_read_text.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_read_text_core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,117 @@
-"""Modin on Ray S3 read text module (PRIVATE)."""
+"""Amazon S3 Read Core Module (PRIVATE)."""
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
-import boto3
-import modin.pandas as pd
-from pyarrow import csv
-from ray.data import read_datasource
+import botocore.exceptions
+import pandas as pd
+import pandas.io.parsers
+from pandas.io.common import infer_compression
 
 from awswrangler import exceptions
-from awswrangler.distributed.ray.datasources import (
-    ArrowCSVDatasource,
-    PandasCSVDataSource,
-    PandasFWFDataSource,
-    PandasJSONDatasource,
-)
-from awswrangler.distributed.ray.modin._utils import ParamConfig, _check_parameters, _to_modin
+from awswrangler.s3._fs import open_s3_object
+from awswrangler.s3._read import _apply_partitions
 
-_logger: logging.Logger = logging.getLogger(__name__)
-
-_CSV_SUPPORTED_PARAMS = {
-    "sep": ParamConfig(default=","),
-    "delimiter": ParamConfig(default=","),
-    "quotechar": ParamConfig(default='"'),
-    "doublequote": ParamConfig(default=True),
-}
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
 
+_logger: logging.Logger = logging.getLogger(__name__)
 
-def _parse_csv_configuration(
-    pandas_kwargs: Dict[str, Any],
-) -> Tuple[csv.ReadOptions, csv.ParseOptions, csv.ConvertOptions]:
-    _check_parameters(pandas_kwargs, _CSV_SUPPORTED_PARAMS)
 
-    read_options = csv.ReadOptions(
-        use_threads=False,
+def _get_read_details(path: str, pandas_kwargs: Dict[str, Any]) -> Tuple[str, Optional[str], Optional[str]]:
+    if pandas_kwargs.get("compression", "infer") == "infer":
+        pandas_kwargs["compression"] = infer_compression(path, compression="infer")
+    mode: str = (
+        "r" if pandas_kwargs.get("compression") is None and pandas_kwargs.get("encoding_errors") != "ignore" else "rb"
     )
-    parse_options = csv.ParseOptions(
-        delimiter=pandas_kwargs.get("sep", _CSV_SUPPORTED_PARAMS["sep"].default),
-        quote_char=pandas_kwargs.get("quotechar", _CSV_SUPPORTED_PARAMS["quotechar"].default),
-        double_quote=pandas_kwargs.get("doublequote", _CSV_SUPPORTED_PARAMS["doublequote"].default),
-    )
-    convert_options = csv.ConvertOptions()
-
-    return read_options, parse_options, convert_options
+    encoding: Optional[str] = pandas_kwargs.get("encoding", "utf-8")
+    newline: Optional[str] = pandas_kwargs.get("lineterminator", None)
+    return mode, encoding, newline
 
 
-def _parse_configuration(
-    file_format: str,
-    version_ids: Dict[str, Optional[str]],
-    s3_additional_kwargs: Optional[Dict[str, str]],
+def _read_text_chunked(
+    path: str,
+    chunksize: int,
+    parser_func: Callable[..., pd.DataFrame],
+    path_root: Optional[str],
+    s3_client: Optional["S3Client"],
     pandas_kwargs: Dict[str, Any],
-) -> Tuple[csv.ReadOptions, csv.ParseOptions, csv.ConvertOptions]:
-    if {key: value for key, value in version_ids.items() if value is not None}:
-        raise exceptions.InvalidArgument("Specific version ID found for object")
-
-    if s3_additional_kwargs:
-        raise exceptions.InvalidArgument(f"Additional S3 args specified: {s3_additional_kwargs}")
-
-    if file_format == "csv":
-        return _parse_csv_configuration(pandas_kwargs)
-
-    raise exceptions.InvalidArgument()
-
-
-def _resolve_format(read_format: str, can_use_arrow: bool) -> Any:
-    if read_format == "csv":
-        return ArrowCSVDatasource() if can_use_arrow else PandasCSVDataSource()
-    if read_format == "fwf":
-        return PandasFWFDataSource()
-    if read_format == "json":
-        return PandasJSONDatasource()
-    raise exceptions.UnsupportedType("Unsupported read format")
+    s3_additional_kwargs: Optional[Dict[str, str]],
+    dataset: bool,
+    use_threads: Union[bool, int],
+    version_id: Optional[str] = None,
+) -> Iterator[pd.DataFrame]:
+    mode, encoding, newline = _get_read_details(path=path, pandas_kwargs=pandas_kwargs)
+    with open_s3_object(
+        path=path,
+        version_id=version_id,
+        mode=mode,
+        s3_block_size=10 * 1024 * 1024,  # 10 MB (10 * 2**20)
+        encoding=encoding,
+        use_threads=use_threads,
+        s3_client=s3_client,
+        s3_additional_kwargs=s3_additional_kwargs,
+        newline=newline,
+    ) as f:
+        reader: pandas.io.parsers.TextFileReader = parser_func(f, chunksize=chunksize, **pandas_kwargs)
+        for df in reader:
+            yield _apply_partitions(df=df, dataset=dataset, path=path, path_root=path_root)
 
 
-def _read_text_distributed(  # pylint: disable=unused-argument
-    read_format: str,
+def _read_text_files_chunked(
     paths: List[str],
+    chunksize: int,
+    parser_func: Callable[..., pd.DataFrame],
     path_root: Optional[str],
+    s3_client: "S3Client",
+    pandas_kwargs: Dict[str, Any],
     s3_additional_kwargs: Optional[Dict[str, str]],
     dataset: bool,
-    ignore_index: bool,
-    parallelism: int,
-    version_id_dict: Dict[str, Optional[str]],
-    pandas_kwargs: Dict[str, Any],
     use_threads: Union[bool, int],
-    boto3_session: Optional["boto3.Session"],
-) -> pd.DataFrame:
-    try:
-        read_options, parse_options, convert_options = _parse_configuration(
-            read_format,
-            version_id_dict,
-            s3_additional_kwargs,
-            pandas_kwargs,
-        )
-        can_use_arrow = True
-    except exceptions.InvalidArgument as e:
-        _logger.warning(
-            "PyArrow method unavailable, defaulting to Pandas I/O functions: %s. "
-            "This will result in slower performance of the read operations",
-            e,
+    version_ids: Optional[Dict[str, str]],
+) -> Iterator[pd.DataFrame]:
+    for path in paths:
+        _logger.debug("path: %s", path)
+
+        yield from _read_text_chunked(
+            path=path,
+            chunksize=chunksize,
+            parser_func=parser_func,
+            path_root=path_root,
+            s3_client=s3_client,
+            pandas_kwargs=pandas_kwargs,
+            s3_additional_kwargs=s3_additional_kwargs,
+            dataset=dataset,
+            use_threads=use_threads,
+            version_id=version_ids.get(path) if version_ids else None,
         )
-        read_options, parse_options, convert_options = None, None, None
-        can_use_arrow = False
 
-    ray_dataset = read_datasource(
-        datasource=_resolve_format(read_format, can_use_arrow),
-        parallelism=parallelism,
-        paths=paths,
-        path_root=path_root,
-        dataset=dataset,
-        version_ids=version_id_dict,
-        s3_additional_kwargs=s3_additional_kwargs,
-        pandas_kwargs=pandas_kwargs,
-        read_options=read_options,
-        parse_options=parse_options,
-        convert_options=convert_options,
-    )
-    return _to_modin(dataset=ray_dataset, ignore_index=ignore_index)
+
+def _read_text_file(
+    s3_client: Optional["S3Client"],
+    path: str,
+    version_id: Optional[str],
+    parser_func: Callable[..., pd.DataFrame],
+    path_root: Optional[str],
+    pandas_kwargs: Dict[str, Any],
+    s3_additional_kwargs: Optional[Dict[str, str]],
+    dataset: bool,
+) -> pd.DataFrame:
+    mode, encoding, newline = _get_read_details(path=path, pandas_kwargs=pandas_kwargs)
+    try:
+        with open_s3_object(
+            path=path,
+            version_id=version_id,
+            mode=mode,
+            use_threads=False,
+            s3_block_size=-1,  # One shot download
+            encoding=encoding,
+            s3_client=s3_client,
+            s3_additional_kwargs=s3_additional_kwargs,
+            newline=newline,
+        ) as f:
+            df: pd.DataFrame = parser_func(f, **pandas_kwargs)
+    except botocore.exceptions.ClientError as e:
+        if e.response["Error"]["Code"] == "404":
+            raise exceptions.NoFilesFound(f"No files Found on: {path}.")
+        raise e
+    return _apply_partitions(df=df, dataset=dataset, path=path, path_root=path_root)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_write_dataset.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Modin on Ray S3 write dataset module (PRIVATE)."""
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
 import boto3
 import modin.pandas as pd
 import numpy as np
-import ray
 from pandas import DataFrame as PandasDataFrame
 
+from awswrangler import _utils, typing
 from awswrangler._distributed import engine
 from awswrangler.distributed.ray import ray_get, ray_remote
 from awswrangler.distributed.ray.modin import modin_repartition
+from awswrangler.distributed.ray.modin._utils import _ray_dataset_from_df
 from awswrangler.s3._write_concurrent import _WriteProxy
 from awswrangler.s3._write_dataset import _delete_objects, _get_bucketing_series, _to_partitions
 
 
 def _retrieve_paths(values: Union[str, List[Any]]) -> Iterator[str]:
     if isinstance(values, (list, np.ndarray)):
         for v in values:
@@ -24,29 +25,29 @@
 
 
 @modin_repartition
 def _to_buckets_distributed(  # pylint: disable=unused-argument
     df: pd.DataFrame,
     func: Callable[..., List[str]],
     path_root: str,
-    bucketing_info: Tuple[List[str], int],
+    bucketing_info: typing.BucketingInfoTuple,
     filename_prefix: str,
-    boto3_session: "boto3.Session",
+    boto3_session: Optional["boto3.Session"],
     use_threads: Union[bool, int],
     proxy: Optional[_WriteProxy] = None,
     **func_kwargs: Any,
 ) -> List[str]:
     df_groups = df.groupby(by=_get_bucketing_series(df=df, bucketing_info=bucketing_info))
     paths: List[str] = []
 
     df_paths = df_groups.apply(
-        engine.dispatch_func(func),  # type: ignore
+        engine.dispatch_func(func),
         path_root=path_root,
         filename_prefix=filename_prefix,
-        boto3_session=None,
+        s3_client=None,
         use_threads=False,
         bucketing=True,
         **func_kwargs,
     )
     for df_path in df_paths.values:
         # The value in df_path can be a string, a list of string, or a list of lists of strings
         row_paths = list(_retrieve_paths(df_path))
@@ -65,15 +66,15 @@
     partitions_types: Optional[Dict[str, str]],
     catalog_id: Optional[str],
     database: Optional[str],
     table: Optional[str],
     table_type: Optional[str],
     transaction_id: Optional[str],
     filename_prefix: str,
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     boto3_session: Optional["boto3.Session"] = None,
     **func_kwargs: Any,
 ) -> pd.DataFrame:
     prefix = _delete_objects(
         keys=df_group.name,
         path_root=path_root,
         use_threads=use_threads,
@@ -96,19 +97,20 @@
             bucketing_info=bucketing_info,
             boto3_session=boto3_session,
             use_threads=use_threads,
             filename_prefix=filename_prefix,
             **func_kwargs,
         )
     else:
-        paths = write_func(  # type: ignore
+        s3_client = _utils.client(service_name="s3", session=boto3_session)
+        paths = write_func(
             df_group.drop(partition_cols, axis="columns"),
             path_root=prefix,
             filename_prefix=filename_prefix,
-            boto3_session=boto3_session,
+            s3_client=s3_client,
             use_threads=use_threads,
             **func_kwargs,
         )
     return prefix, df_group.name, paths
 
 
 @modin_repartition
@@ -122,17 +124,17 @@
     partition_cols: List[str],
     partitions_types: Optional[Dict[str, str]],
     catalog_id: Optional[str],
     database: Optional[str],
     table: Optional[str],
     table_type: Optional[str],
     transaction_id: Optional[str],
-    bucketing_info: Optional[Tuple[List[str], int]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
     filename_prefix: str,
-    boto3_session: "boto3.Session",
+    boto3_session: Optional["boto3.Session"],
     **func_kwargs: Any,
 ) -> Tuple[List[str], Dict[str, List[str]]]:
     paths: List[str]
     partitions_values: Dict[str, List[str]]
 
     if not bucketing_info:
         # If only partitioning (without bucketing), avoid expensive modin groupby
@@ -161,15 +163,15 @@
                 partition_cols=partition_cols,
                 partitions_types=partitions_types,
                 boto3_session=None,
                 **func_kwargs,
             )
             return paths, partitions_values
 
-        block_object_refs = ray.data.from_modin(df).get_internal_block_refs()
+        block_object_refs = _ray_dataset_from_df(df).get_internal_block_refs()
         result = ray_get(
             [write_partitions(object_ref, block_index) for block_index, object_ref in enumerate(block_object_refs)]
         )
         paths = [path for row in result for path in row[0]]
         partitions_values = {
             partition_key: partition_value for row in result for partition_key, partition_value in row[1].items()
         }
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_write_parquet.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_parquet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """Modin on Ray S3 write parquet module (PRIVATE)."""
 import logging
 import math
-from typing import Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-import boto3
 import modin.pandas as pd
 import pyarrow as pa
-from modin.pandas import DataFrame as ModinDataFrame
-from ray.data import from_modin, from_pandas
 from ray.data.datasource.file_based_datasource import DefaultBlockWritePathProvider
 
 from awswrangler import exceptions
 from awswrangler.distributed.ray.datasources import ArrowParquetDatasource, UserProvidedKeyBlockWritePathProvider
+from awswrangler.distributed.ray.modin._utils import _ray_dataset_from_df
+
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _to_parquet_distributed(  # pylint: disable=unused-argument
     df: pd.DataFrame,
     schema: "pa.Schema",
     index: bool,
     compression: Optional[str],
     compression_ext: str,
     pyarrow_additional_kwargs: Optional[Dict[str, Any]],
     cpus: int,
     dtype: Dict[str, str],
-    boto3_session: Optional["boto3.Session"],
+    s3_client: Optional["S3Client"],
     s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
     path: Optional[str] = None,
     path_root: Optional[str] = None,
     filename_prefix: Optional[str] = "",
     max_rows_by_file: Optional[int] = 0,
     bucketing: bool = False,
 ) -> List[str]:
     if bucketing:
         # Add bucket id to the prefix
         path = f"{path_root}{filename_prefix}_bucket-{df.name:05d}{compression_ext}.parquet"
     # Create Ray Dataset
-    ds = from_modin(df) if isinstance(df, ModinDataFrame) else from_pandas(df)
+    ds = _ray_dataset_from_df(df)
     # Repartition into a single block if or writing into a single key or if bucketing is enabled
     if ds.count() > 0 and (path or bucketing) and not max_rows_by_file:
         _logger.warning(
             "Repartitioning frame to single partition as a strict path was defined: %s. "
             "This operation is inefficient for large datasets.",
             path,
         )
@@ -59,15 +60,15 @@
             raise exceptions.InvalidArgumentCombination(
                 "Cannot write indexed file when `max_rows_by_file` is specified"
             )
 
         ds = ds.repartition(math.ceil(ds.count() / max_rows_by_file))
     datasource = ArrowParquetDatasource()
     ds.write_datasource(
-        datasource,  # type: ignore
+        datasource,
         path=path or path_root,
         dataset_uuid=filename_prefix,
         # If user has provided a single key, use that instead of generating a path per block
         # The dataset will be repartitioned into a single block
         block_path_provider=UserProvidedKeyBlockWritePathProvider()
         if path and not path.endswith("/") and not max_rows_by_file
         else DefaultBlockWritePathProvider(),
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/distributed/ray/modin/s3/_write_text.py` & `awswrangler-3.0.0rc3/awswrangler/distributed/ray/modin/s3/_write_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 """Modin on Ray S3 write text module (PRIVATE)."""
 import logging
-from typing import Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
-import boto3
 import modin.pandas as pd
-from modin.pandas import DataFrame as ModinDataFrame
-from ray.data import from_modin, from_pandas
 from ray.data.datasource.file_based_datasource import DefaultBlockWritePathProvider
 
 from awswrangler import exceptions
 from awswrangler.distributed.ray.datasources import (  # pylint: disable=ungrouped-imports
     ArrowCSVDatasource,
     PandasCSVDataSource,
     PandasJSONDatasource,
     UserProvidedKeyBlockWritePathProvider,
 )
 from awswrangler.distributed.ray.datasources.pandas_file_based_datasource import PandasFileBasedDatasource
-from awswrangler.distributed.ray.modin._utils import ParamConfig, _check_parameters
+from awswrangler.distributed.ray.modin._utils import ParamConfig, _check_parameters, _ray_dataset_from_df
 from awswrangler.s3._write import _COMPRESSION_2_EXT
 from awswrangler.s3._write_text import _get_write_details
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 _CSV_SUPPORTED_PARAMS: Dict[str, ParamConfig] = {
     "header": ParamConfig(default=True),
     "sep": ParamConfig(default=",", supported_values={","}),
     "index": ParamConfig(default=True, supported_values={True}),
     "compression": ParamConfig(default=None, supported_values={None}),
     "quoting": ParamConfig(default=None, supported_values={None}),
     "escapechar": ParamConfig(default=None, supported_values={None}),
     "date_format": ParamConfig(default=None, supported_values={None}),
+    "columns": ParamConfig(default=None, supported_values={None}),
 }
 
 
 def _parse_csv_configuration(
     pandas_kwargs: Dict[str, Any],
 ) -> Dict[str, Any]:
     _check_parameters(pandas_kwargs, _CSV_SUPPORTED_PARAMS)
@@ -52,30 +53,30 @@
 ) -> Dict[str, Any]:
     if s3_additional_kwargs:
         raise exceptions.InvalidArgument(f"Additional S3 args specified: {s3_additional_kwargs}")
 
     if file_format == "csv":
         return _parse_csv_configuration(pandas_kwargs)
 
-    raise exceptions.InvalidArgument()
+    raise exceptions.InvalidArgument(f"File is in the {file_format} format")
 
 
-def _datasource_for_format(read_format: str, can_use_arrow: bool) -> PandasFileBasedDatasource:
-    if read_format == "csv":
+def _datasource_for_format(write_format: str, can_use_arrow: bool) -> PandasFileBasedDatasource:
+    if write_format == "csv":
         return ArrowCSVDatasource() if can_use_arrow else PandasCSVDataSource()
-    if read_format == "json":
+    if write_format == "json":
         return PandasJSONDatasource()
-    raise exceptions.UnsupportedType("Unsupported read format")
+    raise exceptions.UnsupportedType(f"Unsupported write format {write_format}")
 
 
 def _to_text_distributed(  # pylint: disable=unused-argument
     df: pd.DataFrame,
     file_format: str,
     use_threads: Union[bool, int],
-    boto3_session: Optional["boto3.Session"],
+    s3_client: Optional["S3Client"],
     s3_additional_kwargs: Optional[Dict[str, str]],
     path: Optional[str] = None,
     path_root: Optional[str] = None,
     filename_prefix: Optional[str] = None,
     bucketing: bool = False,
     **pandas_kwargs: Any,
 ) -> List[str]:
@@ -94,17 +95,17 @@
         file_path = path_root
     elif path is not None and path_root is None:
         file_path = path
     else:
         raise RuntimeError("path and path_root received at the same time.")
 
     # Create Ray Dataset
-    ds = from_modin(df) if isinstance(df, ModinDataFrame) else from_pandas(df)
+    ds = _ray_dataset_from_df(df)
 
-    # Repartition into a single block if or writing into a single key or if bucketing is enabled
+    # Repartition into a single block if writing into a single key or if bucketing is enabled
     if ds.count() > 0 and path:
         ds = ds.repartition(1)
         _logger.warning(
             "Repartitioning frame to single partition as a strict path was defined: %s. "
             "This operation is inefficient for large datasets.",
             path,
         )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/dynamodb/_delete.py` & `awswrangler-3.0.0rc3/awswrangler/dynamodb/_delete.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/dynamodb/_read.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_write.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,105 @@
-"""Amazon DynamoDB Read Module (PRIVATE)."""
+"""Amazon CSV S3 Write Module (PRIVATE)."""
 
 import logging
-import re
+from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple
 
-import boto3
 import pandas as pd
-from boto3.dynamodb.types import TypeDeserializer
 
-from awswrangler import _utils
-from awswrangler._config import apply_configs
+from awswrangler import _data_types, _utils, catalog, exceptions, typing
+from awswrangler._distributed import EngineEnum
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
-
-def _get_terms_groups(terms: List[str]) -> Tuple[List[str], List[str], List[str]]:
-    """Determine to which group of a PartiQL query each term belongs, e.g. it describes a column, table or filter."""
-    is_select_term = False
-    is_from_term = False
-    is_where_term = False
-    select_terms, from_terms, where_terms = [], [], []
-    for term in terms:
-        if term.upper() == "SELECT":
-            is_select_term = True
-            continue
-        if term.upper() == "FROM":
-            is_select_term = False
-            is_from_term = True
-            continue
-        if term.upper() == "WHERE":
-            is_from_term = False
-            is_where_term = True
-            continue
-        if is_select_term:
-            select_terms.append(term)
-        if is_from_term:
-            from_terms.append(term)
-        if is_where_term:
-            where_terms.append(term)
-    return select_terms, from_terms, where_terms
-
-
-def _get_scan_response(
-    table_name: str, select_terms: List[str], boto3_session: Optional[boto3.Session] = None
-) -> List[Dict[str, Any]]:
-    """Perform a scan to the Dynamo DB table and returns the data fetched."""
-    client_dynamodb = _utils.client(service_name="dynamodb", session=boto3_session)
-    scan_config: Dict[str, Any] = {"TableName": table_name}
-    if len(select_terms) > 1 or select_terms[0] != "*":
-        scan_config["AttributesToGet"] = select_terms
-    # get all responses even if pagination is necessary
-    response = client_dynamodb.scan(**scan_config)
-    data: List[Dict[str, Any]] = response["Items"]
-    while "LastEvaluatedKey" in response:
-        scan_config["ExclusiveStartKey"] = response["LastEvaluatedKey"]
-        response = client_dynamodb.scan(**scan_config)
-        data.extend(response["Items"])
-    return data
-
-
-def _get_items(query: str, boto3_session: Optional[boto3.Session] = None) -> List[Dict[str, Any]]:
-    # clean input query from possible excessive whitespace
-    query = re.sub(" +", " ", query).strip()
-    # generate terms list from query
-    terms = re.split(" |,", query)
-    if terms[0].upper() != "SELECT":
-        raise ValueError("The PartiQL query does not start with a 'SELECT'.")
-    select_terms, from_terms, _ = _get_terms_groups(terms)
-    if len(from_terms) > 1:
-        raise ValueError("The PartiQL query contains multiple tables but only one needed.")
-    if len(from_terms) == 0:
-        raise ValueError("The PartiQL query contains no tables.")
-    table_name = from_terms[0]
-    return _get_scan_response(table_name=table_name, select_terms=select_terms, boto3_session=boto3_session)
-
-
-def _deserialize_value(value: Any) -> Any:
-    if not pd.isna(value):
-        return TypeDeserializer().deserialize(value)
-    return value
-
-
-def _deserialize_data(df: pd.DataFrame, columns: pd.Index) -> pd.DataFrame:
-    if df.shape[0] > 0:
-        for column in columns:
-            df[column] = df[column].apply(_deserialize_value)
-    return df
+_COMPRESSION_2_EXT: Dict[Optional[str], str] = {
+    None: "",
+    "gzip": ".gz",
+    "snappy": ".snappy",
+    "bz2": ".bz2",
+    "xz": ".xz",
+    "zip": ".zip",
+    "zstd": ".zstd",
+}
+
+
+def _extract_dtypes_from_table_input(table_input: Dict[str, Any]) -> Dict[str, str]:
+    dtypes: Dict[str, str] = {}
+    for col in table_input["StorageDescriptor"]["Columns"]:
+        dtypes[col["Name"]] = col["Type"]
+    if "PartitionKeys" in table_input:
+        for par in table_input["PartitionKeys"]:
+            dtypes[par["Name"]] = par["Type"]
+    return dtypes
 
 
-def _parse_dynamodb_items(
-    items: List[Dict[str, Any]],
-    dtype: Optional[Dict[str, str]] = None,
+def _apply_dtype(
+    df: pd.DataFrame, dtype: Dict[str, str], catalog_table_input: Optional[Dict[str, Any]], mode: str
 ) -> pd.DataFrame:
-    df = pd.DataFrame(items)
-    df = _deserialize_data(df, df.columns)
-    return df.astype(dtype=dtype) if dtype else df
-
+    if mode in ("append", "overwrite_partitions"):
+        if catalog_table_input is not None:
+            catalog_types: Optional[Dict[str, str]] = _extract_dtypes_from_table_input(table_input=catalog_table_input)
+            if catalog_types is not None:
+                for k, v in catalog_types.items():
+                    dtype[k] = v
+    df = _data_types.cast_pandas_with_athena_types(df=df, dtype=dtype)
+    return df
 
-@apply_configs
-def read_partiql_query(
-    query: str,
-    dtype: Optional[Dict[str, str]] = None,
-    boto3_session: Optional[boto3.Session] = None,
-) -> pd.DataFrame:
-    """Read data from a DynamoDB table via a PartiQL query.
 
-    Parameters
-    ----------
-    query : str
-        The PartiQL query that will be executed.
-    dtype : Dict, optional
-        The data types of the DataFrame columns.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 Session will be used if boto3_session receive None.
-
-    Returns
-    -------
-    pd.DataFrame
-        Result as Pandas DataFrame.
-
-    Examples
-    --------
-    Select all contents from a table
-
-    >>> import awswrangler as wr
-    >>> wr.dynamodb.read_partiql_query(
-    ...     query='SELECT * FROM table'
-    ... )
-
-    Select specific columns from a table
-
-    >>> import awswrangler as wr
-    >>> wr.dynamodb.read_partiql_query(
-    ...     query='SELECT key FROM table'
-    ... )
-
-    Select all contents with dtype set
-
-    >>> import awswrangler as wr
-    >>> wr.dynamodb.read_partiql_query(
-    ...     query='SELECT * FROM table',
-    ...     dtype={'key': int}
-    ... )
-    """
-    _logger.debug("Reading results for PartiQL query:  %s", query)
-    items = _get_items(query=query, boto3_session=boto3_session)
-    return _parse_dynamodb_items(items=items, dtype=dtype)
+def _validate_args(
+    df: pd.DataFrame,
+    table: Optional[str],
+    database: Optional[str],
+    dataset: bool,
+    path: Optional[str],
+    partition_cols: Optional[List[str]],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
+    mode: Optional[str],
+    description: Optional[str],
+    parameters: Optional[Dict[str, str]],
+    columns_comments: Optional[Dict[str, str]],
+    execution_engine: Enum,
+) -> None:
+    if df.empty is True:
+        raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
+    if dataset is False:
+        if path is None:
+            raise exceptions.InvalidArgumentValue("If dataset is False, the `path` argument must be passed.")
+        if execution_engine == EngineEnum.PYTHON and path.endswith("/"):
+            raise exceptions.InvalidArgumentValue(
+                "If <dataset=False>, the argument <path> should be a key, not a prefix."
+            )
+        if partition_cols:
+            raise exceptions.InvalidArgumentCombination("Please, pass dataset=True to be able to use partition_cols.")
+        if bucketing_info:
+            raise exceptions.InvalidArgumentCombination("Please, pass dataset=True to be able to use bucketing_info.")
+        if mode is not None:
+            raise exceptions.InvalidArgumentCombination("Please pass dataset=True to be able to use mode.")
+        if any(arg is not None for arg in (table, description, parameters, columns_comments)):
+            raise exceptions.InvalidArgumentCombination(
+                "Please pass dataset=True to be able to use any one of these "
+                "arguments: database, table, description, parameters, "
+                "columns_comments."
+            )
+    elif (database is None) != (table is None):
+        raise exceptions.InvalidArgumentCombination(
+            "Arguments database and table must be passed together. If you want to store your dataset metadata in "
+            "the Glue Catalog, please ensure you are passing both."
+        )
+    elif all(x is None for x in [path, database, table]):
+        raise exceptions.InvalidArgumentCombination(
+            "You must specify a `path` if dataset is True and database/table are not enabled."
+        )
+    elif bucketing_info and bucketing_info[1] <= 0:
+        raise exceptions.InvalidArgumentValue(
+            "Please pass a value greater than 1 for the number of buckets for bucketing."
+        )
+
+
+def _sanitize(
+    df: pd.DataFrame, dtype: Dict[str, str], partition_cols: List[str]
+) -> Tuple[pd.DataFrame, Dict[str, str], List[str]]:
+    df = catalog.sanitize_dataframe_columns_names(df=df)
+    partition_cols = [catalog.sanitize_column_name(p) for p in partition_cols]
+    dtype = {catalog.sanitize_column_name(k): v.lower() for k, v in dtype.items()}
+    _utils.check_duplicated_columns(df=df)
+    return df, dtype, partition_cols
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/dynamodb/_write.py` & `awswrangler-3.0.0rc3/awswrangler/dynamodb/_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,8 +185,8 @@
     """
     _logger.debug("Inserting items into DynamoDB table")
 
     dynamodb_table = get_table(table_name=table_name, boto3_session=boto3_session)
     _validate_items(items=items, dynamodb_table=dynamodb_table)
     with dynamodb_table.batch_writer() as writer:
         for item in items:
-            writer.put_item(Item=item)
+            writer.put_item(Item=item)  # type: ignore[arg-type]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/emr.py` & `awswrangler-3.0.0rc3/awswrangler/emr.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,24 +61,23 @@
     --------
     >>> import awswrangler as wr
     >>> state = wr.emr._get_default_logging_path("subnet-id")
     's3://aws-logs-{account_id}-{region}/elasticmapreduce/'
 
     """
     if account_id is None:
-        boto3_session = _utils.ensure_session(session=boto3_session)
         _account_id: str = sts.get_account_id(boto3_session=boto3_session)
     else:
         _account_id = account_id
     if (region is None) and (subnet_id is not None):
         _region: str = _utils.get_region_from_session(boto3_session=boto3_session)
     elif (region is None) and (subnet_id is None):
         raise exceptions.InvalidArgumentCombination("You must pass region or subnet_id or both.")
     else:
-        _region = region  # type: ignore
+        _region = cast(str, region)
     return f"s3://aws-logs-{_account_id}-{_region}/elasticmapreduce/"
 
 
 def _build_cluster_args(**pars: Any) -> Dict[str, Any]:  # pylint: disable=too-many-branches,too-many-statements
     account_id: str = sts.get_account_id(boto3_session=pars["boto3_session"])
     region: str = _utils.get_region_from_session(boto3_session=pars["boto3_session"])
 
@@ -126,14 +125,18 @@
             "TerminationProtected": pars["termination_protected"],
             "Ec2SubnetId": pars["subnet_id"],
             "InstanceFleets": [],
         },
         "StepConcurrencyLevel": pars["step_concurrency_level"],
     }
 
+    # Auto Termination Policy
+    if pars["auto_termination_policy"] is not None:
+        args["AutoTerminationPolicy"] = pars["auto_termination_policy"]
+
     # Custom AMI
     if pars["custom_ami_id"] is not None:
         args["CustomAmiId"] = pars["custom_ami_id"]
 
     # EC2 Key Pair
     if pars["key_pair_name"] is not None:
         args["Instances"]["Ec2KeyName"] = pars["key_pair_name"]
@@ -147,23 +150,32 @@
         args["Instances"]["EmrManagedSlaveSecurityGroup"] = pars["security_group_slave"]
     if pars["security_groups_slave_additional"] is not None:
         args["Instances"]["AdditionalSlaveSecurityGroups"] = pars["security_groups_slave_additional"]
     if pars["security_group_service_access"] is not None:
         args["Instances"]["ServiceAccessSecurityGroup"] = pars["security_group_service_access"]
 
     # Configurations
-    args["Configurations"] = [
-        {"Classification": "spark-log4j", "Properties": {"log4j.rootCategory": f"{pars['spark_log_level']}, console"}}
-    ]
+    args["Configurations"] = (
+        [
+            {
+                "Classification": "spark-log4j",
+                "Properties": {"log4j.rootCategory": f"{pars['spark_log_level']}, console"},
+            }
+        ]
+        if not pars["configurations"]
+        else pars["configurations"]
+    )
     if pars["docker"] is True:
-        if pars.get("extra_registries") is None:
-            extra_registries: List[str] = []
+        if pars.get("extra_public_registries") is None:
+            extra_public_registries: List[str] = []
         else:
-            extra_registries = pars["extra_registries"]
-        registries: str = f"local,centos,{account_id}.dkr.ecr.{region}.amazonaws.com,{','.join(extra_registries)}"
+            extra_public_registries = pars["extra_public_registries"]
+        registries: str = (
+            f"local,centos,{account_id}.dkr.ecr.{region}.amazonaws.com,{','.join(extra_public_registries)}"
+        )
         registries = registries[:-1] if registries.endswith(",") else registries
         args["Configurations"].append(
             {
                 "Classification": "container-executor",
                 "Properties": {},
                 "Configurations": [
                     {
@@ -391,15 +403,15 @@
     return args
 
 
 def create_cluster(  # pylint: disable=too-many-arguments,too-many-locals,unused-argument
     subnet_id: str,
     cluster_name: str = "my-emr-cluster",
     logging_s3_path: Optional[str] = None,
-    emr_release: str = "emr-6.0.0",
+    emr_release: str = "emr-6.7.0",
     emr_ec2_role: str = "EMR_EC2_DefaultRole",
     emr_role: str = "EMR_DefaultRole",
     instance_type_master: str = "r5.xlarge",
     instance_type_core: str = "r5.xlarge",
     instance_type_task: str = "r5.xlarge",
     instance_ebs_size_master: int = 64,
     instance_ebs_size_core: int = 64,
@@ -433,29 +445,32 @@
     visible_to_all_users: bool = True,
     key_pair_name: Optional[str] = None,
     security_group_master: Optional[str] = None,
     security_groups_master_additional: Optional[List[str]] = None,
     security_group_slave: Optional[str] = None,
     security_groups_slave_additional: Optional[List[str]] = None,
     security_group_service_access: Optional[str] = None,
+    security_configuration: Optional[str] = None,
     docker: bool = False,
     extra_public_registries: Optional[List[str]] = None,
     spark_log_level: str = "WARN",
     spark_jars_path: Optional[List[str]] = None,
     spark_defaults: Optional[Dict[str, str]] = None,
     spark_pyarrow: bool = False,
     custom_classifications: Optional[List[Dict[str, Any]]] = None,
     maximize_resource_allocation: bool = False,
     steps: Optional[List[Dict[str, Any]]] = None,
     custom_ami_id: Optional[str] = None,
     step_concurrency_level: int = 1,
     keep_cluster_alive_when_no_steps: bool = True,
     termination_protected: bool = False,
+    auto_termination_policy: Optional[Dict[str, int]] = None,
     tags: Optional[Dict[str, str]] = None,
     boto3_session: Optional[boto3.Session] = None,
+    configurations: Optional[List[Dict[str, Any]]] = None,
 ) -> str:
     """Create a EMR cluster with instance fleets configuration.
 
     https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-instance-fleet.html
 
     Parameters
     ----------
@@ -568,14 +583,16 @@
         the core and task nodes.
     security_groups_slave_additional : str, optional
         A list of additional Amazon EC2 security group IDs for
         the core and task nodes.
     security_group_service_access : str, optional
         The identifier of the Amazon EC2 security group for the Amazon EMR
         service to access clusters in VPC private subnets.
+    security_configuration:str, optional
+        The name of a security configuration to apply to the cluster.
     docker : bool
         Enable Docker Hub and ECR registries access.
     extra_public_registries: List[str], optional
         Additional docker registries.
     spark_log_level : str
         log4j.rootCategory log level (ALL, DEBUG, INFO, WARN, ERROR, FATAL, OFF, TRACE).
     spark_jars_path : List[str], optional
@@ -598,20 +615,29 @@
     keep_cluster_alive_when_no_steps : bool
         Specifies whether the cluster should
         remain available after completing all steps
     termination_protected : bool
         Specifies whether the Amazon EC2 instances in the cluster are
         protected from termination by API calls, user intervention,
         or in the event of a job-flow error.
+    auto_termination_policy: Optional[Dict[str, int]]
+        Specifies the auto-termination policy that is attached to an Amazon EMR cluster
+        eg. auto_termination_policy = {'IdleTimeout': 123}
+        IdleTimeout specifies the amount of idle time in seconds after which the cluster automatically terminates.
+        You can specify a minimum of 60 seconds and a maximum of 604800 seconds (seven days).
     tags : Dict[str, str], optional
         Key/Value collection to put on the Cluster.
         e.g. {"foo": "boo", "bar": "xoo"})
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
+    configurations: List[Dict[str, Any]], optional
+        The list of configurations supplied for an EMR cluster instance group.
 
+        By default, adds log4j config as follows:
+        `{"Classification": "spark-log4j", "Properties": {"log4j.rootCategory": f"{pars['spark_log_level']}, console"}}`
     Returns
     -------
     str
         Cluster ID.
 
     Examples
     --------
@@ -684,20 +710,19 @@
     ...     spark_pyarrow=True,
     ...     tags={
     ...         "foo": "boo"
     ...     })
 
     """
     applications = ["Spark"] if applications is None else applications
-    boto3_session = _utils.ensure_session(session=boto3_session)
     args: Dict[str, Any] = _build_cluster_args(**locals())
-    client_emr: boto3.client = _utils.client(service_name="emr", session=boto3_session)
-    response: Dict[str, Any] = client_emr.run_job_flow(**args)
+    client_emr = _utils.client(service_name="emr", session=boto3_session)
+    response = client_emr.run_job_flow(**args)
     _logger.debug("response: \n%s", pprint.pformat(response))
-    return cast(str, response["JobFlowId"])
+    return response["JobFlowId"]
 
 
 def get_cluster_state(cluster_id: str, boto3_session: Optional[boto3.Session] = None) -> str:
     """Get the EMR cluster state.
 
     Possible states: 'STARTING', 'BOOTSTRAPPING', 'RUNNING',
     'WAITING', 'TERMINATING',
@@ -717,18 +742,18 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> state = wr.emr.get_cluster_state("cluster-id")
 
     """
-    client_emr: boto3.client = _utils.client(service_name="emr", session=boto3_session)
-    response: Dict[str, Any] = client_emr.describe_cluster(ClusterId=cluster_id)
+    client_emr = _utils.client(service_name="emr", session=boto3_session)
+    response = client_emr.describe_cluster(ClusterId=cluster_id)
     _logger.debug("response: \n%s", pprint.pformat(response))
-    return cast(str, response["Cluster"]["Status"]["State"])
+    return response["Cluster"]["Status"]["State"]
 
 
 def terminate_cluster(cluster_id: str, boto3_session: Optional[boto3.Session] = None) -> None:
     """Terminate EMR cluster.
 
     Parameters
     ----------
@@ -744,16 +769,16 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.emr.terminate_cluster("cluster-id")
 
     """
-    client_emr: boto3.client = _utils.client(service_name="emr", session=boto3_session)
-    response: Dict[str, Any] = client_emr.terminate_job_flows(JobFlowIds=[cluster_id])
+    client_emr = _utils.client(service_name="emr", session=boto3_session)
+    response = client_emr.terminate_job_flows(JobFlowIds=[cluster_id])
     _logger.debug("response: \n%s", pprint.pformat(response))
 
 
 def submit_steps(
     cluster_id: str, steps: List[Dict[str, Any]], boto3_session: Optional[boto3.Session] = None
 ) -> List[str]:
     """Submit a list of steps.
@@ -776,18 +801,18 @@
     --------
     >>> import awswrangler as wr
     >>> for cmd in ['echo "Hello"', "ls -la"]:
     ...     steps.append(wr.emr.build_step(name=cmd, command=cmd))
     >>> wr.emr.submit_steps(cluster_id="cluster-id", steps=steps)
 
     """
-    client_emr: boto3.client = _utils.client(service_name="emr", session=boto3_session)
-    response: Dict[str, Any] = client_emr.add_job_flow_steps(JobFlowId=cluster_id, Steps=steps)
+    client_emr = _utils.client(service_name="emr", session=boto3_session)
+    response = client_emr.add_job_flow_steps(JobFlowId=cluster_id, Steps=steps)  # type: ignore[arg-type]
     _logger.debug("response: \n%s", pprint.pformat(response))
-    return cast(List[str], response["StepIds"])
+    return response["StepIds"]
 
 
 def submit_step(
     cluster_id: str,
     command: str,
     name: str = "my-step",
     action_on_failure: str = "CONTINUE",
@@ -824,22 +849,21 @@
     >>> step_id = wr.emr.submit_step(
     ...     cluster_id=cluster_id,
     ...     name="step_test",
     ...     command="s3://...script.sh arg1 arg2",
     ...     script=True)
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     step: Dict[str, Any] = build_step(
-        name=name, command=command, action_on_failure=action_on_failure, script=script, boto3_session=session
+        name=name, command=command, action_on_failure=action_on_failure, script=script, boto3_session=boto3_session
     )
-    client_emr: boto3.client = _utils.client(service_name="emr", session=session)
-    response: Dict[str, Any] = client_emr.add_job_flow_steps(JobFlowId=cluster_id, Steps=[step])
+    client_emr = _utils.client(service_name="emr", session=boto3_session)
+    response = client_emr.add_job_flow_steps(JobFlowId=cluster_id, Steps=[step])  # type: ignore[list-item]
     _logger.debug("response: \n%s", pprint.pformat(response))
-    return cast(str, response["StepIds"][0])
+    return response["StepIds"][0]
 
 
 def build_step(
     command: str,
     name: str = "my-step",
     action_on_failure: str = "CONTINUE",
     script: bool = False,
@@ -916,18 +940,18 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> state = wr.emr.get_step_state("cluster-id", "step-id")
 
     """
-    client_emr: boto3.client = _utils.client(service_name="emr", session=boto3_session)
-    response: Dict[str, Any] = client_emr.describe_step(ClusterId=cluster_id, StepId=step_id)
+    client_emr = _utils.client(service_name="emr", session=boto3_session)
+    response = client_emr.describe_step(ClusterId=cluster_id, StepId=step_id)
     _logger.debug("response: \n%s", pprint.pformat(response))
-    return cast(str, response["Step"]["Status"]["State"])
+    return response["Step"]["Status"]["State"]
 
 
 def submit_ecr_credentials_refresh(
     cluster_id: str, path: str, action_on_failure: str = "CONTINUE", boto3_session: Optional[boto3.Session] = None
 ) -> str:
     """Update internal ECR credentials.
 
@@ -951,47 +975,49 @@
     --------
     >>> import awswrangler as wr
     >>> step_id = wr.emr.submit_ecr_credentials_refresh("cluster_id", "s3://bucket/emr/")
 
     """
     path = path[:-1] if path.endswith("/") else path
     path_script: str = f"{path}/ecr_credentials_refresh.py"
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_s3: boto3.client = _utils.client(service_name="s3", session=session)
+    client_s3 = _utils.client(service_name="s3", session=boto3_session)
     bucket, key = _utils.parse_path(path=path_script)
     region: str = _utils.get_region_from_session(boto3_session=boto3_session)
     client_s3.put_object(
         Body=_get_ecr_credentials_refresh_content(region=region).encode(encoding="utf-8"), Bucket=bucket, Key=key
     )
     command: str = f"spark-submit --deploy-mode cluster {path_script}"
     name: str = "ECR Credentials Refresh"
     step: Dict[str, Any] = build_step(
-        name=name, command=command, action_on_failure=action_on_failure, script=False, boto3_session=session
+        name=name, command=command, action_on_failure=action_on_failure, script=False, boto3_session=boto3_session
     )
-    client_emr: boto3.client = _utils.client(service_name="emr", session=session)
-    response: Dict[str, Any] = client_emr.add_job_flow_steps(JobFlowId=cluster_id, Steps=[step])
+    client_emr = _utils.client(service_name="emr", session=boto3_session)
+    response = client_emr.add_job_flow_steps(JobFlowId=cluster_id, Steps=[step])  # type: ignore[list-item]
     _logger.debug("response: \n%s", pprint.pformat(response))
-    return cast(str, response["StepIds"][0])
+    return response["StepIds"][0]
 
 
 def build_spark_step(
     path: str,
+    args: Optional[List[str]] = None,
     deploy_mode: str = "cluster",
     docker_image: Optional[str] = None,
     name: str = "my-step",
     action_on_failure: str = "CONTINUE",
     region: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Dict[str, Any]:
     """Build the Step structure (dictionary).
 
     Parameters
     ----------
     path : str
         Script path. (e.g. s3://bucket/app.py)
+    args : List[str], optional
+        CLI args to use with script
     deploy_mode : str
         "cluster" | "client"
     docker_image : str, optional
         e.g. "{ACCOUNT_ID}.dkr.ecr.{REGION}.amazonaws.com/{IMAGE_NAME}:{TAG}"
     name : str, optional
         Step name.
     action_on_failure : str
@@ -1013,43 +1039,45 @@
     >>>     cluster_id="cluster-id",
     >>>     steps=[
     >>>         wr.emr.build_spark_step(path="s3://bucket/app.py")
     >>>     ]
     >>> )
 
     """
+    script_args = " ".join(args) if args else ""
     if docker_image is None:
-        cmd: str = f"spark-submit --deploy-mode {deploy_mode} {path}"
+        cmd: str = f"spark-submit --deploy-mode {deploy_mode} {path} {script_args}"
     else:
         config: str = "hdfs:///user/hadoop/config.json"
         cmd = (
             f"spark-submit --deploy-mode {deploy_mode} "
             f"--conf spark.executorEnv.YARN_CONTAINER_RUNTIME_TYPE=docker "
             f"--conf spark.executorEnv.YARN_CONTAINER_RUNTIME_DOCKER_IMAGE={docker_image} "
             f"--conf spark.executorEnv.YARN_CONTAINER_RUNTIME_DOCKER_CLIENT_CONFIG={config} "
             f"--conf spark.executorEnv.YARN_CONTAINER_RUNTIME_DOCKER_MOUNTS=/etc/passwd:/etc/passwd:ro "
             f"--conf spark.yarn.appMasterEnv.YARN_CONTAINER_RUNTIME_TYPE=docker "
             f"--conf spark.yarn.appMasterEnv.YARN_CONTAINER_RUNTIME_DOCKER_IMAGE={docker_image} "
             f"--conf spark.yarn.appMasterEnv.YARN_CONTAINER_RUNTIME_DOCKER_CLIENT_CONFIG={config} "
             f"--conf spark.yarn.appMasterEnv.YARN_CONTAINER_RUNTIME_DOCKER_MOUNTS=/etc/passwd:/etc/passwd:ro "
-            f"{path}"
+            f"{path} {script_args}"
         )
     return build_step(
         command=cmd,
         name=name,
         action_on_failure=action_on_failure,
         script=False,
         region=region,
         boto3_session=boto3_session,
     )
 
 
 def submit_spark_step(
     cluster_id: str,
     path: str,
+    args: Optional[List[str]] = None,
     deploy_mode: str = "cluster",
     docker_image: Optional[str] = None,
     name: str = "my-step",
     action_on_failure: str = "CONTINUE",
     region: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> str:
@@ -1057,14 +1085,17 @@
 
     Parameters
     ----------
     cluster_id : str
         Cluster ID.
     path : str
         Script path. (e.g. s3://bucket/app.py)
+    args : List[str], optional
+        CLI args to use with script
+        eg. args = ["--name", "hello-world"]
     deploy_mode : str
         "cluster" | "client"
     docker_image : str, optional
         e.g. "{ACCOUNT_ID}.dkr.ecr.{REGION}.amazonaws.com/{IMAGE_NAME}:{TAG}"
     name : str, optional
         Step name.
     action_on_failure : str
@@ -1084,18 +1115,18 @@
     >>> import awswrangler as wr
     >>> step_id = wr.emr.submit_spark_step(
     >>>     cluster_id="cluster-id",
     >>>     path="s3://bucket/emr/app.py"
     >>> )
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     step = build_spark_step(
         path=path,
+        args=args,
         deploy_mode=deploy_mode,
         docker_image=docker_image,
         name=name,
         action_on_failure=action_on_failure,
         region=region,
-        boto3_session=session,
+        boto3_session=boto3_session,
     )
-    return submit_steps(cluster_id=cluster_id, steps=[step], boto3_session=session)[0]
+    return submit_steps(cluster_id=cluster_id, steps=[step], boto3_session=boto3_session)[0]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/exceptions.py` & `awswrangler-3.0.0rc3/awswrangler/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -111,7 +111,27 @@
 
 class FailedQualityCheck(Exception):
     """FailedQualityCheck."""
 
 
 class AlreadyExists(Exception):
     """AlreadyExists."""
+
+
+class S3SelectRequestIncomplete(Exception):
+    """S3SelectRequestIncomplete."""
+
+
+class ResourceDoesNotExist(Exception):
+    """ResourceDoesNotExist."""
+
+
+class InvalidRulesetDefinition(Exception):
+    """InvalidRulesetDefinition."""
+
+
+class PolicyResourceConflict(Exception):
+    """PolicyResourceConflict."""
+
+
+class NotSupported(Exception):
+    """NotSupported."""
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/lakeformation/__init__.py` & `awswrangler-3.0.0rc3/awswrangler/lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/lakeformation/_read.py` & `awswrangler-3.0.0rc3/awswrangler/lakeformation/_read.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,84 +1,88 @@
 """Amazon Lake Formation Module gathering all read functions."""
 import itertools
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import boto3
 import pandas as pd
 from pyarrow import NativeFile, RecordBatchStreamReader, Table
 
 from awswrangler import _data_types, _utils, catalog
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
 from awswrangler._sql_formatter import _EngineType, _process_sql_params
 from awswrangler._threading import _get_executor
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 from awswrangler.lakeformation._utils import commit_transaction, start_transaction, wait_query
 
+if TYPE_CHECKING:
+    from mypy_boto3_lakeformation.client import LakeFormationClient
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 @engine.dispatch_on_engine
 def _get_work_unit_results(
-    boto3_session: Optional[boto3.Session],
+    client_lakeformation: Optional["LakeFormationClient"],
     query_id: str,
     token_work_unit: Tuple[str, int],
 ) -> Table:
-    _logger.debug("Query id: %s Token work unit: %s", query_id, token_work_unit)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=boto3_session)
-
+    client_lakeformation = client_lakeformation if client_lakeformation else _utils.client(service_name="lakeformation")
     token, work_unit = token_work_unit
     messages: NativeFile = client_lakeformation.get_work_unit_results(
         QueryId=query_id, WorkUnitToken=token, WorkUnitId=work_unit
     )["ResultStream"]
     return RecordBatchStreamReader(messages.read()).read_all()
 
 
 def _resolve_sql_query(
     query_id: str,
     use_threads: bool,
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     arrow_kwargs: Dict[str, Any],
 ) -> pd.DataFrame:
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=boto3_session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
 
     wait_query(query_id=query_id, boto3_session=boto3_session)
 
     # The LF Query Engine distributes the load across workers
     # Retrieve the tokens and their associated work units until NextToken is ''
     # One Token can span multiple work units
     # PageSize determines the size of the "Units" array in each call
     scan_kwargs: Dict[str, Union[str, int]] = {"QueryId": query_id, "PageSize": 10}
-    next_token: str = "init_token"  # Dummy token
+    next_token: Optional[str] = "init_token"  # Dummy token
     token_work_units: List[Tuple[str, int]] = []
     while next_token:
-        response = client_lakeformation.get_work_units(**scan_kwargs)
+        response = client_lakeformation.get_work_units(**scan_kwargs)  # type: ignore[arg-type]
         token_work_units.extend(  # [(Token0, WorkUnitId0), (Token0, WorkUnitId1), (Token1, WorkUnitId2) ... ]
             [
                 (unit["WorkUnitToken"], unit_id)
                 for unit in response["WorkUnitRanges"]
                 for unit_id in range(unit["WorkUnitIdMin"], unit["WorkUnitIdMax"] + 1)  # Max is inclusive
             ]
         )
         next_token = response.get("NextToken", None)
-        scan_kwargs["NextToken"] = next_token
+        scan_kwargs["NextToken"] = next_token  # type: ignore[assignment]
 
     executor = _get_executor(use_threads=use_threads)
 
     tables = executor.map(
         _get_work_unit_results,
-        boto3_session,
+        client_lakeformation,
         itertools.repeat(query_id),
         token_work_units,
     )
     return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
 
 
 @apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def read_sql_query(
     sql: str,
     database: str,
     transaction_id: Optional[str] = None,
     query_as_of_time: Optional[str] = None,
     catalog_id: Optional[str] = None,
     use_threads: bool = True,
@@ -158,42 +162,48 @@
     ...     sql="SELECT * FROM my_table WHERE name=:name AND city=:city",
     ...     database="my_db",
     ...     query_as_of_time="1611142914",
     ...     params={"name": "filtered_name", "city": "filtered_city"}
     ... )
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
     commit_trans: bool = False
 
     sql = _process_sql_params(sql, params, engine=_EngineType.PARTIQL)
 
     if not any([transaction_id, query_as_of_time]):
         _logger.debug("Neither `transaction_id` nor `query_as_of_time` were specified, starting transaction")
-        transaction_id = start_transaction(read_only=True, boto3_session=session)
+        transaction_id = start_transaction(read_only=True, boto3_session=boto3_session)
         commit_trans = True
     args: Dict[str, Optional[str]] = _catalog_id(
         catalog_id=catalog_id,
         **_transaction_id(transaction_id=transaction_id, query_as_of_time=query_as_of_time, DatabaseName=database),
     )
-    query_id: str = client_lakeformation.start_query_planning(QueryString=sql, QueryPlanningContext=args)["QueryId"]
+    result = client_lakeformation.start_query_planning(
+        QueryString=sql,
+        QueryPlanningContext=args,  # type: ignore[arg-type]
+    )
+    query_id: str = result["QueryId"]
     arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
     df = _resolve_sql_query(
         query_id=query_id,
         use_threads=use_threads,
-        boto3_session=session,
+        boto3_session=boto3_session,
         arrow_kwargs=arrow_kwargs,
     )
     if commit_trans:
-        commit_transaction(transaction_id=transaction_id)  # type: ignore
+        commit_transaction(transaction_id=transaction_id, boto3_session=boto3_session)  # type: ignore[arg-type]
     return df
 
 
 @apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def read_sql_table(
     table: str,
     database: str,
     transaction_id: Optional[str] = None,
     query_as_of_time: Optional[str] = None,
     catalog_id: Optional[str] = None,
     use_threads: bool = True,
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/lakeformation/_utils.py` & `awswrangler-3.0.0rc3/awswrangler/lakeformation/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Utilities Module for Amazon Lake Formation."""
 import logging
 import time
 from math import inf
 from threading import Thread
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Literal, Optional, Union
 
 import boto3
 import botocore.exceptions
 
 from awswrangler import _utils, exceptions
+from awswrangler._config import apply_configs
 from awswrangler.catalog._utils import _catalog_id, _transaction_id
 from awswrangler.s3._describe import describe_objects
 
 _QUERY_FINAL_STATES: List[str] = ["ERROR", "FINISHED"]
 _QUERY_WAIT_POLLING_DELAY: float = 2  # SECONDS
 _TRANSACTION_FINAL_STATES: List[str] = ["aborted", "committed"]
 _TRANSACTION_WAIT_COMMIT_DELAY: float = 5  # SECONDS
@@ -68,42 +69,41 @@
     transaction_id: str,
     boto3_session: Optional[boto3.Session],
     partition_cols: Optional[List[str]] = None,
     partitions_types: Optional[Dict[str, str]] = None,
     partitions_values: Optional[List[str]] = None,
 ) -> List[Dict[str, Any]]:
     """Get Governed Table Objects from Lake Formation Engine."""
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
 
-    scan_kwargs: Dict[str, Union[str, int]] = _catalog_id(
+    scan_kwargs: Dict[str, Union[str, int, None]] = _catalog_id(
         catalog_id=catalog_id,
         **_transaction_id(transaction_id=transaction_id, DatabaseName=database, TableName=table, MaxResults=100),
     )
     if partition_cols and partitions_types and partitions_values:
         scan_kwargs["PartitionPredicate"] = _build_partition_predicate(
             partition_cols=partition_cols, partitions_types=partitions_types, partitions_values=partitions_values
         )
 
-    next_token: str = "init_token"  # Dummy token
+    next_token: Optional[str] = "init_token"  # Dummy token
     table_objects: List[Dict[str, Any]] = []
     while next_token:
         response = _utils.try_it(
             f=client_lakeformation.get_table_objects,
             ex=botocore.exceptions.ClientError,
             ex_code="ResourceNotReadyException",
             base=1.0,
             max_num_tries=5,
             **scan_kwargs,
         )
         for objects in response["Objects"]:
             for table_object in objects["Objects"]:
                 if objects["PartitionValues"]:
-                    table_object["PartitionValues"] = objects["PartitionValues"]
-                table_objects.append(table_object)
+                    table_object["PartitionValues"] = objects["PartitionValues"]  # type: ignore[typeddict-item]
+                table_objects.append(table_object)  # type: ignore[arg-type]
         next_token = response.get("NextToken", None)
         scan_kwargs["NextToken"] = next_token
     return table_objects
 
 
 def _update_table_objects(
     catalog_id: Optional[str],
@@ -111,29 +111,28 @@
     table: str,
     transaction_id: str,
     boto3_session: Optional[boto3.Session],
     add_objects: Optional[List[Dict[str, Any]]] = None,
     del_objects: Optional[List[Dict[str, Any]]] = None,
 ) -> None:
     """Register Governed Table Objects changes to Lake Formation Engine."""
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
 
     update_kwargs: Dict[str, Union[str, int, List[Dict[str, Dict[str, Any]]]]] = _catalog_id(
         catalog_id=catalog_id, **_transaction_id(transaction_id=transaction_id, DatabaseName=database, TableName=table)
     )
 
     write_operations: List[Dict[str, Dict[str, Any]]] = []
     if add_objects:
         write_operations.extend({"AddObject": obj} for obj in add_objects)
     if del_objects:
         write_operations.extend({"DeleteObject": _without_keys(obj, ["Size"])} for obj in del_objects)
     update_kwargs["WriteOperations"] = write_operations
 
-    client_lakeformation.update_table_objects(**update_kwargs)
+    client_lakeformation.update_table_objects(**update_kwargs)  # type: ignore[arg-type]
 
 
 def _monitor_transaction(transaction_id: str, time_out: float, boto3_session: Optional[boto3.Session] = None) -> None:
     start = time.time()
     elapsed_time = 0.0
     state: str = describe_transaction(transaction_id=transaction_id, boto3_session=boto3_session)
     while (state not in _TRANSACTION_FINAL_STATES) and (time_out > elapsed_time):
@@ -167,20 +166,17 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> status = wr.lakeformation.describe_transaction(transaction_id="...")
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
-    details: Dict[str, Any] = client_lakeformation.describe_transaction(TransactionId=transaction_id)[
-        "TransactionDescription"
-    ]
-    return details["TransactionStatus"]  # type: ignore
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
+    details = client_lakeformation.describe_transaction(TransactionId=transaction_id)["TransactionDescription"]
+    return details["TransactionStatus"]
 
 
 def cancel_transaction(transaction_id: str, boto3_session: Optional[boto3.Session] = None) -> None:
     """Cancel the specified transaction. Returns exception if the transaction was previously committed.
 
     Parameters
     ----------
@@ -196,16 +192,15 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.lakeformation.cancel_transaction(transaction_id="...")
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
 
     client_lakeformation.cancel_transaction(TransactionId=transaction_id)
 
 
 def start_transaction(
     read_only: Optional[bool] = False, time_out: Optional[float] = inf, boto3_session: Optional[boto3.Session] = None
 ) -> str:
@@ -231,17 +226,16 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> transaction_id = wr.lakeformation.start_transaction(read_only=False)
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
-    transaction_type: str = "READ_ONLY" if read_only else "READ_AND_WRITE"
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
+    transaction_type: Literal["READ_AND_WRITE", "READ_ONLY"] = "READ_ONLY" if read_only else "READ_AND_WRITE"
     transaction_id: str = client_lakeformation.start_transaction(TransactionType=transaction_type)["TransactionId"]
     # Extend the transaction while in "active" state in a separate thread
     t = Thread(target=_monitor_transaction, args=(transaction_id, time_out, boto3_session))
     t.daemon = True  # Ensures thread is killed when any exception is raised
     t.start()
     return transaction_id
 
@@ -264,21 +258,21 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.lakeformation.commit_transaction(transaction_id="...")
 
     """
     session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=session)
 
     client_lakeformation.commit_transaction(TransactionId=transaction_id)
     committed: bool = False
     # Confirm transaction was committed
     while not committed:
-        state: str = describe_transaction(transaction_id=transaction_id, boto3_session=session)
+        state = describe_transaction(transaction_id=transaction_id, boto3_session=session)
         if state == "committed":
             committed = True
         elif state == "aborted":
             raise exceptions.CommitCancelled(f"Transaction commit with id {transaction_id} was aborted.")
         time.sleep(_TRANSACTION_WAIT_COMMIT_DELAY)
 
 
@@ -299,47 +293,53 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.lakeformation.extend_transaction(transaction_id="...")
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
 
     client_lakeformation.extend_transaction(TransactionId=transaction_id)
 
 
-def wait_query(query_id: str, boto3_session: Optional[boto3.Session] = None) -> Dict[str, Any]:
+@apply_configs
+def wait_query(
+    query_id: str,
+    boto3_session: Optional[boto3.Session] = None,
+    lakeformation_query_wait_polling_delay: float = _QUERY_WAIT_POLLING_DELAY,
+) -> Dict[str, Any]:
     """Wait for the query to end.
 
     Parameters
     ----------
     query_id : str
         Lake Formation query execution ID.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session received None.
+    lakeformation_query_wait_polling_delay: float, default: 2 seconds
+        Interval in seconds for how often the function will check if the LakeFormation query has completed.
+
 
     Returns
     -------
     Dict[str, Any]
         Dictionary with the get_query_state response.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> res = wr.lakeformation.wait_query(query_id='query-id')
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client_lakeformation: boto3.client = _utils.client(service_name="lakeformation", session=session)
+    client_lakeformation = _utils.client(service_name="lakeformation", session=boto3_session)
 
-    response: Dict[str, Any] = client_lakeformation.get_query_state(QueryId=query_id)
-    state: str = response["State"]
+    response = client_lakeformation.get_query_state(QueryId=query_id)
+    state = response["State"]
     while state not in _QUERY_FINAL_STATES:
-        time.sleep(_QUERY_WAIT_POLLING_DELAY)
+        time.sleep(lakeformation_query_wait_polling_delay)
         response = client_lakeformation.get_query_state(QueryId=query_id)
         state = response["State"]
     _logger.debug("state: %s", state)
     if state == "ERROR":
         raise exceptions.QueryFailed(response.get("Error"))
-    return response
+    return response  # type: ignore[return-value]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/mysql.py` & `awswrangler-3.0.0rc3/awswrangler/oracle.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,198 +1,240 @@
-"""Amazon MySQL Module."""
+# mypy: disable-error-code=name-defined
+"""Amazon Oracle Database Module."""
 
 import logging
-import uuid
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, Union
+from decimal import Decimal
+from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, TypeVar, Union, overload
 
 import boto3
 import pandas as pd
 import pyarrow as pa
-import pymysql
-from pymysql.cursors import Cursor
 
-from awswrangler import _data_types
+from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
-from awswrangler import exceptions
 from awswrangler._config import apply_configs
 
+__all__ = ["connect", "read_sql_query", "read_sql_table", "to_sql"]
+
+oracledb = _utils.import_optional_dependency("oracledb")
+
 _logger: logging.Logger = logging.getLogger(__name__)
+FuncT = TypeVar("FuncT", bound=Callable[..., Any])
 
 
-def _validate_connection(con: "pymysql.connections.Connection[Any]") -> None:
-    if not isinstance(con, pymysql.connections.Connection):
+def _validate_connection(con: "oracledb.Connection") -> None:
+    if not isinstance(con, oracledb.Connection):
         raise exceptions.InvalidConnection(
             "Invalid 'conn' argument, please pass a "
-            "pymysql.connections.Connection object. Use pymysql.connect() to use "
-            "credentials directly or wr.mysql.connect() to fetch it from the Glue Catalog."
+            "oracledb.Connection object. Use oracledb.connect() to use "
+            "credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog."
         )
 
 
-def _drop_table(cursor: Cursor, schema: Optional[str], table: str) -> None:
-    schema_str = f"`{schema}`." if schema else ""
-    sql = f"DROP TABLE IF EXISTS {schema_str}`{table}`"
+def _get_table_identifier(schema: Optional[str], table: str) -> str:
+    schema_str = f'"{schema}".' if schema else ""
+    table_identifier = f'{schema_str}"{table}"'
+    return table_identifier
+
+
+def _drop_table(cursor: "oracledb.Cursor", schema: Optional[str], table: str) -> None:
+    table_identifier = _get_table_identifier(schema, table)
+    sql = f"""
+BEGIN
+    EXECUTE IMMEDIATE 'DROP TABLE {table_identifier}';
+EXCEPTION
+    WHEN OTHERS THEN
+        IF SQLCODE != -942 THEN
+            RAISE;
+        END IF;
+END;
+"""
     _logger.debug("Drop table query:\n%s", sql)
     cursor.execute(sql)
 
 
-def _does_table_exist(cursor: Cursor, schema: Optional[str], table: str) -> bool:
-    schema_str = f"TABLE_SCHEMA = '{schema}' AND" if schema else ""
-    cursor.execute(f"SELECT * FROM INFORMATION_SCHEMA.TABLES WHERE " f"{schema_str} TABLE_NAME = '{table}'")
+def _does_table_exist(cursor: "oracledb.Cursor", schema: Optional[str], table: str) -> bool:
+    schema_str = f"OWNER = '{schema}' AND" if schema else ""
+    cursor.execute(f"SELECT * FROM ALL_TABLES WHERE {schema_str} TABLE_NAME = '{table}'")
     return len(cursor.fetchall()) > 0
 
 
 def _create_table(
     df: pd.DataFrame,
-    cursor: Cursor,
+    cursor: "oracledb.Cursor",
     table: str,
     schema: str,
     mode: str,
     index: bool,
     dtype: Optional[Dict[str, str]],
     varchar_lengths: Optional[Dict[str, int]],
 ) -> None:
     if mode == "overwrite":
         _drop_table(cursor=cursor, schema=schema, table=table)
     elif _does_table_exist(cursor=cursor, schema=schema, table=table):
         return
-    mysql_types: Dict[str, str] = _data_types.database_types_from_pandas(
+    oracle_types: Dict[str, str] = _data_types.database_types_from_pandas(
         df=df,
         index=index,
         dtype=dtype,
-        varchar_lengths_default="TEXT",
+        varchar_lengths_default="CLOB",
         varchar_lengths=varchar_lengths,
-        converter_func=_data_types.pyarrow2mysql,
+        converter_func=_data_types.pyarrow2oracle,
     )
-    cols_str: str = "".join([f"`{k}` {v},\n" for k, v in mysql_types.items()])[:-2]
-    sql = f"CREATE TABLE IF NOT EXISTS `{schema}`.`{table}` (\n{cols_str})"
+    cols_str: str = "".join([f'"{k}" {v},\n' for k, v in oracle_types.items()])[:-2]
+    table_identifier = _get_table_identifier(schema, table)
+    sql = f"CREATE TABLE {table_identifier} (\n{cols_str})"
     _logger.debug("Create table query:\n%s", sql)
     cursor.execute(sql)
 
 
+@_utils.check_optional_dependency(oracledb, "oracledb")
 def connect(
     connection: Optional[str] = None,
     secret_id: Optional[str] = None,
     catalog_id: Optional[str] = None,
     dbname: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
-    read_timeout: Optional[int] = None,
-    write_timeout: Optional[int] = None,
-    connect_timeout: int = 10,
-    cursorclass: Type[Cursor] = Cursor,
-) -> "pymysql.connections.Connection[Any]":
-    """Return a pymysql connection from a Glue Catalog Connection or Secrets Manager.
+    call_timeout: Optional[int] = 0,
+) -> "oracledb.Connection":
+    """Return a oracledb connection from a Glue Catalog Connection.
 
-    https://pymysql.readthedocs.io
+    https://github.com/oracle/python-oracledb
 
     Note
     ----
     You MUST pass a `connection` OR `secret_id`.
     Here is an example of the secret structure in Secrets Manager:
     {
-    "host":"mysql-instance-wrangler.dr8vkeyrb9m1.us-east-1.rds.amazonaws.com",
+    "host":"oracle-instance-wrangler.cr4trrvge8rz.us-east-1.rds.amazonaws.com",
     "username":"test",
     "password":"test",
-    "engine":"mysql",
-    "port":"3306",
+    "engine":"oracle",
+    "port":"1521",
     "dbname": "mydb" # Optional
     }
 
-    Note
-    ----
-    It is only possible to configure SSL using Glue Catalog Connection. More at:
-    https://docs.aws.amazon.com/glue/latest/dg/connection-defining.html
-
-    Note
-    ----
-    Consider using SSCursor `cursorclass` for queries that return a lot of data. More at:
-    https://pymysql.readthedocs.io/en/latest/modules/cursors.html#pymysql.cursors.SSCursor
-
     Parameters
     ----------
-    connection : str
+    connection : Optional[str]
         Glue Catalog Connection name.
     secret_id: Optional[str]:
         Specifies the secret containing the connection details that you want to retrieve.
         You can specify either the Amazon Resource Name (ARN) or the friendly name of the secret.
     catalog_id : str, optional
         The ID of the Data Catalog.
         If none is provided, the AWS account ID is used by default.
     dbname: Optional[str]
         Optional database name to overwrite the stored one.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    read_timeout: Optional[int]
-        The timeout for reading from the connection in seconds (default: None - no timeout).
-        This parameter is forward to pymysql.
-        https://pymysql.readthedocs.io/en/latest/modules/connections.html
-    write_timeout: Optional[int]
-        The timeout for writing to the connection in seconds (default: None - no timeout)
-        This parameter is forward to pymysql.
-        https://pymysql.readthedocs.io/en/latest/modules/connections.html
-    connect_timeout: int
-        Timeout before throwing an exception when connecting.
-        (default: 10, min: 1, max: 31536000)
-        This parameter is forward to pymysql.
-        https://pymysql.readthedocs.io/en/latest/modules/connections.html
-    cursorclass : Cursor
-        Cursor class to use, e.g. SSCursor; defaults to :class:`pymysql.cursors.Cursor`
-        https://pymysql.readthedocs.io/en/latest/modules/cursors.html
+    call_timeout: Optional[int]
+        This is the time in milliseconds that a single round-trip to the database may take before a timeout will occur.
+        The default is None which means no timeout.
+        This parameter is forwarded to oracledb.
+        https://cx-oracle.readthedocs.io/en/latest/api_manual/connection.html#Connection.call_timeout
 
     Returns
     -------
-    pymysql.connections.Connection
-        pymysql connection.
+    oracledb.Connection
+        oracledb connection.
 
     Examples
     --------
     >>> import awswrangler as wr
-    >>> con = wr.mysql.connect("MY_GLUE_CONNECTION")
+    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
     >>> with con.cursor() as cursor:
-    >>>     cursor.execute("SELECT 1")
+    >>>     cursor.execute("SELECT 1 FROM DUAL")
     >>>     print(cursor.fetchall())
     >>> con.close()
 
     """
     attrs: _db_utils.ConnectionAttributes = _db_utils.get_connection_attributes(
         connection=connection, secret_id=secret_id, catalog_id=catalog_id, dbname=dbname, boto3_session=boto3_session
     )
-    if attrs.kind != "mysql":
-        raise exceptions.InvalidDatabaseType(f"Invalid connection type ({attrs.kind}. It must be a MySQL connection.)")
-    return pymysql.connect(
+    if attrs.kind != "oracle":
+        raise exceptions.InvalidDatabaseType(
+            f"Invalid connection type ({attrs.kind}. It must be an oracle connection.)"
+        )
+
+    connection_dsn = oracledb.makedsn(attrs.host, attrs.port, service_name=attrs.database)
+    _logger.debug("DSN: %s", connection_dsn)
+    oracle_connection = oracledb.connect(
         user=attrs.user,
-        database=attrs.database,
         password=attrs.password,
-        port=attrs.port,
-        host=attrs.host,
-        ssl=attrs.ssl_context,  # type: ignore
-        read_timeout=read_timeout,
-        write_timeout=write_timeout,
-        connect_timeout=connect_timeout,
-        cursorclass=cursorclass,
+        dsn=connection_dsn,
     )
+    # oracledb.connect does not have a call_timeout attribute, it has to be set separatly
+    oracle_connection.call_timeout = call_timeout
+    return oracle_connection
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "oracledb.Connection",
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "oracledb.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
 
 
+@overload
 def read_sql_query(
     sql: str,
-    con: "pymysql.connections.Connection[Any]",
+    con: "oracledb.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(oracledb, "oracledb")
+def read_sql_query(
+    sql: str,
+    con: "oracledb.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding to the result set of the query string.
 
     Parameters
     ----------
     sql : str
         SQL query.
-    con : pymysql.connections.Connection
-        Use pymysql.connect() to use credentials directly or wr.mysql.connect() to fetch it from the Glue Catalog.
+    con : oracledb.Connection
+        Use oracledb.connect() to use credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog.
     index_col : Union[str, List[str]], optional
         Column(s) to set as index(MultiIndex).
     params :  Union[List, Tuple, Dict], optional
         List of parameters to pass to execute method.
         The syntax used to pass parameters is database driver dependent.
         Check your database driver documentation for which of the five syntax styles,
         described in PEP 249’s paramstyle, is supported.
@@ -209,60 +251,107 @@
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
     --------
-    Reading from MySQL using a Glue Catalog Connections
+    Reading from Oracle Database using a Glue Catalog Connections
 
     >>> import awswrangler as wr
-    >>> con = wr.mysql.connect("MY_GLUE_CONNECTION")
-    >>> df = wr.mysql.read_sql_query(
+    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
+    >>> df = wr.oracle.read_sql_query(
     ...     sql="SELECT * FROM test.my_table",
     ...     con=con
     ... )
     >>> con.close()
-
     """
     _validate_connection(con=con)
     return _db_utils.read_sql_query(
         sql=sql,
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+@overload
 def read_sql_table(
     table: str,
-    con: "pymysql.connections.Connection[Any]",
+    con: "oracledb.Connection",
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    con: "oracledb.Connection",
+    *,
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    con: "oracledb.Connection",
+    *,
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(oracledb, "oracledb")
+def read_sql_table(
+    table: str,
+    con: "oracledb.Connection",
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding the table.
 
     Parameters
     ----------
     table : str
         Table name.
-    con : pymysql.connections.Connection
-        Use pymysql.connect() to use credentials directly or wr.mysql.connect() to fetch it from the Glue Catalog.
+    con : oracledb.Connection
+        Use oracledb.connect() to use credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog.
     schema : str, optional
-        Name of SQL schema in database to query.
-        Uses default schema if None.
+        Name of SQL schema in database to query (if database flavor supports this).
+        Uses default schema if None (default).
     index_col : Union[str, List[str]], optional
         Column(s) to set as index(MultiIndex).
     params :  Union[List, Tuple, Dict], optional
         List of parameters to pass to execute method.
         The syntax used to pass parameters is database driver dependent.
         Check your database driver documentation for which of the five syntax styles,
         described in PEP 249’s paramstyle, is supported.
@@ -279,173 +368,165 @@
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
     --------
-    Reading from MySQL using a Glue Catalog Connections
+    Reading from Oracle Database using a Glue Catalog Connections
 
     >>> import awswrangler as wr
-    >>> con = wr.mysql.connect("MY_GLUE_CONNECTION")
-    >>> df = wr.mysql.read_sql_table(
+    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
+    >>> df = wr.oracle.read_sql_table(
     ...     table="my_table",
     ...     schema="test",
     ...     con=con
     ... )
     >>> con.close()
-
     """
-    sql: str = f"SELECT * FROM `{table}`" if schema is None else f"SELECT * FROM `{schema}`.`{table}`"
+    table_identifier = _get_table_identifier(schema, table)
+    sql: str = f"SELECT * FROM {table_identifier}"
     return read_sql_query(
         sql=sql,
         con=con,
         index_col=index_col,
         params=params,
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+@_utils.check_optional_dependency(oracledb, "oracledb")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
-    con: "pymysql.connections.Connection[Any]",
+    con: "oracledb.Connection",
     table: str,
     schema: str,
     mode: str = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
     chunksize: int = 200,
-    cursorclass: Type[Cursor] = Cursor,
 ) -> None:
-    """Write records stored in a DataFrame into MySQL.
+    """Write records stored in a DataFrame into Oracle Database.
 
     Parameters
     ----------
     df : pandas.DataFrame
         Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
-    con : pymysql.connections.Connection
-        Use pymysql.connect() to use credentials directly or wr.mysql.connect() to fetch it from the Glue Catalog.
+    con : oracledb.Connection
+        Use oracledb.connect() to use credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog.
     table : str
         Table name
     schema : str
         Schema name
     mode : str
-        Append, overwrite, upsert_duplicate_key, upsert_replace_into, upsert_distinct, ignore.
-            append: Inserts new records into table.
-            overwrite: Drops table and recreates.
-            upsert_duplicate_key: Performs an upsert using `ON DUPLICATE KEY` clause. Requires table schema to have
-            defined keys, otherwise duplicate records will be inserted.
-            upsert_replace_into: Performs upsert using `REPLACE INTO` clause. Less efficient and still requires the
-            table schema to have keys or else duplicate records will be inserted
-            upsert_distinct: Inserts new records, including duplicates, then recreates the table and inserts `DISTINCT`
-            records from old table. This is the least efficient approach but handles scenarios where there are no
-            keys on table.
-            ignore: Inserts new records into table using `INSERT IGNORE` clause.
-
+        Append or overwrite.
     index : bool
         True to store the DataFrame index as a column in the table,
         otherwise False to ignore it.
     dtype: Dict[str, str], optional
-        Dictionary of columns names and MySQL types to be casted.
+        Dictionary of columns names and Oracle types to be casted.
         Useful when you have columns with undetermined or mixed data types.
         (e.g. {'col name': 'TEXT', 'col2 name': 'FLOAT'})
     varchar_lengths : Dict[str, int], optional
         Dict of VARCHAR length by columns. (e.g. {"col1": 10, "col5": 200}).
     use_column_names: bool
         If set to True, will use the column names of the DataFrame for generating the INSERT SQL Query.
         E.g. If the DataFrame has two columns `col1` and `col3` and `use_column_names` is True, data will only be
         inserted into the database columns `col1` and `col3`.
     chunksize: int
         Number of rows which are inserted with each SQL query. Defaults to inserting 200 rows per query.
-    cursorclass : Cursor
-        Cursor class to use, e.g. SSCrusor; defaults to :class:`pymysql.cursors.Cursor`
-        https://pymysql.readthedocs.io/en/latest/modules/cursors.html
 
     Returns
     -------
     None
         None.
 
     Examples
     --------
-    Writing to MySQL using a Glue Catalog Connections
+    Writing to Oracle Database using a Glue Catalog Connections
 
     >>> import awswrangler as wr
-    >>> con = wr.mysql.connect("MY_GLUE_CONNECTION")
-    >>> wr.mysql.to_sql(
+    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
+    >>> wr.oracle.to_sql(
     ...     df=df,
-    ...     table="my_table",
-    ...     schema="test",
+    ...     table="table",
+    ...     schema="ORCL",
     ...     con=con
     ... )
     >>> con.close()
 
     """
     if df.empty is True:
         raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
-
-    mode = mode.strip().lower()
-    allowed_modes = [
-        "append",
-        "overwrite",
-        "upsert_replace_into",
-        "upsert_duplicate_key",
-        "upsert_distinct",
-        "ignore",
-    ]
-    _db_utils.validate_mode(mode=mode, allowed_modes=allowed_modes)
     _validate_connection(con=con)
     try:
-        with con.cursor(cursor=cursorclass) as cursor:  # type: ignore
+        with con.cursor() as cursor:
             _create_table(
                 df=df,
                 cursor=cursor,
                 table=table,
                 schema=schema,
                 mode=mode,
                 index=index,
                 dtype=dtype,
                 varchar_lengths=varchar_lengths,
             )
             if index:
                 df.reset_index(level=df.index.names, inplace=True)
-            column_placeholders: str = ", ".join(["%s"] * len(df.columns))
+            column_placeholders: str = f"({', '.join([':' + str(i + 1) for i in range(len(df.columns))])})"
+            table_identifier = _get_table_identifier(schema, table)
             insertion_columns = ""
-            upsert_columns = ""
-            upsert_str = ""
-            ignore_str = " IGNORE" if mode == "ignore" else ""
             if use_column_names:
-                insertion_columns = f"(`{'`, `'.join(df.columns)}`)"
-            if mode == "upsert_duplicate_key":
-                upsert_columns = ", ".join(df.columns.map(lambda column: f"`{column}`=VALUES(`{column}`)"))
-                upsert_str = f" ON DUPLICATE KEY UPDATE {upsert_columns}"
+                insertion_columns = "(" + ", ".join('"' + column + '"' for column in df.columns) + ")"
+
             placeholder_parameter_pair_generator = _db_utils.generate_placeholder_parameter_pairs(
                 df=df, column_placeholders=column_placeholders, chunksize=chunksize
             )
-            sql: str
-            for placeholders, parameters in placeholder_parameter_pair_generator:
-                if mode == "upsert_replace_into":
-                    sql = f"REPLACE INTO `{schema}`.`{table}` {insertion_columns} VALUES {placeholders}"
-                else:
-                    sql = f"""INSERT{ignore_str} INTO `{schema}`.`{table}` {insertion_columns}
-VALUES {placeholders}{upsert_str}"""
+            for _, parameters in placeholder_parameter_pair_generator:
+                parameters = list(zip(*[iter(parameters)] * len(df.columns)))
+                sql: str = f"INSERT INTO {table_identifier} {insertion_columns} VALUES {column_placeholders}"
                 _logger.debug("sql: %s", sql)
-                cursor.executemany(sql, (parameters,))
+                cursor.executemany(sql, parameters)
             con.commit()
-            if mode == "upsert_distinct":
-                temp_table = f"{table}_{uuid.uuid4().hex}"
-                cursor.execute(f"CREATE TABLE `{schema}`.`{temp_table}` LIKE `{schema}`.`{table}`")
-                cursor.execute(f"INSERT INTO `{schema}`.`{temp_table}` SELECT DISTINCT * FROM `{schema}`.`{table}`")
-                cursor.execute(f"DROP TABLE IF EXISTS `{schema}`.`{table}`")
-                cursor.execute(f"ALTER TABLE `{schema}`.`{temp_table}` RENAME TO `{table}`")
-                con.commit()
-
     except Exception as ex:
         con.rollback()
         _logger.error(ex)
         raise
+
+
+def detect_oracle_decimal_datatype(cursor: Any) -> Dict[str, pa.DataType]:
+    """Determine if a given Oracle column is a decimal, not just a standard float value."""
+    dtype = {}
+    _logger.debug("cursor type: %s", type(cursor))
+    if isinstance(cursor, oracledb.Cursor):
+        # Oracle stores DECIMAL as the NUMBER type
+        for row in cursor.description:
+            if row[1] == oracledb.DB_TYPE_NUMBER and row[5] > 0:  # pylint: disable=no-member
+                dtype[row[0]] = pa.decimal128(row[4], row[5])
+
+    _logger.debug("decimal dtypes: %s", dtype)
+    return dtype
+
+
+def handle_oracle_objects(
+    col_values: List[Any], col_name: str, dtype: Optional[Dict[str, pa.DataType]] = None
+) -> List[Any]:
+    """Get the string representation of an Oracle LOB value, and convert float to decimal."""
+    if any(isinstance(col_value, oracledb.LOB) for col_value in col_values):
+        col_values = [
+            col_value.read() if isinstance(col_value, oracledb.LOB) else col_value for col_value in col_values
+        ]
+
+    if dtype is not None:
+        if isinstance(dtype[col_name], pa.Decimal128Type):
+            _logger.debug("decimal_col_values:\n%s", col_values)
+            col_values = [
+                Decimal(repr(col_value)) if isinstance(col_value, float) else col_value for col_value in col_values
+            ]
+
+    return col_values
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/neptune/_utils.py` & `awswrangler-3.0.0rc3/awswrangler/neptune/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 from gremlin_python.process.graph_traversal import GraphTraversalSource, __
 from gremlin_python.process.translator import Translator
 from gremlin_python.process.traversal import Cardinality, T
 from gremlin_python.structure.graph import Graph
 
 from awswrangler import exceptions
-from awswrangler.neptune.client import NeptuneClient
+from awswrangler.neptune._client import NeptuneClient
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 class WriteDFType(Enum):
     """Dataframe type enum."""
 
@@ -41,15 +41,15 @@
     Returns
     -------
     bool
         True if the write operation succeeded
     """
     g = Graph().traversal()
     # Loop through items in the DF
-    for (index, row) in df.iterrows():
+    for index, row in df.iterrows():
         # build up a query
         if mode == WriteDFType.EDGE:
             g = _build_gremlin_edges(g, row.to_dict())
         elif mode == WriteDFType.VERTEX:
             g = _build_gremlin_vertices(g, row.to_dict())
         else:
             g = _build_gremlin_update(g, row.to_dict())
@@ -104,15 +104,15 @@
     )
     g = _build_gremlin_properties(g, row)
 
     return g
 
 
 def _build_gremlin_properties(g: GraphTraversalSource, row: Any) -> GraphTraversalSource:
-    for (column, value) in row.items():
+    for column, value in row.items():
         if column not in ["~id", "~label", "~to", "~from"]:
             if isinstance(value, list) and len(value) > 0:
                 for item in value:
                     g = g.property(Cardinality.set_, column, item)
             elif not pd.isna(value) and not pd.isnull(value):
                 g = g.property(column, value)
     return g
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/neptune/client.py` & `awswrangler-3.0.0rc3/awswrangler/neptune/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+# mypy: disable-error-code=name-defined
 """Amazon NeptuneClient Module."""
 
-import importlib.util
 import logging
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 import boto3
-import requests
 from botocore.auth import SigV4Auth
-from botocore.awsrequest import AWSRequest
-from gremlin_python.driver import client
+from botocore.awsrequest import AWSPreparedRequest, AWSRequest
 
-from awswrangler import exceptions
-from awswrangler.neptune.gremlin_parser import GremlinParser
-
-_SPARQLWrapper_found = importlib.util.find_spec("SPARQLWrapper")
-if _SPARQLWrapper_found:
-    from SPARQLWrapper import SPARQLWrapper  # pylint: disable=import-error
+import awswrangler.neptune._gremlin_init as gremlin
+from awswrangler import _utils, exceptions
+from awswrangler.neptune._gremlin_parser import GremlinParser
+
+gremlin_python = _utils.import_optional_dependency("gremlin_python")
+opencypher = _utils.import_optional_dependency("requests")
+sparql = _utils.import_optional_dependency("SPARQLWrapper")
+if any((gremlin_python, opencypher, sparql)):
+    import requests
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 DEFAULT_PORT = 8182
 NEPTUNE_SERVICE_NAME = "neptune-db"
 HTTP_PROTOCOL = "https"
@@ -46,26 +47,26 @@
         else:
             self.region = region
         self._http_session = requests.Session()
         self.gremlin_connection = None
 
     def __del__(self) -> None:
         """Close the Gremlin connection."""
-        if isinstance(self.gremlin_connection, client.Client):
+        if isinstance(self.gremlin_connection, gremlin.Client):
             self.gremlin_connection.close()
 
     def __get_region_from_session(self) -> str:
         """Extract region from session."""
         region: Optional[str] = self.boto3_session.region_name
         if region is not None:
             return region
         raise exceptions.InvalidArgument("There is no region_name defined on boto3, please configure it.")
 
     @staticmethod
-    def __ensure_session(session: boto3.Session = None) -> boto3.Session:
+    def __ensure_session(session: Optional[boto3.Session] = None) -> boto3.Session:
         """Ensure that a valid boto3.Session will be returned."""
         if session is not None:
             return session
         if boto3.DEFAULT_SESSION:
             return boto3.DEFAULT_SESSION
 
         return boto3.Session()
@@ -75,15 +76,15 @@
         method: str,
         url: str,
         *,
         data: Any = None,
         params: Any = None,
         headers: Any = None,
         service: str = NEPTUNE_SERVICE_NAME,
-    ) -> requests.PreparedRequest:
+    ) -> "requests.PreparedRequest":
         request = requests.Request(method=method, url=url, data=data, params=params, headers=headers)
         if self.boto3_session is not None:
             aws_request = self._get_aws_request(
                 method=method, url=url, data=data, params=params, headers=headers, service=service
             )
             request.headers = dict(aws_request.headers)
 
@@ -94,15 +95,15 @@
         method: str,
         url: str,
         *,
         data: Any = None,
         params: Any = None,
         headers: Any = None,
         service: str = NEPTUNE_SERVICE_NAME,
-    ) -> AWSRequest:
+    ) -> Union[AWSRequest, AWSPreparedRequest]:
         req = AWSRequest(method=method, url=url, data=data, params=params, headers=headers)
         if self.iam_enabled:
             credentials = self.boto3_session.get_credentials()
             try:
                 frozen_creds = credentials.get_frozen_credentials()
             except AttributeError:
                 _logger.warning("Could not find valid IAM credentials in any the following locations:\n")
@@ -186,26 +187,26 @@
         try:
             c = self._get_gremlin_connection(headers)
             result = c.submit(query)
             future_results = result.all()
             results = future_results.result()
             return GremlinParser.gremlin_results_to_dict(results)
         except Exception as e:
-            if isinstance(self.gremlin_connection, client.Client):
+            if isinstance(self.gremlin_connection, gremlin.Client):
                 self.gremlin_connection.close()
             self.gremlin_connection = None
             _logger.error(e)
             raise exceptions.QueryFailed(e)
 
-    def _get_gremlin_connection(self, headers: Any = None) -> client.Client:
+    def _get_gremlin_connection(self, headers: Any = None) -> "gremlin.Client":
         if self.gremlin_connection is None:
             uri = f"{HTTP_PROTOCOL}://{self.host}:{self.port}/gremlin"
             request = self._prepare_request("GET", uri, headers=headers)
             ws_url = f"{WS_PROTOCOL}://{self.host}:{self.port}/gremlin"
-            self.gremlin_connection = client.Client(
+            self.gremlin_connection = gremlin.Client(
                 ws_url, "g", headers=dict(request.headers), call_from_event_loop=True
             )
         return self.gremlin_connection
 
     def read_sparql(self, query: str, headers: Any = None) -> Any:
         """Execute the given query and returns the results.
 
@@ -243,15 +244,15 @@
         self._execute_sparql(query, headers)
         return True
 
     def _execute_sparql(self, query: str, headers: Any) -> Any:
         if headers is None:
             headers = {}
 
-        s = SPARQLWrapper("")
+        s = sparql.SPARQLWrapper("")
         s.setQuery(query)
         query_type = str(s.queryType).upper()
         if query_type in ["SELECT", "CONSTRUCT", "ASK", "DESCRIBE"]:
             data = {"query": query}
         else:
             data = {"update": query}
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/neptune/gremlin_parser.py` & `awswrangler-3.0.0rc3/awswrangler/neptune/_gremlin_parser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+# mypy: disable-error-code=name-defined
 """Amazon Neptune GremlinParser Module (PRIVATE)."""
 from typing import Any, Dict, List
 
-from gremlin_python.structure.graph import Edge, Path, Property, Vertex, VertexProperty
+import awswrangler.neptune._gremlin_init as gremlin
 
 
 class GremlinParser:
     """Class representing a parser for returning Gremlin results as a dictionary."""
 
     @staticmethod
     def gremlin_results_to_dict(result: Any) -> List[Dict[str, Any]]:
         """Take a Gremlin ResultSet and return a dictionary.
 
         Parameters
         ----------
         result : Any
-            The Gremlin resultset to convert
+            The Gremlin result set to convert
 
         Returns
         -------
         List[Dict[str, Any]]
             A list of dictionary results
         """
         res = []
 
         # For lists or paths unwind them
-        if isinstance(result, (list, Path)):
+        if isinstance(result, (list, gremlin.Path)):
             for x in result:
                 res.append(GremlinParser._parse_dict(x))
 
         # For dictionaries just add them
         elif isinstance(result, dict):
             res.append(result)
 
@@ -38,36 +39,52 @@
         return res
 
     @staticmethod
     def _parse_dict(data: Any) -> Any:
         d: Dict[str, Any] = {}
 
         # If this is a list or Path then unwind it
-        if isinstance(data, (list, Path)):
+        if isinstance(data, (list, gremlin.Path)):
             res = []
             for x in data:
                 res.append(GremlinParser._parse_dict(x))
             return res
 
         # If this is an element then make it a dictionary
-        if isinstance(data, (Vertex, Edge, VertexProperty, Property)):
+        if isinstance(
+            data,
+            (
+                gremlin.Vertex,
+                gremlin.Edge,
+                gremlin.VertexProperty,
+                gremlin.Property,
+            ),
+        ):
             data = data.__dict__
 
         # If this is a scalar then create a Map with it
         elif not hasattr(data, "__len__") or isinstance(data, str):
             data = {0: data}
 
-        for (k, v) in data.items():
+        for k, v in data.items():
             # If the key is a Vertex or an Edge do special processing
-            if isinstance(k, (Vertex, Edge)):
+            if isinstance(k, (gremlin.Vertex, gremlin.Edge)):
                 k = k.id
 
             # If the value is a list do special processing to make it a scalar if the list is of length 1
             if isinstance(v, list) and len(v) == 1:
                 d[k] = v[0]
             else:
                 d[k] = v
 
             # If the value is a Vertex or Edge do special processing
-            if isinstance(data, (Vertex, Edge, VertexProperty, Property)):
+            if isinstance(
+                data,
+                (
+                    gremlin.Vertex,
+                    gremlin.Edge,
+                    gremlin.VertexProperty,
+                    gremlin.Property,
+                ),
+            ):
                 d[k] = d[k].__dict__
         return d
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/neptune/neptune.py` & `awswrangler-3.0.0rc3/awswrangler/neptune/_neptune.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,37 @@
+# mypy: disable-error-code=name-defined
 """Amazon Neptune Module."""
 
-import importlib.util
-import inspect
 import logging
 import re
 from typing import Any, Callable, TypeVar
 
 import pandas as pd
-from gremlin_python.process.anonymous_traversal import traversal
-from gremlin_python.process.graph_traversal import GraphTraversalSource, __
-from gremlin_python.process.translator import Translator
-from gremlin_python.process.traversal import Cardinality, T
-from gremlin_python.structure.graph import Graph
 
-from awswrangler import exceptions
-from awswrangler.neptune.client import NeptuneClient
-
-_SPARQLWrapper_found = importlib.util.find_spec("SPARQLWrapper")
+import awswrangler.neptune._gremlin_init as gremlin
+from awswrangler import _utils, exceptions
+from awswrangler.neptune._client import NeptuneClient
+
+gremlin_python = _utils.import_optional_dependency("gremlin_python")
+opencypher = _utils.import_optional_dependency("requests")
+sparql = _utils.import_optional_dependency("SPARQLWrapper")
 
 _logger: logging.Logger = logging.getLogger(__name__)
 FuncT = TypeVar("FuncT", bound=Callable[..., Any])
 
 
-def _check_for_sparqlwrapper(func: FuncT) -> FuncT:
-    def inner(*args: Any, **kwargs: Any) -> Any:
-        if not _SPARQLWrapper_found:
-            raise ModuleNotFoundError(
-                "You need to install SPARQLWrapper respectively the "
-                "AWS SDK for pandas package with the `sparql` extra for being able to use SPARQL "
-            )
-        return func(*args, **kwargs)
-
-    inner.__doc__ = func.__doc__
-    inner.__name__ = func.__name__
-    inner.__setattr__("__signature__", inspect.signature(func))  # pylint: disable=no-member
-    return inner  # type: ignore
-
-
+@_utils.check_optional_dependency(gremlin_python, "gremlin_python")
 def execute_gremlin(client: NeptuneClient, query: str) -> pd.DataFrame:
     """Return results of a Gremlin traversal as pandas dataframe.
 
     Parameters
     ----------
     client : neptune.Client
         instance of the neptune client to use
-    traversal : str
+    query : str
         The gremlin traversal to execute
 
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Results as Pandas DataFrame
 
@@ -61,14 +44,15 @@
     >>> df = wr.neptune.execute_gremlin(client, "g.V().limit(1)")
     """
     results = client.read_gremlin(query)
     df = pd.DataFrame.from_records(results)
     return df
 
 
+@_utils.check_optional_dependency(opencypher, "opencypher")
 def execute_opencypher(client: NeptuneClient, query: str) -> pd.DataFrame:
     """Return results of a openCypher traversal as pandas dataframe.
 
     Parameters
     ----------
     client : NeptuneClient
         instance of the neptune client to use
@@ -89,15 +73,15 @@
     >>> resp = wr.neptune.execute_opencypher(client, "MATCH (n) RETURN n LIMIT 1")
     """
     resp = client.read_opencypher(query)
     df = pd.DataFrame.from_dict(resp)
     return df
 
 
-@_check_for_sparqlwrapper
+@_utils.check_optional_dependency(sparql, "SPARQLWrapper")
 def execute_sparql(client: NeptuneClient, query: str) -> pd.DataFrame:
     """Return results of a SPARQL query as pandas dataframe.
 
     Parameters
     ----------
     client : NeptuneClient
         instance of the neptune client to use
@@ -127,14 +111,15 @@
         df.applymap(lambda x: x["value"])
     else:
         df = pd.DataFrame(data)
 
     return df
 
 
+@_utils.check_optional_dependency(gremlin_python, "gremlin_python")
 def to_property_graph(
     client: NeptuneClient, df: pd.DataFrame, batch_size: int = 50, use_header_cardinality: bool = True
 ) -> bool:
     """Write records stored in a DataFrame into Amazon Neptune.
 
     If writing to a property graph then DataFrames for vertices and edges must be written separately.
     DataFrames for vertices must have a ~label column with the label and a ~id column for the vertex id.
@@ -172,46 +157,46 @@
     >>> import awswrangler as wr
     >>> client = wr.neptune.connect(neptune_endpoint, neptune_port, iam_enabled=False)
     >>> wr.neptune.gremlin.to_property_graph(
     ...     df=df
     ... )
     """
     # check if ~id and ~label column exist and if not throw error
-    g = traversal().withGraph(Graph())
+    g = gremlin.traversal().withGraph(gremlin.Graph())
     is_edge_df = False
     is_update_df = True
     if "~id" in df.columns:
         if "~label" in df.columns:
             is_update_df = False
             if "~to" in df.columns and "~from" in df.columns:
                 is_edge_df = True
     else:
         raise exceptions.InvalidArgumentValue(
             "Dataframe must contain at least a ~id and a ~label column to be saved to Amazon Neptune"
         )
 
     # Loop through items in the DF
-    for (index, row) in df.iterrows():
+    for index, row in df.iterrows():
         # build up a query
         if is_update_df:
             g = _build_gremlin_update(g, row, use_header_cardinality)
         elif is_edge_df:
             g = _build_gremlin_insert_edges(g, row.to_dict(), use_header_cardinality)
         else:
             g = _build_gremlin_insert_vertices(g, row.to_dict(), use_header_cardinality)
         # run the query
         if index > 0 and index % batch_size == 0:
             res = _run_gremlin_insert(client, g)
             if res:
-                g = Graph().traversal()
+                g = gremlin.Graph().traversal()
 
     return _run_gremlin_insert(client, g)
 
 
-@_check_for_sparqlwrapper
+@_utils.check_optional_dependency(sparql, "SPARQLWrapper")
 def to_rdf_graph(
     client: NeptuneClient,
     df: pd.DataFrame,
     batch_size: int = 50,
     subject_column: str = "s",
     predicate_column: str = "p",
     object_column: str = "o",
@@ -260,15 +245,15 @@
         raise exceptions.InvalidArgumentValue(
             """Dataframe must contain at least the subject, predicate, and object columns defined or the defaults
             (s, p, o) to be saved to Amazon Neptune"""
         )
 
     query = ""
     # Loop through items in the DF
-    for (index, row) in df.iterrows():
+    for index, row in df.iterrows():
         # build up a query
         if is_quads:
             insert = f"""INSERT DATA {{ GRAPH <{row[graph_column]}> {{<{row[subject_column]}>
                     <{str(row[predicate_column])}> <{row[object_column]}> . }} }}; """
             query = query + insert
         else:
             insert = f"""INSERT DATA {{ <{row[subject_column]}> <{str(row[predicate_column])}>
@@ -305,113 +290,131 @@
 def _get_column_name(column: str) -> str:
     if "(single)" in column.lower():
         return re.compile(r"\(single\)", re.IGNORECASE).sub("", column)
     return column
 
 
 def _set_properties(
-    g: GraphTraversalSource, use_header_cardinality: bool, row: Any, ignore_cardinality: bool = False
-) -> GraphTraversalSource:
-    for (column, value) in row.items():
+    g: "gremlin.GraphTraversalSource",
+    use_header_cardinality: bool,
+    row: Any,
+    ignore_cardinality: bool = False,
+) -> "gremlin.GraphTraversalSource":
+    for column, value in row.items():
         if column not in ["~id", "~label", "~to", "~from"]:
             if ignore_cardinality and pd.notna(value):
                 g = g.property(_get_column_name(column), value)
             else:
                 # If the column header is specifying the cardinality then use it
                 if use_header_cardinality:
                     if column.lower().find("(single)") > 0 and pd.notna(value):
-                        g = g.property(Cardinality.single, _get_column_name(column), value)
+                        g = g.property(gremlin.Cardinality.single, _get_column_name(column), value)
                     else:
                         g = _expand_properties(g, _get_column_name(column), value)
                 else:
                     # If not using header cardinality then use the default of set
                     g = _expand_properties(g, column, value)
     return g
 
 
-def _expand_properties(g: GraphTraversalSource, column: str, value: Any) -> GraphTraversalSource:
+def _expand_properties(g: "gremlin.GraphTraversalSource", column: str, value: Any) -> "gremlin.GraphTraversalSource":
     # If this is a list then expand it out into multiple property calls
     if isinstance(value, list) and len(value) > 0:
         for item in value:
-            g = g.property(Cardinality.set_, column, item)
+            g = g.property(gremlin.Cardinality.set_, column, item)
     elif pd.notna(value):
-        g = g.property(Cardinality.set_, column, value)
+        g = g.property(gremlin.Cardinality.set_, column, value)
     return g
 
 
-def _build_gremlin_update(g: GraphTraversalSource, row: Any, use_header_cardinality: bool) -> GraphTraversalSource:
+def _build_gremlin_update(
+    g: "gremlin.GraphTraversalSource", row: Any, use_header_cardinality: bool
+) -> "gremlin.GraphTraversalSource":
     g = g.V(str(row["~id"]))
     g = _set_properties(g, use_header_cardinality, row)
     return g
 
 
 def _build_gremlin_insert_vertices(
-    g: GraphTraversalSource, row: Any, use_header_cardinality: bool = False
-) -> GraphTraversalSource:
-    g = g.V(str(row["~id"])).fold().coalesce(__.unfold(), __.addV(row["~label"]).property(T.id, str(row["~id"])))
+    g: "gremlin.GraphTraversalSource", row: Any, use_header_cardinality: bool = False
+) -> "gremlin.GraphTraversalSource":
+    g = (
+        g.V(str(row["~id"]))
+        .fold()
+        .coalesce(
+            gremlin.__.unfold(),
+            gremlin.__.addV(row["~label"]).property(gremlin.T.id, str(row["~id"])),
+        )
+    )
     g = _set_properties(g, use_header_cardinality, row)
     return g
 
 
 def _build_gremlin_insert_edges(
-    g: GraphTraversalSource, row: pd.Series, use_header_cardinality: bool
-) -> GraphTraversalSource:
+    g: "gremlin.GraphTraversalSource", row: pd.Series, use_header_cardinality: bool
+) -> "gremlin.GraphTraversalSource":
     g = (
         g.V(str(row["~from"]))
         .fold()
-        .coalesce(__.unfold(), _build_gremlin_insert_vertices(__, {"~id": row["~from"], "~label": "Vertex"}))
+        .coalesce(
+            gremlin.__.unfold(),
+            _build_gremlin_insert_vertices(gremlin.__, {"~id": row["~from"], "~label": "Vertex"}),
+        )
         .addE(row["~label"])
-        .property(T.id, str(row["~id"]))
+        .property(gremlin.T.id, str(row["~id"]))
         .to(
-            __.V(str(row["~to"]))
+            gremlin.__.V(str(row["~to"]))
             .fold()
-            .coalesce(__.unfold(), _build_gremlin_insert_vertices(__, {"~id": row["~to"], "~label": "Vertex"}))
+            .coalesce(
+                gremlin.__.unfold(),
+                _build_gremlin_insert_vertices(gremlin.__, {"~id": row["~to"], "~label": "Vertex"}),
+            )
         )
     )
     g = _set_properties(g, use_header_cardinality, row, ignore_cardinality=True)
 
     return g
 
 
-def _run_gremlin_insert(client: NeptuneClient, g: GraphTraversalSource) -> bool:
-    translator = Translator("g")
+def _run_gremlin_insert(client: NeptuneClient, g: "gremlin.GraphTraversalSource") -> bool:
+    translator = gremlin.Translator("g")
     s = translator.translate(g.bytecode)
     s = s.replace("Cardinality.", "")  # hack to fix parser error for set cardinality
     s = s.replace(
         ".values('shape')", ""
     )  # hack to fix parser error for adding unknown values('shape') steps to translation.
     _logger.debug(s)
     res = client.write_gremlin(s)
     return res
 
 
 def flatten_nested_df(
-    df: pd.DataFrame, include_prefix: bool = True, seperator: str = "_", recursive: bool = True
+    df: pd.DataFrame, include_prefix: bool = True, separator: str = "_", recursive: bool = True
 ) -> pd.DataFrame:
     """Flatten the lists and dictionaries of the input data frame.
 
     Parameters
     ----------
     df : pd.DataFrame
         The input data frame
     include_prefix : bool, optional
         If True, then it will prefix the new column name with the original column name.
         Defaults to True.
-    seperator : str, optional
-        The seperator to use between field names when a dictionary is exploded.
+    separator : str, optional
+        The separator to use between field names when a dictionary is exploded.
         Defaults to "_".
     recursive : bool, optional
         If True, then this will recurse the fields in the data frame. Defaults to True.
 
     Returns
     -------
         pd.DataFrame: The flattened data frame
     """
-    if seperator is None:
-        seperator = "_"
+    if separator is None:
+        separator = "_"
     df = df.reset_index()
 
     # search for list and map
     s = (df.applymap(type) == list).all()
     list_columns = s[s].index.tolist()
 
     s = (df.applymap(type) == dict).all()
@@ -420,17 +423,17 @@
     if len(list_columns) > 0 or len(dict_columns) > 0:
         new_columns = []
 
         for col in dict_columns:
             # expand dictionaries horizontally
             expanded = None
             if include_prefix:
-                expanded = pd.json_normalize(df[col], sep=seperator).add_prefix(f"{col}{seperator}")
+                expanded = pd.json_normalize(df[col], sep=separator).add_prefix(f"{col}{separator}")
             else:
-                expanded = pd.json_normalize(df[col], sep=seperator).add_prefix(f"{seperator}")
+                expanded = pd.json_normalize(df[col], sep=separator).add_prefix(f"{separator}")
             expanded.index = df.index
             df = pd.concat([df, expanded], axis=1).drop(columns=[col])
             new_columns.extend(expanded.columns)
 
         for col in list_columns:
             df = df.drop(columns=[col]).join(df[col].explode().to_frame())
             new_columns.append(col)
@@ -438,10 +441,10 @@
         # check if there are still dict o list fields to flatten
         s = (df[new_columns].applymap(type) == list).all()
         list_columns = s[s].index.tolist()
 
         s = (df[new_columns].applymap(type) == dict).all()
         dict_columns = s[s].index.tolist()
         if recursive and (len(list_columns) > 0 or len(dict_columns) > 0):
-            df = flatten_nested_df(df, include_prefix=include_prefix, seperator=seperator, recursive=recursive)
+            df = flatten_nested_df(df, include_prefix=include_prefix, separator=separator, recursive=recursive)
 
     return df
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/opensearch/_read.py` & `awswrangler-3.0.0rc3/awswrangler/opensearch/_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+# mypy: disable-error-code=name-defined
 """Amazon OpenSearch Read Module (PRIVATE)."""
 
 from typing import Any, Collection, Dict, List, Mapping, Optional, Union
 
 import pandas as pd
-from opensearchpy import OpenSearch
-from opensearchpy.helpers import scan
 
-from awswrangler.opensearch._utils import _get_distribution
+from awswrangler import _utils, exceptions
+from awswrangler.opensearch._utils import _get_distribution, _is_serverless
+
+opensearchpy = _utils.import_optional_dependency("opensearchpy")
 
 
 def _resolve_fields(row: Mapping[str, Any]) -> Mapping[str, Any]:
     fields = {}
     for field in row:
         if isinstance(row[field], dict):
             nested_fields = _resolve_fields(row[field])
@@ -29,23 +31,24 @@
             row.update(solved_fields)
         elif k.startswith("_"):
             row[k] = hit[k]
     return row
 
 
 def _search_response_to_documents(response: Mapping[str, Any]) -> List[Mapping[str, Any]]:
-    return [_hit_to_row(hit) for hit in response["hits"]["hits"]]
+    return [_hit_to_row(hit) for hit in response.get("hits", {}).get("hits", [])]
 
 
 def _search_response_to_df(response: Union[Mapping[str, Any], Any]) -> pd.DataFrame:
     return pd.DataFrame(_search_response_to_documents(response))
 
 
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def search(
-    client: OpenSearch,
+    client: "opensearchpy.OpenSearch",
     index: Optional[str] = "_all",
     search_body: Optional[Dict[str, Any]] = None,
     doc_type: Optional[str] = None,
     is_scroll: Optional[bool] = False,
     filter_path: Optional[Union[str, Collection[str]]] = None,
     **kwargs: Any,
 ) -> pd.DataFrame:
@@ -98,34 +101,40 @@
     ...             }
     ...           }
     ...         }
     ...      )
 
 
     """
+    if is_scroll and _is_serverless(client):
+        raise exceptions.NotSupported("Scrolled search is not currently available for OpenSearch Serverless.")
+
     if doc_type:
         kwargs["doc_type"] = doc_type
 
     if filter_path is None:
         filter_path = ["hits.hits._id", "hits.hits._source"]
 
     if is_scroll:
         if isinstance(filter_path, str):
             filter_path = [filter_path]
         filter_path = ["_scroll_id", "_shards"] + list(filter_path)  # required for scroll
-        documents_generator = scan(client, index=index, query=search_body, filter_path=filter_path, **kwargs)
+        documents_generator = opensearchpy.helpers.scan(
+            client, index=index, query=search_body, filter_path=filter_path, **kwargs
+        )
         documents = [_hit_to_row(doc) for doc in documents_generator]
         df = pd.DataFrame(documents)
     else:
         response = client.search(index=index, body=search_body, filter_path=filter_path, **kwargs)
         df = _search_response_to_df(response)
     return df
 
 
-def search_by_sql(client: OpenSearch, sql_query: str, **kwargs: Any) -> pd.DataFrame:
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
+def search_by_sql(client: "opensearchpy.OpenSearch", sql_query: str, **kwargs: Any) -> pd.DataFrame:
     """Return results matching `SQL query <https://opensearch.org/docs/search-plugins/sql/index/>`_ as pandas dataframe.
 
     Parameters
     ----------
     client : OpenSearch
         instance of opensearchpy.OpenSearch to use.
     sql_query : str
@@ -147,23 +156,26 @@
     >>> df = wr.opensearch.search_by_sql(
     >>>         client=client,
     >>>         sql_query='SELECT * FROM my-index LIMIT 50'
     >>>      )
 
 
     """
+    if _is_serverless(client):
+        raise exceptions.NotSupported("SQL plugin is not currently available for OpenSearch Serverless.")
+
     if _get_distribution(client) == "opensearch":
         url = "/_plugins/_sql"
     else:
         url = "/_opendistro/_sql"
 
     kwargs["format"] = "json"
     body = {"query": sql_query}
     for size_att in ["size", "fetch_size"]:
         if size_att in kwargs:
             body["fetch_size"] = kwargs[size_att]
             del kwargs[size_att]  # unrecognized parameter
     response = client.transport.perform_request(
-        "POST", url, headers={"Content-Type": "application/json"}, body=body, params=kwargs
+        "POST", url, headers={"content-type": "application/json"}, body=body, params=kwargs
     )
     df = _search_response_to_df(response)
     return df
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/opensearch/_write.py` & `awswrangler-3.0.0rc3/awswrangler/opensearch/_write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+# mypy: disable-error-code=name-defined
 """Amazon OpenSearch Write Module (PRIVATE)."""
 
 import ast
 import json
 import logging
 import uuid
 from typing import Any, Dict, Generator, Iterable, List, Mapping, Optional, Tuple, Union
 
 import boto3
 import numpy as np
 import pandas as pd
-import progressbar
-from jsonpath_ng import parse
-from jsonpath_ng.exceptions import JsonPathParserError
-from opensearchpy import OpenSearch, TransportError
-from opensearchpy.exceptions import NotFoundError
-from opensearchpy.helpers import bulk
 from pandas import notna
 
+from awswrangler import _utils, exceptions
 from awswrangler._utils import parse_path
-from awswrangler.opensearch._utils import _get_distribution, _get_version_major
+from awswrangler.opensearch._utils import _get_distribution, _get_version_major, _is_serverless
+
+progressbar = _utils.import_optional_dependency("progressbar")
+opensearchpy = _utils.import_optional_dependency("opensearchpy")
+if opensearchpy:
+    from jsonpath_ng import parse
+    from jsonpath_ng.exceptions import JsonPathParserError
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 _DEFAULT_REFRESH_INTERVAL = "1s"
 
 
 def _selected_keys(document: Mapping[str, Any], keys_to_write: Optional[List[str]]) -> Mapping[str, Any]:
@@ -108,42 +110,44 @@
                 output_documents.append(match_value)
             else:
                 msg = f"expected json_path value to be a list/dict. received type {type(match_value)} ({match_value})"
                 raise ValueError(msg)
     return output_documents
 
 
-def _get_refresh_interval(client: OpenSearch, index: str) -> Any:
+def _get_refresh_interval(client: "opensearchpy.OpenSearch", index: str) -> Any:
     url = f"/{index}/_settings"
     try:
         response = client.transport.perform_request("GET", url)
-        index_settings = response.get(index, {}).get("index", {})  # type: ignore
+        index_settings = response.get(index, {}).get("index", {})
         refresh_interval = index_settings.get("refresh_interval", _DEFAULT_REFRESH_INTERVAL)
         return refresh_interval
-    except NotFoundError:
-        return None
+    except opensearchpy.exceptions.NotFoundError:
+        return _DEFAULT_REFRESH_INTERVAL
 
 
-def _set_refresh_interval(client: OpenSearch, index: str, refresh_interval: Optional[Any]) -> Any:
+def _set_refresh_interval(client: "opensearchpy.OpenSearch", index: str, refresh_interval: Optional[Any]) -> Any:
     url = f"/{index}/_settings"
     body = {"index": {"refresh_interval": refresh_interval}}
-    response = client.transport.perform_request("PUT", url, headers={"Content-Type": "application/json"}, body=body)
-
-    return response
+    try:
+        return client.transport.perform_request("PUT", url, headers={"content-type": "application/json"}, body=body)
+    except opensearchpy.exceptions.RequestError:
+        return None
 
 
 def _disable_refresh_interval(
-    client: OpenSearch,
+    client: "opensearchpy.OpenSearch",
     index: str,
 ) -> Any:
     return _set_refresh_interval(client=client, index=index, refresh_interval="-1")
 
 
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def create_index(
-    client: OpenSearch,
+    client: "opensearchpy.OpenSearch",
     index: str,
     doc_type: Optional[str] = None,
     settings: Optional[Dict[str, Any]] = None,
     mappings: Optional[Dict[str, Any]] = None,
 ) -> Dict[str, Any]:
     """Create an index.
 
@@ -199,26 +203,27 @@
             if doc_type:
                 body["mappings"] = {doc_type: mappings}
             else:
                 body["mappings"] = {index: mappings}
     if settings:
         body["settings"] = settings
     if not body:
-        body = None  # type: ignore
+        body = None  # type: ignore[assignment]
 
     # ignore 400 cause by IndexAlreadyExistsException when creating an index
     response: Dict[str, Any] = client.indices.create(index, body=body, ignore=400)
     if "error" in response:
         _logger.warning(response)
         if str(response["error"]).startswith("MapperParsingException"):
             raise ValueError(response["error"])
     return response
 
 
-def delete_index(client: OpenSearch, index: str) -> Dict[str, Any]:
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
+def delete_index(client: "opensearchpy.OpenSearch", index: str) -> Dict[str, Any]:
     """Delete an index.
 
     Parameters
     ----------
     client : OpenSearch
         instance of opensearchpy.OpenSearch to use.
     index : str
@@ -244,23 +249,24 @@
     # ignore 400/404 IndexNotFoundError exception
     response: Dict[str, Any] = client.indices.delete(index, ignore=[400, 404])
     if "error" in response:
         _logger.warning(response)
     return response
 
 
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def index_json(
-    client: OpenSearch,
+    client: "opensearchpy.OpenSearch",
     path: str,
     index: str,
     doc_type: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = boto3.Session(),
     json_path: Optional[str] = None,
     **kwargs: Any,
-) -> Dict[str, Any]:
+) -> Any:
     """Index all documents from JSON file to OpenSearch index.
 
     The JSON file should be in a JSON-Lines text format (newline-delimited JSON) - https://jsonlines.org/
     OR if the is a single large JSON please provide `json_path`.
 
     Parameters
     ----------
@@ -318,22 +324,23 @@
     else:  # local path
         documents = list(_file_line_generator(path, is_json=True))
         if json_path:
             documents = _get_documents_w_json_path(documents, json_path)
     return index_documents(client=client, documents=documents, index=index, doc_type=doc_type, **kwargs)
 
 
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def index_csv(
-    client: OpenSearch,
+    client: "opensearchpy.OpenSearch",
     path: str,
     index: str,
     doc_type: Optional[str] = None,
     pandas_kwargs: Optional[Dict[str, Any]] = None,
     **kwargs: Any,
-) -> Dict[str, Any]:
+) -> Any:
     """Index all documents from a CSV file to OpenSearch index.
 
     Parameters
     ----------
     client : OpenSearch
         instance of opensearchpy.OpenSearch to use.
     path : str
@@ -389,17 +396,18 @@
         # Note: if the user will pass na_filter=False null fields will be indexed as well ({"k1": null, "k2": null})
     }
     pandas_kwargs.update(enforced_pandas_params)
     df = pd.read_csv(path, **pandas_kwargs)
     return index_df(client, df=df, index=index, doc_type=doc_type, **kwargs)
 
 
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def index_df(
-    client: OpenSearch, df: pd.DataFrame, index: str, doc_type: Optional[str] = None, **kwargs: Any
-) -> Dict[str, Any]:
+    client: "opensearchpy.OpenSearch", df: pd.DataFrame, index: str, doc_type: Optional[str] = None, **kwargs: Any
+) -> Any:
     """Index all documents from a DataFrame to OpenSearch index.
 
     Parameters
     ----------
     client : OpenSearch
         instance of opensearchpy.OpenSearch to use.
     df : pd.DataFrame
@@ -430,16 +438,17 @@
     ...     df=pd.DataFrame([{'_id': '1'}, {'_id': '2'}, {'_id': '3'}]),
     ...     index='sample-index1'
     ... )
     """
     return index_documents(client=client, documents=_df_doc_generator(df), index=index, doc_type=doc_type, **kwargs)
 
 
+@_utils.check_optional_dependency(opensearchpy, "opensearchpy")
 def index_documents(
-    client: OpenSearch,
+    client: "opensearchpy.OpenSearch",
     documents: Iterable[Mapping[str, Any]],
     index: str,
     doc_type: Optional[str] = None,
     keys_to_write: Optional[List[str]] = None,
     id_keys: Optional[List[str]] = None,
     ignore_status: Optional[Union[List[Any], Tuple[Any]]] = None,
     bulk_size: int = 1000,
@@ -513,56 +522,63 @@
     >>> import awswrangler as wr
     >>> client = wr.opensearch.connect(host='DOMAIN-ENDPOINT')
     >>> wr.opensearch.index_documents(
     ...     documents=[{'_id': '1', 'value': 'foo'}, {'_id': '2', 'value': 'bar'}],
     ...     index='sample-index1'
     ... )
     """
+    if "refresh" in kwargs and _is_serverless(client):
+        raise exceptions.NotSupported("Refresh policy not supported in OpenSearch Serverless.")
+
     if not isinstance(documents, list):
         documents = list(documents)
     total_documents = len(documents)
     _logger.debug("indexing %s documents into %s", total_documents, index)
 
     actions = _actions_generator(
         documents, index, doc_type, keys_to_write=keys_to_write, id_keys=id_keys, bulk_size=bulk_size
     )
 
     success = 0
     errors: List[Any] = []
     refresh_interval = None
     try:
-        widgets = [
-            progressbar.Percentage(),
-            progressbar.SimpleProgress(format=" (%(value_s)s/%(max_value_s)s)"),
-            progressbar.Bar(),
-            progressbar.Timer(),
-        ]
-        progress_bar = progressbar.ProgressBar(widgets=widgets, max_value=total_documents, prefix="Indexing: ").start()
+        if progressbar:
+            widgets = [
+                progressbar.Percentage(),
+                progressbar.SimpleProgress(format=" (%(value_s)s/%(max_value_s)s)"),
+                progressbar.Bar(),
+                progressbar.Timer(),
+            ]
+            progress_bar = progressbar.ProgressBar(
+                widgets=widgets, max_value=total_documents, prefix="Indexing: "
+            ).start()
         for i, bulk_chunk_documents in enumerate(actions):
             if i == 1:  # second bulk iteration, in case the index didn't exist before
                 refresh_interval = _get_refresh_interval(client, index)
                 _disable_refresh_interval(client, index)
             _logger.debug("running bulk index of %s documents", len(bulk_chunk_documents))
-            _success, _errors = bulk(
+            _success, _errors = opensearchpy.helpers.bulk(
                 client=client,
                 actions=bulk_chunk_documents,
                 ignore_status=ignore_status,
                 chunk_size=chunk_size,
                 max_chunk_bytes=max_chunk_bytes,
                 max_retries=max_retries,
                 initial_backoff=initial_backoff,
                 max_backoff=max_backoff,
                 request_timeout=30,
                 **kwargs,
             )
             success += _success
-            errors += _errors  # type: ignore
+            errors += _errors
             _logger.debug("indexed %s documents (%s/%s)", _success, success, total_documents)
-            progress_bar.update(success, force=True)
-    except TransportError as e:
+            if progressbar:
+                progress_bar.update(success, force=True)
+    except opensearchpy.TransportError as e:
         if str(e.status_code) == "429":  # Too Many Requests
             _logger.error(
                 "Error 429 (Too Many Requests):"
                 "Try to tune bulk_size parameter."
                 "Read more here: https://aws.amazon.com/premiumsupport/knowledge-center/resolve-429-error-es"
             )
             raise e
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/oracle.py` & `awswrangler-3.0.0rc3/awswrangler/sqlserver.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,138 +1,112 @@
-"""Amazon Oracle Database Module."""
+# mypy: disable-error-code=name-defined
+"""Amazon Microsoft SQL Server Module."""
 
-import importlib.util
-import inspect
 import logging
-from decimal import Decimal
-from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, TypeVar, Union, overload
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 
-from awswrangler import _data_types
+from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
-from awswrangler import exceptions
 from awswrangler._config import apply_configs
 
 __all__ = ["connect", "read_sql_query", "read_sql_table", "to_sql"]
 
-_oracledb_found = importlib.util.find_spec("oracledb")
-if _oracledb_found:
-    import oracledb  # pylint: disable=import-error
+pyodbc = _utils.import_optional_dependency("pyodbc")
 
 _logger: logging.Logger = logging.getLogger(__name__)
 FuncT = TypeVar("FuncT", bound=Callable[..., Any])
 
 
-def _check_for_oracledb(func: FuncT) -> FuncT:
-    def inner(*args: Any, **kwargs: Any) -> Any:
-        if not _oracledb_found:
-            raise ModuleNotFoundError(
-                "You need to install oracledb respectively the "
-                "AWS SDK for pandas package with the `oracle` extra for using the oracle module"
-            )
-        return func(*args, **kwargs)
-
-    inner.__doc__ = func.__doc__
-    inner.__name__ = func.__name__
-    inner.__setattr__("__signature__", inspect.signature(func))  # pylint: disable=no-member
-    return inner  # type: ignore
-
-
-def _validate_connection(con: "oracledb.Connection") -> None:
-    if not isinstance(con, oracledb.Connection):
+def _validate_connection(con: "pyodbc.Connection") -> None:
+    if not isinstance(con, pyodbc.Connection):
         raise exceptions.InvalidConnection(
             "Invalid 'conn' argument, please pass a "
-            "oracledb.Connection object. Use oracledb.connect() to use "
-            "credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog."
+            "pyodbc.Connection object. Use pyodbc.connect() to use "
+            "credentials directly or wr.sqlserver.connect() to fetch it from the Glue Catalog."
         )
 
 
 def _get_table_identifier(schema: Optional[str], table: str) -> str:
     schema_str = f'"{schema}".' if schema else ""
     table_identifier = f'{schema_str}"{table}"'
     return table_identifier
 
 
-def _drop_table(cursor: "oracledb.Cursor", schema: Optional[str], table: str) -> None:
+def _drop_table(cursor: "pyodbc.Cursor", schema: Optional[str], table: str) -> None:
     table_identifier = _get_table_identifier(schema, table)
-    sql = f"""
-BEGIN
-    EXECUTE IMMEDIATE 'DROP TABLE {table_identifier}';
-EXCEPTION
-    WHEN OTHERS THEN
-        IF SQLCODE != -942 THEN
-            RAISE;
-        END IF;
-END;
-"""
+    sql = f"IF OBJECT_ID(N'{table_identifier}', N'U') IS NOT NULL DROP TABLE {table_identifier}"
     _logger.debug("Drop table query:\n%s", sql)
     cursor.execute(sql)
 
 
-def _does_table_exist(cursor: "oracledb.Cursor", schema: Optional[str], table: str) -> bool:
-    schema_str = f"OWNER = '{schema}' AND" if schema else ""
-    cursor.execute(f"SELECT * FROM ALL_TABLES WHERE {schema_str} TABLE_NAME = '{table}'")
+def _does_table_exist(cursor: "pyodbc.Cursor", schema: Optional[str], table: str) -> bool:
+    schema_str = f"TABLE_SCHEMA = '{schema}' AND" if schema else ""
+    cursor.execute(f"SELECT * FROM INFORMATION_SCHEMA.TABLES WHERE " f"{schema_str} TABLE_NAME = '{table}'")
     return len(cursor.fetchall()) > 0
 
 
 def _create_table(
     df: pd.DataFrame,
-    cursor: "oracledb.Cursor",
+    cursor: "pyodbc.Cursor",
     table: str,
     schema: str,
     mode: str,
     index: bool,
     dtype: Optional[Dict[str, str]],
     varchar_lengths: Optional[Dict[str, int]],
 ) -> None:
     if mode == "overwrite":
         _drop_table(cursor=cursor, schema=schema, table=table)
     elif _does_table_exist(cursor=cursor, schema=schema, table=table):
         return
-    oracle_types: Dict[str, str] = _data_types.database_types_from_pandas(
+    sqlserver_types: Dict[str, str] = _data_types.database_types_from_pandas(
         df=df,
         index=index,
         dtype=dtype,
-        varchar_lengths_default="CLOB",
+        varchar_lengths_default="VARCHAR(MAX)",
         varchar_lengths=varchar_lengths,
-        converter_func=_data_types.pyarrow2oracle,
+        converter_func=_data_types.pyarrow2sqlserver,
     )
-    cols_str: str = "".join([f'"{k}" {v},\n' for k, v in oracle_types.items()])[:-2]
+    cols_str: str = "".join([f'"{k}" {v},\n' for k, v in sqlserver_types.items()])[:-2]
     table_identifier = _get_table_identifier(schema, table)
-    sql = f"CREATE TABLE {table_identifier} (\n{cols_str})"
+    sql = (
+        f"IF OBJECT_ID(N'{table_identifier}', N'U') IS NULL BEGIN CREATE TABLE {table_identifier} (\n{cols_str}); END;"
+    )
     _logger.debug("Create table query:\n%s", sql)
     cursor.execute(sql)
 
 
-@_check_for_oracledb
+@_utils.check_optional_dependency(pyodbc, "pyodbc")
 def connect(
     connection: Optional[str] = None,
     secret_id: Optional[str] = None,
     catalog_id: Optional[str] = None,
     dbname: Optional[str] = None,
+    odbc_driver_version: int = 17,
     boto3_session: Optional[boto3.Session] = None,
-    call_timeout: Optional[int] = 0,
-) -> "oracledb.Connection":
-    """Return a oracledb connection from a Glue Catalog Connection.
+    timeout: Optional[int] = 0,
+) -> "pyodbc.Connection":
+    """Return a pyodbc connection from a Glue Catalog Connection.
 
-    https://github.com/oracle/python-oracledb
+    https://github.com/mkleehammer/pyodbc
 
     Note
     ----
     You MUST pass a `connection` OR `secret_id`.
     Here is an example of the secret structure in Secrets Manager:
     {
-    "host":"oracle-instance-wrangler.cr4trrvge8rz.us-east-1.rds.amazonaws.com",
+    "host":"sqlserver-instance-wrangler.dr8vkeyrb9m1.us-east-1.rds.amazonaws.com",
     "username":"test",
     "password":"test",
-    "engine":"oracle",
-    "port":"1521",
+    "engine":"sqlserver",
+    "port":"1433",
     "dbname": "mydb" # Optional
     }
 
     Parameters
     ----------
     connection : Optional[str]
         Glue Catalog Connection name.
@@ -140,76 +114,120 @@
         Specifies the secret containing the connection details that you want to retrieve.
         You can specify either the Amazon Resource Name (ARN) or the friendly name of the secret.
     catalog_id : str, optional
         The ID of the Data Catalog.
         If none is provided, the AWS account ID is used by default.
     dbname: Optional[str]
         Optional database name to overwrite the stored one.
+    odbc_driver_version : int
+        Major version of the OBDC Driver version that is installed and should be used.
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    call_timeout: Optional[int]
-        This is the time in milliseconds that a single round-trip to the database may take before a timeout will occur.
+    timeout: Optional[int]
+        This is the time in seconds before the connection to the server will time out.
         The default is None which means no timeout.
-        This parameter is forwarded to oracledb.
-        https://cx-oracle.readthedocs.io/en/latest/api_manual/connection.html#Connection.call_timeout
+        This parameter is forwarded to pyodbc.
+        https://github.com/mkleehammer/pyodbc/wiki/The-pyodbc-Module#connect
 
     Returns
     -------
-    oracledb.Connection
-        oracledb connection.
+    pyodbc.Connection
+        pyodbc connection.
 
     Examples
     --------
     >>> import awswrangler as wr
-    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
+    >>> con = wr.sqlserver.connect(connection="MY_GLUE_CONNECTION", odbc_driver_version=17)
     >>> with con.cursor() as cursor:
-    >>>     cursor.execute("SELECT 1 FROM DUAL")
+    >>>     cursor.execute("SELECT 1")
     >>>     print(cursor.fetchall())
     >>> con.close()
 
     """
     attrs: _db_utils.ConnectionAttributes = _db_utils.get_connection_attributes(
         connection=connection, secret_id=secret_id, catalog_id=catalog_id, dbname=dbname, boto3_session=boto3_session
     )
-    if attrs.kind != "oracle":
+    if attrs.kind != "sqlserver":
         raise exceptions.InvalidDatabaseType(
-            f"Invalid connection type ({attrs.kind}. It must be an oracle connection.)"
+            f"Invalid connection type ({attrs.kind}. It must be a sqlserver connection.)"
         )
-
-    connection_dsn = oracledb.makedsn(attrs.host, attrs.port, service_name=attrs.database)
-    _logger.debug("DSN: %s", connection_dsn)
-    oracle_connection = oracledb.connect(
-        user=attrs.user,
-        password=attrs.password,
-        dsn=connection_dsn,
+    connection_str = (
+        f"DRIVER={{ODBC Driver {odbc_driver_version} for SQL Server}};"
+        f"SERVER={attrs.host},{attrs.port};"
+        f"DATABASE={attrs.database};"
+        f"UID={attrs.user};"
+        f"PWD={attrs.password}"
     )
-    # oracledb.connect does not have a call_timeout attribute, it has to be set separatly
-    oracle_connection.call_timeout = call_timeout
-    return oracle_connection
+
+    return pyodbc.connect(connection_str, timeout=timeout)
 
 
-@_check_for_oracledb
+@overload
 def read_sql_query(
     sql: str,
-    con: "oracledb.Connection",
+    con: "pyodbc.Connection",
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "pyodbc.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "pyodbc.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(pyodbc, "pyodbc")
+def read_sql_query(
+    sql: str,
+    con: "pyodbc.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding to the result set of the query string.
 
     Parameters
     ----------
     sql : str
         SQL query.
-    con : oracledb.Connection
-        Use oracledb.connect() to use credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog.
+    con : pyodbc.Connection
+        Use pyodbc.connect() to use credentials directly or wr.sqlserver.connect() to fetch it from the Glue Catalog.
     index_col : Union[str, List[str]], optional
         Column(s) to set as index(MultiIndex).
     params :  Union[List, Tuple, Dict], optional
         List of parameters to pass to execute method.
         The syntax used to pass parameters is database driver dependent.
         Check your database driver documentation for which of the five syntax styles,
         described in PEP 249’s paramstyle, is supported.
@@ -226,20 +244,20 @@
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
     --------
-    Reading from Oracle Database using a Glue Catalog Connections
+    Reading from Microsoft SQL Server using a Glue Catalog Connections
 
     >>> import awswrangler as wr
-    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
-    >>> df = wr.oracle.read_sql_query(
-    ...     sql="SELECT * FROM test.my_table",
+    >>> con = wr.sqlserver.connect(connection="MY_GLUE_CONNECTION", odbc_driver_version=17)
+    >>> df = wr.sqlserver.read_sql_query(
+    ...     sql="SELECT * FROM dbo.my_table",
     ...     con=con
     ... )
     >>> con.close()
     """
     _validate_connection(con=con)
     return _db_utils.read_sql_query(
         sql=sql,
@@ -249,34 +267,81 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
-@_check_for_oracledb
+@overload
+def read_sql_table(
+    table: str,
+    con: "pyodbc.Connection",
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    con: "pyodbc.Connection",
+    *,
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
 def read_sql_table(
     table: str,
-    con: "oracledb.Connection",
+    con: "pyodbc.Connection",
+    *,
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(pyodbc, "pyodbc")
+def read_sql_table(
+    table: str,
+    con: "pyodbc.Connection",
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Return a DataFrame corresponding the table.
 
     Parameters
     ----------
     table : str
         Table name.
-    con : oracledb.Connection
-        Use oracledb.connect() to use credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog.
+    con : pyodbc.Connection
+        Use pyodbc.connect() to use credentials directly or wr.sqlserver.connect() to fetch it from the Glue Catalog.
     schema : str, optional
         Name of SQL schema in database to query (if database flavor supports this).
         Uses default schema if None (default).
     index_col : Union[str, List[str]], optional
         Column(s) to set as index(MultiIndex).
     params :  Union[List, Tuple, Dict], optional
         List of parameters to pass to execute method.
@@ -296,21 +361,21 @@
     Returns
     -------
     Union[pandas.DataFrame, Iterator[pandas.DataFrame]]
         Result as Pandas DataFrame(s).
 
     Examples
     --------
-    Reading from Oracle Database using a Glue Catalog Connections
+    Reading from Microsoft SQL Server using a Glue Catalog Connections
 
     >>> import awswrangler as wr
-    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
-    >>> df = wr.oracle.read_sql_table(
+    >>> con = wr.sqlserver.connect(connection="MY_GLUE_CONNECTION", odbc_driver_version=17)
+    >>> df = wr.sqlserver.read_sql_table(
     ...     table="my_table",
-    ...     schema="test",
+    ...     schema="dbo",
     ...     con=con
     ... )
     >>> con.close()
     """
     table_identifier = _get_table_identifier(schema, table)
     sql: str = f"SELECT * FROM {table_identifier}"
     return read_sql_query(
@@ -321,140 +386,118 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
-@_check_for_oracledb
+@_utils.check_optional_dependency(pyodbc, "pyodbc")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
-    con: "oracledb.Connection",
+    con: "pyodbc.Connection",
     table: str,
     schema: str,
     mode: str = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
     chunksize: int = 200,
+    fast_executemany: bool = False,
 ) -> None:
-    """Write records stored in a DataFrame into Oracle Database.
+    """Write records stored in a DataFrame into Microsoft SQL Server.
 
     Parameters
     ----------
     df : pandas.DataFrame
         Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
-    con : oracledb.Connection
-        Use oracledb.connect() to use credentials directly or wr.oracle.connect() to fetch it from the Glue Catalog.
+    con : pyodbc.Connection
+        Use pyodbc.connect() to use credentials directly or wr.sqlserver.connect() to fetch it from the Glue Catalog.
     table : str
         Table name
     schema : str
         Schema name
     mode : str
         Append or overwrite.
     index : bool
         True to store the DataFrame index as a column in the table,
         otherwise False to ignore it.
     dtype: Dict[str, str], optional
-        Dictionary of columns names and Oracle types to be casted.
+        Dictionary of columns names and Microsoft SQL Server types to be casted.
         Useful when you have columns with undetermined or mixed data types.
         (e.g. {'col name': 'TEXT', 'col2 name': 'FLOAT'})
     varchar_lengths : Dict[str, int], optional
         Dict of VARCHAR length by columns. (e.g. {"col1": 10, "col5": 200}).
     use_column_names: bool
         If set to True, will use the column names of the DataFrame for generating the INSERT SQL Query.
         E.g. If the DataFrame has two columns `col1` and `col3` and `use_column_names` is True, data will only be
         inserted into the database columns `col1` and `col3`.
     chunksize: int
         Number of rows which are inserted with each SQL query. Defaults to inserting 200 rows per query.
+    fast_executemany: bool
+        Mode of execution which greatly reduces round trips for a DBAPI executemany() call when using
+        Microsoft ODBC drivers, for limited size batches that fit in memory. `False` by default.
+
+        https://github.com/mkleehammer/pyodbc/wiki/Cursor#executemanysql-params-with-fast_executemanytrue
+
+        Note: when using this mode, pyodbc converts the Python parameter values to their ODBC "C" equivalents,
+        based on the target column types in the database which may lead to subtle data type conversion
+        diffferences depending on whether fast_executemany is True or False.
 
     Returns
     -------
     None
         None.
 
     Examples
     --------
-    Writing to Oracle Database using a Glue Catalog Connections
+    Writing to Microsoft SQL Server using a Glue Catalog Connections
 
     >>> import awswrangler as wr
-    >>> con = wr.oracle.connect(connection="MY_GLUE_CONNECTION")
-    >>> wr.oracle.to_sql(
+    >>> con = wr.sqlserver.connect(connection="MY_GLUE_CONNECTION", odbc_driver_version=17)
+    >>> wr.sqlserver.to_sql(
     ...     df=df,
     ...     table="table",
-    ...     schema="ORCL",
+    ...     schema="dbo",
     ...     con=con
     ... )
     >>> con.close()
 
     """
     if df.empty is True:
         raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
     _validate_connection(con=con)
     try:
         with con.cursor() as cursor:
+            if fast_executemany:
+                cursor.fast_executemany = True
             _create_table(
                 df=df,
                 cursor=cursor,
                 table=table,
                 schema=schema,
                 mode=mode,
                 index=index,
                 dtype=dtype,
                 varchar_lengths=varchar_lengths,
             )
             if index:
                 df.reset_index(level=df.index.names, inplace=True)
-            column_placeholders: str = f"({', '.join([':' + str(i + 1) for i in range(len(df.columns))])})"
+            column_placeholders: str = ", ".join(["?"] * len(df.columns))
             table_identifier = _get_table_identifier(schema, table)
             insertion_columns = ""
             if use_column_names:
-                insertion_columns = "(" + ", ".join('"' + column + '"' for column in df.columns) + ")"
-
+                quoted_columns = ", ".join(f'"{col}"' for col in df.columns)
+                insertion_columns = f"({quoted_columns})"
             placeholder_parameter_pair_generator = _db_utils.generate_placeholder_parameter_pairs(
                 df=df, column_placeholders=column_placeholders, chunksize=chunksize
             )
-            for _, parameters in placeholder_parameter_pair_generator:
-                parameters = list(zip(*[iter(parameters)] * len(df.columns)))
-                sql: str = f"INSERT INTO {table_identifier} {insertion_columns} VALUES {column_placeholders}"
+            for placeholders, parameters in placeholder_parameter_pair_generator:
+                sql: str = f"INSERT INTO {table_identifier} {insertion_columns} VALUES {placeholders}"
                 _logger.debug("sql: %s", sql)
-                cursor.executemany(sql, parameters)
+                cursor.executemany(sql, (parameters,))
             con.commit()
     except Exception as ex:
         con.rollback()
         _logger.error(ex)
         raise
-
-
-def detect_oracle_decimal_datatype(cursor: Any) -> Dict[str, pa.DataType]:
-    """Determine if a given Oracle column is a decimal, not just a standard float value."""
-    dtype = {}
-    _logger.debug("cursor type: %s", type(cursor))
-    if isinstance(cursor, oracledb.Cursor):
-        # Oracle stores DECIMAL as the NUMBER type
-        for row in cursor.description:
-            if row[1] == oracledb.DB_TYPE_NUMBER and row[5] > 0:  # pylint: disable=no-member
-                dtype[row[0]] = pa.decimal128(row[4], row[5])
-
-    _logger.debug("decimal dtypes: %s", dtype)
-    return dtype
-
-
-def handle_oracle_objects(
-    col_values: List[Any], col_name: str, dtype: Optional[Dict[str, pa.DataType]] = None
-) -> List[Any]:
-    """Get the string representation of an Oracle LOB value, and convert float to decimal."""
-    if any(isinstance(col_value, oracledb.LOB) for col_value in col_values):
-        col_values = [
-            col_value.read() if isinstance(col_value, oracledb.LOB) else col_value for col_value in col_values
-        ]
-
-    if dtype is not None:
-        if isinstance(dtype[col_name], pa.Decimal128Type):
-            _logger.debug("decimal_col_values:\n%s", col_values)
-            col_values = [
-                Decimal(repr(col_value)) if isinstance(col_value, float) else col_value for col_value in col_values
-            ]
-
-    return col_values
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/postgresql.py` & `awswrangler-3.0.0rc3/awswrangler/postgresql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,57 @@
+# mypy: disable-error-code=name-defined
 """Amazon PostgreSQL Module."""
 
 import logging
 from ssl import SSLContext
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Union, overload
 
 import boto3
 import pandas as pd
-import pg8000
 import pyarrow as pa
 
-from awswrangler import _data_types
+from awswrangler import _data_types, _utils, exceptions
 from awswrangler import _databases as _db_utils
-from awswrangler import exceptions
 from awswrangler._config import apply_configs
 
+pg8000 = _utils.import_optional_dependency("pg8000")
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _validate_connection(con: pg8000.Connection) -> None:
+def _validate_connection(con: "pg8000.Connection") -> None:
     if not isinstance(con, pg8000.Connection):
         raise exceptions.InvalidConnection(
             "Invalid 'conn' argument, please pass a "
             "pg8000.Connection object. Use pg8000.connect() to use "
             "credentials directly or wr.postgresql.connect() to fetch it from the Glue Catalog."
         )
 
 
-def _drop_table(cursor: pg8000.Cursor, schema: Optional[str], table: str) -> None:
+def _drop_table(cursor: "pg8000.Cursor", schema: Optional[str], table: str) -> None:
     schema_str = f'"{schema}".' if schema else ""
     sql = f'DROP TABLE IF EXISTS {schema_str}"{table}"'
     _logger.debug("Drop table query:\n%s", sql)
     cursor.execute(sql)
 
 
-def _does_table_exist(cursor: pg8000.Cursor, schema: Optional[str], table: str) -> bool:
+def _does_table_exist(cursor: "pg8000.Cursor", schema: Optional[str], table: str) -> bool:
     schema_str = f"TABLE_SCHEMA = '{schema}' AND" if schema else ""
     cursor.execute(
         f"SELECT true WHERE EXISTS ("
         f"SELECT * FROM INFORMATION_SCHEMA.TABLES WHERE "
         f"{schema_str} TABLE_NAME = '{table}'"
         f");"
     )
     return len(cursor.fetchall()) > 0
 
 
 def _create_table(
     df: pd.DataFrame,
-    cursor: pg8000.Cursor,
+    cursor: "pg8000.Cursor",
     table: str,
     schema: str,
     mode: str,
     index: bool,
     dtype: Optional[Dict[str, str]],
     varchar_lengths: Optional[Dict[str, int]],
 ) -> None:
@@ -68,24 +69,25 @@
     )
     cols_str: str = "".join([f'"{k}" {v},\n' for k, v in postgresql_types.items()])[:-2]
     sql = f'CREATE TABLE IF NOT EXISTS "{schema}"."{table}" (\n{cols_str})'
     _logger.debug("Create table query:\n%s", sql)
     cursor.execute(sql)
 
 
+@_utils.check_optional_dependency(pg8000, "pg8000")
 def connect(
     connection: Optional[str] = None,
     secret_id: Optional[str] = None,
     catalog_id: Optional[str] = None,
     dbname: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     ssl_context: Optional[Union[bool, SSLContext]] = None,
     timeout: Optional[int] = None,
     tcp_keepalive: bool = True,
-) -> pg8000.Connection:
+) -> "pg8000.Connection":
     """Return a pg8000 connection from a Glue Catalog Connection.
 
     https://github.com/tlocke/pg8000
 
     Note
     ----
     You MUST pass a `connection` OR `secret_id`.
@@ -157,17 +159,62 @@
         host=attrs.host,
         ssl_context=ssl_context,
         timeout=timeout,
         tcp_keepalive=tcp_keepalive,
     )
 
 
+@overload
+def read_sql_query(
+    sql: str,
+    con: "pg8000.Connection",
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "pg8000.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "pg8000.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(pg8000, "pg8000")
 def read_sql_query(
     sql: str,
-    con: pg8000.Connection,
+    con: "pg8000.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
@@ -223,17 +270,65 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+@overload
+def read_sql_table(
+    table: str,
+    con: "pg8000.Connection",
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    con: "pg8000.Connection",
+    *,
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    con: "pg8000.Connection",
+    *,
+    schema: Optional[str] = ...,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(pg8000, "pg8000")
 def read_sql_table(
     table: str,
-    con: pg8000.Connection,
+    con: "pg8000.Connection",
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
@@ -294,18 +389,19 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+@_utils.check_optional_dependency(pg8000, "pg8000")
 @apply_configs
 def to_sql(
     df: pd.DataFrame,
-    con: pg8000.Connection,
+    con: "pg8000.Connection",
     table: str,
     schema: str,
     mode: str = "append",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     varchar_lengths: Optional[Dict[str, int]] = None,
     use_column_names: bool = False,
@@ -400,18 +496,18 @@
             column_names = [f'"{column}"' for column in df.columns]
             insertion_columns = ""
             upsert_str = ""
             if use_column_names:
                 insertion_columns = f"({', '.join(column_names)})"
             if mode == "upsert":
                 upsert_columns = ", ".join(f"{column}=EXCLUDED.{column}" for column in column_names)
-                conflict_columns = ", ".join(upsert_conflict_columns)  # type: ignore
+                conflict_columns = ", ".join(upsert_conflict_columns)  # type: ignore[arg-type]
                 upsert_str = f" ON CONFLICT ({conflict_columns}) DO UPDATE SET {upsert_columns}"
             if mode == "append" and insert_conflict_columns:
-                conflict_columns = ", ".join(insert_conflict_columns)  # type: ignore
+                conflict_columns = ", ".join(insert_conflict_columns)
                 upsert_str = f" ON CONFLICT ({conflict_columns}) DO NOTHING"
             placeholder_parameter_pair_generator = _db_utils.generate_placeholder_parameter_pairs(
                 df=df, column_placeholders=column_placeholders, chunksize=chunksize
             )
             for placeholders, parameters in placeholder_parameter_pair_generator:
                 sql: str = f'INSERT INTO "{schema}"."{table}" {insertion_columns} VALUES {placeholders}{upsert_str}'
                 _logger.debug("sql: %s", sql)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/quicksight/__init__.py` & `awswrangler-3.0.0rc3/awswrangler/quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `awswrangler-3.0.0rc2/awswrangler/quicksight/_cancel.py` & `awswrangler-3.0.0rc3/awswrangler/quicksight/_cancel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Amazon QuickSight Cancel Module."""
 
 import logging
-from typing import Optional
+from typing import Optional, cast
 
 import boto3
 
 from awswrangler import _utils, exceptions, sts
 from awswrangler.quicksight._get_list import get_dataset_id
 
 _logger: logging.Logger = logging.getLogger(__name__)
@@ -45,14 +45,14 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>>  wr.quicksight.cancel_ingestion(ingestion_id="...", dataset_name="...")
     """
     if (dataset_name is None) and (dataset_id is None):
         raise exceptions.InvalidArgument("You must pass a not None name or dataset_id argument.")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
     if (dataset_id is None) and (dataset_name is not None):
-        dataset_id = get_dataset_id(name=dataset_name, account_id=account_id, boto3_session=session)
-    client: boto3.client = _utils.client(service_name="quicksight", session=session)
+        dataset_id = get_dataset_id(name=dataset_name, account_id=account_id, boto3_session=boto3_session)
+    client = _utils.client(service_name="quicksight", session=boto3_session)
+    dataset_id = cast(str, dataset_id)
     client.cancel_ingestion(IngestionId=ingestion_id, AwsAccountId=account_id, DataSetId=dataset_id)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/quicksight/_create.py` & `awswrangler-3.0.0rc3/awswrangler/quicksight/_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     return [cast(str, u["Arn"]) for u in all_users if u.get("UserName") in user_names]
 
 
 def _generate_permissions(
     resource: str,
     namespace: str,
     account_id: str,
-    boto3_session: boto3.Session,
+    boto3_session: Optional[boto3.Session],
     allowed_to_use: Optional[List[str]] = None,
     allowed_to_manage: Optional[List[str]] = None,
 ) -> List[Dict[str, Union[str, List[str]]]]:
     permissions: List[Dict[str, Union[str, List[str]]]] = []
     if (allowed_to_use is None) and (allowed_to_manage is None):
         return permissions
 
@@ -163,30 +163,29 @@
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.create_athena_data_source(
     ...     name="...",
     ...     allowed_to_manage=["john"]
     ... )
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client: boto3.client = _utils.client(service_name="quicksight", session=session)
+    client = _utils.client(service_name="quicksight", session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
     args: Dict[str, Any] = {
         "AwsAccountId": account_id,
         "DataSourceId": name,
         "Name": name,
         "Type": "ATHENA",
         "DataSourceParameters": {"AthenaParameters": {"WorkGroup": workgroup}},
         "SslProperties": {"DisableSsl": True},
     }
     permissions: List[Dict[str, Union[str, List[str]]]] = _generate_permissions(
         resource="data_source",
         account_id=account_id,
-        boto3_session=session,
+        boto3_session=boto3_session,
         allowed_to_use=allowed_to_use,
         allowed_to_manage=allowed_to_manage,
         namespace=namespace,
     )
     if permissions:
         args["Permissions"] = permissions
     if tags is not None:
@@ -196,15 +195,15 @@
 
 
 def create_athena_dataset(
     name: str,
     database: Optional[str] = None,
     table: Optional[str] = None,
     sql: Optional[str] = None,
-    sql_name: str = "CustomSQL",
+    sql_name: Optional[str] = None,
     data_source_name: Optional[str] = None,
     data_source_arn: Optional[str] = None,
     import_mode: str = "DIRECT_QUERY",
     allowed_to_use: Optional[List[str]] = None,
     allowed_to_manage: Optional[List[str]] = None,
     logical_table_alias: str = "LogicalTable",
     rename_columns: Optional[Dict[str, str]] = None,
@@ -236,15 +235,15 @@
         Dataset name.
     database : str
         Athena's database name.
     table : str
         Athena's table name.
     sql : str
         Use a SQL query to define your table.
-    sql_name : str
+    sql_name : str, optional
         Query name.
     data_source_name : str, optional
         QuickSight data source name.
     data_source_arn : str, optional
         QuickSight data source ARN.
     import_mode : str
         Indicates whether you want to import the data into SPICE.
@@ -298,44 +297,43 @@
     if ((database is None) and (table is None)) and (sql is None):
         raise exceptions.InvalidArgument("You must pass database/table OR sql argument.")
     if (database is not None) and (sql is not None):
         raise exceptions.InvalidArgument(
             "If you provide sql argument, please include the database name inside the sql statement."
             "Do NOT pass in with database argument."
         )
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client: boto3.client = _utils.client(service_name="quicksight", session=session)
+    client = _utils.client(service_name="quicksight", session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
     if (data_source_arn is None) and (data_source_name is not None):
-        data_source_arn = get_data_source_arn(name=data_source_name, account_id=account_id, boto3_session=session)
+        data_source_arn = get_data_source_arn(name=data_source_name, account_id=account_id, boto3_session=boto3_session)
     if sql is not None:
         physical_table: Dict[str, Dict[str, Any]] = {
             "CustomSql": {
                 "DataSourceArn": data_source_arn,
-                "Name": sql_name,
+                "Name": sql_name if sql_name else f"CustomSQL-{uuid.uuid4().hex[:8]}",
                 "SqlQuery": sql,
                 "Columns": extract_athena_query_columns(
                     sql=sql,
-                    data_source_arn=data_source_arn,  # type: ignore
+                    data_source_arn=data_source_arn,  # type: ignore[arg-type]
                     account_id=account_id,
-                    boto3_session=session,
+                    boto3_session=boto3_session,
                 ),
             }
         }
     else:
         physical_table = {
             "RelationalTable": {
                 "DataSourceArn": data_source_arn,
                 "Schema": database,
                 "Name": table,
                 "InputColumns": extract_athena_table_columns(
-                    database=database,  # type: ignore
-                    table=table,  # type: ignore
-                    boto3_session=session,
+                    database=database,  # type: ignore[arg-type]
+                    table=table,  # type: ignore[arg-type]
+                    boto3_session=boto3_session,
                 ),
             }
         }
     table_uuid: str = uuid.uuid4().hex
     dataset_id: str = uuid.uuid4().hex
     args: Dict[str, Any] = {
         "AwsAccountId": account_id,
@@ -349,15 +347,15 @@
         rename_columns=rename_columns, cast_columns_types=cast_columns_types, tag_columns=tag_columns
     )
     if trans:
         args["LogicalTableMap"][table_uuid]["DataTransforms"] = trans
     permissions: List[Dict[str, Union[str, List[str]]]] = _generate_permissions(
         resource="dataset",
         account_id=account_id,
-        boto3_session=session,
+        boto3_session=boto3_session,
         allowed_to_use=allowed_to_use,
         allowed_to_manage=allowed_to_manage,
         namespace=namespace,
     )
     if permissions:
         args["Permissions"] = permissions
     if tags is not None:
@@ -399,21 +397,21 @@
         Ingestion ID
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> status = wr.quicksight.create_ingestion("my_dataset")
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
     if (dataset_name is None) and (dataset_id is None):
         raise exceptions.InvalidArgument("You must pass a not None dataset_name or dataset_id argument.")
     if (dataset_id is None) and (dataset_name is not None):
-        dataset_id = get_dataset_id(name=dataset_name, account_id=account_id, boto3_session=session)
+        dataset_id = get_dataset_id(name=dataset_name, account_id=account_id, boto3_session=boto3_session)
     if ingestion_id is None:
         ingestion_id = uuid.uuid4().hex
-    client: boto3.client = _utils.client(service_name="quicksight", session=session)
-    response: Dict[str, Any] = client.create_ingestion(
-        DataSetId=dataset_id, IngestionId=ingestion_id, AwsAccountId=account_id
-    )
-    return cast(str, response["IngestionId"])
+
+    client = _utils.client(service_name="quicksight", session=boto3_session)
+    dataset_id = cast(str, dataset_id)
+
+    response = client.create_ingestion(DataSetId=dataset_id, IngestionId=ingestion_id, AwsAccountId=account_id)
+    return response["IngestionId"]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/quicksight/_delete.py` & `awswrangler-3.0.0rc3/awswrangler/quicksight/_delete.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Amazon QuickSight Delete Module."""
 
 import logging
+import re
 from typing import Any, Callable, Dict, Optional
 
 import boto3
 
 from awswrangler import _utils, exceptions, sts
 from awswrangler.quicksight._get_list import (
     get_dashboard_id,
@@ -19,18 +20,17 @@
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _delete(
     func_name: str, account_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None, **kwargs: Any
 ) -> None:
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
-    client: boto3.client = _utils.client(service_name="quicksight", session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    client = _utils.client(service_name="quicksight", session=boto3_session)
     func: Callable[..., None] = getattr(client, func_name)
     func(AwsAccountId=account_id, **kwargs)
 
 
 def delete_dashboard(
     name: Optional[str] = None,
     dashboard_id: Optional[str] = None,
@@ -66,21 +66,20 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_dashboard(name="...")
     """
     if (name is None) and (dashboard_id is None):
         raise exceptions.InvalidArgument("You must pass a not None name or dashboard_id argument.")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if (dashboard_id is None) and (name is not None):
-        dashboard_id = get_dashboard_id(name=name, account_id=account_id, boto3_session=session)
+        dashboard_id = get_dashboard_id(name=name, account_id=account_id, boto3_session=boto3_session)
     args: Dict[str, Any] = {
         "func_name": "delete_dashboard",
         "account_id": account_id,
-        "boto3_session": session,
+        "boto3_session": boto3_session,
         "DashboardId": dashboard_id,
     }
     if version_number is not None:
         args["VersionNumber"] = version_number
     _delete(**args)
 
 
@@ -115,21 +114,20 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_dataset(name="...")
     """
     if (name is None) and (dataset_id is None):
         raise exceptions.InvalidArgument("You must pass a not None name or dataset_id argument.")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if (dataset_id is None) and (name is not None):
-        dataset_id = get_dataset_id(name=name, account_id=account_id, boto3_session=session)
+        dataset_id = get_dataset_id(name=name, account_id=account_id, boto3_session=boto3_session)
     args: Dict[str, Any] = {
         "func_name": "delete_data_set",
         "account_id": account_id,
-        "boto3_session": session,
+        "boto3_session": boto3_session,
         "DataSetId": dataset_id,
     }
     _delete(**args)
 
 
 def delete_data_source(
     name: Optional[str] = None,
@@ -162,21 +160,20 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_data_source(name="...")
     """
     if (name is None) and (data_source_id is None):
         raise exceptions.InvalidArgument("You must pass a not None name or data_source_id argument.")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if (data_source_id is None) and (name is not None):
-        data_source_id = get_data_source_id(name=name, account_id=account_id, boto3_session=session)
+        data_source_id = get_data_source_id(name=name, account_id=account_id, boto3_session=boto3_session)
     args: Dict[str, Any] = {
         "func_name": "delete_data_source",
         "account_id": account_id,
-        "boto3_session": session,
+        "boto3_session": boto3_session,
         "DataSourceId": data_source_id,
     }
     _delete(**args)
 
 
 def delete_template(
     name: Optional[str] = None,
@@ -213,127 +210,152 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_template(name="...")
     """
     if (name is None) and (template_id is None):
         raise exceptions.InvalidArgument("You must pass a not None name or template_id argument.")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if (template_id is None) and (name is not None):
-        template_id = get_template_id(name=name, account_id=account_id, boto3_session=session)
+        template_id = get_template_id(name=name, account_id=account_id, boto3_session=boto3_session)
     args: Dict[str, Any] = {
         "func_name": "delete_template",
         "account_id": account_id,
-        "boto3_session": session,
+        "boto3_session": boto3_session,
         "TemplateId": template_id,
     }
     if version_number is not None:
         args["VersionNumber"] = version_number
     _delete(**args)
 
 
-def delete_all_dashboards(account_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None) -> None:
+def delete_all_dashboards(
+    account_id: Optional[str] = None, regex_filter: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
+) -> None:
     """Delete all dashboards.
 
     Parameters
     ----------
     account_id : str, optional
         If None, the account ID will be inferred from your boto3 session.
+    regex_filter : str, optional
+        Regex regex_filter that will delete all dashboards with a match in their ``Name``
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_all_dashboards()
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
-    for dashboard in list_dashboards(account_id=account_id, boto3_session=session):
-        delete_dashboard(dashboard_id=dashboard["DashboardId"], account_id=account_id, boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    for dashboard in list_dashboards(account_id=account_id, boto3_session=boto3_session):
+        if regex_filter:
+            if not re.search(f"^{regex_filter}$", dashboard["Name"]):
+                continue
+        delete_dashboard(dashboard_id=dashboard["DashboardId"], account_id=account_id, boto3_session=boto3_session)
 
 
-def delete_all_datasets(account_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None) -> None:
+def delete_all_datasets(
+    account_id: Optional[str] = None, regex_filter: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
+) -> None:
     """Delete all datasets.
 
     Parameters
     ----------
     account_id : str, optional
         If None, the account ID will be inferred from your boto3 session.
+    regex_filter : str, optional
+        Regex regex_filter that will delete all datasets with a match in their ``Name``
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_all_datasets()
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
-    for dataset in list_datasets(account_id=account_id, boto3_session=session):
-        delete_dataset(dataset_id=dataset["DataSetId"], account_id=account_id, boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    for dataset in list_datasets(account_id=account_id, boto3_session=boto3_session):
+        if regex_filter:
+            if not re.search(f"^{regex_filter}$", dataset["Name"]):
+                continue
+        delete_dataset(dataset_id=dataset["DataSetId"], account_id=account_id, boto3_session=boto3_session)
 
 
-def delete_all_data_sources(account_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None) -> None:
+def delete_all_data_sources(
+    account_id: Optional[str] = None, regex_filter: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
+) -> None:
     """Delete all data sources.
 
     Parameters
     ----------
     account_id : str, optional
         If None, the account ID will be inferred from your boto3 session.
+    regex_filter : str, optional
+        Regex regex_filter that will delete all data sources with a match in their ``Name``
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_all_data_sources()
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
-    for data_source in list_data_sources(account_id=account_id, boto3_session=session):
-        delete_data_source(data_source_id=data_source["DataSourceId"], account_id=account_id, boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    for data_source in list_data_sources(account_id=account_id, boto3_session=boto3_session):
+        if regex_filter:
+            if not re.search(f"^{regex_filter}$", data_source["Name"]):
+                continue
+        delete_data_source(
+            data_source_id=data_source["DataSourceId"], account_id=account_id, boto3_session=boto3_session
+        )
 
 
-def delete_all_templates(account_id: Optional[str] = None, boto3_session: Optional[boto3.Session] = None) -> None:
+def delete_all_templates(
+    account_id: Optional[str] = None, regex_filter: Optional[str] = None, boto3_session: Optional[boto3.Session] = None
+) -> None:
     """Delete all templates.
 
     Parameters
     ----------
     account_id : str, optional
         If None, the account ID will be inferred from your boto3 session.
+    regex_filter : str, optional
+        Regex regex_filter that will delete all templates with a match in their ``Name``
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
 
     Returns
     -------
     None
         None.
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.quicksight.delete_all_templates()
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
-    for template in list_templates(account_id=account_id, boto3_session=session):
-        delete_template(template_id=template["TemplateId"], account_id=account_id, boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    for template in list_templates(account_id=account_id, boto3_session=boto3_session):
+        if regex_filter:
+            if not re.search(f"^{regex_filter}$", template["Name"]):
+                continue
+        delete_template(template_id=template["TemplateId"], account_id=account_id, boto3_session=boto3_session)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/quicksight/_get_list.py` & `awswrangler-3.0.0rc3/awswrangler/quicksight/_get_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 def _list(
     func_name: str,
     attr_name: str,
     account_id: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     **kwargs: Any,
 ) -> List[Dict[str, Any]]:
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
-    client: boto3.client = _utils.client(service_name="quicksight", session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
+    client = _utils.client(service_name="quicksight", session=boto3_session)
     func: Callable[..., Dict[str, Any]] = getattr(client, func_name)
     response: Dict[str, Any] = func(AwsAccountId=account_id, **kwargs)
     next_token: str = response.get("NextToken", None)
     result: List[Dict[str, Any]] = response[attr_name]
     while next_token is not None:
         response = func(AwsAccountId=account_id, NextToken=next_token, **kwargs)
         next_token = response.get("NextToken", None)
@@ -402,19 +401,18 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> ingestions = wr.quicksight.list_ingestions()
     """
     if (dataset_name is None) and (dataset_id is None):
         raise exceptions.InvalidArgument("You must pass a not None name or dataset_id argument.")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     if account_id is None:
-        account_id = sts.get_account_id(boto3_session=session)
+        account_id = sts.get_account_id(boto3_session=boto3_session)
     if (dataset_id is None) and (dataset_name is not None):
-        dataset_id = get_dataset_id(name=dataset_name, account_id=account_id, boto3_session=session)
+        dataset_id = get_dataset_id(name=dataset_name, account_id=account_id, boto3_session=boto3_session)
     return _list(
         func_name="list_ingestions",
         attr_name="Ingestions",
         account_id=account_id,
         boto3_session=boto3_session,
         DataSetId=dataset_id,
     )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/quicksight/_utils.py` & `awswrangler-3.0.0rc3/awswrangler/quicksight/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,31 @@
 
 from awswrangler import _data_types, athena, catalog, exceptions
 from awswrangler.quicksight._get_list import list_data_sources
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def extract_athena_table_columns(database: str, table: str, boto3_session: boto3.Session) -> List[Dict[str, str]]:
+def extract_athena_table_columns(
+    database: str, table: str, boto3_session: Optional[boto3.Session]
+) -> List[Dict[str, str]]:
     """Extract athena columns data types from table and raising an exception if not exist."""
     dtypes: Optional[Dict[str, str]] = catalog.get_table_types(
         database=database, table=table, boto3_session=boto3_session
     )
     if dtypes is None:
         raise exceptions.InvalidArgument(f"{database}.{table} does not exist on Athena.")
     return [{"Name": name, "Type": _data_types.athena2quicksight(dtype=dtype)} for name, dtype in dtypes.items()]
 
 
 def extract_athena_query_columns(
-    sql: str, data_source_arn: str, account_id: str, boto3_session: boto3.Session
+    sql: str, data_source_arn: str, account_id: str, boto3_session: Optional[boto3.Session]
 ) -> List[Dict[str, str]]:
     """Extract athena columns data types from a SQL query."""
     data_sources: List[Dict[str, Any]] = list_data_sources(account_id=account_id, boto3_session=boto3_session)
     data_source: Dict[str, Any] = [x for x in data_sources if x["Arn"] == data_source_arn][0]
     workgroup: str = data_source["DataSourceParameters"]["AthenaParameters"]["WorkGroup"]
     sql_wrapped: str = f"/* QuickSight */\nSELECT ds.* FROM ( {sql} ) ds LIMIT 0"
-    query_id: str = athena.start_query_execution(sql=sql_wrapped, workgroup=workgroup, boto3_session=boto3_session)
+    query_id = athena.start_query_execution(sql=sql_wrapped, workgroup=workgroup, boto3_session=boto3_session)
     athena.wait_query(query_execution_id=query_id, boto3_session=boto3_session)
     dtypes: Dict[str, str] = athena.get_query_columns_types(query_execution_id=query_id, boto3_session=boto3_session)
     return [{"Name": name, "Type": _data_types.athena2quicksight(dtype=dtype)} for name, dtype in dtypes.items()]
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/redshift.py` & `awswrangler-3.0.0rc3/awswrangler/redshift.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,94 @@
-"""Amazon Redshift Module."""
+# mypy: disable-error-code=name-defined
 # pylint: disable=too-many-lines
+"""Amazon Redshift Module."""
 
 import json
 import logging
 import uuid
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Union, overload
 
 import boto3
 import botocore
 import pandas as pd
 import pyarrow as pa
-import redshift_connector
 
-from awswrangler import _data_types
+from awswrangler import _data_types, _utils, exceptions, s3
 from awswrangler import _databases as _db_utils
-from awswrangler import _utils, exceptions, s3
 from awswrangler._config import apply_configs
+from awswrangler._distributed import EngineEnum, engine
+
+redshift_connector = _utils.import_optional_dependency("redshift_connector")
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 _RS_DISTSTYLES: List[str] = ["AUTO", "EVEN", "ALL", "KEY"]
 _RS_SORTSTYLES: List[str] = ["COMPOUND", "INTERLEAVED"]
 
 
-def _validate_connection(con: redshift_connector.Connection) -> None:
+def _validate_connection(con: "redshift_connector.Connection") -> None:
     if not isinstance(con, redshift_connector.Connection):
         raise exceptions.InvalidConnection(
             "Invalid 'conn' argument, please pass a "
             "redshift_connector.Connection object. Use redshift_connector.connect() to use "
             "credentials directly or wr.redshift.connect() to fetch it from the Glue Catalog."
         )
 
 
-def _begin_transaction(cursor: redshift_connector.Cursor) -> None:
+def _begin_transaction(cursor: "redshift_connector.Cursor") -> None:
     sql = "BEGIN TRANSACTION"
     _logger.debug("Begin transaction query:\n%s", sql)
     cursor.execute(sql)
 
 
-def _drop_table(cursor: redshift_connector.Cursor, schema: Optional[str], table: str, cascade: bool = False) -> None:
+def _drop_table(cursor: "redshift_connector.Cursor", schema: Optional[str], table: str, cascade: bool = False) -> None:
     schema_str = f'"{schema}".' if schema else ""
     cascade_str = " CASCADE" if cascade else ""
     sql = f'DROP TABLE IF EXISTS {schema_str}"{table}"' f"{cascade_str}"
     _logger.debug("Drop table query:\n%s", sql)
     cursor.execute(sql)
 
 
-def _truncate_table(cursor: redshift_connector.Cursor, schema: Optional[str], table: str) -> None:
+def _truncate_table(cursor: "redshift_connector.Cursor", schema: Optional[str], table: str) -> None:
     schema_str = f'"{schema}".' if schema else ""
     sql = f'TRUNCATE TABLE {schema_str}"{table}"'
     _logger.debug("Truncate table query:\n%s", sql)
     cursor.execute(sql)
 
 
-def _delete_all(cursor: redshift_connector.Cursor, schema: Optional[str], table: str) -> None:
+def _delete_all(cursor: "redshift_connector.Cursor", schema: Optional[str], table: str) -> None:
     schema_str = f'"{schema}".' if schema else ""
     sql = f'DELETE FROM {schema_str}"{table}"'
     _logger.debug("Delete query:\n%s", sql)
     cursor.execute(sql)
 
 
-def _get_primary_keys(cursor: redshift_connector.Cursor, schema: str, table: str) -> List[str]:
+def _get_primary_keys(cursor: "redshift_connector.Cursor", schema: str, table: str) -> List[str]:
     cursor.execute(f"SELECT indexdef FROM pg_indexes WHERE schemaname = '{schema}' AND tablename = '{table}'")
     result: str = cursor.fetchall()[0][0]
     rfields: List[str] = result.split("(")[1].strip(")").split(",")
     fields: List[str] = [field.strip().strip('"') for field in rfields]
     return fields
 
 
-def _does_table_exist(cursor: redshift_connector.Cursor, schema: Optional[str], table: str) -> bool:
+def _does_table_exist(cursor: "redshift_connector.Cursor", schema: Optional[str], table: str) -> bool:
     schema_str = f"TABLE_SCHEMA = '{schema}' AND" if schema else ""
     cursor.execute(
         f"SELECT true WHERE EXISTS ("
         f"SELECT * FROM INFORMATION_SCHEMA.TABLES WHERE "
         f"{schema_str} TABLE_NAME = '{table}'"
         f");"
     )
     return len(cursor.fetchall()) > 0
 
 
 def _get_paths_from_manifest(path: str, boto3_session: Optional[boto3.Session] = None) -> List[str]:
-    resource_s3: boto3.resource = _utils.resource(service_name="s3", session=boto3_session)
+    client_s3 = _utils.client(service_name="s3", session=boto3_session)
     bucket, key = _utils.parse_path(path)
-    content_object = resource_s3.Object(bucket, key)
-    manifest_content = json.loads(content_object.get()["Body"].read().decode("utf-8"))
+    manifest_content = json.loads(client_s3.get_object(Bucket=bucket, Key=key)["Body"].read().decode("utf-8"))
     return [path["url"] for path in manifest_content["entries"]]
 
 
 def _make_s3_auth_string(
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     aws_session_token: Optional[str] = None,
@@ -115,23 +116,23 @@
         if credentials.token is not None:
             auth_str += f"SESSION_TOKEN '{credentials.token}'\n"
 
     return auth_str
 
 
 def _copy(
-    cursor: redshift_connector.Cursor,
+    cursor: "redshift_connector.Cursor",
     path: str,
     table: str,
     serialize_to_json: bool,
     iam_role: Optional[str] = None,
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     aws_session_token: Optional[str] = None,
-    boto3_session: Optional[str] = None,
+    boto3_session: Optional[boto3.Session] = None,
     schema: Optional[str] = None,
     manifest: Optional[bool] = False,
     sql_copy_extra_params: Optional[List[str]] = None,
     column_names: Optional[List[str]] = None,
 ) -> None:
     if schema is None:
         table_name: str = f'"{table}"'
@@ -155,74 +156,77 @@
         for param in sql_copy_extra_params:
             sql += f"\n{param}"
     _logger.debug("copy query:\n%s", sql)
     cursor.execute(sql)
 
 
 def _lock(
-    cursor: redshift_connector.Cursor,
+    cursor: "redshift_connector.Cursor",
     table_names: List[str],
     schema: Optional[str] = None,
 ) -> None:
     fmt = '"{schema}"."{table}"' if schema else '"{table}"'
     tables = ", ".join([fmt.format(schema=schema, table=table) for table in table_names])
     sql: str = f"LOCK {tables};\n"
     _logger.debug("lock query:\n%s", sql)
     cursor.execute(sql)
 
 
 def _upsert(
-    cursor: redshift_connector.Cursor,
+    cursor: "redshift_connector.Cursor",
     table: str,
     temp_table: str,
     schema: str,
     primary_keys: Optional[List[str]] = None,
     precombine_key: Optional[str] = None,
     column_names: Optional[List[str]] = None,
 ) -> None:
     if not primary_keys:
         primary_keys = _get_primary_keys(cursor=cursor, schema=schema, table=table)
     _logger.debug("primary_keys: %s", primary_keys)
     if not primary_keys:
         raise exceptions.InvalidRedshiftPrimaryKeys()
-    equals_clause: str = f"{table}.%s = {temp_table}.%s"
+    equals_clause: str = f'"{table}".%s = "{temp_table}".%s'
     join_clause: str = " AND ".join([equals_clause % (pk, pk) for pk in primary_keys])
     if precombine_key:
         delete_from_target_filter: str = f"AND {table}.{precombine_key} <= {temp_table}.{precombine_key}"
         delete_from_temp_filter: str = f"AND {table}.{precombine_key} > {temp_table}.{precombine_key}"
         target_del_sql: str = (
-            f'DELETE FROM "{schema}"."{table}" USING {temp_table} WHERE {join_clause} {delete_from_target_filter}'
+            f'DELETE FROM "{schema}"."{table}" USING "{temp_table}" WHERE {join_clause} {delete_from_target_filter}'
         )
         _logger.debug(target_del_sql)
         cursor.execute(target_del_sql)
         source_del_sql: str = (
-            f'DELETE FROM {temp_table} USING "{schema}"."{table}" WHERE {join_clause} {delete_from_temp_filter}'
+            f'DELETE FROM "{temp_table}" USING "{schema}"."{table}" WHERE {join_clause} {delete_from_temp_filter}'
         )
         _logger.debug(source_del_sql)
         cursor.execute(source_del_sql)
     else:
-        sql: str = f'DELETE FROM "{schema}"."{table}" USING {temp_table} WHERE {join_clause}'
+        sql: str = f'DELETE FROM "{schema}"."{table}" USING "{temp_table}" WHERE {join_clause}'
         _logger.debug(sql)
         cursor.execute(sql)
     if column_names:
         column_names_str = ",".join(column_names)
-        insert_sql = f'INSERT INTO "{schema}"."{table}"({column_names_str}) SELECT {column_names_str} FROM {temp_table}'
+        insert_sql = (
+            f'INSERT INTO "{schema}"."{table}"({column_names_str}) SELECT {column_names_str} FROM "{temp_table}"'
+        )
     else:
-        insert_sql = f'INSERT INTO "{schema}"."{table}" SELECT * FROM {temp_table}'
+        insert_sql = f'INSERT INTO "{schema}"."{table}" SELECT * FROM "{temp_table}"'
     _logger.debug(insert_sql)
     cursor.execute(insert_sql)
     _drop_table(cursor=cursor, schema=schema, table=temp_table)
 
 
 def _validate_parameters(
     redshift_types: Dict[str, str],
     diststyle: str,
     distkey: Optional[str],
     sortstyle: str,
     sortkey: Optional[List[str]],
+    primary_keys: Optional[List[str]],
 ) -> None:
     if diststyle not in _RS_DISTSTYLES:
         raise exceptions.InvalidRedshiftDiststyle(f"diststyle must be in {_RS_DISTSTYLES}")
     cols = list(redshift_types.keys())
     _logger.debug("Redshift columns: %s", cols)
     if (diststyle == "KEY") and (not distkey):
         raise exceptions.InvalidRedshiftDistkey("You must pass a distkey if you intend to use KEY diststyle")
@@ -236,54 +240,61 @@
                 f"sortkey must be a List of items in the columns list: {cols}. " f"Currently value: {sortkey}"
             )
         for key in sortkey:
             if key not in cols:
                 raise exceptions.InvalidRedshiftSortkey(
                     f"sortkey must be a List of items in the columns list: {cols}. " f"Currently value: {key}"
                 )
+    if primary_keys:
+        if not isinstance(primary_keys, list):
+            raise exceptions.InvalidArgumentType(
+                f"""
+                    primary keys should be of type list[str].
+                    Current value: {primary_keys} is of type {type(primary_keys)}
+                """
+            )
 
 
 def _redshift_types_from_path(
-    path: Optional[Union[str, List[str]]],
+    path: Union[str, List[str]],
     varchar_lengths_default: int,
     varchar_lengths: Optional[Dict[str, int]],
     parquet_infer_sampling: float,
     path_suffix: Optional[str],
     path_ignore_suffix: Optional[str],
     use_threads: Union[bool, int],
     boto3_session: Optional[boto3.Session],
     s3_additional_kwargs: Optional[Dict[str, str]],
 ) -> Dict[str, str]:
     """Extract Redshift data types from a Pandas DataFrame."""
     _varchar_lengths: Dict[str, int] = {} if varchar_lengths is None else varchar_lengths
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     _logger.debug("Scanning parquet schemas on s3...")
     athena_types, _ = s3.read_parquet_metadata(
         path=path,
         sampling=parquet_infer_sampling,
         path_suffix=path_suffix,
         path_ignore_suffix=path_ignore_suffix,
         dataset=False,
         use_threads=use_threads,
-        boto3_session=session,
+        boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
     )
     _logger.debug("athena_types: %s", athena_types)
     redshift_types: Dict[str, str] = {}
     for col_name, col_type in athena_types.items():
         length: int = _varchar_lengths[col_name] if col_name in _varchar_lengths else varchar_lengths_default
         redshift_types[col_name] = _data_types.athena2redshift(dtype=col_type, varchar_length=length)
     return redshift_types
 
 
 def _create_table(  # pylint: disable=too-many-locals,too-many-arguments,too-many-branches,too-many-statements
     df: Optional[pd.DataFrame],
     path: Optional[Union[str, List[str]]],
-    con: redshift_connector.Connection,
-    cursor: redshift_connector.Cursor,
+    con: "redshift_connector.Connection",
+    cursor: "redshift_connector.Cursor",
     table: str,
     schema: str,
     mode: str,
     overwrite_method: str,
     index: bool,
     dtype: Optional[Dict[str, str]],
     diststyle: str,
@@ -375,14 +386,15 @@
         raise ValueError("df and path are None.You MUST pass at least one.")
     _validate_parameters(
         redshift_types=redshift_types,
         diststyle=diststyle,
         distkey=distkey,
         sortstyle=sortstyle,
         sortkey=sortkey,
+        primary_keys=primary_keys,
     )
     cols_str: str = "".join([f'"{k}" {v},\n' for k, v in redshift_types.items()])[:-2]
     primary_keys_str: str = f",\nPRIMARY KEY ({', '.join(primary_keys)})" if primary_keys else ""
     distkey_str: str = f"\nDISTKEY({distkey})" if distkey and diststyle == "KEY" else ""
     sortkey_str: str = f"\n{sortstyle} SORTKEY({','.join(sortkey)})" if sortkey else ""
     sql = (
         f'CREATE TABLE IF NOT EXISTS "{schema}"."{table}" (\n'
@@ -420,26 +432,27 @@
     yield from dfs
     if keep_files is False:
         s3.delete_objects(
             path=path, use_threads=use_threads, boto3_session=boto3_session, s3_additional_kwargs=s3_additional_kwargs
         )
 
 
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def connect(
     connection: Optional[str] = None,
     secret_id: Optional[str] = None,
     catalog_id: Optional[str] = None,
     dbname: Optional[str] = None,
     boto3_session: Optional[boto3.Session] = None,
     ssl: bool = True,
     timeout: Optional[int] = None,
     max_prepared_statements: int = 1000,
     tcp_keepalive: bool = True,
     **kwargs: Any,
-) -> redshift_connector.Connection:
+) -> "redshift_connector.Connection":
     """Return a redshift_connector connection from a Glue Catalog or Secret Manager.
 
     Note
     ----
     You MUST pass a `connection` OR `secret_id`.
     Here is an example of the secret structure in Secrets Manager:
     {
@@ -531,28 +544,29 @@
         timeout=timeout,
         max_prepared_statements=max_prepared_statements,
         tcp_keepalive=tcp_keepalive,
         **kwargs,
     )
 
 
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def connect_temp(
     cluster_identifier: str,
     user: str,
     database: Optional[str] = None,
     duration: int = 900,
     auto_create: bool = True,
     db_groups: Optional[List[str]] = None,
     boto3_session: Optional[boto3.Session] = None,
     ssl: bool = True,
     timeout: Optional[int] = None,
     max_prepared_statements: int = 1000,
     tcp_keepalive: bool = True,
     **kwargs: Any,
-) -> redshift_connector.Connection:
+) -> "redshift_connector.Connection":
     """Return a redshift_connector temporary connection (No password required).
 
     https://github.com/aws/amazon-redshift-python-driver
 
     Parameters
     ----------
     cluster_identifier : str
@@ -604,27 +618,27 @@
     >>> con = wr.redshift.connect_temp(cluster_identifier="my-cluster", user="test")
     >>> with con.cursor() as cursor:
     >>>     cursor.execute("SELECT 1")
     >>>     print(cursor.fetchall())
     >>> con.close()
 
     """
-    client_redshift: boto3.client = _utils.client(service_name="redshift", session=boto3_session)
+    client_redshift = _utils.client(service_name="redshift", session=boto3_session)
     args: Dict[str, Any] = {
         "DbUser": user,
         "ClusterIdentifier": cluster_identifier,
         "DurationSeconds": duration,
         "AutoCreate": auto_create,
     }
     if db_groups is not None:
         args["DbGroups"] = db_groups
     else:
         db_groups = []
-    res: Dict[str, Any] = client_redshift.get_cluster_credentials(**args)
-    cluster: Dict[str, Any] = client_redshift.describe_clusters(ClusterIdentifier=cluster_identifier)["Clusters"][0]
+    res = client_redshift.get_cluster_credentials(**args)
+    cluster = client_redshift.describe_clusters(ClusterIdentifier=cluster_identifier)["Clusters"][0]
     return redshift_connector.connect(
         user=res["DbUser"],
         database=database if database else cluster["DBName"],
         password=res["DbPassword"],
         port=cluster["Endpoint"]["Port"],
         host=cluster["Endpoint"]["Address"],
         ssl=ssl,
@@ -632,17 +646,62 @@
         max_prepared_statements=max_prepared_statements,
         tcp_keepalive=tcp_keepalive,
         db_groups=db_groups,
         **kwargs,
     )
 
 
+@overload
 def read_sql_query(
     sql: str,
-    con: redshift_connector.Connection,
+    con: "redshift_connector.Connection",
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "redshift_connector.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_sql_query(
+    sql: str,
+    con: "redshift_connector.Connection",
+    *,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
+def read_sql_query(
+    sql: str,
+    con: "redshift_connector.Connection",
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
@@ -703,17 +762,66 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+@overload
+def read_sql_table(
+    table: str,
+    con: "redshift_connector.Connection",
+    *,
+    schema: Optional[str] = None,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: None = ...,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_sql_table(
+    table: str,
+    con: "redshift_connector.Connection",
+    *,
+    schema: Optional[str] = None,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: int,
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
 def read_sql_table(
     table: str,
-    con: redshift_connector.Connection,
+    con: "redshift_connector.Connection",
+    *,
+    schema: Optional[str] = None,
+    index_col: Optional[Union[str, List[str]]] = ...,
+    params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = ...,
+    chunksize: Optional[int],
+    dtype: Optional[Dict[str, pa.DataType]] = ...,
+    safe: bool = ...,
+    timestamp_as_object: bool = ...,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
+def read_sql_table(
+    table: str,
+    con: "redshift_connector.Connection",
     schema: Optional[str] = None,
     index_col: Optional[Union[str, List[str]]] = None,
     params: Optional[Union[List[Any], Tuple[Any, ...], Dict[Any, Any]]] = None,
     chunksize: Optional[int] = None,
     dtype: Optional[Dict[str, pa.DataType]] = None,
     safe: bool = True,
     timestamp_as_object: bool = False,
@@ -779,18 +887,19 @@
         chunksize=chunksize,
         dtype=dtype,
         safe=safe,
         timestamp_as_object=timestamp_as_object,
     )
 
 
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 @apply_configs
 def to_sql(  # pylint: disable=too-many-locals
     df: pd.DataFrame,
-    con: redshift_connector.Connection,
+    con: "redshift_connector.Connection",
     table: str,
     schema: str,
     mode: str = "append",
     overwrite_method: str = "drop",
     index: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     diststyle: str = "AUTO",
@@ -950,18 +1059,19 @@
         con.rollback()
         _logger.error(ex)
         raise
     finally:
         con.autocommit = autocommit_temp
 
 
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def unload_to_files(
     sql: str,
     path: str,
-    con: redshift_connector.Connection,
+    con: "redshift_connector.Connection",
     iam_role: Optional[str] = None,
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     aws_session_token: Optional[str] = None,
     region: Optional[str] = None,
     unload_format: Optional[str] = None,
     max_file_size: Optional[float] = None,
@@ -1035,29 +1145,34 @@
     ... )
     >>> con.close()
 
 
     """
     if unload_format not in [None, "CSV", "PARQUET"]:
         raise exceptions.InvalidArgumentValue("<unload_format> argument must be 'CSV' or 'PARQUET'")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     with con.cursor() as cursor:
         format_str: str = unload_format or "PARQUET"
         partition_str: str = f"\nPARTITION BY ({','.join(partition_cols)})" if partition_cols else ""
         manifest_str: str = "\nmanifest" if manifest is True else ""
         region_str: str = f"\nREGION AS '{region}'" if region is not None else ""
+        if not max_file_size and engine.get() == EngineEnum.RAY:
+            _logger.warning(
+                "Unload `MAXFILESIZE` is not specified. "
+                "Defaulting to `512.0 MB` corresponding to the recommended Ray target block size."
+            )
+            max_file_size = 512.0
         max_file_size_str: str = f"\nMAXFILESIZE AS {max_file_size} MB" if max_file_size is not None else ""
         kms_key_id_str: str = f"\nKMS_KEY_ID '{kms_key_id}'" if kms_key_id is not None else ""
 
         auth_str: str = _make_s3_auth_string(
             iam_role=iam_role,
             aws_access_key_id=aws_access_key_id,
             aws_secret_access_key=aws_secret_access_key,
             aws_session_token=aws_session_token,
-            boto3_session=session,
+            boto3_session=boto3_session,
         )
 
         sql = (
             f"UNLOAD ('{sql}')\n"
             f"TO '{path}'\n"
             f"{auth_str}"
             "ALLOWOVERWRITE\n"
@@ -1070,18 +1185,22 @@
             f"{max_file_size_str}"
             f"{manifest_str};"
         )
         _logger.debug("sql: \n%s", sql)
         cursor.execute(sql)
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def unload(
     sql: str,
     path: str,
-    con: redshift_connector.Connection,
+    con: "redshift_connector.Connection",
     iam_role: Optional[str] = None,
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     aws_session_token: Optional[str] = None,
     region: Optional[str] = None,
     max_file_size: Optional[float] = None,
     kms_key_id: Optional[str] = None,
@@ -1108,17 +1227,18 @@
     ----
     ``Batching`` (`chunked` argument) (Memory Friendly):
 
     Will enable the function to return an Iterable of DataFrames instead of a regular DataFrame.
 
     There are two batching strategies on awswrangler:
 
-    - If **chunked=True**, a new DataFrame will be returned for each file in your path/dataset.
+    - If **chunked=True**, depending on the size of the data, one or more data frames are returned per file.
+      Unlike **chunked=INTEGER**, rows from different files are not be mixed in the resulting data frames.
 
-    - If **chunked=INTEGER**, awswrangler will iterate on the data by number of rows (equal to the received INTEGER).
+    - If **chunked=INTEGER**, awswrangler iterates on the data by number of rows (equal to the received INTEGER).
 
     `P.S.` `chunked=True` is faster and uses less memory while `chunked=INTEGER` is more precise
     in the number of rows for each Dataframe.
 
 
     Note
     ----
@@ -1189,58 +1309,61 @@
     ...     con=con,
     ...     iam_role="arn:aws:iam::XXX:role/XXX"
     ... )
     >>> con.close()
 
     """
     path = path if path.endswith("/") else f"{path}/"
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     unload_to_files(
         sql=sql,
         path=path,
         con=con,
         iam_role=iam_role,
         aws_access_key_id=aws_access_key_id,
         aws_secret_access_key=aws_secret_access_key,
         aws_session_token=aws_session_token,
         region=region,
         max_file_size=max_file_size,
         kms_key_id=kms_key_id,
         manifest=False,
-        boto3_session=session,
+        boto3_session=boto3_session,
     )
     if chunked is False:
         df: pd.DataFrame = s3.read_parquet(
             path=path,
             chunked=chunked,
             dataset=False,
             use_threads=use_threads,
-            boto3_session=session,
+            boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
             pyarrow_additional_kwargs=pyarrow_additional_kwargs,
         )
         if keep_files is False:
             s3.delete_objects(
-                path=path, use_threads=use_threads, boto3_session=session, s3_additional_kwargs=s3_additional_kwargs
+                path=path,
+                use_threads=use_threads,
+                boto3_session=boto3_session,
+                s3_additional_kwargs=s3_additional_kwargs,
             )
         return df
     return _read_parquet_iterator(
         path=path,
         chunked=chunked,
         use_threads=use_threads,
-        boto3_session=session,
+        boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
         keep_files=keep_files,
         pyarrow_additional_kwargs=pyarrow_additional_kwargs,
     )
 
 
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def copy_from_files(  # pylint: disable=too-many-locals,too-many-arguments
     path: str,
-    con: redshift_connector.Connection,
+    con: "redshift_connector.Connection",
     table: str,
     schema: str,
     iam_role: Optional[str] = None,
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     aws_session_token: Optional[str] = None,
     parquet_infer_sampling: float = 1.0,
@@ -1451,18 +1574,22 @@
         con.rollback()
         _logger.error(ex)
         raise
     finally:
         con.autocommit = autocommit_temp
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
+@_utils.check_optional_dependency(redshift_connector, "redshift_connector")
 def copy(  # pylint: disable=too-many-arguments,too-many-locals
     df: pd.DataFrame,
     path: str,
-    con: redshift_connector.Connection,
+    con: "redshift_connector.Connection",
     table: str,
     schema: str,
     iam_role: Optional[str] = None,
     aws_access_key_id: Optional[str] = None,
     aws_secret_access_key: Optional[str] = None,
     aws_session_token: Optional[str] = None,
     index: bool = False,
@@ -1476,14 +1603,15 @@
     primary_keys: Optional[List[str]] = None,
     varchar_lengths_default: int = 256,
     varchar_lengths: Optional[Dict[str, int]] = None,
     serialize_to_json: bool = False,
     keep_files: bool = False,
     use_threads: Union[bool, int] = True,
     lock: bool = False,
+    commit_transaction: bool = True,
     sql_copy_extra_params: Optional[List[str]] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, str]] = None,
     max_rows_by_file: Optional[int] = 10_000_000,
     precombine_key: Optional[str] = None,
     use_column_names: bool = False,
 ) -> None:
@@ -1569,14 +1697,16 @@
         Should keep stage files?
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     lock : bool
         True to execute LOCK command inside the transaction to force serializable isolation.
+    commit_transaction : bool
+        Whether to commit the transaction. True by default.
     sql_copy_extra_params : Optional[List[str]]
         Additional copy parameters to pass to the command. For example: ["STATUPDATE ON"]
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     s3_additional_kwargs : Dict[str, str], optional
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'ServerSideEncryption': 'aws:kms', 'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'}
@@ -1612,30 +1742,29 @@
     ... )
     >>> con.close()
 
     """
     path = path[:-1] if path.endswith("*") else path
     path = path if path.endswith("/") else f"{path}/"
     column_names = [f'"{column}"' for column in df.columns] if use_column_names else []
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    if s3.list_objects(path=path, boto3_session=session, s3_additional_kwargs=s3_additional_kwargs):
+    if s3.list_objects(path=path, boto3_session=boto3_session, s3_additional_kwargs=s3_additional_kwargs):
         raise exceptions.InvalidArgument(
             f"The received S3 path ({path}) is not empty. "
             "Please, provide a different path or use wr.s3.delete_objects() to clean up the current one."
         )
     try:
         s3.to_parquet(
             df=df,
             path=path,
             index=index,
             dataset=True,
             mode="append",
             dtype=dtype,
             use_threads=use_threads,
-            boto3_session=session,
+            boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
             max_rows_by_file=max_rows_by_file,
         )
         copy_from_files(
             path=path,
             con=con,
             table=table,
@@ -1652,18 +1781,22 @@
             sortkey=sortkey,
             primary_keys=primary_keys,
             varchar_lengths_default=varchar_lengths_default,
             varchar_lengths=varchar_lengths,
             serialize_to_json=serialize_to_json,
             use_threads=use_threads,
             lock=lock,
-            boto3_session=session,
+            commit_transaction=commit_transaction,
+            boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
             sql_copy_extra_params=sql_copy_extra_params,
             precombine_key=precombine_key,
             column_names=column_names,
         )
     finally:
         if keep_files is False:
             s3.delete_objects(
-                path=path, use_threads=use_threads, boto3_session=session, s3_additional_kwargs=s3_additional_kwargs
+                path=path,
+                use_threads=use_threads,
+                boto3_session=boto3_session,
+                s3_additional_kwargs=s3_additional_kwargs,
             )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/__init__.py` & `awswrangler-3.0.0rc3/awswrangler/s3/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Amazon S3 Read Module."""
 
 from awswrangler.s3._copy import copy_objects, merge_datasets  # noqa
 from awswrangler.s3._delete import delete_objects  # noqa
 from awswrangler.s3._describe import describe_objects, get_bucket_region, size_objects  # noqa
 from awswrangler.s3._download import download  # noqa
 from awswrangler.s3._list import does_object_exist, list_buckets, list_directories, list_objects  # noqa
-from awswrangler.s3._merge_upsert_table import merge_upsert_table  # noqa
+from awswrangler.s3._read_deltalake import read_deltalake  # noqa
 from awswrangler.s3._read_excel import read_excel  # noqa
 from awswrangler.s3._read_parquet import read_parquet, read_parquet_metadata, read_parquet_table  # noqa
 from awswrangler.s3._read_text import read_csv, read_fwf, read_json  # noqa
 from awswrangler.s3._select import select_query
 from awswrangler.s3._upload import upload  # noqa
 from awswrangler.s3._wait import wait_objects_exist, wait_objects_not_exist  # noqa
 from awswrangler.s3._write_excel import to_excel  # noqa
@@ -23,14 +23,15 @@
     "describe_objects",
     "get_bucket_region",
     "size_objects",
     "does_object_exist",
     "list_buckets",
     "list_directories",
     "list_objects",
+    "read_deltalake",
     "read_parquet",
     "read_parquet_metadata",
     "read_parquet_table",
     "read_csv",
     "read_fwf",
     "read_json",
     "wait_objects_exist",
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_copy.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_copy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,79 @@
 """Amazon S3 Copy Module (PRIVATE)."""
 
+import itertools
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import boto3
 from boto3.s3.transfer import TransferConfig
 
 from awswrangler import _utils, exceptions
+from awswrangler._distributed import engine
+from awswrangler._threading import _get_executor
+from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._delete import delete_objects
 from awswrangler.s3._fs import get_botocore_valid_kwargs
 from awswrangler.s3._list import list_objects
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+    from mypy_boto3_s3.type_defs import CopySourceTypeDef
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+@engine.dispatch_on_engine
 def _copy_objects(
+    s3_client: Optional["S3Client"],
     batch: List[Tuple[str, str]],
     use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
     s3_additional_kwargs: Optional[Dict[str, Any]],
 ) -> None:
     _logger.debug("len(batch): %s", len(batch))
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-    resource_s3: boto3.resource = _utils.resource(service_name="s3", session=boto3_session)
-    if s3_additional_kwargs is None:
-        boto3_kwargs: Optional[Dict[str, Any]] = None
-    else:
-        boto3_kwargs = get_botocore_valid_kwargs(function_name="copy_object", s3_additional_kwargs=s3_additional_kwargs)
+    s3_client = s3_client if s3_client else _utils.client(service_name="s3")
     for source, target in batch:
         source_bucket, source_key = _utils.parse_path(path=source)
-        copy_source: Dict[str, str] = {"Bucket": source_bucket, "Key": source_key}
+        copy_source: CopySourceTypeDef = {"Bucket": source_bucket, "Key": source_key}
         target_bucket, target_key = _utils.parse_path(path=target)
-        resource_s3.meta.client.copy(
+        s3_client.copy(
             CopySource=copy_source,
             Bucket=target_bucket,
             Key=target_key,
-            SourceClient=client_s3,
-            ExtraArgs=boto3_kwargs,
-            Config=TransferConfig(num_download_attempts=10, use_threads=use_threads),
+            ExtraArgs=s3_additional_kwargs,  # type: ignore[arg-type]
+            Config=TransferConfig(num_download_attempts=10, use_threads=use_threads),  # type: ignore[arg-type]
         )
 
 
+def _copy(
+    batches: List[List[Tuple[str, str]]],
+    use_threads: Union[bool, int],
+    boto3_session: Optional[boto3.Session],
+    s3_additional_kwargs: Optional[Dict[str, Any]],
+) -> None:
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
+    if s3_additional_kwargs is None:
+        boto3_kwargs: Optional[Dict[str, Any]] = None
+    else:
+        boto3_kwargs = get_botocore_valid_kwargs(function_name="copy_object", s3_additional_kwargs=s3_additional_kwargs)
+    executor = _get_executor(use_threads=use_threads)
+    ray_get(
+        executor.map(
+            _copy_objects,
+            s3_client,
+            batches,
+            itertools.repeat(use_threads),
+            itertools.repeat(boto3_kwargs),
+        )
+    )
+
+
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def merge_datasets(
     source_path: str,
     target_path: str,
     mode: str = "append",
     ignore_empty: bool = False,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
@@ -119,49 +148,49 @@
     ...     }
     ... )
     ["s3://bucket1/dir1/key0", "s3://bucket1/dir1/key1"]
 
     """
     source_path = source_path[:-1] if source_path[-1] == "/" else source_path
     target_path = target_path[:-1] if target_path[-1] == "/" else target_path
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
 
-    paths: List[str] = list_objects(  # type: ignore
-        path=f"{source_path}/", ignore_empty=ignore_empty, boto3_session=session
-    )
+    paths: List[str] = list_objects(path=f"{source_path}/", ignore_empty=ignore_empty, boto3_session=boto3_session)
     _logger.debug("len(paths): %s", len(paths))
     if len(paths) < 1:
         return []
 
     if mode == "overwrite":
         _logger.debug("Deleting to overwrite: %s/", target_path)
-        delete_objects(path=f"{target_path}/", use_threads=use_threads, boto3_session=session)
+        delete_objects(path=f"{target_path}/", use_threads=use_threads, boto3_session=boto3_session)
     elif mode == "overwrite_partitions":
         paths_wo_prefix: List[str] = [x.replace(f"{source_path}/", "") for x in paths]
         paths_wo_filename: List[str] = [f"{x.rpartition('/')[0]}/" for x in paths_wo_prefix]
         partitions_paths: List[str] = list(set(paths_wo_filename))
         target_partitions_paths = [f"{target_path}/{x}" for x in partitions_paths]
         for path in target_partitions_paths:
             _logger.debug("Deleting to overwrite_partitions: %s", path)
-            delete_objects(path=path, use_threads=use_threads, boto3_session=session)
+            delete_objects(path=path, use_threads=use_threads, boto3_session=boto3_session)
     elif mode != "append":
         raise exceptions.InvalidArgumentValue(f"{mode} is a invalid mode option.")
 
     new_objects: List[str] = copy_objects(
         paths=paths,
         source_path=source_path,
         target_path=target_path,
         use_threads=use_threads,
-        boto3_session=session,
+        boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
     )
     _logger.debug("len(new_objects): %s", len(new_objects))
     return new_objects
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def copy_objects(
     paths: List[str],
     source_path: str,
     target_path: str,
     replace_filenames: Optional[Dict[str, str]] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
@@ -227,15 +256,14 @@
 
     """
     _logger.debug("len(paths): %s", len(paths))
     if len(paths) < 1:
         return []
     source_path = source_path[:-1] if source_path[-1] == "/" else source_path
     target_path = target_path[:-1] if target_path[-1] == "/" else target_path
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     batch: List[Tuple[str, str]] = []
     new_objects: List[str] = []
     for path in paths:
         path_wo_prefix: str = path.replace(f"{source_path}/", "")
         path_final: str = f"{target_path}/{path_wo_prefix}"
         if replace_filenames is not None:
             parts: List[str] = path_final.rsplit(sep="/", maxsplit=1)
@@ -245,11 +273,14 @@
                 if filename in replace_filenames:
                     new_filename: str = replace_filenames[filename]
                     _logger.debug("Replacing filename: %s -> %s", filename, new_filename)
                     path_final = f"{path_wo_filename}/{new_filename}"
         new_objects.append(path_final)
         batch.append((path, path_final))
     _logger.debug("len(new_objects): %s", len(new_objects))
-    _copy_objects(
-        batch=batch, use_threads=use_threads, boto3_session=session, s3_additional_kwargs=s3_additional_kwargs
+    _copy(
+        batches=_utils.chunkify(lst=batch, max_length=1_000),
+        use_threads=use_threads,
+        boto3_session=boto3_session,
+        s3_additional_kwargs=s3_additional_kwargs,
     )
     return new_objects
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_delete.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_delete.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Amazon S3 Delete Module (PRIVATE)."""
 
 import datetime
 import itertools
 import logging
-from typing import Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import boto3
 
 from awswrangler import _utils, exceptions
 from awswrangler._distributed import engine
 from awswrangler._threading import _get_executor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._fs import get_botocore_valid_kwargs
 from awswrangler.s3._list import _path2list
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _split_paths_by_bucket(paths: List[str]) -> Dict[str, List[str]]:
     buckets: Dict[str, List[str]] = {}
     bucket: str
     for path in paths:
@@ -26,42 +29,45 @@
             buckets[bucket] = []
         buckets[bucket].append(path)
     return buckets
 
 
 @engine.dispatch_on_engine
 def _delete_objects(
-    boto3_session: Optional[boto3.Session],
+    s3_client: Optional["S3Client"],
     paths: List[str],
     s3_additional_kwargs: Optional[Dict[str, Any]],
 ) -> None:
-    client_s3: boto3.client = _utils.client(
-        service_name="s3",
-        session=boto3_session,
-    )
+    s3_client = s3_client if s3_client else _utils.client(service_name="s3")
     _logger.debug("len(paths): %s", len(paths))
     if s3_additional_kwargs:
         extra_kwargs: Dict[str, Any] = get_botocore_valid_kwargs(
             function_name="list_objects_v2", s3_additional_kwargs=s3_additional_kwargs
         )
     else:
         extra_kwargs = {}
     bucket = _utils.parse_path(path=paths[0])[0]
     batch: List[Dict[str, str]] = [{"Key": _utils.parse_path(path)[1]} for path in paths]
-    res = client_s3.delete_objects(Bucket=bucket, Delete={"Objects": batch}, **extra_kwargs)
-    deleted: List[Dict[str, Any]] = res.get("Deleted", [])
-    for obj in deleted:
-        _logger.debug("s3://%s/%s has been deleted.", bucket, obj.get("Key"))
-    errors: List[Dict[str, Any]] = res.get("Errors", [])
+    res = s3_client.delete_objects(
+        Bucket=bucket,
+        Delete={"Objects": batch},  # type: ignore[typeddict-item]
+        **extra_kwargs,
+    )
+    deleted = res.get("Deleted", [])
+    _logger.debug("len(deleted): %s", len(deleted))
+    errors = res.get("Errors", [])
     for error in errors:
         _logger.debug("error: %s", error)
         if "Code" not in error or error["Code"] != "InternalError":
             raise exceptions.ServiceApiError(errors)
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def delete_objects(
     path: Union[str, List[str]],
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
@@ -112,29 +118,30 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.s3.delete_objects(['s3://bucket/key0', 's3://bucket/key1'])  # Delete both objects
     >>> wr.s3.delete_objects('s3://bucket/prefix')  # Delete all objects under the received prefix
 
     """
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     paths: List[str] = _path2list(
         path=path,
-        boto3_session=boto3_session,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
+        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
     )
     paths_by_bucket: Dict[str, List[str]] = _split_paths_by_bucket(paths)
 
     chunks = []
     for _, paths in paths_by_bucket.items():
         chunks += _utils.chunkify(lst=paths, max_length=1_000)
 
     executor = _get_executor(use_threads=use_threads)
     ray_get(
         executor.map(
             _delete_objects,
-            boto3_session,
+            s3_client,
             chunks,
             itertools.repeat(s3_additional_kwargs),
         )
     )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_describe.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_describe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,56 @@
 """Amazon S3 Describe Module (INTERNAL)."""
 
-import concurrent.futures
 import datetime
 import itertools
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 import boto3
 
 from awswrangler import _utils
+from awswrangler._distributed import engine
+from awswrangler._threading import _get_executor
+from awswrangler.distributed.ray import ray_get
 from awswrangler.s3 import _fs
 from awswrangler.s3._list import _path2list
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+@engine.dispatch_on_engine
 def _describe_object(
+    s3_client: "S3Client",
     path: str,
-    boto3_session: boto3.Session,
     s3_additional_kwargs: Optional[Dict[str, Any]],
     version_id: Optional[str] = None,
 ) -> Tuple[str, Dict[str, Any]]:
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-    bucket: str
-    key: str
+    s3_client = s3_client if s3_client else _utils.client(service_name="s3")
+
     bucket, key = _utils.parse_path(path=path)
     if s3_additional_kwargs:
         extra_kwargs: Dict[str, Any] = _fs.get_botocore_valid_kwargs(
             function_name="head_object", s3_additional_kwargs=s3_additional_kwargs
         )
     else:
         extra_kwargs = {}
-    desc: Dict[str, Any]
     if version_id:
         extra_kwargs["VersionId"] = version_id
     desc = _utils.try_it(
-        f=client_s3.head_object, ex=client_s3.exceptions.NoSuchKey, Bucket=bucket, Key=key, **extra_kwargs
-    )
-    return path, desc
-
-
-def _describe_object_concurrent(
-    path: str,
-    boto3_primitives: _utils.Boto3PrimitivesType,
-    s3_additional_kwargs: Optional[Dict[str, Any]],
-    version_id: Optional[str] = None,
-) -> Tuple[str, Dict[str, Any]]:
-    boto3_session = _utils.boto3_from_primitives(primitives=boto3_primitives)
-    return _describe_object(
-        path=path, boto3_session=boto3_session, s3_additional_kwargs=s3_additional_kwargs, version_id=version_id
+        f=s3_client.head_object, ex=s3_client.exceptions.NoSuchKey, Bucket=bucket, Key=key, **extra_kwargs
     )
+    return path, cast(Dict[str, Any], desc)
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
 def describe_objects(
     path: Union[str, List[str]],
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
@@ -116,60 +111,43 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> descs0 = wr.s3.describe_objects(['s3://bucket/key0', 's3://bucket/key1'])  # Describe both objects
     >>> descs1 = wr.s3.describe_objects('s3://bucket/prefix')  # Describe all objects under the prefix
 
     """
-    paths: List[str] = _path2list(
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
+
+    paths = _path2list(
         path=path,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         s3_additional_kwargs=s3_additional_kwargs,
     )
+    _logger.debug("len(paths): %s", len(paths))
     if len(paths) < 1:
         return {}
-    resp_list: List[Tuple[str, Dict[str, Any]]]
-    if len(paths) == 1:
-        resp_list = [
-            _describe_object(
-                path=paths[0],
-                version_id=version_id.get(paths[0]) if isinstance(version_id, dict) else version_id,
-                boto3_session=boto3_session,
-                s3_additional_kwargs=s3_additional_kwargs,
-            )
-        ]
-    elif use_threads is False:
-        resp_list = [
-            _describe_object(
-                path=p,
-                version_id=version_id.get(p) if isinstance(version_id, dict) else version_id,
-                boto3_session=boto3_session,
-                s3_additional_kwargs=s3_additional_kwargs,
-            )
-            for p in paths
-        ]
-    else:
-        cpus: int = _utils.ensure_cpu_count(use_threads=use_threads)
-        versions = [version_id.get(p) if isinstance(version_id, dict) else version_id for p in paths]
-        with concurrent.futures.ThreadPoolExecutor(max_workers=cpus) as executor:
-            resp_list = list(
-                executor.map(
-                    _describe_object_concurrent,
-                    paths,
-                    versions,
-                    itertools.repeat(_utils.boto3_to_primitives(boto3_session=boto3_session)),
-                    itertools.repeat(s3_additional_kwargs),
-                )
-            )
-    desc_dict: Dict[str, Dict[str, Any]] = dict(resp_list)
-    return desc_dict
+
+    executor = _get_executor(use_threads=use_threads)
+    resp_list = ray_get(
+        executor.map(
+            _describe_object,
+            s3_client,
+            paths,
+            itertools.repeat(s3_additional_kwargs),
+            [version_id.get(p) if isinstance(version_id, dict) else version_id for p in paths],
+        )
+    )
+    return dict(resp_list)
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
 def size_objects(
     path: Union[str, List[str]],
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     use_threads: Union[bool, int] = True,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
 ) -> Dict[str, Optional[int]]:
@@ -212,23 +190,22 @@
     Examples
     --------
     >>> import awswrangler as wr
     >>> sizes0 = wr.s3.size_objects(['s3://bucket/key0', 's3://bucket/key1'])  # Get the sizes of both objects
     >>> sizes1 = wr.s3.size_objects('s3://bucket/prefix')  # Get the sizes of all objects under the received prefix
 
     """
-    desc_list: Dict[str, Dict[str, Any]] = describe_objects(
+    desc_list = describe_objects(
         path=path,
         version_id=version_id,
         use_threads=use_threads,
         boto3_session=boto3_session,
         s3_additional_kwargs=s3_additional_kwargs,
     )
-    size_dict: Dict[str, Optional[int]] = {k: d.get("ContentLength", None) for k, d in desc_list.items()}
-    return size_dict
+    return {k: d.get("ContentLength", None) for k, d in desc_list.items()}
 
 
 def get_bucket_region(bucket: str, boto3_session: Optional[boto3.Session] = None) -> str:
     """Get bucket region name.
 
     Parameters
     ----------
@@ -252,13 +229,13 @@
     Using a custom boto3 session
 
     >>> import boto3
     >>> import awswrangler as wr
     >>> region = wr.s3.get_bucket_region('bucket-name', boto3_session=boto3.Session())
 
     """
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
+    client_s3 = _utils.client(service_name="s3", session=boto3_session)
     _logger.debug("bucket: %s", bucket)
     region: str = client_s3.get_bucket_location(Bucket=bucket)["LocationConstraint"]
     region = "us-east-1" if region is None else region
     _logger.debug("region: %s", region)
     return region
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_download.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_download.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Amazon S3 Download Module (PRIVATE)."""
 
 import logging
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union, cast
 
 import boto3
 
-from awswrangler import _utils
 from awswrangler.s3._fs import open_s3_object
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def download(
     path: str,
@@ -58,25 +57,24 @@
     Downloading a file using a file-like object
 
     >>> import awswrangler as wr
     >>> with open(file='./key', mode='wb') as local_f:
     >>>     wr.s3.download(path='s3://bucket/key', local_file=local_f)
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     _logger.debug("path: %s", path)
     with open_s3_object(
         path=path,
         mode="rb",
         use_threads=use_threads,
         version_id=version_id,
         s3_block_size=-1,  # One shot download
         s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=session,
+        boto3_session=boto3_session,
     ) as s3_f:
         if isinstance(local_file, str):
             _logger.debug("Downloading local_file: %s", local_file)
             with open(file=local_file, mode="wb") as local_f:
-                local_f.write(s3_f.read())
+                local_f.write(cast(bytes, s3_f.read()))
         else:
             _logger.debug("Downloading file-like object.")
             local_file.write(s3_f.read())
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_fs.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_fs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 import io
 import itertools
 import logging
 import math
 import socket
 from contextlib import contextmanager
 from errno import ESPIPE
-from typing import Any, BinaryIO, Dict, Iterator, List, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, BinaryIO, Dict, Iterator, List, Optional, Tuple, Union, cast
 
 import boto3
 from botocore.exceptions import ReadTimeoutError
 from botocore.loaders import Loader
 from botocore.model import ServiceModel
 
 from awswrangler import _utils, exceptions
 from awswrangler._config import apply_configs
-from awswrangler.s3._describe import size_objects
+from awswrangler._distributed import engine
+from awswrangler.s3._describe import _describe_object
+
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 _S3_RETRYABLE_ERRORS: Tuple[Any, Any, Any] = (socket.timeout, ConnectionError, ReadTimeoutError)
 
 _MIN_WRITE_BLOCK: int = 5_242_880  # 5 MB (5 * 2**20)
 _MIN_PARALLEL_READ_BLOCK: int = 5_242_880  # 5 MB (5 * 2**20)
@@ -42,34 +47,33 @@
     return {k: v for k, v in s3_additional_kwargs.items() if k in allowed_kwargs}
 
 
 def _fetch_range(
     range_values: Tuple[int, int],
     bucket: str,
     key: str,
-    s3_client: boto3.client,
+    s3_client: "S3Client",
     boto3_kwargs: Dict[str, Any],
     version_id: Optional[str] = None,
 ) -> Tuple[int, bytes]:
     start, end = range_values
     _logger.debug("Fetching: s3://%s/%s - VersionId: %s - Range: %s-%s", bucket, key, version_id, start, end)
-    resp: Dict[str, Any]
     if version_id:
         boto3_kwargs["VersionId"] = version_id
     resp = _utils.try_it(
         f=s3_client.get_object,
         ex=_S3_RETRYABLE_ERRORS,
         base=0.5,
         max_num_tries=6,
         Bucket=bucket,
         Key=key,
         Range=f"bytes={start}-{end - 1}",
         **boto3_kwargs,
     )
-    return start, cast(bytes, resp["Body"].read())
+    return start, resp["Body"].read()
 
 
 class _UploadProxy:
     def __init__(self, use_threads: Union[bool, int]):
         self.closed = False
         self._exec: Optional[concurrent.futures.ThreadPoolExecutor]
         self._results: List[Dict[str, Union[str, int]]] = []
@@ -87,22 +91,20 @@
     @staticmethod
     def _caller(
         bucket: str,
         key: str,
         part: int,
         upload_id: str,
         data: bytes,
-        boto3_primitives: _utils.Boto3PrimitivesType,
+        s3_client: "S3Client",
         boto3_kwargs: Dict[str, Any],
     ) -> Dict[str, Union[str, int]]:
         _logger.debug("Upload part %s started.", part)
-        boto3_session: boto3.Session = _utils.boto3_from_primitives(primitives=boto3_primitives)
-        client: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-        resp: Dict[str, Any] = _utils.try_it(
-            f=client.upload_part,
+        resp = _utils.try_it(
+            f=s3_client.upload_part,
             ex=_S3_RETRYABLE_ERRORS,
             base=0.5,
             max_num_tries=6,
             Bucket=bucket,
             Key=key,
             Body=data,
             PartNumber=part,
@@ -115,40 +117,40 @@
     def upload(
         self,
         bucket: str,
         key: str,
         part: int,
         upload_id: str,
         data: bytes,
-        boto3_session: boto3.Session,
+        s3_client: "S3Client",
         boto3_kwargs: Dict[str, Any],
     ) -> None:
         """Upload Part."""
         if self._exec is not None:
             _utils.block_waiting_available_thread(seq=self._futures, max_workers=self._cpus)
             future = self._exec.submit(
                 _UploadProxy._caller,
                 bucket=bucket,
                 key=key,
                 part=part,
                 upload_id=upload_id,
                 data=data,
-                boto3_primitives=_utils.boto3_to_primitives(boto3_session=boto3_session),
+                s3_client=s3_client,
                 boto3_kwargs=boto3_kwargs,
             )
             self._futures.append(future)
         else:
             self._results.append(
                 self._caller(
                     bucket=bucket,
                     key=key,
                     part=part,
                     upload_id=upload_id,
                     data=data,
-                    boto3_primitives=_utils.boto3_to_primitives(boto3_session=boto3_session),
+                    s3_client=s3_client,
                     boto3_kwargs=boto3_kwargs,
                 )
             )
 
     def close(self) -> List[Dict[str, Union[str, int]]]:
         """Close the proxy."""
         if self.closed is True:
@@ -168,27 +170,26 @@
 
     def __init__(
         self,
         path: str,
         s3_block_size: int,
         mode: str,
         use_threads: Union[bool, int],
+        s3_client: "S3Client",
         s3_additional_kwargs: Optional[Dict[str, str]],
-        boto3_session: Optional[boto3.Session],
         newline: Optional[str],
         encoding: Optional[str],
         version_id: Optional[str] = None,
     ) -> None:
         super().__init__()
         self._use_threads = use_threads
         self._newline: str = "\n" if newline is None else newline
         self._encoding: str = "utf-8" if encoding is None else encoding
         self._bucket, self._key = _utils.parse_path(path=path)
         self._version_id = version_id
-        self._boto3_session: boto3.Session = _utils.ensure_session(session=boto3_session)
         if mode not in {"rb", "wb", "r", "w"}:
             raise NotImplementedError(f"File mode must be {'rb', 'wb', 'r', 'w'}, not {mode}")
         self._mode: str = "rb" if mode is None else mode
         self._one_shot_download: bool = False
         if 0 < s3_block_size < 3:
             raise exceptions.InvalidArgumentValue(
                 "s3_block_size MUST > 2 to define a valid size or "
@@ -196,43 +197,44 @@
             )
         if s3_block_size <= 0:
             _logger.debug("s3_block_size of %d, enabling one_shot_download.", s3_block_size)
             self._one_shot_download = True
         self._s3_block_size: int = s3_block_size
         self._s3_half_block_size: int = s3_block_size // 2
         self._s3_additional_kwargs: Dict[str, str] = {} if s3_additional_kwargs is None else s3_additional_kwargs
-        self._client: boto3.client = _utils.client(service_name="s3", session=self._boto3_session)
+        self._client: "S3Client" = s3_client
         self._loc: int = 0
 
         if self.readable() is True:
             self._cache: bytes = b""
             self._start: int = 0
             self._end: int = 0
-            size: Optional[int] = size_objects(
-                path=[path],
-                version_id=version_id,
-                use_threads=False,
-                boto3_session=self._boto3_session,
+            func = engine.dispatch_func(_describe_object, "python")
+            _, desc = func(
+                s3_client=self._client,
+                path=path,
                 s3_additional_kwargs=self._s3_additional_kwargs,
-            )[path]
+                version_id=version_id,
+            )
+            size: Optional[int] = desc.get("ContentLength", None)
             if size is None:
                 raise exceptions.InvalidArgumentValue(f"S3 object w/o defined size: {path}")
             self._size: int = size
             _logger.debug("self._size: %s", self._size)
             _logger.debug("self._s3_block_size: %s", self._s3_block_size)
         elif self.writable() is True:
             self._mpu: Dict[str, Any] = {}
             self._buffer: io.BytesIO = io.BytesIO()
             self._parts_count: int = 0
             self._size = 0
             self._upload_proxy: _UploadProxy = _UploadProxy(use_threads=self._use_threads)
         else:
             raise RuntimeError(f"Invalid mode: {self._mode}")
 
-    def __enter__(self) -> Union["_S3ObjectBase"]:
+    def __enter__(self) -> "_S3ObjectBase":
         return self
 
     def __exit__(self, exc_type: Any, exc_value: Any, exc_traceback: Any) -> None:
         """Close the context."""
         _logger.debug("exc_type: %s", exc_type)
         _logger.debug("exc_value: %s", exc_value)
         _logger.debug("exc_traceback: %s", exc_traceback)
@@ -257,26 +259,25 @@
 
     @staticmethod
     def _merge_range(ranges: List[Tuple[int, bytes]]) -> bytes:
         return b"".join(data for start, data in sorted(ranges, key=lambda r: r[0]))
 
     def _fetch_range_proxy(self, start: int, end: int) -> bytes:
         _logger.debug("Fetching: s3://%s/%s - Range: %s-%s", self._bucket, self._key, start, end)
-        s3_client: boto3.client = _utils.client(service_name="s3", session=self._boto3_session)
         boto3_kwargs: Dict[str, Any] = get_botocore_valid_kwargs(
             function_name="get_object", s3_additional_kwargs=self._s3_additional_kwargs
         )
         cpus: int = _utils.ensure_cpu_count(use_threads=self._use_threads)
         range_size: int = end - start
         if cpus < 2 or range_size < (2 * _MIN_PARALLEL_READ_BLOCK):
             return _fetch_range(
                 range_values=(start, end),
                 bucket=self._bucket,
                 key=self._key,
-                s3_client=s3_client,
+                s3_client=self._client,
                 boto3_kwargs=boto3_kwargs,
                 version_id=self._version_id,
             )[1]
         sizes: Tuple[int, ...] = _utils.get_even_chunks_sizes(
             total_size=range_size, chunk_size=_MIN_PARALLEL_READ_BLOCK, upper_bound=False
         )
         ranges: List[Tuple[int, int]] = []
@@ -288,15 +289,15 @@
             return self._merge_range(
                 ranges=list(
                     executor.map(
                         _fetch_range,
                         ranges,
                         itertools.repeat(self._bucket),
                         itertools.repeat(self._key),
-                        itertools.repeat(s3_client),
+                        itertools.repeat(self._client),
                         itertools.repeat(boto3_kwargs),
                         itertools.repeat(self._version_id),
                     )
                 ),
             )
 
     def _fetch(self, start: int, end: int) -> None:
@@ -395,15 +396,15 @@
             total_size: int = self._buffer.tell()
             if total_size < _MIN_WRITE_BLOCK and force is False:
                 return None
             if total_size == 0:
                 return None
             _logger.debug("Flushing: %s bytes", total_size)
             self._mpu = self._mpu or _utils.try_it(
-                f=self._client.create_multipart_upload,
+                f=self._client.create_multipart_upload,  # type: ignore[arg-type]
                 ex=_S3_RETRYABLE_ERRORS,
                 base=0.5,
                 max_num_tries=6,
                 Bucket=self._bucket,
                 Key=self._key,
                 **get_botocore_valid_kwargs(
                     function_name="create_multipart_upload", s3_additional_kwargs=self._s3_additional_kwargs
@@ -417,15 +418,15 @@
                 self._parts_count += 1
                 self._upload_proxy.upload(
                     bucket=self._bucket,
                     key=self._key,
                     part=self._parts_count,
                     upload_id=self._mpu["UploadId"],
                     data=self._buffer.read(chunk_size),
-                    boto3_session=self._boto3_session,
+                    s3_client=self._client,
                     boto3_kwargs=get_botocore_valid_kwargs(
                         function_name="upload_part", s3_additional_kwargs=self._s3_additional_kwargs
                     ),
                 )
             self._buffer.seek(0)
             self._buffer.truncate(0)
             self._buffer.close()
@@ -525,15 +526,15 @@
             if self._end >= self._size:
                 return self.read(-1)
 
             end = self._end + self._s3_half_block_size
             end = self._size if end > self._size else end
             self._fetch(self._loc, end)
 
-    def write(self, data: Union[bytes, bytearray, memoryview]) -> int:  # type: ignore
+    def write(self, data: Union[bytes, bytearray, memoryview]) -> int:  # type: ignore[override]
         """Write data to buffer and only upload on close() or if buffer is greater than or equal to _MIN_WRITE_BLOCK."""
         if self.writable() is False:
             raise RuntimeError("File not in write mode.")
         if self.closed:  # pylint: disable=using-constant-test
             raise RuntimeError("I/O operation on closed file.")
         n: int = self._buffer.write(data)
         self._loc += n
@@ -548,29 +549,31 @@
     path: str,
     mode: str,
     version_id: Optional[str] = None,
     use_threads: Union[bool, int] = False,
     s3_additional_kwargs: Optional[Dict[str, str]] = None,
     s3_block_size: int = -1,  # One shot download
     boto3_session: Optional[boto3.Session] = None,
+    s3_client: Optional["S3Client"] = None,
     newline: Optional[str] = "\n",
     encoding: Optional[str] = "utf-8",
 ) -> Iterator[Union[_S3ObjectBase, io.TextIOWrapper]]:
-    """Return a _S3Object or TextIOWrapper based in the received mode."""
+    """Return a _S3Object or TextIOWrapper based on the received mode."""
     s3obj: Optional[_S3ObjectBase] = None
     text_s3obj: Optional[io.TextIOWrapper] = None
+    s3_client = _utils.client(service_name="s3", session=boto3_session) if not s3_client else s3_client
     try:
         s3obj = _S3ObjectBase(
             path=path,
             s3_block_size=s3_block_size,
             mode=mode,
             version_id=version_id,
             use_threads=use_threads,
+            s3_client=s3_client,
             s3_additional_kwargs=s3_additional_kwargs,
-            boto3_session=boto3_session,
             encoding=encoding,
             newline=newline,
         )
         if "b" in mode:  # binary
             yield s3obj
         else:  # text
             text_s3obj = io.TextIOWrapper(
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_list.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_write_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,377 +1,344 @@
-"""Amazon S3 List Module (PRIVATE)."""
+"""Amazon S3 Write Dataset (PRIVATE)."""
 
-import datetime
-import fnmatch
 import logging
-from typing import Any, Dict, Iterator, List, Optional, Sequence, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import boto3
-import botocore.exceptions
+import numpy as np
+import pandas as pd
 
-from awswrangler import _utils, exceptions
-from awswrangler.s3 import _fs
+from awswrangler import exceptions, lakeformation, typing
+from awswrangler._distributed import engine
+from awswrangler._utils import client
+from awswrangler.s3._delete import delete_objects
+from awswrangler.s3._write_concurrent import _WriteProxy
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _path2list(
-    path: Union[str, Sequence[str]],
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, Any]],
-    last_modified_begin: Optional[datetime.datetime] = None,
-    last_modified_end: Optional[datetime.datetime] = None,
-    suffix: Union[str, List[str], None] = None,
-    ignore_suffix: Union[str, List[str], None] = None,
-    ignore_empty: bool = False,
-) -> List[str]:
-    """Convert Amazon S3 path to list of objects."""
-    _suffix: Optional[List[str]] = [suffix] if isinstance(suffix, str) else suffix
-    _ignore_suffix: Optional[List[str]] = [ignore_suffix] if isinstance(ignore_suffix, str) else ignore_suffix
-    if isinstance(path, str):  # prefix
-        paths: List[str] = list_objects(  # type: ignore
-            path=path,
-            suffix=_suffix,
-            ignore_suffix=_ignore_suffix,
-            boto3_session=boto3_session,
-            last_modified_begin=last_modified_begin,
-            last_modified_end=last_modified_end,
-            ignore_empty=ignore_empty,
-            s3_additional_kwargs=s3_additional_kwargs,
+def _get_bucketing_series(df: pd.DataFrame, bucketing_info: typing.BucketingInfoTuple) -> pd.Series:
+    bucket_number_series = (
+        df[bucketing_info[0]]
+        # Prevent "upcasting" mixed types by casting to object
+        .astype("O").apply(
+            lambda row: _get_bucket_number(bucketing_info[1], [row[col_name] for col_name in bucketing_info[0]]),
+            axis="columns",
         )
-    elif isinstance(path, list):
-        if last_modified_begin or last_modified_end:
-            raise exceptions.InvalidArgumentCombination(
-                "Specify a list of files or (last_modified_begin and last_modified_end)"
-            )
-        paths = path if _suffix is None else [x for x in path if x.endswith(tuple(_suffix))]
-        paths = path if _ignore_suffix is None else [x for x in paths if x.endswith(tuple(_ignore_suffix)) is False]
-    else:
-        raise exceptions.InvalidArgumentType(f"{type(path)} is not a valid path type. Please, use str or List[str].")
-    return paths
+    )
+    return bucket_number_series.astype(pd.CategoricalDtype(range(bucketing_info[1])))
 
 
-def _validate_datetimes(
-    last_modified_begin: Optional[datetime.datetime] = None, last_modified_end: Optional[datetime.datetime] = None
-) -> None:
-    if (last_modified_begin is not None) and (last_modified_begin.tzinfo is None):
-        raise exceptions.InvalidArgumentValue("Timezone is not defined for last_modified_begin.")
-    if (last_modified_end is not None) and (last_modified_end.tzinfo is None):
-        raise exceptions.InvalidArgumentValue("Timezone is not defined for last_modified_end.")
-    if (last_modified_begin is not None) and (last_modified_end is not None):
-        if last_modified_begin > last_modified_end:
-            raise exceptions.InvalidArgumentValue("last_modified_begin is bigger than last_modified_end.")
-
-
-def _prefix_cleanup(prefix: str) -> str:
-    for n, c in enumerate(prefix):
-        if c in ["*", "?", "["]:
-            return prefix[:n]
-    return prefix
+def _simulate_overflow(value: int, bits: int = 31, signed: bool = False) -> int:
+    base = 1 << bits
+    value %= base
+    return value - base if signed and value.bit_length() == bits else value
+
+
+def _get_bucket_number(number_of_buckets: int, values: List[Union[str, int, bool]]) -> int:
+    hash_code = 0
+    for value in values:
+        hash_code = 31 * hash_code + _get_value_hash(value)
+        hash_code = _simulate_overflow(hash_code)
+
+    return hash_code % number_of_buckets
+
+
+def _get_value_hash(value: Union[str, int, bool]) -> int:
+    if isinstance(value, (int, np.int_)):
+        value = int(value)
+        bigint_min, bigint_max = -(2**63), 2**63 - 1
+        int_min, int_max = -(2**31), 2**31 - 1
+        if not bigint_min <= value <= bigint_max:
+            raise ValueError(f"{value} exceeds the range that Athena cannot handle as bigint.")
+        if not int_min <= value <= int_max:
+            value = (value >> 32) ^ value
+        if value < 0:
+            return -value - 1
+        return int(value)
+    if isinstance(value, (str, np.str_)):
+        value_hash = 0
+        for byte in value.encode():
+            value_hash = value_hash * 31 + byte
+            value_hash = _simulate_overflow(value_hash)
+        return value_hash
+    if isinstance(value, (bool, np.bool_)):
+        return int(value)
 
+    raise exceptions.InvalidDataFrame(
+        "Column specified for bucketing contains invalid data type. Only string, int and bool are supported."
+    )
 
-def _list_objects(  # pylint: disable=too-many-branches
-    path: str,
-    s3_additional_kwargs: Optional[Dict[str, Any]],
-    delimiter: Optional[str] = None,
-    suffix: Union[str, List[str], None] = None,
-    ignore_suffix: Union[str, List[str], None] = None,
-    last_modified_begin: Optional[datetime.datetime] = None,
-    last_modified_end: Optional[datetime.datetime] = None,
+
+def _get_subgroup_prefix(keys: Tuple[str, None], partition_cols: List[str], path_root: str) -> str:
+    subdir = "/".join([f"{name}={val}" for name, val in zip(partition_cols, keys)])
+    return f"{path_root}{subdir}/"
+
+
+def _delete_objects(
+    keys: Tuple[str, None],
+    path_root: str,
+    use_threads: Union[bool, int],
+    mode: str,
+    partition_cols: List[str],
+    partitions_types: Optional[Dict[str, str]],
+    catalog_id: Optional[str],
+    database: Optional[str],
+    table: Optional[str],
+    table_type: Optional[str],
+    transaction_id: Optional[str],
     boto3_session: Optional[boto3.Session] = None,
-    ignore_empty: bool = False,
-) -> Iterator[List[str]]:
-    bucket: str
-    prefix_original: str
-    bucket, prefix_original = _utils.parse_path(path=path)
-    prefix: str = _prefix_cleanup(prefix=prefix_original)
-    _suffix: Union[List[str], None] = [suffix] if isinstance(suffix, str) else suffix
-    _ignore_suffix: Union[List[str], None] = [ignore_suffix] if isinstance(ignore_suffix, str) else ignore_suffix
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-    default_pagination: Dict[str, int] = {"PageSize": 1000}
-    extra_kwargs: Dict[str, Any] = {"PaginationConfig": default_pagination}
-    if s3_additional_kwargs:
-        extra_kwargs = _fs.get_botocore_valid_kwargs(
-            function_name="list_objects_v2", s3_additional_kwargs=s3_additional_kwargs
-        )
-        extra_kwargs["PaginationConfig"] = (
-            s3_additional_kwargs["PaginationConfig"]
-            if "PaginationConfig" in s3_additional_kwargs
-            else default_pagination
+    **func_kwargs: Any,
+) -> str:
+    # Keys are either a primitive type or a tuple if partitioning by multiple cols
+    keys = (keys,) if not isinstance(keys, tuple) else keys
+    prefix = _get_subgroup_prefix(keys, partition_cols, path_root)
+    if mode == "overwrite_partitions":
+        if (table_type == "GOVERNED") and (table is not None) and (database is not None):
+            transaction_id = cast(str, transaction_id)
+            del_objects: List[Dict[str, Any]] = lakeformation._get_table_objects(  # pylint: disable=protected-access
+                catalog_id=catalog_id,
+                database=database,
+                table=table,
+                transaction_id=transaction_id,
+                partition_cols=partition_cols,
+                partitions_values=keys,  # type: ignore[arg-type]
+                partitions_types=partitions_types,
+                boto3_session=boto3_session,
+            )
+            if del_objects:
+                lakeformation._update_table_objects(  # pylint: disable=protected-access
+                    catalog_id=catalog_id,
+                    database=database,
+                    table=table,
+                    transaction_id=transaction_id,
+                    del_objects=del_objects,
+                    boto3_session=boto3_session,
+                )
+        else:
+            delete_objects(
+                path=prefix,
+                use_threads=use_threads,
+                boto3_session=boto3_session,
+                s3_additional_kwargs=func_kwargs.get("s3_additional_kwargs"),
+            )
+    return prefix
+
+
+@engine.dispatch_on_engine
+def _to_partitions(
+    df: pd.DataFrame,
+    func: Callable[..., List[str]],
+    concurrent_partitioning: bool,
+    path_root: str,
+    use_threads: Union[bool, int],
+    mode: str,
+    partition_cols: List[str],
+    partitions_types: Optional[Dict[str, str]],
+    catalog_id: Optional[str],
+    database: Optional[str],
+    table: Optional[str],
+    table_type: Optional[str],
+    transaction_id: Optional[str],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
+    filename_prefix: str,
+    boto3_session: Optional[boto3.Session],
+    **func_kwargs: Any,
+) -> Tuple[List[str], Dict[str, List[str]]]:
+    partitions_values: Dict[str, List[str]] = {}
+    proxy: _WriteProxy = _WriteProxy(use_threads=concurrent_partitioning)
+    s3_client = client(service_name="s3", session=boto3_session)
+    for keys, subgroup in df.groupby(by=partition_cols, observed=True):
+        # Keys are either a primitive type or a tuple if partitioning by multiple cols
+        keys = (keys,) if not isinstance(keys, tuple) else keys
+        subgroup = subgroup.drop(partition_cols, axis="columns")
+        prefix = _delete_objects(
+            keys=keys,
+            path_root=path_root,
+            use_threads=use_threads,
+            mode=mode,
+            partition_cols=partition_cols,
+            partitions_types=partitions_types,
+            catalog_id=catalog_id,
+            database=database,
+            table=table,
+            table_type=table_type,
+            transaction_id=transaction_id,
+            boto3_session=boto3_session,
+            **func_kwargs,
         )
-    paginator = client_s3.get_paginator("list_objects_v2")
-    args: Dict[str, Any] = {"Bucket": bucket, "Prefix": prefix, **extra_kwargs}
-    if delimiter is not None:
-        args["Delimiter"] = delimiter
-    _logger.debug("args: %s", args)
-    response_iterator = paginator.paginate(**args)
-    paths: List[str] = []
-    _validate_datetimes(last_modified_begin=last_modified_begin, last_modified_end=last_modified_end)
-
-    for page in response_iterator:  # pylint: disable=too-many-nested-blocks
-        if delimiter is None:
-            contents: Optional[List[Dict[str, Any]]] = page.get("Contents")
-            if contents is not None:
-                for content in contents:
-                    key: str = content["Key"]
-                    if ignore_empty and content.get("Size", 0) == 0:
-                        _logger.debug("Skipping empty file: %s", f"s3://{bucket}/{key}")
-                    elif (content is not None) and ("Key" in content):
-                        if (_suffix is None) or key.endswith(tuple(_suffix)):
-                            if last_modified_begin is not None:
-                                if content["LastModified"] < last_modified_begin:
-                                    continue
-                            if last_modified_end is not None:
-                                if content["LastModified"] > last_modified_end:
-                                    continue
-                            paths.append(f"s3://{bucket}/{key}")
+        if bucketing_info:
+            _to_buckets(
+                subgroup,
+                func=func,
+                path_root=prefix,
+                bucketing_info=bucketing_info,
+                boto3_session=boto3_session,
+                use_threads=use_threads,
+                proxy=proxy,
+                filename_prefix=filename_prefix,
+                **func_kwargs,
+            )
         else:
-            prefixes: Optional[List[Optional[Dict[str, str]]]] = page.get("CommonPrefixes")
-            if prefixes is not None:
-                for pfx in prefixes:
-                    if (pfx is not None) and ("Prefix" in pfx):
-                        key = pfx["Prefix"]
-                        paths.append(f"s3://{bucket}/{key}")
-
-        if prefix != prefix_original:
-            paths = fnmatch.filter(paths, path)
-
-        if _ignore_suffix is not None:
-            paths = [p for p in paths if p.endswith(tuple(_ignore_suffix)) is False]
-
-        if paths:
-            yield paths
-        paths = []
-
-
-def does_object_exist(
-    path: str,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-    boto3_session: Optional[boto3.Session] = None,
-    version_id: Optional[str] = None,
-) -> bool:
-    """Check if object exists on S3.
-
-    Parameters
-    ----------
-    path: str
-        S3 path (e.g. s3://bucket/key).
-    s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forwarded to botocore requests.
-        e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    version_id: str, optional
-        Specific version of the object that should exist.
-
-    Returns
-    -------
-    bool
-        True if exists, False otherwise.
-
-    Examples
-    --------
-    Using the default boto3 session
-
-    >>> import awswrangler as wr
-    >>> wr.s3.does_object_exist('s3://bucket/key_real')
-    True
-    >>> wr.s3.does_object_exist('s3://bucket/key_unreal')
-    False
-
-    Using a custom boto3 session
-
-    >>> import boto3
-    >>> import awswrangler as wr
-    >>> wr.s3.does_object_exist('s3://bucket/key_real', boto3_session=boto3.Session())
-    True
-    >>> wr.s3.does_object_exist('s3://bucket/key_unreal', boto3_session=boto3.Session())
-    False
-
-    """
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-    bucket: str
-    key: str
-    bucket, key = _utils.parse_path(path=path)
-    if s3_additional_kwargs:
-        extra_kwargs: Dict[str, Any] = _fs.get_botocore_valid_kwargs(
-            function_name="head_object", s3_additional_kwargs=s3_additional_kwargs
+            proxy.write(
+                func,
+                subgroup,
+                path_root=prefix,
+                filename_prefix=filename_prefix,
+                s3_client=s3_client,
+                use_threads=use_threads,
+                **func_kwargs,
+            )
+        partitions_values[prefix] = [str(k) for k in keys]
+    paths: List[str] = proxy.close()  # blocking
+    return paths, partitions_values
+
+
+@engine.dispatch_on_engine
+def _to_buckets(
+    df: pd.DataFrame,
+    func: Callable[..., List[str]],
+    path_root: str,
+    bucketing_info: typing.BucketingInfoTuple,
+    filename_prefix: str,
+    boto3_session: Optional[boto3.Session],
+    use_threads: Union[bool, int],
+    proxy: Optional[_WriteProxy] = None,
+    **func_kwargs: Any,
+) -> List[str]:
+    _proxy: _WriteProxy = proxy if proxy else _WriteProxy(use_threads=False)
+    s3_client = client(service_name="s3", session=boto3_session)
+    for bucket_number, subgroup in df.groupby(by=_get_bucketing_series(df=df, bucketing_info=bucketing_info)):
+        _proxy.write(
+            func,
+            subgroup,
+            path_root=path_root,
+            filename_prefix=f"{filename_prefix}_bucket-{bucket_number:05d}",
+            use_threads=use_threads,
+            s3_client=s3_client,
+            **func_kwargs,
         )
-    else:
-        extra_kwargs = {}
-    try:
-        if version_id:
-            extra_kwargs["VersionId"] = version_id
-        client_s3.head_object(Bucket=bucket, Key=key, **extra_kwargs)
-        return True
-    except botocore.exceptions.ClientError as ex:
-        if ex.response["ResponseMetadata"]["HTTPStatusCode"] == 404:
-            return False
-        raise ex
-
-
-def list_directories(
-    path: str,
-    chunked: bool = False,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-    boto3_session: Optional[boto3.Session] = None,
-) -> Union[List[str], Iterator[List[str]]]:
-    """List Amazon S3 objects from a prefix.
+    if proxy:
+        return []
+    paths: List[str] = _proxy.close()  # blocking
+    return paths
 
-    This function accepts Unix shell-style wildcards in the path argument.
-    * (matches everything), ? (matches any single character),
-    [seq] (matches any character in seq), [!seq] (matches any character not in seq).
-    If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
-    you can use `glob.escape(path)` before passing the path to this function.
-
-    Parameters
-    ----------
-    path : str
-        S3 path (e.g. s3://bucket/prefix).
-    chunked: bool
-        If True returns iterator, and a single list otherwise. False by default.
-    s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forwarded to botocore requests.
-        e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-
-    Returns
-    -------
-    Union[List[str], Iterator[List[str]]]
-        List of objects paths.
-
-    Examples
-    --------
-    Using the default boto3 session
-
-    >>> import awswrangler as wr
-    >>> wr.s3.list_directories('s3://bucket/prefix/')
-    ['s3://bucket/prefix/dir0/', 's3://bucket/prefix/dir1/', 's3://bucket/prefix/dir2/']
-
-    Using a custom boto3 session
-
-    >>> import boto3
-    >>> import awswrangler as wr
-    >>> wr.s3.list_directories('s3://bucket/prefix/', boto3_session=boto3.Session())
-    ['s3://bucket/prefix/dir0/', 's3://bucket/prefix/dir1/', 's3://bucket/prefix/dir2/']
-
-    """
-    result_iterator = _list_objects(
-        path=path,
-        delimiter="/",
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-    )
-    if chunked:
-        return result_iterator
-    return [path for paths in result_iterator for path in paths]
 
+def _to_dataset(
+    func: Callable[..., List[str]],
+    concurrent_partitioning: bool,
+    df: pd.DataFrame,
+    path_root: str,
+    filename_prefix: str,
+    index: bool,
+    use_threads: Union[bool, int],
+    mode: str,
+    partition_cols: Optional[List[str]],
+    partitions_types: Optional[Dict[str, str]],
+    catalog_id: Optional[str],
+    database: Optional[str],
+    table: Optional[str],
+    table_type: Optional[str],
+    transaction_id: Optional[str],
+    bucketing_info: Optional[typing.BucketingInfoTuple],
+    boto3_session: Optional[boto3.Session],
+    **func_kwargs: Any,
+) -> Tuple[List[str], Dict[str, List[str]]]:
+    path_root = path_root if path_root.endswith("/") else f"{path_root}/"
+    # Evaluate mode
+    if mode not in ["append", "overwrite", "overwrite_partitions"]:
+        raise exceptions.InvalidArgumentValue(
+            f"{mode} is a invalid mode, please use append, overwrite or overwrite_partitions."
+        )
+    if (mode == "overwrite") or ((mode == "overwrite_partitions") and (not partition_cols)):
+        if (table_type == "GOVERNED") and (table is not None) and (database is not None):
+            transaction_id = cast(str, transaction_id)
+            del_objects: List[Dict[str, Any]] = lakeformation._get_table_objects(  # pylint: disable=protected-access
+                catalog_id=catalog_id,
+                database=database,
+                table=table,
+                transaction_id=transaction_id,
+                boto3_session=boto3_session,
+            )
+            if del_objects:
+                lakeformation._update_table_objects(  # pylint: disable=protected-access
+                    catalog_id=catalog_id,
+                    database=database,
+                    table=table,
+                    transaction_id=transaction_id,
+                    del_objects=del_objects,
+                    boto3_session=boto3_session,
+                )
+        else:
+            delete_objects(path=path_root, use_threads=use_threads, boto3_session=boto3_session)
 
-def list_objects(
-    path: str,
-    suffix: Union[str, List[str], None] = None,
-    ignore_suffix: Union[str, List[str], None] = None,
-    last_modified_begin: Optional[datetime.datetime] = None,
-    last_modified_end: Optional[datetime.datetime] = None,
-    ignore_empty: bool = False,
-    chunked: bool = False,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-    boto3_session: Optional[boto3.Session] = None,
-) -> Union[List[str], Iterator[List[str]]]:
-    """List Amazon S3 objects from a prefix.
+    # Writing
+    partitions_values: Dict[str, List[str]] = {}
+    paths: List[str]
+    if partition_cols:
+        paths, partitions_values = _to_partitions(
+            df,
+            func=func,
+            concurrent_partitioning=concurrent_partitioning,
+            path_root=path_root,
+            use_threads=use_threads,
+            mode=mode,
+            catalog_id=catalog_id,
+            database=database,
+            table=table,
+            table_type=table_type,
+            transaction_id=transaction_id,
+            bucketing_info=bucketing_info,
+            filename_prefix=filename_prefix,
+            partition_cols=partition_cols,
+            partitions_types=partitions_types,
+            boto3_session=boto3_session,
+            index=index,
+            **func_kwargs,
+        )
+    elif bucketing_info:
+        paths = _to_buckets(
+            df,
+            func=func,
+            path_root=path_root,
+            use_threads=use_threads,
+            bucketing_info=bucketing_info,
+            filename_prefix=filename_prefix,
+            boto3_session=boto3_session,
+            index=index,
+            **func_kwargs,
+        )
+    else:
+        s3_client = client(service_name="s3", session=boto3_session)
+        paths = func(
+            df,
+            path_root=path_root,
+            filename_prefix=filename_prefix,
+            use_threads=use_threads,
+            index=index,
+            s3_client=s3_client,
+            **func_kwargs,
+        )
+    _logger.debug("paths: %s", paths)
+    _logger.debug("partitions_values: %s", partitions_values)
+    if (table_type == "GOVERNED") and (table is not None) and (database is not None):
+        list_add_objects: List[
+            List[Dict[str, Any]]
+        ] = lakeformation._build_table_objects(  # pylint: disable=protected-access
+            paths, partitions_values, use_threads=use_threads, boto3_session=boto3_session
+        )
+        try:
+            if list_add_objects:
+                for add_objects in list_add_objects:
+                    lakeformation._update_table_objects(  # pylint: disable=protected-access
+                        catalog_id=catalog_id,
+                        database=database,
+                        table=table,
+                        transaction_id=transaction_id,  # type: ignore[arg-type]
+                        add_objects=add_objects,
+                        boto3_session=boto3_session,
+                    )
+        except Exception as ex:
+            _logger.error(ex)
+            raise
 
-    This function accepts Unix shell-style wildcards in the path argument.
-    * (matches everything), ? (matches any single character),
-    [seq] (matches any character in seq), [!seq] (matches any character not in seq).
-    If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
-    you can use `glob.escape(path)` before passing the path to this function.
-
-    Note
-    ----
-    The filter by last_modified begin last_modified end is applied after list all S3 files
-
-    Parameters
-    ----------
-    path : str
-        S3 path (e.g. s3://bucket/prefix).
-    suffix: Union[str, List[str], None]
-        Suffix or List of suffixes for filtering S3 keys.
-    ignore_suffix: Union[str, List[str], None]
-        Suffix or List of suffixes for S3 keys to be ignored.
-    last_modified_begin
-        Filter the s3 files by the Last modified date of the object.
-        The filter is applied only after list all s3 files.
-    last_modified_end: datetime, optional
-        Filter the s3 files by the Last modified date of the object.
-        The filter is applied only after list all s3 files.
-    ignore_empty: bool
-        Ignore files with 0 bytes.
-    chunked: bool
-        If True returns iterator, and a single list otherwise. False by default.
-    s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forwarded to botocore requests.
-        e.g. s3_additional_kwargs={'RequestPayer': 'requester'}
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-
-    Returns
-    -------
-    Union[List[str], Iterator[List[str]]]
-        List of objects paths.
-
-    Examples
-    --------
-    Using the default boto3 session
-
-    >>> import awswrangler as wr
-    >>> wr.s3.list_objects('s3://bucket/prefix')
-    ['s3://bucket/prefix0', 's3://bucket/prefix1', 's3://bucket/prefix2']
-
-    Using a custom boto3 session
-
-    >>> import boto3
-    >>> import awswrangler as wr
-    >>> wr.s3.list_objects('s3://bucket/prefix', boto3_session=boto3.Session())
-    ['s3://bucket/prefix0', 's3://bucket/prefix1', 's3://bucket/prefix2']
-
-    """
-    # On top of user provided ignore_suffix input, add "/"
-    ignore_suffix_acc = set("/")
-    if isinstance(ignore_suffix, str):
-        ignore_suffix_acc.add(ignore_suffix)
-    elif isinstance(ignore_suffix, list):
-        ignore_suffix_acc.update(ignore_suffix)
-
-    result_iterator = _list_objects(
-        path=path,
-        delimiter=None,
-        suffix=suffix,
-        ignore_suffix=list(ignore_suffix_acc),
-        boto3_session=boto3_session,
-        last_modified_begin=last_modified_begin,
-        last_modified_end=last_modified_end,
-        ignore_empty=ignore_empty,
-        s3_additional_kwargs=s3_additional_kwargs,
-    )
-    if chunked:
-        return result_iterator
-    return [path for paths in result_iterator for path in paths]
-
-
-def list_buckets(boto3_session: Optional[boto3.Session] = None) -> List[str]:
-    """List Amazon S3 buckets.
-
-    Parameters
-    ----------
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session to use, default to None.
-
-    Returns
-    -------
-    List[str]
-        List of bucket names.
-
-    """
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-    buckets = client_s3.list_buckets()["Buckets"]
-    return [bucket["Name"] for bucket in buckets]
+    return paths, partitions_values
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_list.pyi` & `awswrangler-3.0.0rc3/awswrangler/s3/_list.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 import datetime
-from typing import Any, Dict, Iterator, List, Literal, Optional, Sequence, Union, overload
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Optional, Sequence, Union, overload
 
 import boto3
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 def _path2list(
     path: Union[str, Sequence[str]],
-    boto3_session: boto3.Session,
+    s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     last_modified_begin: Optional[datetime.datetime] = ...,
     last_modified_end: Optional[datetime.datetime] = ...,
     suffix: Union[str, List[str], None] = ...,
     ignore_suffix: Union[str, List[str], None] = ...,
     ignore_empty: bool = ...,
 ) -> List[str]: ...
 def _prefix_cleanup(prefix: str) -> str: ...
+def _list_objects_paginate(  # pylint: disable=too-many-branches
+    bucket: str,
+    pattern: str,
+    prefix: str,
+    s3_client: "S3Client",
+    delimiter: Optional[str],
+    s3_additional_kwargs: Optional[Dict[str, Any]],
+    suffix: Union[List[str], None],
+    ignore_suffix: Union[List[str], None],
+    last_modified_begin: Optional[datetime.datetime],
+    last_modified_end: Optional[datetime.datetime],
+    ignore_empty: bool,
+) -> Iterator[List[str]]: ...
 def does_object_exist(
     path: str,
     s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
     boto3_session: Optional[boto3.Session] = ...,
     version_id: Optional[str] = ...,
 ) -> bool: ...
 def list_buckets(boto3_session: Optional[boto3.Session] = ...) -> List[str]: ...
@@ -49,31 +65,46 @@
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> Union[List[str], Iterator[List[str]]]: ...
 @overload
 def list_objects(
     path: str,
     chunked: Literal[False],
+    ignore_suffix: Union[str, List[str], None] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> List[str]: ...
 @overload
 def list_objects(
     path: str,
-    *,
+    ignore_suffix: Union[str, List[str], None] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> List[str]: ...
 @overload
 def list_objects(
     path: str,
     chunked: Literal[True],
+    ignore_suffix: Union[str, List[str], None] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> Iterator[List[str]]: ...
 @overload
 def list_objects(
     path: str,
     chunked: bool,
+    ignore_suffix: Union[str, List[str], None] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    ignore_empty: bool = ...,
     s3_additional_kwargs: Union[Dict[str, Any], Dict[str, str], None] = ...,
     boto3_session: Optional[boto3.Session] = ...,
 ) -> Union[List[str], Iterator[List[str]]]: ...
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_read.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_read.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Amazon S3 Read Module (PRIVATE)."""
 
-import concurrent.futures
 import logging
-from functools import partial
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union, cast
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Set, Tuple, Union, cast
 
 import numpy as np
 import pandas as pd
 from pandas.api.types import union_categoricals
 
 from awswrangler import exceptions
 from awswrangler._arrow import _extract_partitions_from_path
-from awswrangler._utils import boto3_to_primitives, ensure_cpu_count
 from awswrangler.s3._list import _prefix_cleanup
 
+if TYPE_CHECKING:
+    from mypy_boto3_glue.type_defs import GetTableResponseTypeDef
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _get_path_root(path: Union[str, List[str]], dataset: bool) -> Optional[str]:
     if (dataset is True) and (not isinstance(path, str)):
         raise exceptions.InvalidArgument("The path argument must be a string if dataset=True (Amazon S3 prefix).")
     return _prefix_cleanup(str(path)) if dataset is True else None
@@ -41,18 +41,18 @@
     partitions_types: Dict[str, str] = {}
     partitions_values: Dict[str, List[str]] = {}
     for p in paths:
         if path not in p:
             raise exceptions.InvalidArgumentValue(f"Object {p} is not under the root path ({path}).")
         path_wo_filename: str = p.rpartition("/")[0] + "/"
         if path_wo_filename not in partitions_values:
-            path_wo_prefix: str = path_wo_filename.replace(f"{path}/", "")
-            dirs: Tuple[str, ...] = tuple(x for x in path_wo_prefix.split("/") if (x != "") and (x.count("=") == 1))
+            path_wo_prefix: str = path_wo_filename.replace(f"{path}", "")
+            dirs: Tuple[str, ...] = tuple(x for x in path_wo_prefix.split("/") if (x != "") and (x.count("=") > 0))
             if dirs:
-                values_tups = cast(Tuple[Tuple[str, str]], tuple(tuple(x.split("=")[:2]) for x in dirs))
+                values_tups = cast(Tuple[Tuple[str, str]], tuple(tuple(x.split("=", maxsplit=1)[:2]) for x in dirs))
                 values_dics: Dict[str, str] = dict(values_tups)
                 p_values: List[str] = list(values_dics.values())
                 p_types: Dict[str, str] = {x: "string" for x in values_dics.keys()}
                 if not partitions_types:
                     partitions_types = p_types
                 if p_values:
                     partitions_types = p_types
@@ -84,54 +84,35 @@
     count: int = len(df.index)
     _logger.debug("count: %s", count)
     for name, value in partitions.items():
         df[name] = pd.Categorical.from_codes(np.repeat([0], count), categories=[value])
     return df
 
 
-def _extract_partitions_dtypes_from_table_details(response: Dict[str, Any]) -> Dict[str, str]:
+def _extract_partitions_dtypes_from_table_details(response: "GetTableResponseTypeDef") -> Dict[str, str]:
     dtypes: Dict[str, str] = {}
-    if "PartitionKeys" in response["Table"]:
-        for par in response["Table"]["PartitionKeys"]:
-            dtypes[par["Name"]] = par["Type"]
+    for par in response["Table"].get("PartitionKeys", []):
+        dtypes[par["Name"]] = par["Type"]
     return dtypes
 
 
-def _union(dfs: List[pd.DataFrame], ignore_index: Optional[bool]) -> pd.DataFrame:
-    if ignore_index is None:
-        ignore_index = False
-        for df in dfs:
-            if hasattr(df, "_awswrangler_ignore_index"):
-                if df._awswrangler_ignore_index is True:  # pylint: disable=protected-access
-                    ignore_index = True
-                    break
+def _union(dfs: List[pd.DataFrame], ignore_index: bool) -> pd.DataFrame:
     cats: Tuple[Set[str], ...] = tuple(set(df.select_dtypes(include="category").columns) for df in dfs)
     for col in set.intersection(*cats):
         cat = union_categoricals([df[col] for df in dfs])
         for df in dfs:
             df[col] = pd.Categorical(df[col].values, categories=cat.categories)
     return pd.concat(objs=dfs, sort=False, copy=False, ignore_index=ignore_index)
 
 
-def _read_dfs_from_multiple_paths(
-    read_func: Callable[..., pd.DataFrame],
-    paths: List[str],
-    version_ids: Optional[Dict[str, str]],
-    use_threads: Union[bool, int],
-    kwargs: Dict[str, Any],
-) -> List[pd.DataFrame]:
-    cpus = ensure_cpu_count(use_threads)
-    if cpus < 2:
-        return [
-            read_func(
-                path,
-                version_id=version_ids.get(path) if version_ids else None,
-                **kwargs,
-            )
-            for path in paths
-        ]
-
-    with concurrent.futures.ThreadPoolExecutor(max_workers=ensure_cpu_count(use_threads)) as executor:
-        kwargs["boto3_session"] = boto3_to_primitives(kwargs["boto3_session"])
-        partial_read_func = partial(read_func, **kwargs)
-        versions = [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths]
-        return list(df for df in executor.map(partial_read_func, paths, versions))
+def _check_version_id(
+    paths: List[str], version_id: Optional[Union[str, Dict[str, str]]] = None
+) -> Optional[Dict[str, str]]:
+    if len(paths) > 1 and version_id is not None and not isinstance(version_id, dict):
+        raise exceptions.InvalidArgumentCombination(
+            "If multiple paths are provided along with a file version ID, the version ID parameter must be a dict."
+        )
+    if isinstance(version_id, dict) and not all(version_id.values()):
+        raise exceptions.InvalidArgumentValue("Values in version ID dict cannot be None.")
+    return (
+        version_id if isinstance(version_id, dict) else {paths[0]: version_id} if isinstance(version_id, str) else None
+    )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_read_excel.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_read_excel.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 
 import boto3
 import pandas as pd
 
 from awswrangler import _utils, exceptions
 from awswrangler.s3._fs import open_s3_object
 
+openpyxl = _utils.import_optional_dependency("openpyxl")
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+@_utils.check_optional_dependency(openpyxl, "openpyxl")
 def read_excel(
     path: str,
     version_id: Optional[str] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     **pandas_kwargs: Any,
@@ -26,15 +29,15 @@
     ----
     This function accepts any Pandas's read_excel() argument.
     https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_excel.html
 
     Note
     ----
     Depending on the file extension ('xlsx', 'xls', 'odf'...), an additional library
-    might have to be installed first (e.g. xlrd).
+    might have to be installed first.
 
     Note
     ----
     In case of `use_threads=True` the number of threads
     that will be spawned will be gotten from os.cpu_count().
 
     Parameters
@@ -73,19 +76,18 @@
     """
     if "pandas_kwargs" in pandas_kwargs:
         raise exceptions.InvalidArgument(
             "You can NOT pass `pandas_kwargs` explicit, just add valid "
             "Pandas arguments in the function call and awswrangler will accept it."
             "e.g. wr.s3.read_excel('s3://bucket/key.xlsx', na_rep='', verbose=True)"
         )
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     with open_s3_object(
         path=path,
         mode="rb",
         version_id=version_id,
         use_threads=use_threads,
         s3_block_size=-1,  # One shot download
         s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=session,
+        boto3_session=boto3_session,
     ) as f:
         _logger.debug("pandas_kwargs: %s", pandas_kwargs)
         return pd.read_excel(f, **pandas_kwargs)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_read_parquet.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_write_parquet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,845 +1,1026 @@
-"""Amazon S3 Read PARQUET Module (PRIVATE)."""
+"""Amazon PARQUET S3 Parquet Write Module (PRIVATE)."""
 
-import datetime
-import functools
-import itertools
 import logging
-from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Tuple, Union
+import math
+import uuid
+from contextlib import contextmanager
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Union, cast
 
 import boto3
 import pandas as pd
 import pyarrow as pa
-import pyarrow.dataset
+import pyarrow.lib
 import pyarrow.parquet
 
-from awswrangler import _data_types, _utils, exceptions
-from awswrangler._arrow import _add_table_partitions, _table_to_df
+from awswrangler import _data_types, _utils, catalog, exceptions, lakeformation, typing
+from awswrangler._arrow import _df_to_table
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
-from awswrangler.catalog._get import _get_partitions
-from awswrangler.catalog._utils import _catalog_id
-from awswrangler.distributed.ray import ray_get
+from awswrangler._utils import copy_df_shallow
+from awswrangler.s3._delete import delete_objects
 from awswrangler.s3._fs import open_s3_object
-from awswrangler.s3._list import _path2list
-from awswrangler.s3._read import (
-    _apply_partition_filter,
-    _extract_partitions_dtypes_from_table_details,
-    _extract_partitions_metadata_from_paths,
-    _get_path_ignore_suffix,
-    _get_path_root,
-)
+from awswrangler.s3._read_parquet import _read_parquet_metadata
+from awswrangler.s3._write import _COMPRESSION_2_EXT, _apply_dtype, _sanitize, _validate_args
+from awswrangler.s3._write_concurrent import _WriteProxy
+from awswrangler.s3._write_dataset import _to_dataset
+from awswrangler.typing import BucketingInfoTuple, GlueTableSettings, _S3WriteDataReturnValue
 
-BATCH_READ_BLOCK_SIZE = 65_536
-CHUNKED_READ_S3_BLOCK_SIZE = 10_485_760  # 10 MB (20 * 2**20)
-FULL_READ_S3_BLOCK_SIZE = 20_971_520  # 20 MB (20 * 2**20)
-METADATA_READ_S3_BLOCK_SIZE = 131_072  # 128 KB (128 * 2**10)
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _ensure_locations_are_valid(paths: Iterable[str]) -> Iterator[str]:
-    for path in paths:
-        suffix: str = path.rpartition("/")[2]
-        # If the suffix looks like a partition,
-        if (suffix != "") and (suffix.count("=") == 1):
-            # the path should end in a '/' character.
-            path = f"{path}/"
-        yield path
-
-
-def _pyarrow_parquet_file_wrapper(
-    source: Any, coerce_int96_timestamp_unit: Optional[str] = None
-) -> pyarrow.parquet.ParquetFile:
-    try:
-        return pyarrow.parquet.ParquetFile(source=source, coerce_int96_timestamp_unit=coerce_int96_timestamp_unit)
-    except pyarrow.ArrowInvalid as ex:
-        if str(ex) == "Parquet file size is 0 bytes":
-            _logger.warning("Ignoring empty file...")
-            return None
-        raise
-
-
-@engine.dispatch_on_engine
-def _read_parquet_metadata_file(
-    boto3_session: boto3.Session,
-    path: str,
+def _get_file_path(
+    path_root: Optional[str] = None,
+    path: Optional[str] = None,
+    filename_prefix: Optional[str] = None,
+    compression_ext: str = "",
+    bucket_id: Optional[int] = None,
+    extension: str = ".parquet",
+) -> str:
+    if bucket_id is not None:
+        filename_prefix = f"{filename_prefix}_bucket-{bucket_id:05d}"
+    if path is None and path_root is not None:
+        file_path: str = f"{path_root}{filename_prefix}{compression_ext}{extension}"
+    elif path is not None and path_root is None:
+        file_path = path
+    else:
+        raise RuntimeError("path and path_root received at the same time.")
+    return file_path
+
+
+def _get_chunk_file_path(file_counter: int, file_path: str) -> str:
+    slash_index: int = file_path.rfind("/")
+    dot_index: int = file_path.find(".", slash_index)
+    file_index: str = "_" + str(file_counter)
+    if dot_index == -1:
+        file_path = file_path + file_index
+    else:
+        file_path = file_path[:dot_index] + file_index + file_path[dot_index:]
+    return file_path
+
+
+def _get_write_table_args(pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
+    write_table_args: Dict[str, Any] = {}
+    if pyarrow_additional_kwargs and "write_table_args" in pyarrow_additional_kwargs:
+        write_table_args = pyarrow_additional_kwargs.pop("write_table_args")
+    return write_table_args
+
+
+@contextmanager
+def _new_writer(
+    file_path: str,
+    compression: Optional[str],
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]],
+    schema: pa.Schema,
+    s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
-    version_id: Optional[str] = None,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-) -> pa.schema:
+) -> Iterator[pyarrow.parquet.ParquetWriter]:
+    writer: Optional[pyarrow.parquet.ParquetWriter] = None
+    if not pyarrow_additional_kwargs:
+        pyarrow_additional_kwargs = {}
+    if not pyarrow_additional_kwargs.get("coerce_timestamps"):
+        pyarrow_additional_kwargs["coerce_timestamps"] = "ms"
+    if "flavor" not in pyarrow_additional_kwargs:
+        pyarrow_additional_kwargs["flavor"] = "spark"
+    if "version" not in pyarrow_additional_kwargs:
+        # By default, use version 1.0 logical type set to maximize compatibility
+        pyarrow_additional_kwargs["version"] = "1.0"
+    if not pyarrow_additional_kwargs.get("use_dictionary"):
+        pyarrow_additional_kwargs["use_dictionary"] = True
+    if not pyarrow_additional_kwargs.get("write_statistics"):
+        pyarrow_additional_kwargs["write_statistics"] = True
+
     with open_s3_object(
-        path=path,
-        mode="rb",
-        version_id=version_id,
+        path=file_path,
+        mode="wb",
         use_threads=use_threads,
-        s3_block_size=METADATA_READ_S3_BLOCK_SIZE,
         s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
     ) as f:
-        pq_file: Optional[pyarrow.parquet.ParquetFile] = _pyarrow_parquet_file_wrapper(
-            source=f, coerce_int96_timestamp_unit=coerce_int96_timestamp_unit
-        )
-        if pq_file:
-            return pq_file.schema.to_arrow_schema()
-        return None
-
-
-def _read_schemas_from_files(
-    paths: List[str],
-    sampling: float,
-    use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    version_ids: Optional[Dict[str, str]] = None,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-) -> List[pa.schema]:
-    paths = _utils.list_sampling(lst=paths, sampling=sampling)
-
-    executor = _get_executor(use_threads=use_threads)
-    schemas = ray_get(
-        executor.map(
-            _read_parquet_metadata_file,
-            boto3_session,
-            paths,
-            itertools.repeat(s3_additional_kwargs),
-            itertools.repeat(use_threads),
-            [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
-            itertools.repeat(coerce_int96_timestamp_unit),
-        )
-    )
-    return [schema for schema in schemas if schema is not None]
-
-
-def _validate_schemas(schemas: List[pa.schema], validate_schema: bool) -> pa.schema:
-    first: pa.schema = schemas[0]
-    if len(schemas) == 1:
-        return first
-    first_dict = {s.name: s.type for s in first}
-    if validate_schema:
-        for schema in schemas[1:]:
-            if first_dict != {s.name: s.type for s in schema}:
-                raise exceptions.InvalidSchemaConvergence(
-                    f"At least 2 different schemas were detected:\n    1 - {first}\n    2 - {schema}."
-                )
-    return pa.unify_schemas(schemas)
+        try:
+            writer = pyarrow.parquet.ParquetWriter(
+                where=f,
+                compression="NONE" if compression is None else compression,
+                schema=schema,
+                **pyarrow_additional_kwargs,
+            )
+            yield writer
+        finally:
+            if writer is not None and writer.is_open is True:
+                writer.close()
 
 
-def _validate_schemas_from_files(
-    validate_schema: bool,
-    paths: List[str],
-    sampling: float,
-    use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
+def _write_chunk(
+    file_path: str,
+    s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
-    version_ids: Optional[Dict[str, str]] = None,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-) -> pa.schema:
-    schemas: List[pa.schema] = _read_schemas_from_files(
-        paths=paths,
-        sampling=sampling,
-        use_threads=use_threads,
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-        version_ids=version_ids,
-        coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-    )
-    return _validate_schemas(schemas, validate_schema)
-
-
-def _read_parquet_metadata(
-    path: Union[str, List[str]],
-    path_suffix: Optional[str],
-    path_ignore_suffix: Optional[str],
-    ignore_empty: bool,
-    ignore_null: bool,
-    dtype: Optional[Dict[str, str]],
-    sampling: float,
-    dataset: bool,
+    compression: Optional[str],
+    pyarrow_additional_kwargs: Dict[str, str],
+    table: pa.Table,
+    offset: int,
+    chunk_size: int,
     use_threads: Union[bool, int],
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    version_id: Optional[Union[str, Dict[str, str]]] = None,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-) -> Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]:
-    """Handle wr.s3.read_parquet_metadata internally."""
-    boto3_session = _utils.ensure_session(session=boto3_session)
-    path_root: Optional[str] = _get_path_root(path=path, dataset=dataset)
-    paths: List[str] = _path2list(
-        path=path,
-        boto3_session=boto3_session,
-        suffix=path_suffix,
-        ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=path_ignore_suffix),
-        ignore_empty=ignore_empty,
-        s3_additional_kwargs=s3_additional_kwargs,
-    )
-    version_ids = (
-        version_id if isinstance(version_id, dict) else {paths[0]: version_id} if isinstance(version_id, str) else None
-    )
-
-    # Files
-    schemas: List[pa.schema] = _read_schemas_from_files(
-        paths=paths,
-        sampling=sampling,
-        use_threads=use_threads,
-        boto3_session=boto3_session,
+) -> List[str]:
+    write_table_args = _get_write_table_args(pyarrow_additional_kwargs)
+    with _new_writer(
+        file_path=file_path,
+        compression=compression,
+        pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+        schema=table.schema,
+        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
-        version_ids=version_ids,
-        coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-    )
-    merged_schemas = _validate_schemas(schemas=schemas, validate_schema=False)
-
-    columns_types: Dict[str, str] = _data_types.athena_types_from_pyarrow_schema(
-        schema=merged_schemas, partitions=None, ignore_null=ignore_null
-    )[0]
-
-    # Partitions
-    partitions_types: Optional[Dict[str, str]] = None
-    partitions_values: Optional[Dict[str, List[str]]] = None
-    if (dataset is True) and (path_root is not None):
-        partitions_types, partitions_values = _extract_partitions_metadata_from_paths(path=path_root, paths=paths)
-
-    # Casting
-    if dtype:
-        for k, v in dtype.items():
-            if columns_types and k in columns_types:
-                columns_types[k] = v
-            if partitions_types and k in partitions_types:
-                partitions_types[k] = v
-
-    return columns_types, partitions_types, partitions_values
-
-
-def _read_parquet_file(
-    boto3_session: boto3.Session,
-    path: str,
-    path_root: Optional[str],
-    columns: Optional[List[str]],
-    coerce_int96_timestamp_unit: Optional[str],
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    use_threads: Union[bool, int],
-    version_id: Optional[str] = None,
-) -> pa.Table:
-    s3_block_size: int = FULL_READ_S3_BLOCK_SIZE if columns else -1  # One shot for a full read or see constant
-    with open_s3_object(
-        path=path,
-        mode="rb",
-        version_id=version_id,
         use_threads=use_threads,
-        s3_block_size=s3_block_size,
-        s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=boto3_session,
-    ) as f:
-        pq_file: Optional[pyarrow.parquet.ParquetFile] = _pyarrow_parquet_file_wrapper(
-            source=f,
-            coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-        )
-        if pq_file is None:
-            raise exceptions.InvalidFile(f"Invalid Parquet file: {path}")
-        return _add_table_partitions(
-            table=pq_file.read(columns=columns, use_threads=False, use_pandas_metadata=False),
-            path=path,
-            path_root=path_root,
-        )
+    ) as writer:
+        writer.write_table(table.slice(offset, chunk_size), **write_table_args)
+    return [file_path]
 
 
-def _read_parquet_chunked(
-    boto3_session: boto3.Session,
-    paths: List[str],
-    path_root: Optional[str],
-    columns: Optional[List[str]],
-    coerce_int96_timestamp_unit: Optional[str],
-    chunked: Union[int, bool],
-    use_threads: Union[bool, int],
+def _to_parquet_chunked(
+    file_path: str,
+    s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
-    arrow_kwargs: Dict[str, Any],
-    version_ids: Optional[Dict[str, str]] = None,
-) -> Iterator[pd.DataFrame]:
-    next_slice: Optional[pd.DataFrame] = None
-    batch_size = BATCH_READ_BLOCK_SIZE if chunked is True else chunked
-
-    for path in paths:
-        with open_s3_object(
-            path=path,
-            version_id=version_ids.get(path) if version_ids else None,
-            mode="rb",
-            use_threads=use_threads,
-            s3_block_size=CHUNKED_READ_S3_BLOCK_SIZE,
+    compression: Optional[str],
+    pyarrow_additional_kwargs: Dict[str, Any],
+    table: pa.Table,
+    max_rows_by_file: int,
+    num_of_rows: int,
+    cpus: int,
+) -> List[str]:
+    chunks: int = math.ceil(num_of_rows / max_rows_by_file)
+    use_threads: Union[bool, int] = cpus > 1
+    proxy: _WriteProxy = _WriteProxy(use_threads=use_threads)
+    for chunk in range(chunks):
+        offset: int = chunk * max_rows_by_file
+        write_path: str = _get_chunk_file_path(chunk, file_path)
+        proxy.write(
+            func=_write_chunk,
+            file_path=write_path,
+            s3_client=s3_client,
             s3_additional_kwargs=s3_additional_kwargs,
-            boto3_session=boto3_session,
-        ) as f:
-            pq_file: Optional[pyarrow.parquet.ParquetFile] = _pyarrow_parquet_file_wrapper(
-                source=f,
-                coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-            )
-            if pq_file is None:
-                continue
-
-            use_threads_flag: bool = use_threads if isinstance(use_threads, bool) else bool(use_threads > 1)
-            chunks = pq_file.iter_batches(
-                batch_size=batch_size, columns=columns, use_threads=use_threads_flag, use_pandas_metadata=False
-            )
-            table = _add_table_partitions(
-                table=pa.Table.from_batches(chunks),
-                path=path,
-                path_root=path_root,
-            )
-            df = _table_to_df(table=table, kwargs=arrow_kwargs)
-            if chunked is True:
-                yield df
-            else:
-                if next_slice is not None:
-                    df = pd.concat(objs=[next_slice, df], sort=False, copy=False)
-                while len(df.index) >= chunked:
-                    yield df.iloc[:chunked, :].copy()
-                    df = df.iloc[chunked:, :]
-                if df.empty:
-                    next_slice = None
-                else:
-                    next_slice = df
-    if next_slice is not None:
-        yield next_slice
+            compression=compression,
+            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            table=table,
+            offset=offset,
+            chunk_size=max_rows_by_file,
+            use_threads=use_threads,
+        )
+    return proxy.close()  # blocking
 
 
 @engine.dispatch_on_engine
-def _read_parquet(  # pylint: disable=W0613
-    paths: List[str],
-    path_root: Optional[str],
-    schema: pa.schema,
-    columns: Optional[List[str]],
-    coerce_int96_timestamp_unit: Optional[str],
-    boto3_session: Optional[boto3.Session],
+def _to_parquet(
+    df: pd.DataFrame,
+    schema: pa.Schema,
+    index: bool,
+    compression: Optional[str],
+    compression_ext: str,
+    pyarrow_additional_kwargs: Dict[str, Any],
+    cpus: int,
+    dtype: Dict[str, str],
+    s3_client: Optional["S3Client"],
+    s3_additional_kwargs: Optional[Dict[str, str]],
     use_threads: Union[bool, int],
-    parallelism: int,
-    version_ids: Optional[Dict[str, str]],
-    s3_additional_kwargs: Optional[Dict[str, Any]],
-    arrow_kwargs: Dict[str, Any],
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    executor = _get_executor(use_threads=use_threads)
-    tables = executor.map(
-        _read_parquet_file,
-        boto3_session,
-        paths,
-        itertools.repeat(path_root),
-        itertools.repeat(columns),
-        itertools.repeat(coerce_int96_timestamp_unit),
-        itertools.repeat(s3_additional_kwargs),
-        itertools.repeat(use_threads),
-        [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
+    path: Optional[str] = None,
+    path_root: Optional[str] = None,
+    filename_prefix: Optional[str] = None,
+    max_rows_by_file: Optional[int] = 0,
+) -> List[str]:
+    s3_client = s3_client if s3_client else _utils.client(service_name="s3")
+    file_path = _get_file_path(
+        path_root=path_root, path=path, filename_prefix=filename_prefix, compression_ext=compression_ext
     )
-    return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
+    table: pa.Table = _df_to_table(df, schema, index, dtype)
+    if max_rows_by_file is not None and max_rows_by_file > 0:
+        paths: List[str] = _to_parquet_chunked(
+            file_path=file_path,
+            s3_client=s3_client,
+            s3_additional_kwargs=s3_additional_kwargs,
+            compression=compression,
+            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            table=table,
+            max_rows_by_file=max_rows_by_file,
+            num_of_rows=df.shape[0],
+            cpus=cpus,
+        )
+    else:
+        write_table_args = _get_write_table_args(pyarrow_additional_kwargs)
+        with _new_writer(
+            file_path=file_path,
+            compression=compression,
+            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            schema=table.schema,
+            s3_client=s3_client,
+            s3_additional_kwargs=s3_additional_kwargs,
+            use_threads=use_threads,
+        ) as writer:
+            writer.write_table(table, **write_table_args)
+        paths = [file_path]
+    return paths
 
 
-def read_parquet(
-    path: Union[str, List[str]],
-    path_root: Optional[str] = None,
-    dataset: bool = False,
-    path_suffix: Union[str, List[str], None] = None,
-    path_ignore_suffix: Union[str, List[str], None] = None,
-    ignore_empty: bool = True,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
-    columns: Optional[List[str]] = None,
-    validate_schema: bool = False,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-    last_modified_begin: Optional[datetime.datetime] = None,
-    last_modified_end: Optional[datetime.datetime] = None,
-    version_id: Optional[Union[str, Dict[str, str]]] = None,
-    chunked: Union[bool, int] = False,
+@apply_configs
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session", "s3_additional_kwargs"],
+)
+def to_parquet(  # pylint: disable=too-many-arguments,too-many-locals,too-many-branches,too-many-statements
+    df: pd.DataFrame,
+    path: Optional[str] = None,
+    index: bool = False,
+    compression: Optional[str] = "snappy",
+    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
+    max_rows_by_file: Optional[int] = None,
     use_threads: Union[bool, int] = True,
-    parallelism: int = -1,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    """Read Parquet file(s) from an S3 prefix or list of S3 objects paths.
+    sanitize_columns: bool = False,
+    dataset: bool = False,
+    filename_prefix: Optional[str] = None,
+    partition_cols: Optional[List[str]] = None,
+    bucketing_info: Optional[BucketingInfoTuple] = None,
+    concurrent_partitioning: bool = False,
+    mode: Optional[str] = None,
+    catalog_versioning: bool = False,
+    schema_evolution: bool = True,
+    database: Optional[str] = None,
+    table: Optional[str] = None,
+    glue_table_settings: Optional[GlueTableSettings] = None,
+    dtype: Optional[Dict[str, str]] = None,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
+    catalog_id: Optional[str] = None,
+) -> _S3WriteDataReturnValue:
+    """Write Parquet file or dataset on Amazon S3.
 
-    The concept of `dataset` enables more complex features like partitioning
-    and catalog integration (AWS Glue Catalog).
-
-    This function accepts Unix shell-style wildcards in the path argument.
-    * (matches everything), ? (matches any single character),
-    [seq] (matches any character in seq), [!seq] (matches any character not in seq).
-    If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
-    you can use `glob.escape(path)` before passing the argument to this function.
+    The concept of Dataset goes beyond the simple idea of ordinary files and enable more
+    complex features like partitioning and catalog integration (Amazon Athena/AWS Glue Catalog).
 
     Note
     ----
-    ``Batching`` (`chunked` argument) (Memory Friendly):
-
-    Used to return an Iterable of DataFrames instead of a regular DataFrame.
-
-    Two batching strategies are available:
-
-    - **chunked=True**, a DataFrame is returned for each file in the dataset.
-
-    - **chunked=INTEGER**, a DataFrame is returned with maximum rows equal to the received INTEGER.
-
-    `P.S.` `chunked=True` if faster and uses less memory while `chunked=INTEGER` is more precise
-    in the number of rows.
+    This operation may mutate the original pandas dataframe in-place. To avoid this behaviour
+    please pass in a deep copy instead (i.e. `df.copy()`)
 
     Note
     ----
-    If `use_threads=True`, the number of threads is obtained from os.cpu_count().
+    If `database` and `table` arguments are passed, the table name and all column names
+    will be automatically sanitized using `wr.catalog.sanitize_table_name` and `wr.catalog.sanitize_column_name`.
+    Please, pass `sanitize_columns=True` to enforce this behaviour always.
 
     Note
     ----
-    Filtering by `last_modified begin` and `last_modified end` is applied after listing all S3 files
+    In case of `use_threads=True` the number of threads
+    that will be spawned will be gotten from os.cpu_count().
 
     Parameters
     ----------
-    path : Union[str, List[str]]
-        S3 prefix (accepts Unix shell-style wildcards)
-        (e.g. s3://bucket/prefix) or list of S3 objects paths (e.g. [s3://bucket/key0, s3://bucket/key1]).
-    path_root : str, optional
-        Root path of the dataset. If dataset=`True`, it is used as a starting point to load partition columns.
-    dataset : bool, default False
-        If `True`, read a parquet dataset instead of individual file(s), loading all related partitions as columns.
-    path_suffix : Union[str, List[str], None]
-        Suffix or List of suffixes to be read (e.g. [".gz.parquet", ".snappy.parquet"]).
-        If None, reads all files. (default)
-    path_ignore_suffix : Union[str, List[str], None]
-        Suffix or List of suffixes to be ignored.(e.g. [".csv", "_SUCCESS"]).
-        If None, reads all files. (default)
-    ignore_empty : bool, default True
-        Ignore files with 0 bytes.
-    partition_filter : Callable[[Dict[str, str]], bool], optional
-        Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
-        This function must receive a single argument (Dict[str, str]) where keys are partitions
-        names and values are partitions values. Partitions values must be strings and the function
-        must return a bool, True to read the partition or False to ignore it.
-        Ignored if `dataset=False`.
-        E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-data-wrangler.readthedocs.io/en/3.0.0rc2/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
-    columns : List[str], optional
-        List of columns to read from the file(s).
-    validate_schema : bool, default False
-        Check that the schema is consistent across individual files.
-    coerce_int96_timestamp_unit : str, optional
-        Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
-        Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
-    last_modified_begin : datetime, optional
-        Filter S3 objects by Last modified date.
-        Filter is only applied after listing all objects.
-    last_modified_end : datetime, optional
-        Filter S3 objects by Last modified date.
-        Filter is only applied after listing all objects.
-    version_id: Optional[Union[str, Dict[str, str]]]
-        Version id of the object or mapping of object path to version id.
-        (e.g. {'s3://bucket/key0': '121212', 's3://bucket/key1': '343434'})
-    chunked : Union[int, bool]
-        If passed, the data is split into an iterable of DataFrames (Memory friendly).
-        If `True` an iterable of DataFrames is returned without guarantee of chunksize.
-        If an `INTEGER` is passed, an iterable of DataFrames is returned with maximum rows
-        equal to the received INTEGER.
-    use_threads : Union[bool, int], default True
+    df: pandas.DataFrame
+        Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
+    path : str, optional
+        S3 path (for file e.g. ``s3://bucket/prefix/filename.parquet``) (for dataset e.g. ``s3://bucket/prefix``).
+        Required if dataset=False or when dataset=True and creating a new dataset
+    index : bool
+        True to store the DataFrame index in file, otherwise False to ignore it.
+        Is not supported in conjunction with `max_rows_by_file` when running the library with Ray/Modin.
+    compression: str, optional
+        Compression style (``None``, ``snappy``, ``gzip``, ``zstd``).
+    pyarrow_additional_kwargs : Optional[Dict[str, Any]]
+        Additional parameters forwarded to pyarrow.
+        e.g. pyarrow_additional_kwargs={'coerce_timestamps': 'ns', 'use_deprecated_int96_timestamps': False,
+        'allow_truncated_timestamps'=False}
+    max_rows_by_file : int
+        Max number of rows in each file.
+        Default is None i.e. dont split the files.
+        (e.g. 33554432, 268435456)
+        Is not supported in conjuction with `index=True` when running the library with Ray/Modin.
+    use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
-        If enabled, os.cpu_count() is used as the max number of threads.
+        If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
-    parallelism : int, optional
-        The requested parallelism of the read. Only used when `distributed` add-on is installed.
-        Parallelism may be limited by the number of files of the dataset. -1 (autodetect) by default.
     boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session is used if None is received.
+        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
     s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to S3 botocore requests.
-    pyarrow_additional_kwargs : Dict[str, Any], optional
-        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
-        Valid values include "split_blocks", "self_destruct", "ignore_metadata".
-        e.g. pyarrow_additional_kwargs={'split_blocks': True}.
+        Forwarded to botocore requests.
+        e.g. s3_additional_kwargs={'ServerSideEncryption': 'aws:kms', 'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'}
+    sanitize_columns : bool
+        True to sanitize columns names (using `wr.catalog.sanitize_table_name` and `wr.catalog.sanitize_column_name`)
+        or False to keep it as is.
+        True value behaviour is enforced if `database` and `table` arguments are passed.
+    dataset : bool
+        If True store a parquet dataset instead of a ordinary file(s)
+        If True, enable all follow arguments:
+        partition_cols, mode, database, table, description, parameters, columns_comments, concurrent_partitioning,
+        catalog_versioning, projection_params, catalog_id, schema_evolution.
+    filename_prefix: str, optional
+        If dataset=True, add a filename prefix to the output files.
+    partition_cols: List[str], optional
+        List of column names that will be used to create partitions. Only takes effect if dataset=True.
+    bucketing_info: Tuple[List[str], int], optional
+        Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
+        second element.
+        Only `str`, `int` and `bool` are supported as column data types for bucketing.
+    concurrent_partitioning: bool
+        If True will increase the parallelism level during the partitions writing. It will decrease the
+        writing time and increase the memory usage.
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+    mode: str, optional
+        ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
+        For details check the related tutorial:
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/004%20-%20Parquet%20Datasets.html
+    catalog_versioning : bool
+        If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
+    schema_evolution : bool
+        If True allows schema evolution (new or missing columns), otherwise a exception will be raised. True by default.
+        (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
+        Related tutorial:
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/014%20-%20Schema%20Evolution.html
+    database : str, optional
+        Glue/Athena catalog: Database name.
+    table : str, optional
+        Glue/Athena catalog: Table name.
+    glue_table_settings: dict (GlueTableSettings), optional
+        Settings for writing to the Glue table.
+    dtype : Dict[str, str], optional
+        Dictionary of columns names and Athena/Glue types to be casted.
+        Useful when you have columns with undetermined or mixed data types.
+        (e.g. {'col name': 'bigint', 'col2 name': 'int'})
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    catalog_id : str, optional
+        The ID of the Data Catalog from which to retrieve Databases.
+        If none is provided, the AWS account ID is used by default.
 
     Returns
     -------
-    Union[pandas.DataFrame, Generator[pandas.DataFrame, None, None]]
-        Pandas DataFrame or a Generator in case of `chunked=True`.
+    wr.typing._S3WriteDataReturnValue
+        Dictionary with:
+        'paths': List of all stored files paths on S3.
+        'partitions_values': Dictionary of partitions added with keys as S3 path locations
+        and values as a list of partitions values as str.
 
     Examples
     --------
-    Reading all Parquet files under a prefix
+    Writing single file
 
     >>> import awswrangler as wr
-    >>> df = wr.s3.read_parquet(path='s3://bucket/prefix/')
+    >>> import pandas as pd
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({'col': [1, 2, 3]}),
+    ...     path='s3://bucket/prefix/my_file.parquet',
+    ... )
+    {
+        'paths': ['s3://bucket/prefix/my_file.parquet'],
+        'partitions_values': {}
+    }
 
-    Reading all Parquet files from a list
+    Writing single file encrypted with a KMS key
 
     >>> import awswrangler as wr
-    >>> df = wr.s3.read_parquet(path=['s3://bucket/filename0.parquet', 's3://bucket/filename1.parquet'])
+    >>> import pandas as pd
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({'col': [1, 2, 3]}),
+    ...     path='s3://bucket/prefix/my_file.parquet',
+    ...     s3_additional_kwargs={
+    ...         'ServerSideEncryption': 'aws:kms',
+    ...         'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'
+    ...     }
+    ... )
+    {
+        'paths': ['s3://bucket/prefix/my_file.parquet'],
+        'partitions_values': {}
+    }
 
-    Reading in chunks (Chunk by file)
+    Writing partitioned dataset
 
     >>> import awswrangler as wr
-    >>> dfs = wr.s3.read_parquet(path=['s3://bucket/filename0.csv', 's3://bucket/filename1.csv'], chunked=True)
-    >>> for df in dfs:
-    >>>     print(df)  # Smaller Pandas DataFrame
+    >>> import pandas as pd
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({
+    ...         'col': [1, 2, 3],
+    ...         'col2': ['A', 'A', 'B']
+    ...     }),
+    ...     path='s3://bucket/prefix',
+    ...     dataset=True,
+    ...     partition_cols=['col2']
+    ... )
+    {
+        'paths': ['s3://.../col2=A/x.parquet', 's3://.../col2=B/y.parquet'],
+        'partitions_values: {
+            's3://.../col2=A/': ['A'],
+            's3://.../col2=B/': ['B']
+        }
+    }
 
-    Reading in chunks (Chunk by 1MM rows)
+    Writing partitioned dataset with partition projection
 
     >>> import awswrangler as wr
-    >>> dfs = wr.s3.read_parquet(path=['s3://bucket/filename0.csv', 's3://bucket/filename1.csv'], chunked=1_000_000)
-    >>> for df in dfs:
-    >>>     print(df)  # 1MM Pandas DataFrame
+    >>> import pandas as pd
+    >>> from datetime import datetime
+    >>> dt = lambda x: datetime.strptime(x, "%Y-%m-%d").date()
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({
+    ...         "id": [1, 2, 3],
+    ...         "value": [1000, 1001, 1002],
+    ...         "category": ['A', 'B', 'C'],
+    ...     }),
+    ...     path='s3://bucket/prefix',
+    ...     dataset=True,
+    ...     partition_cols=['value', 'category'],
+    ...     athena_partition_projection_settings={
+    ...        "projection_types": {
+    ...             "value": "integer",
+    ...             "category": "enum",
+    ...         },
+    ...         "projection_ranges": {
+    ...             "value": "1000,2000",
+    ...             "category": "A,B,C",
+    ...         },
+    ...     },
+    ... )
+    {
+        'paths': [
+            's3://.../value=1000/category=A/x.snappy.parquet', ...
+        ],
+        'partitions_values': {
+            's3://.../value=1000/category=A/': [
+                '1000',
+                'A',
+            ], ...
+        }
+    }
 
-    Reading Parquet Dataset with PUSH-DOWN filter over partitions
+    Writing bucketed dataset
 
     >>> import awswrangler as wr
-    >>> my_filter = lambda x: True if x["city"].startswith("new") else False
-    >>> df = wr.s3.read_parquet(path, dataset=True, partition_filter=my_filter)
-
-    """
-    paths: List[str] = _path2list(
-        path=path,
-        boto3_session=boto3_session,
-        suffix=path_suffix,
-        ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=path_ignore_suffix),
-        last_modified_begin=last_modified_begin,
-        last_modified_end=last_modified_end,
-        ignore_empty=ignore_empty,
-        s3_additional_kwargs=s3_additional_kwargs,
-    )
-    if not path_root:
-        path_root = _get_path_root(path=path, dataset=dataset)
-    if path_root and partition_filter:
-        paths = _apply_partition_filter(path_root=path_root, paths=paths, filter_func=partition_filter)
-    if len(paths) < 1:
-        raise exceptions.NoFilesFound(f"No files Found on: {path}.")
-    _logger.debug("paths:\n%s", paths)
-
-    version_ids: Optional[Dict[str, str]] = (
-        version_id if isinstance(version_id, dict) else {paths[0]: version_id} if isinstance(version_id, str) else None
-    )
-
-    # Create PyArrow schema based on file metadata, columns filter, and partitions
-    schema = _validate_schemas_from_files(
-        validate_schema=validate_schema,
-        paths=paths,
-        sampling=1.0,
-        use_threads=use_threads,
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-        coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-        version_ids=version_ids,
-    )
-    if path_root:
-        partition_types, _ = _extract_partitions_metadata_from_paths(path=path_root, paths=paths)
-        if partition_types:
-            partition_schema = pa.schema(
-                fields={k: _data_types.athena2pyarrow(dtype=v) for k, v in partition_types.items()}
-            )
-            schema = pa.unify_schemas([schema, partition_schema])
-    if columns:
-        schema = pa.schema([schema.field(column) for column in columns], schema.metadata)
-    _logger.debug("schema:\n%s", schema)
+    >>> import pandas as pd
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({
+    ...         'col': [1, 2, 3],
+    ...         'col2': ['A', 'A', 'B']
+    ...     }),
+    ...     path='s3://bucket/prefix',
+    ...     dataset=True,
+    ...     bucketing_info=(["col2"], 2)
+    ... )
+    {
+        'paths': ['s3://.../x_bucket-00000.csv', 's3://.../col2=B/x_bucket-00001.csv'],
+        'partitions_values: {}
+    }
 
-    arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
+    Writing dataset to S3 with metadata on Athena/Glue Catalog.
 
-    if chunked:
-        return _read_parquet_chunked(
-            boto3_session=boto3_session,
-            paths=paths,
-            path_root=path_root,
-            columns=columns,
-            coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-            chunked=chunked,
-            use_threads=use_threads,
-            s3_additional_kwargs=s3_additional_kwargs,
-            arrow_kwargs=arrow_kwargs,
-            version_ids=version_ids,
-        )
-
-    return _read_parquet(
-        paths,
-        path_root=path_root,
-        schema=schema,
-        columns=columns,
-        coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-        use_threads=use_threads,
-        parallelism=parallelism,
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-        arrow_kwargs=arrow_kwargs,
-        version_ids=version_ids,
-    )
-
-
-@apply_configs
-def read_parquet_table(
-    table: str,
-    database: str,
-    filename_suffix: Union[str, List[str], None] = None,
-    filename_ignore_suffix: Union[str, List[str], None] = None,
-    catalog_id: Optional[str] = None,
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
-    columns: Optional[List[str]] = None,
-    validate_schema: bool = True,
-    coerce_int96_timestamp_unit: Optional[str] = None,
-    chunked: Union[bool, int] = False,
-    use_threads: Union[bool, int] = True,
-    parallelism: int = 200,
-    boto3_session: Optional[boto3.Session] = None,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
-    """Read Apache Parquet table registered in the AWS Glue Catalog.
-
-    Note
-    ----
-    ``Batching`` (`chunked` argument) (Memory Friendly):
-
-    Used to return an Iterable of DataFrames instead of a regular DataFrame.
-
-    Two batching strategies are available:
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({
+    ...         'col': [1, 2, 3],
+    ...         'col2': ['A', 'A', 'B']
+    ...     }),
+    ...     path='s3://bucket/prefix',
+    ...     dataset=True,
+    ...     partition_cols=['col2'],
+    ...     database='default',  # Athena/Glue database
+    ...     table='my_table'  # Athena/Glue table
+    ... )
+    {
+        'paths': ['s3://.../col2=A/x.parquet', 's3://.../col2=B/y.parquet'],
+        'partitions_values: {
+            's3://.../col2=A/': ['A'],
+            's3://.../col2=B/': ['B']
+        }
+    }
 
-    - **chunked=True**, a DataFrame is returned for each file in the dataset.
+    Writing dataset to Glue governed table
 
-    - **chunked=INTEGER**, a DataFrame is returned with maximum rows equal to the received INTEGER.
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({
+    ...         'col': [1, 2, 3],
+    ...         'col2': ['A', 'A', 'B'],
+    ...         'col3': [None, None, None]
+    ...     }),
+    ...     dataset=True,
+    ...     mode='append',
+    ...     database='default',  # Athena/Glue database
+    ...     table='my_table',  # Athena/Glue table
+    ...     glue_table_settings=wr.typing.GlueTableSettings(
+    ...         table_type="GOVERNED",
+    ...         transaction_id="xxx",
+    ...     ),
+    ... )
+    {
+        'paths': ['s3://.../x.parquet'],
+        'partitions_values: {}
+    }
 
-    `P.S.` `chunked=True` if faster and uses less memory while `chunked=INTEGER` is more precise
-    in the number of rows.
+    Writing dataset casting empty column data type
 
-    Note
-    ----
-    If `use_threads=True`, the number of threads is obtained from os.cpu_count().
-
-    Parameters
-    ----------
-    table : str
-        AWS Glue Catalog table name.
-    database : str
-        AWS Glue Catalog database name.
-    filename_suffix : Union[str, List[str], None]
-        Suffix or List of suffixes to be read (e.g. [".gz.parquet", ".snappy.parquet"]).
-        If None, read all files. (default)
-    filename_ignore_suffix : Union[str, List[str], None]
-        Suffix or List of suffixes for S3 keys to be ignored.(e.g. [".csv", "_SUCCESS"]).
-        If None, read all files. (default)
-    catalog_id : str, optional
-        The ID of the Data Catalog from which to retrieve Databases.
-        If none is provided, the AWS account ID is used by default.
-    partition_filter: Optional[Callable[[Dict[str, str]], bool]]
-        Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
-        This function must receive a single argument (Dict[str, str]) where keys are partitions
-        names and values are partitions values. Partitions values must be strings and the function
-        must return a bool, True to read the partition or False to ignore it.
-        Ignored if `dataset=False`.
-        E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
-    columns : List[str], optional
-        List of columns to read from the file(s).
-    validate_schema : bool, default False
-        Check that the schema is consistent across individual files.
-    coerce_int96_timestamp_unit : str, optional
-        Cast timestamps that are stored in INT96 format to a particular resolution (e.g. "ms").
-        Setting to None is equivalent to "ns" and therefore INT96 timestamps are inferred as in nanoseconds.
-    chunked : Union[int, bool]
-        If passed, the data is split into an iterable of DataFrames (Memory friendly).
-        If `True` an iterable of DataFrames is returned without guarantee of chunksize.
-        If an `INTEGER` is passed, an iterable of DataFrames is returned with maximum rows
-        equal to the received INTEGER.
-    use_threads : Union[bool, int], default True
-        True to enable concurrent requests, False to disable multiple threads.
-        If enabled, os.cpu_count() is used as the max number of threads.
-        If integer is provided, specified number is used.
-    parallelism : int, optional
-        The requested parallelism of the read. Only used when `distributed` add-on is installed.
-        Parallelism may be limited by the number of files of the dataset. 200 by default.
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session is used if None is received.
-    s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to S3 botocore requests.
-    pyarrow_additional_kwargs : Dict[str, Any], optional
-        Forwarded to `to_pandas` method converting from PyArrow tables to Pandas DataFrame.
-        Valid values include "split_blocks", "self_destruct", "ignore_metadata".
-        e.g. pyarrow_additional_kwargs={'split_blocks': True}.
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> wr.s3.to_parquet(
+    ...     df=pd.DataFrame({
+    ...         'col': [1, 2, 3],
+    ...         'col2': ['A', 'A', 'B'],
+    ...         'col3': [None, None, None]
+    ...     }),
+    ...     path='s3://bucket/prefix',
+    ...     dataset=True,
+    ...     database='default',  # Athena/Glue database
+    ...     table='my_table'  # Athena/Glue table
+    ...     dtype={'col3': 'date'}
+    ... )
+    {
+        'paths': ['s3://.../x.parquet'],
+        'partitions_values: {}
+    }
 
-    Returns
-    -------
-    Union[pandas.DataFrame, Generator[pandas.DataFrame, None, None]]
-        Pandas DataFrame or a Generator in case of `chunked=True`.
+    """
+    glue_table_settings = cast(
+        GlueTableSettings,
+        glue_table_settings if glue_table_settings else {},
+    )
 
-    Examples
-    --------
-    Reading Parquet Table
+    table_type = glue_table_settings.get("table_type")
+    transaction_id = glue_table_settings.get("transaction_id")
+    description = glue_table_settings.get("description")
+    parameters = glue_table_settings.get("parameters")
+    columns_comments = glue_table_settings.get("columns_comments")
+    regular_partitions = glue_table_settings.get("regular_partitions", True)
+
+    _validate_args(
+        df=df,
+        table=table,
+        database=database,
+        dataset=dataset,
+        path=path,
+        partition_cols=partition_cols,
+        bucketing_info=bucketing_info,
+        mode=mode,
+        description=description,
+        parameters=parameters,
+        columns_comments=columns_comments,
+        execution_engine=engine.get(),
+    )
 
-    >>> import awswrangler as wr
-    >>> df = wr.s3.read_parquet_table(database='...', table='...')
+    # Evaluating compression
+    if _COMPRESSION_2_EXT.get(compression, None) is None:
+        raise exceptions.InvalidCompression(f"{compression} is invalid, please use None, 'snappy', 'gzip' or 'zstd'.")
+    compression_ext: str = _COMPRESSION_2_EXT[compression]
+
+    # Initializing defaults
+    partition_cols = partition_cols if partition_cols else []
+    dtype = dtype if dtype else {}
+    partitions_values: Dict[str, List[str]] = {}
+    mode = "append" if mode is None else mode
+    commit_trans: bool = False
+    if transaction_id:
+        table_type = "GOVERNED"
+
+    filename_prefix = filename_prefix + uuid.uuid4().hex if filename_prefix else uuid.uuid4().hex
+    cpus: int = _utils.ensure_cpu_count(use_threads=use_threads)
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
+    # Pyarrow defaults
+    if not pyarrow_additional_kwargs:
+        pyarrow_additional_kwargs = {}
+    if not pyarrow_additional_kwargs.get("coerce_timestamps"):
+        pyarrow_additional_kwargs["coerce_timestamps"] = "ms"
+    if "flavor" not in pyarrow_additional_kwargs:
+        pyarrow_additional_kwargs["flavor"] = "spark"
+
+    # Sanitize table to respect Athena's standards
+    if (sanitize_columns is True) or (database is not None and table is not None):
+        df, dtype, partition_cols = _sanitize(
+            df=copy_df_shallow(df),
+            dtype=dtype,
+            partition_cols=partition_cols,
+        )
 
-    Reading Parquet Table in chunks (Chunk by file)
+    # Evaluating dtype
+    catalog_table_input: Optional[Dict[str, Any]] = None
+    if database is not None and table is not None:
+        catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
+            database=database,
+            table=table,
+            boto3_session=boto3_session,
+            transaction_id=transaction_id,
+            catalog_id=catalog_id,
+        )
+        catalog_path: Optional[str] = None
+        if catalog_table_input:
+            table_type = catalog_table_input["TableType"]
+            catalog_path = catalog_table_input["StorageDescriptor"]["Location"]
+        if path is None:
+            if catalog_path:
+                path = catalog_path
+            else:
+                raise exceptions.InvalidArgumentValue(
+                    "Glue table does not exist in the catalog. Please pass the `path` argument to create it."
+                )
+        elif path and catalog_path:
+            if path.rstrip("/") != catalog_path.rstrip("/"):
+                raise exceptions.InvalidArgumentValue(
+                    f"The specified path: {path}, does not match the existing Glue catalog table path: {catalog_path}"
+                )
+        if (table_type == "GOVERNED") and (not transaction_id):
+            _logger.debug("`transaction_id` not specified for GOVERNED table, starting transaction")
+            transaction_id = lakeformation.start_transaction(
+                read_only=False,
+                boto3_session=boto3_session,
+            )
+            commit_trans = True
 
-    >>> import awswrangler as wr
-    >>> dfs = wr.s3.read_parquet_table(database='...', table='...', chunked=True)
-    >>> for df in dfs:
-    >>>     print(df)  # Smaller Pandas DataFrame
+    df = _apply_dtype(df=df, dtype=dtype, catalog_table_input=catalog_table_input, mode=mode)
+    schema: pa.Schema = _data_types.pyarrow_schema_from_pandas(
+        df=df, index=index, ignore_cols=partition_cols, dtype=dtype
+    )
+    _logger.debug("schema: \n%s", schema)
 
-    Reading Parquet Dataset with PUSH-DOWN filter over partitions
+    if dataset is False:
+        paths = _to_parquet(
+            df,
+            path=path,
+            filename_prefix=filename_prefix,
+            schema=schema,
+            index=index,
+            cpus=cpus,
+            compression=compression,
+            compression_ext=compression_ext,
+            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            s3_client=s3_client,
+            s3_additional_kwargs=s3_additional_kwargs,
+            dtype=dtype,
+            max_rows_by_file=max_rows_by_file,
+            use_threads=use_threads,
+        )
+    else:
+        columns_types: Dict[str, str] = {}
+        partitions_types: Dict[str, str] = {}
+        if (database is not None) and (table is not None):
+            columns_types, partitions_types = _data_types.athena_types_from_pandas_partitioned(
+                df=df, index=index, partition_cols=partition_cols, dtype=dtype
+            )
+            if schema_evolution is False:
+                _utils.check_schema_changes(columns_types=columns_types, table_input=catalog_table_input, mode=mode)
 
-    >>> import awswrangler as wr
-    >>> my_filter = lambda x: True if x["city"].startswith("new") else False
-    >>> df = wr.s3.read_parquet_table(path, dataset=True, partition_filter=my_filter)
+            create_table_args: Dict[str, Any] = {
+                "database": database,
+                "table": table,
+                "path": path,
+                "columns_types": columns_types,
+                "table_type": table_type,
+                "partitions_types": partitions_types,
+                "bucketing_info": bucketing_info,
+                "compression": compression,
+                "description": description,
+                "parameters": parameters,
+                "columns_comments": columns_comments,
+                "boto3_session": boto3_session,
+                "mode": mode,
+                "transaction_id": transaction_id,
+                "catalog_versioning": catalog_versioning,
+                "athena_partition_projection_settings": athena_partition_projection_settings,
+                "catalog_id": catalog_id,
+                "catalog_table_input": catalog_table_input,
+            }
+
+            if (catalog_table_input is None) and (table_type == "GOVERNED"):
+                catalog._create_parquet_table(**create_table_args)  # pylint: disable=protected-access
+                create_table_args["catalog_table_input"] = catalog._get_table_input(  # pylint: disable=protected-access
+                    database=database,
+                    table=table,
+                    boto3_session=boto3_session,
+                    transaction_id=transaction_id,
+                    catalog_id=catalog_id,
+                )
 
-    """
-    client_glue: boto3.client = _utils.client(service_name="glue", session=boto3_session)
-    res: Dict[str, Any] = client_glue.get_table(**_catalog_id(catalog_id=catalog_id, DatabaseName=database, Name=table))
-    try:
-        location: str = res["Table"]["StorageDescriptor"]["Location"]
-        path: str = location if location.endswith("/") else f"{location}/"
-    except KeyError as ex:
-        raise exceptions.InvalidTable(f"Missing s3 location for {database}.{table}.") from ex
-    path_root: Optional[str] = None
-    paths: Union[str, List[str]] = path
-    # If filter is available, fetch & filter out partitions
-    # Then list objects & process individual object keys under path_root
-    if partition_filter:
-        available_partitions_dict = _get_partitions(
+        paths, partitions_values = _to_dataset(
+            func=_to_parquet,
+            concurrent_partitioning=concurrent_partitioning,
+            df=df,
+            path_root=path,  # type: ignore[arg-type]
+            filename_prefix=filename_prefix,
+            index=index,
+            compression=compression,
+            compression_ext=compression_ext,
+            catalog_id=catalog_id,
             database=database,
             table=table,
-            catalog_id=catalog_id,
+            table_type=table_type,
+            transaction_id=transaction_id,
+            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
+            cpus=cpus,
+            use_threads=use_threads,
+            partition_cols=partition_cols,
+            partitions_types=partitions_types,
+            bucketing_info=bucketing_info,
+            dtype=dtype,
+            mode=mode,
             boto3_session=boto3_session,
+            s3_additional_kwargs=s3_additional_kwargs,
+            schema=schema,
+            max_rows_by_file=max_rows_by_file,
         )
-        available_partitions = list(_ensure_locations_are_valid(available_partitions_dict.keys()))
-        if available_partitions:
-            paths = []
-            path_root = path
-            partitions: Union[str, List[str]] = _apply_partition_filter(
-                path_root=path_root, paths=available_partitions, filter_func=partition_filter
-            )
-            for partition in partitions:
-                paths += _path2list(
-                    path=partition,
+        if (database is not None) and (table is not None):
+            try:
+                catalog._create_parquet_table(**create_table_args)  # pylint: disable=protected-access
+                if partitions_values and (regular_partitions is True) and (table_type != "GOVERNED"):
+                    _logger.debug("partitions_values:\n%s", partitions_values)
+                    catalog.add_parquet_partitions(
+                        database=database,
+                        table=table,
+                        partitions_values=partitions_values,
+                        bucketing_info=bucketing_info,
+                        compression=compression,
+                        boto3_session=boto3_session,
+                        catalog_id=catalog_id,
+                        columns_types=columns_types,
+                    )
+                if commit_trans:
+                    lakeformation.commit_transaction(
+                        transaction_id=transaction_id,  # type: ignore[arg-type]
+                        boto3_session=boto3_session,
+                    )
+            except Exception:
+                _logger.debug("Catalog write failed, cleaning up S3 objects (len(paths): %s).", len(paths))
+                delete_objects(
+                    path=paths,
+                    use_threads=use_threads,
                     boto3_session=boto3_session,
-                    suffix=filename_suffix,
-                    ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=filename_ignore_suffix),
                     s3_additional_kwargs=s3_additional_kwargs,
                 )
-    df = read_parquet(
-        path=paths,
-        path_root=path_root,
-        dataset=True,
-        path_suffix=filename_suffix if path_root is None else None,
-        path_ignore_suffix=filename_ignore_suffix if path_root is None else None,
-        columns=columns,
-        validate_schema=validate_schema,
-        coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-        chunked=chunked,
-        use_threads=use_threads,
-        parallelism=parallelism,
-        boto3_session=boto3_session,
-        pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-    )
-
-    partial_cast_function = functools.partial(
-        _data_types.cast_pandas_with_athena_types, dtype=_extract_partitions_dtypes_from_table_details(response=res)
-    )
-    if _utils.is_pandas_frame(df):
-        return partial_cast_function(df)
-    # df is a generator, so map is needed for casting dtypes
-    return map(partial_cast_function, df)
+                raise
+    return {"paths": paths, "partitions_values": partitions_values}
 
 
 @apply_configs
-def read_parquet_metadata(
-    path: Union[str, List[str]],
-    dataset: bool = False,
-    version_id: Optional[Union[str, Dict[str, str]]] = None,
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
+def store_parquet_metadata(  # pylint: disable=too-many-arguments,too-many-locals
+    path: str,
+    database: str,
+    table: str,
+    catalog_id: Optional[str] = None,
     path_suffix: Optional[str] = None,
     path_ignore_suffix: Optional[str] = None,
     ignore_empty: bool = True,
-    ignore_null: bool = False,
     dtype: Optional[Dict[str, str]] = None,
     sampling: float = 1.0,
-    coerce_int96_timestamp_unit: Optional[str] = None,
+    dataset: bool = False,
     use_threads: Union[bool, int] = True,
-    boto3_session: Optional[boto3.Session] = None,
+    description: Optional[str] = None,
+    parameters: Optional[Dict[str, str]] = None,
+    columns_comments: Optional[Dict[str, str]] = None,
+    compression: Optional[str] = None,
+    mode: str = "overwrite",
+    catalog_versioning: bool = False,
+    regular_partitions: bool = True,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
-) -> Tuple[Dict[str, str], Optional[Dict[str, str]]]:
-    """Read Apache Parquet file(s) metadata from an S3 prefix or list of S3 objects paths.
+    boto3_session: Optional[boto3.Session] = None,
+) -> Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]:
+    """Infer and store parquet metadata on AWS Glue Catalog.
 
-    The concept of `dataset` enables more complex features like partitioning
-    and catalog integration (AWS Glue Catalog).
+    Infer Apache Parquet file(s) metadata from a received S3 prefix
+    And then stores it on AWS Glue Catalog including all inferred partitions
+    (No need for 'MSCK REPAIR TABLE')
+
+    The concept of Dataset goes beyond the simple idea of files and enables more
+    complex features like partitioning and catalog integration (AWS Glue Catalog).
 
     This function accepts Unix shell-style wildcards in the path argument.
     * (matches everything), ? (matches any single character),
     [seq] (matches any character in seq), [!seq] (matches any character not in seq).
     If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
-    you can use `glob.escape(path)` before passing the argument to this function.
+    you can use `glob.escape(path)` before passing the path to this function.
 
     Note
     ----
-    If `use_threads=True`, the number of threads is obtained from os.cpu_count().
+    In case of `use_threads=True` the number of threads
+    that will be spawned will be gotten from os.cpu_count().
 
     Parameters
     ----------
-    path : Union[str, List[str]]
-        S3 prefix (accepts Unix shell-style wildcards)
-        (e.g. s3://bucket/prefix) or list of S3 objects paths (e.g. [s3://bucket/key0, s3://bucket/key1]).
-    dataset : bool, default False
-        If `True`, read a parquet dataset instead of individual file(s), loading all related partitions as columns.
-    version_id : Union[str, Dict[str, str]], optional
-        Version id of the object or mapping of object path to version id.
-        (e.g. {'s3://bucket/key0': '121212', 's3://bucket/key1': '343434'})
-    path_suffix : Union[str, List[str], None]
-        Suffix or List of suffixes to be read (e.g. [".gz.parquet", ".snappy.parquet"]).
-        If None, reads all files. (default)
-    path_ignore_suffix : Union[str, List[str], None]
-        Suffix or List of suffixes to be ignored.(e.g. [".csv", "_SUCCESS"]).
-        If None, reads all files. (default)
-    ignore_empty : bool, default True
+    path : str
+        S3 prefix (accepts Unix shell-style wildcards) (e.g. s3://bucket/prefix).
+    table : str
+        Glue/Athena catalog: Table name.
+    database : str
+        AWS Glue Catalog database name.
+    catalog_id : str, optional
+        The ID of the Data Catalog from which to retrieve Databases.
+        If none is provided, the AWS account ID is used by default.
+    path_suffix: Union[str, List[str], None]
+        Suffix or List of suffixes for filtering S3 keys.
+    path_ignore_suffix: Union[str, List[str], None]
+        Suffix or List of suffixes for S3 keys to be ignored.
+    ignore_empty: bool
         Ignore files with 0 bytes.
-    ignore_null : bool, default False
-        Ignore columns with null type.
     dtype : Dict[str, str], optional
-        Dictionary of columns names and Athena/Glue types to cast.
-        Use when you have columns with undetermined data types as partitions columns.
+        Dictionary of columns names and Athena/Glue types to be casted.
+        Useful when you have columns with undetermined data types as partitions columns.
         (e.g. {'col name': 'bigint', 'col2 name': 'int'})
     sampling : float
-        Ratio of files metadata to inspect.
+        Random sample ratio of files that will have the metadata inspected.
         Must be `0.0 < sampling <= 1.0`.
         The higher, the more accurate.
         The lower, the faster.
+    dataset: bool
+        If True read a parquet dataset instead of simple file(s) loading all the related partitions as columns.
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
+    description: str, optional
+        Glue/Athena catalog: Table description
+    parameters: Dict[str, str], optional
+        Glue/Athena catalog: Key/value pairs to tag the table.
+    columns_comments: Dict[str, str], optional
+        Glue/Athena catalog:
+        Columns names and the related comments (e.g. {'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}).
+    compression: str, optional
+        Compression style (``None``, ``snappy``, ``gzip``, etc).
+    mode: str
+        'overwrite' to recreate any possible existing table or 'append' to keep any possible existing table.
+    catalog_versioning : bool
+        If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
+    regular_partitions : bool
+        Create regular partitions (Non projected partitions) on Glue Catalog.
+        Disable when you will work only with Partition Projection.
+        Keep enabled even when working with projections is useful to keep
+        Redshift Spectrum working with the regular partitions.
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    s3_additional_kwargs : Optional[Dict[str, Any]]
+        Forwarded to botocore requests.
+        e.g. s3_additional_kwargs={'ServerSideEncryption': 'aws:kms', 'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'}
     boto3_session : boto3.Session(), optional
         Boto3 Session. The default boto3 session will be used if boto3_session receive None.
-    s3_additional_kwargs : Optional[Dict[str, Any]]
-        Forward to S3 botocore requests.
 
     Returns
     -------
-    Tuple[Dict[str, str], Optional[Dict[str, str]]]
+    Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]
+        The metadata used to create the Glue Table.
         columns_types: Dictionary with keys as column names and values as
         data types (e.g. {'col0': 'bigint', 'col1': 'double'}). /
         partitions_types: Dictionary with keys as partition names
-        and values as data types (e.g. {'col2': 'date'}).
+        and values as data types (e.g. {'col2': 'date'}). /
+        partitions_values: Dictionary with keys as S3 path locations and values as a
+        list of partitions values as str (e.g. {'s3://bucket/prefix/y=2020/m=10/': ['2020', '10']}).
 
     Examples
     --------
-    Reading all Parquet files (with partitions) metadata under a prefix
+    Reading all Parquet files metadata under a prefix
 
     >>> import awswrangler as wr
-    >>> columns_types, partitions_types = wr.s3.read_parquet_metadata(path='s3://bucket/prefix/', dataset=True)
-
-    Reading all Parquet files metadata from a list
-
-    >>> import awswrangler as wr
-    >>> columns_types, partitions_types = wr.s3.read_parquet_metadata(path=[
-    ...     's3://bucket/filename0.parquet',
-    ...     's3://bucket/filename1.parquet'
-    ... ])
+    >>> columns_types, partitions_types, partitions_values = wr.s3.store_parquet_metadata(
+    ...     path='s3://bucket/prefix/',
+    ...     database='...',
+    ...     table='...',
+    ...     dataset=True
+    ... )
 
     """
-    return _read_parquet_metadata(
+    columns_types: Dict[str, str]
+    partitions_types: Optional[Dict[str, str]]
+    partitions_values: Optional[Dict[str, List[str]]]
+    columns_types, partitions_types, partitions_values = _read_parquet_metadata(
         path=path,
-        version_id=version_id,
-        path_suffix=path_suffix,
-        path_ignore_suffix=path_ignore_suffix,
-        ignore_empty=ignore_empty,
-        ignore_null=ignore_null,
         dtype=dtype,
         sampling=sampling,
         dataset=dataset,
+        path_suffix=path_suffix,
+        path_ignore_suffix=path_ignore_suffix,
+        ignore_empty=ignore_empty,
+        ignore_null=False,
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
         boto3_session=boto3_session,
-        coerce_int96_timestamp_unit=coerce_int96_timestamp_unit,
-    )[:2]
+    )
+    _logger.debug("columns_types: %s", columns_types)
+    _logger.debug("partitions_types: %s", partitions_types)
+    _logger.debug("partitions_values: %s", partitions_values)
+    catalog.create_parquet_table(
+        database=database,
+        table=table,
+        path=path,
+        columns_types=columns_types,
+        partitions_types=partitions_types,
+        description=description,
+        parameters=parameters,
+        columns_comments=columns_comments,
+        mode=mode,
+        compression=compression,
+        catalog_versioning=catalog_versioning,
+        athena_partition_projection_settings=athena_partition_projection_settings,
+        boto3_session=boto3_session,
+        catalog_id=catalog_id,
+    )
+    if (partitions_types is not None) and (partitions_values is not None) and (regular_partitions is True):
+        catalog.add_parquet_partitions(
+            database=database,
+            table=table,
+            partitions_values=partitions_values,
+            compression=compression,
+            boto3_session=boto3_session,
+            catalog_id=catalog_id,
+            columns_types=columns_types,
+        )
+    return columns_types, partitions_types, partitions_values
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_read_text.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_read_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 """Amazon S3 Read Module (PRIVATE)."""
 import datetime
 import itertools
 import logging
 import pprint
-from typing import Any, Callable, Dict, Iterator, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterator, List, Optional, Union, overload
 
 import boto3
 import pandas as pd
 
 from awswrangler import _utils, exceptions
 from awswrangler._distributed import engine
 from awswrangler._threading import _get_executor
 from awswrangler.s3._list import _path2list
-from awswrangler.s3._read import _apply_partition_filter, _get_path_ignore_suffix, _get_path_root, _union
+from awswrangler.s3._read import (
+    _apply_partition_filter,
+    _check_version_id,
+    _get_path_ignore_suffix,
+    _get_path_root,
+    _union,
+)
 from awswrangler.s3._read_text_core import _read_text_file, _read_text_files_chunked
+from awswrangler.typing import RaySettings
+
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _resolve_format(read_format: str) -> Any:
     if read_format == "csv":
         return pd.read_csv
     if read_format == "fwf":
         return pd.read_fwf
     if read_format == "json":
         return pd.read_json
     raise exceptions.UnsupportedType("Unsupported read format")
 
 
-def _get_version_id_for(version_id: Optional[Union[str, Dict[str, str]]], path: str) -> Optional[str]:
-    if isinstance(version_id, dict):
-        return version_id.get(path, None)
-
-    return version_id
-
-
 @engine.dispatch_on_engine
 def _read_text(  # pylint: disable=W0613
     read_format: str,
     paths: List[str],
     path_root: Optional[str],
     use_threads: Union[bool, int],
-    boto3_session: Optional[boto3.Session],
+    s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
     dataset: bool,
     ignore_index: bool,
     parallelism: int,
-    version_id_dict: Dict[str, Optional[str]],
+    version_ids: Optional[Dict[str, str]],
     pandas_kwargs: Dict[str, Any],
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     parser_func = _resolve_format(read_format)
     executor = _get_executor(use_threads=use_threads)
     tables = executor.map(
         _read_text_file,
-        boto3_session,
+        s3_client,
         paths,
-        [version_id_dict[path] for path in paths],
+        [version_ids.get(p) if isinstance(version_ids, dict) else None for p in paths],
         itertools.repeat(parser_func),
         itertools.repeat(path_root),
         itertools.repeat(pandas_kwargs),
         itertools.repeat(s3_additional_kwargs),
         itertools.repeat(dataset),
     )
     return _union(dfs=tables, ignore_index=ignore_index)
@@ -70,101 +73,165 @@
     path: Union[str, List[str]],
     path_suffix: Union[str, List[str], None],
     path_ignore_suffix: Union[str, List[str], None],
     ignore_empty: bool,
     use_threads: Union[bool, int],
     last_modified_begin: Optional[datetime.datetime],
     last_modified_end: Optional[datetime.datetime],
-    boto3_session: Optional[boto3.Session],
+    s3_client: "S3Client",
     s3_additional_kwargs: Optional[Dict[str, str]],
     chunksize: Optional[int],
     dataset: bool,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]],
     ignore_index: bool,
-    parallelism: int,
+    ray_args: Optional[RaySettings],
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     if "iterator" in pandas_kwargs:
         raise exceptions.InvalidArgument("Please, use the chunksize argument instead of iterator.")
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-
     paths: List[str] = _path2list(
         path=path,
-        boto3_session=session,
+        s3_client=s3_client,
         suffix=path_suffix,
         ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=path_ignore_suffix),
         ignore_empty=ignore_empty,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         s3_additional_kwargs=s3_additional_kwargs,
     )
 
     path_root: Optional[str] = _get_path_root(path=path, dataset=dataset)
     if path_root is not None:
         paths = _apply_partition_filter(path_root=path_root, paths=paths, filter_func=partition_filter)
     if len(paths) < 1:
         raise exceptions.NoFilesFound(f"No files Found on: {path}.")
-    _logger.debug("paths:\n%s", paths)
+    _logger.debug("len(paths): %s", len(paths))
 
-    if len(paths) > 1 and version_id is not None and not isinstance(version_id, dict):
-        raise exceptions.InvalidArgumentCombination(
-            "If multiple paths are provided along with a file version ID, the version ID parameter must be a dict."
-        )
-    version_id_dict = {path: _get_version_id_for(version_id, path) for path in paths}
+    version_ids = _check_version_id(paths=paths, version_id=version_id)
 
     args: Dict[str, Any] = {
         "parser_func": _resolve_format(read_format),
-        "boto3_session": boto3_session,
+        "s3_client": s3_client,
         "dataset": dataset,
         "path_root": path_root,
         "pandas_kwargs": pandas_kwargs,
         "s3_additional_kwargs": s3_additional_kwargs,
         "use_threads": use_threads,
     }
     _logger.debug("args:\n%s", pprint.pformat(args))
 
     if chunksize is not None:
         return _read_text_files_chunked(
             paths=paths,
-            version_ids=version_id_dict,
+            version_ids=version_ids,
             chunksize=chunksize,
             **args,
         )
 
+    ray_args = ray_args if ray_args else {}
     return _read_text(
         read_format,
         paths=paths,
         path_root=path_root,
         use_threads=use_threads,
-        boto3_session=session,
+        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
         dataset=dataset,
         ignore_index=ignore_index,
-        parallelism=parallelism,
-        version_id_dict=version_id_dict,
+        parallelism=ray_args.get("parallelism", -1),
+        version_ids=version_ids,
         pandas_kwargs=pandas_kwargs,
     )
 
 
+@overload
+def read_csv(
+    path: Union[str, List[str]],
+    *,
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: None = ...,
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_csv(
+    path: Union[str, List[str]],
+    *,
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: int,
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_csv(
+    path: Union[str, List[str]],
+    *,
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: Optional[int],
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def read_csv(
     path: Union[str, List[str]],
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     ignore_empty: bool = True,
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     chunksize: Optional[int] = None,
     dataset: bool = False,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
-    parallelism: int = 200,
+    ray_args: Optional[RaySettings] = None,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Read CSV file(s) from a received S3 prefix or list of S3 objects paths.
 
     This function accepts Unix shell-style wildcards in the path argument.
     * (matches everything), ? (matches any single character),
     [seq] (matches any character in seq), [!seq] (matches any character not in seq).
@@ -221,20 +288,19 @@
     partition_filter : Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
-    parallelism : int, optional
-        The requested parallelism of the read. Only used when `distributed` add-on is installed.
-        Parallelism may be limited by the number of files of the dataset. 200 by default.
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+    ray_args: typing.RaySettings, optional
+        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs :
-        KEYWORD arguments forwarded to pandas.read_csv(). You can NOT pass `pandas_kwargs` explicit, just add valid
+        KEYWORD arguments forwarded to pandas.read_csv(). You can NOT pass `pandas_kwargs` explicitly, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', na_values=['null', 'none'], skip_blank_lines=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
 
     Returns
     -------
     Union[pandas.DataFrame, Generator[pandas.DataFrame, None, None]]
@@ -269,55 +335,124 @@
     >>> import awswrangler as wr
     >>> my_filter = lambda x: True if x["city"].startswith("new") else False
     >>> df = wr.s3.read_csv(path, dataset=True, partition_filter=my_filter)
 
     """
     if "pandas_kwargs" in pandas_kwargs:
         raise exceptions.InvalidArgument(
-            "You can NOT pass `pandas_kwargs` explicit, just add valid "
+            "You can NOT pass `pandas_kwargs` explicitly, just add valid "
             "Pandas arguments in the function call and awswrangler will accept it."
             "e.g. wr.s3.read_csv('s3://bucket/prefix/', sep='|', skip_blank_lines=True)"
         )
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     ignore_index: bool = "index_col" not in pandas_kwargs
     return _read_text_format(
         read_format="csv",
         path=path,
         path_suffix=path_suffix,
         path_ignore_suffix=path_ignore_suffix,
         version_id=version_id,
         ignore_empty=ignore_empty,
         use_threads=use_threads,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
         chunksize=chunksize,
         dataset=dataset,
         partition_filter=partition_filter,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         ignore_index=ignore_index,
-        parallelism=parallelism,
+        ray_args=ray_args,
         **pandas_kwargs,
     )
 
 
+@overload
+def read_fwf(
+    path: Union[str, List[str]],
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: None = ...,
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_fwf(
+    path: Union[str, List[str]],
+    *,
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: int,
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_fwf(
+    path: Union[str, List[str]],
+    *,
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: Optional[int],
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def read_fwf(
     path: Union[str, List[str]],
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     ignore_empty: bool = True,
     use_threads: Union[bool, int] = True,
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     chunksize: Optional[int] = None,
     dataset: bool = False,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
-    parallelism: int = 200,
+    ray_args: Optional[RaySettings] = None,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Read fixed-width formatted file(s) from a received S3 prefix or list of S3 objects paths.
 
     This function accepts Unix shell-style wildcards in the path argument.
     * (matches everything), ? (matches any single character),
     [seq] (matches any character in seq), [!seq] (matches any character not in seq).
@@ -374,18 +509,17 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
-    parallelism : int, optional
-        The requested parallelism of the read. Only used when `distributed` add-on is installed.
-        Parallelism may be limited by the number of files of the dataset. 200 by default.
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+    ray_args: typing.RaySettings, optional
+        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_fwf(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_fwf(path='s3://bucket/prefix/', widths=[1, 3], names=["c0", "c1"])
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_fwf.html
 
     Returns
@@ -426,36 +560,108 @@
     """
     if "pandas_kwargs" in pandas_kwargs:
         raise exceptions.InvalidArgument(
             "You can NOT pass `pandas_kwargs` explicit, just add valid "
             "Pandas arguments in the function call and awswrangler will accept it."
             "e.g. wr.s3.read_fwf(path, widths=[1, 3], names=['c0', 'c1'])"
         )
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     return _read_text_format(
         read_format="fwf",
         path=path,
         path_suffix=path_suffix,
         path_ignore_suffix=path_ignore_suffix,
         version_id=version_id,
         ignore_empty=ignore_empty,
         use_threads=use_threads,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
         chunksize=chunksize,
         dataset=dataset,
         partition_filter=partition_filter,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         ignore_index=True,
         sort_index=False,
-        parallelism=parallelism,
+        ray_args=ray_args,
         **pandas_kwargs,
     )
 
 
+@overload
+def read_json(
+    path: Union[str, List[str]],
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    orient: str = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: None = ...,
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> pd.DataFrame:
+    ...
+
+
+@overload
+def read_json(
+    path: Union[str, List[str]],
+    *,
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    orient: str = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: int,
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> Iterator[pd.DataFrame]:
+    ...
+
+
+@overload
+def read_json(
+    path: Union[str, List[str]],
+    *,
+    path_suffix: Union[str, List[str], None] = ...,
+    path_ignore_suffix: Union[str, List[str], None] = ...,
+    version_id: Optional[Union[str, Dict[str, str]]] = ...,
+    ignore_empty: bool = ...,
+    orient: str = ...,
+    use_threads: Union[bool, int] = ...,
+    last_modified_begin: Optional[datetime.datetime] = ...,
+    last_modified_end: Optional[datetime.datetime] = ...,
+    boto3_session: Optional[boto3.Session] = ...,
+    s3_additional_kwargs: Optional[Dict[str, Any]] = ...,
+    chunksize: Optional[int],
+    dataset: bool = ...,
+    partition_filter: Optional[Callable[[Dict[str, str]], bool]] = ...,
+    ray_args: Optional[RaySettings] = ...,
+    **pandas_kwargs: Any,
+) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
+    ...
+
+
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def read_json(
     path: Union[str, List[str]],
     path_suffix: Union[str, List[str], None] = None,
     path_ignore_suffix: Union[str, List[str], None] = None,
     version_id: Optional[Union[str, Dict[str, str]]] = None,
     ignore_empty: bool = True,
     orient: str = "columns",
@@ -463,15 +669,15 @@
     last_modified_begin: Optional[datetime.datetime] = None,
     last_modified_end: Optional[datetime.datetime] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     chunksize: Optional[int] = None,
     dataset: bool = False,
     partition_filter: Optional[Callable[[Dict[str, str]], bool]] = None,
-    parallelism: int = 200,
+    ray_args: Optional[RaySettings] = None,
     **pandas_kwargs: Any,
 ) -> Union[pd.DataFrame, Iterator[pd.DataFrame]]:
     """Read JSON file(s) from a received S3 prefix or list of S3 objects paths.
 
     This function accepts Unix shell-style wildcards in the path argument.
     * (matches everything), ? (matches any single character),
     [seq] (matches any character in seq), [!seq] (matches any character not in seq).
@@ -531,18 +737,17 @@
     partition_filter: Optional[Callable[[Dict[str, str]], bool]]
         Callback Function filters to apply on PARTITION columns (PUSH-DOWN filter).
         This function MUST receive a single argument (Dict[str, str]) where keys are partitions
         names and values are partitions values. Partitions values will be always strings extracted from S3.
         This function MUST return a bool, True to read the partition or False to ignore it.
         Ignored if `dataset=False`.
         E.g ``lambda x: True if x["year"] == "2020" and x["month"] == "1" else False``
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
-    parallelism : int, optional
-        The requested parallelism of the read. Only used when `distributed` add-on is installed.
-        Parallelism may be limited by the number of files of the dataset. 200 by default.
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/023%20-%20Flexible%20Partitions%20Filter.html
+    ray_args: typing.RaySettings, optional
+        Params of the Ray Modin settings. Only used when distributed computing is used with Ray and Modin installed.
     pandas_kwargs:
         KEYWORD arguments forwarded to pandas.read_json(). You can NOT pass `pandas_kwargs` explicit, just add valid
         Pandas arguments in the function call and awswrangler will accept it.
         e.g. wr.s3.read_json('s3://bucket/prefix/', lines=True, keep_default_dates=True)
         https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_json.html
 
     Returns
@@ -583,30 +788,31 @@
     """
     if "pandas_kwargs" in pandas_kwargs:
         raise exceptions.InvalidArgument(
             "You can NOT pass `pandas_kwargs` explicit, just add valid "
             "Pandas arguments in the function call and awswrangler will accept it."
             "e.g. wr.s3.read_json(path, lines=True, keep_default_dates=True)"
         )
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     if (dataset is True) and ("lines" not in pandas_kwargs):
         pandas_kwargs["lines"] = True
     pandas_kwargs["orient"] = orient
     ignore_index: bool = orient not in ("split", "index", "columns")
     return _read_text_format(
         read_format="json",
         path=path,
         path_suffix=path_suffix,
         path_ignore_suffix=path_ignore_suffix,
         version_id=version_id,
         ignore_empty=ignore_empty,
         use_threads=use_threads,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
         chunksize=chunksize,
         dataset=dataset,
         partition_filter=partition_filter,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         ignore_index=ignore_index,
-        parallelism=parallelism,
+        ray_args=ray_args,
         **pandas_kwargs,
     )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_select.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_select.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,92 +1,101 @@
 """Amazon S3 Select Module (PRIVATE)."""
 
 import datetime
 import itertools
 import json
 import logging
 import pprint
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Tuple, Union
 
 import boto3
 import pandas as pd
 import pyarrow as pa
 
 from awswrangler import _data_types, _utils, exceptions
 from awswrangler._distributed import engine
-from awswrangler._threading import _get_executor
+from awswrangler._threading import _get_executor, _ThreadPoolExecutor
 from awswrangler.distributed.ray import ray_get
 from awswrangler.s3._describe import size_objects
 from awswrangler.s3._list import _path2list
 from awswrangler.s3._read import _get_path_ignore_suffix
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 _RANGE_CHUNK_SIZE: int = int(1024 * 1024)
 
 
-def _flatten_list(elements: List[List[Any]]) -> List[Any]:
-    return [item for sublist in elements for item in sublist]
-
-
 def _gen_scan_range(obj_size: int, scan_range_chunk_size: Optional[int] = None) -> Iterator[Tuple[int, int]]:
     chunk_size = scan_range_chunk_size or _RANGE_CHUNK_SIZE
     for i in range(0, obj_size, chunk_size):
         yield (i, i + min(chunk_size, obj_size - i))
 
 
 @engine.dispatch_on_engine
+@_utils.retry(
+    ex=exceptions.S3SelectRequestIncomplete,
+)
 def _select_object_content(
-    boto3_session: Optional[boto3.Session],
+    s3_client: Optional["S3Client"],
     args: Dict[str, Any],
     scan_range: Optional[Tuple[int, int]] = None,
 ) -> pa.Table:
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-
+    client_s3: "S3Client" = s3_client if s3_client else _utils.client(service_name="s3")
     if scan_range:
-        _logger.debug("scan_range: %s, key: %s", scan_range, args["Key"])
         response = client_s3.select_object_content(**args, ScanRange={"Start": scan_range[0], "End": scan_range[1]})
     else:
         response = client_s3.select_object_content(**args)
 
     payload_records = []
     partial_record: str = ""
     request_complete: bool = False
     for event in response["Payload"]:
         if "Records" in event:
-            records = event["Records"]["Payload"].decode(encoding="utf-8", errors="ignore").split("\n")
+            records = (
+                event["Records"]["Payload"]  # type: ignore[index]
+                .decode(  # type: ignore[attr-defined]
+                    encoding="utf-8",
+                    errors="ignore",
+                )
+                .split("\n")
+            )
             records[0] = partial_record + records[0]
             # Record end can either be a partial record or a return char
             partial_record = records.pop()
             payload_records.extend([json.loads(record) for record in records])
         elif "End" in event:
             # End Event signals the request was successful
             _logger.debug("Received End Event. Result is complete")
             request_complete = True
     # If the End Event is not received, the results may be incomplete
     if not request_complete:
-        raise Exception(f"S3 Select request for path {args['Key']} is incomplete as End Event was not received")
+        raise exceptions.S3SelectRequestIncomplete(
+            f"S3 Select request for path {args['Key']} is incomplete as End Event was not received"
+        )
 
     return _utils.list_to_arrow_table(mapping=payload_records)
 
 
 @engine.dispatch_on_engine
 def _select_query(
     path: str,
-    executor: Any,
+    executor: _ThreadPoolExecutor,
     sql: str,
     input_serialization: str,
     input_serialization_params: Dict[str, Union[bool, str]],
     compression: Optional[str] = None,
     scan_range_chunk_size: Optional[int] = None,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
 ) -> List[pa.Table]:
     bucket, key = _utils.parse_path(path)
-
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     args: Dict[str, Any] = {
         "Bucket": bucket,
         "Key": key,
         "Expression": sql,
         "ExpressionType": "SQL",
         "RequestProgress": {"Enabled": False},
         "InputSerialization": {
@@ -97,15 +106,15 @@
             "JSON": {},
         },
     }
     if s3_additional_kwargs:
         args.update(s3_additional_kwargs)
     _logger.debug("args:\n%s", pprint.pformat(args))
 
-    obj_size: int = size_objects(  # type: ignore
+    obj_size: int = size_objects(  # type: ignore[assignment]
         path=[path],
         use_threads=False,
         boto3_session=boto3_session,
     ).get(path)
     if obj_size is None:
         raise exceptions.InvalidArgumentValue(f"S3 object w/o defined size: {path}")
     scan_ranges: Iterator[Optional[Tuple[int, int]]] = _gen_scan_range(
@@ -115,19 +124,22 @@
         [
             compression,
             input_serialization_params.get("AllowQuotedRecordDelimiter"),
             input_serialization_params.get("Type") == "Document",
         ]
     ):  # Scan range is only supported for uncompressed CSV/JSON, CSV (without quoted delimiters)
         # and JSON objects (in LINES mode only)
-        scan_ranges = [None]  # type: ignore
+        scan_ranges = [None]  # type: ignore[assignment]
 
-    return executor.map(_select_object_content, boto3_session, itertools.repeat(args), scan_ranges)  # type: ignore
+    return executor.map(_select_object_content, s3_client, itertools.repeat(args), scan_ranges)
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def select_query(
     sql: str,
     path: Union[str, List[str]],
     input_serialization: str,
     input_serialization_params: Dict[str, Union[bool, str]],
     compression: Optional[str] = None,
     scan_range_chunk_size: Optional[int] = None,
@@ -239,37 +251,39 @@
         raise exceptions.InvalidArgumentValue("<input_serialization> argument must be 'CSV', 'JSON' or 'Parquet'")
     if compression not in [None, "gzip", "bzip2"]:
         raise exceptions.InvalidCompression(f"Invalid {compression} compression, please use None, 'gzip' or 'bzip2'.")
     if compression and (input_serialization not in ["CSV", "JSON"]):
         raise exceptions.InvalidArgumentCombination(
             "'gzip' or 'bzip2' are only valid for input 'CSV' or 'JSON' objects."
         )
-
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     paths: List[str] = _path2list(
         path=path,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
         suffix=path_suffix,
         ignore_suffix=_get_path_ignore_suffix(path_ignore_suffix=path_ignore_suffix),
         ignore_empty=ignore_empty,
         last_modified_begin=last_modified_begin,
         last_modified_end=last_modified_end,
         s3_additional_kwargs=s3_additional_kwargs,
     )
     if len(paths) < 1:
         raise exceptions.NoFilesFound(f"No files Found: {path}.")
-    _logger.debug("paths:\n%s", paths)
+    _logger.debug("len(paths): %s", len(paths))
 
     select_kwargs: Dict[str, Any] = {
         "sql": sql,
         "input_serialization": input_serialization,
         "input_serialization_params": input_serialization_params,
         "compression": compression,
         "scan_range_chunk_size": scan_range_chunk_size,
         "boto3_session": boto3_session,
         "s3_additional_kwargs": s3_additional_kwargs,
     }
     _logger.debug("kwargs:\n%s", pprint.pformat(select_kwargs))
 
     arrow_kwargs = _data_types.pyarrow2pandas_defaults(use_threads=use_threads, kwargs=pyarrow_additional_kwargs)
     executor = _get_executor(use_threads=use_threads)
-    tables = _flatten_list(ray_get([_select_query(path=path, executor=executor, **select_kwargs) for path in paths]))
+    tables = list(
+        itertools.chain(*ray_get([_select_query(path=path, executor=executor, **select_kwargs) for path in paths]))
+    )
     return _utils.table_refs_to_df(tables, kwargs=arrow_kwargs)
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_upload.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Amazon S3 Upload Module (PRIVATE)."""
 
 import logging
 from typing import Any, Dict, Optional, Union
 
 import boto3
 
-from awswrangler import _utils
 from awswrangler.s3._fs import open_s3_object
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
 def upload(
     local_file: Union[str, Any],
@@ -54,24 +53,23 @@
     Uploading a file using a file-like object
 
     >>> import awswrangler as wr
     >>> with open(file='./key', mode='wb') as local_f:
     >>>     wr.s3.upload(local_file=local_f, path='s3://bucket/key')
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     _logger.debug("path: %s", path)
     with open_s3_object(
         path=path,
         mode="wb",
         use_threads=use_threads,
         s3_block_size=-1,  # One shot download
         s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=session,
+        boto3_session=boto3_session,
     ) as s3_f:
         if isinstance(local_file, str):
             _logger.debug("Uploading local_file: %s", local_file)
             with open(file=local_file, mode="rb") as local_f:
-                s3_f.write(local_f.read())
+                s3_f.write(local_f.read())  # type: ignore[arg-type]
         else:
             _logger.debug("Uploading file-like object.")
             s3_f.write(local_file.read())
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_wait.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_wait.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 """Amazon S3 Wait Module (PRIVATE)."""
 
 import itertools
 import logging
-from typing import List, Optional, Union
+from typing import TYPE_CHECKING, List, Optional, Union
 
 import boto3
 
 from awswrangler import _utils
 from awswrangler._distributed import engine
 from awswrangler._threading import _get_executor
 from awswrangler.distributed.ray import ray_get
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _wait_object(
-    boto3_session: Optional[boto3.Session], path: str, waiter_name: str, delay: int, max_attempts: int
-) -> None:
-    client_s3: boto3.client = _utils.client(service_name="s3", session=boto3_session)
-    waiter = client_s3.get_waiter(waiter_name)
+def _wait_object(s3_client: "S3Client", path: str, waiter_name: str, delay: int, max_attempts: int) -> None:
+    waiter = s3_client.get_waiter(waiter_name)  # type: ignore[call-overload]
 
     bucket, key = _utils.parse_path(path=path)
     waiter.wait(Bucket=bucket, Key=key, WaiterConfig={"Delay": delay, "MaxAttempts": max_attempts})
 
 
 @engine.dispatch_on_engine
 def _wait_object_batch(
-    boto3_session: Optional[boto3.Session], paths: List[str], waiter_name: str, delay: int, max_attempts: int
+    s3_client: Optional["S3Client"], paths: List[str], waiter_name: str, delay: int, max_attempts: int
 ) -> None:
+    s3_client = s3_client if s3_client else _utils.client(service_name="s3")
     for path in paths:
-        _wait_object(boto3_session, path, waiter_name, delay, max_attempts)
+        _wait_object(s3_client, path, waiter_name, delay, max_attempts)
 
 
 def _wait_objects(
     waiter_name: str,
     paths: List[str],
     delay: Optional[float],
     max_attempts: Optional[int],
     use_threads: Union[bool, int],
     parallelism: Optional[int],
-    boto3_session: Optional[boto3.Session],
+    s3_client: "S3Client",
 ) -> None:
     delay = 5 if delay is None else delay
     max_attempts = 20 if max_attempts is None else max_attempts
     parallelism = 100 if parallelism is None else parallelism
 
     if len(paths) < 1:
         return None
@@ -54,25 +55,28 @@
         else _utils.chunkify(paths, max_length=1)
     )
 
     executor = _get_executor(use_threads=use_threads)
     ray_get(
         executor.map(
             _wait_object_batch,
-            boto3_session,
+            s3_client,
             path_batches,
             itertools.repeat(waiter_name),
             itertools.repeat(int(delay)),
             itertools.repeat(max_attempts),
         )
     )
 
     return None
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def wait_objects_exist(
     paths: List[str],
     delay: Optional[float] = None,
     max_attempts: Optional[int] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     parallelism: Optional[int] = None,
@@ -113,25 +117,29 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.s3.wait_objects_exist(['s3://bucket/key0', 's3://bucket/key1'])  # wait both objects
 
     """
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     return _wait_objects(
         waiter_name="object_exists",
         paths=paths,
         delay=delay,
         max_attempts=max_attempts,
         use_threads=use_threads,
         parallelism=parallelism,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
     )
 
 
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
 def wait_objects_not_exist(
     paths: List[str],
     delay: Optional[float] = None,
     max_attempts: Optional[int] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     parallelism: Optional[int] = None,
@@ -172,16 +180,17 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> wr.s3.wait_objects_not_exist(['s3://bucket/key0', 's3://bucket/key1'])  # wait both objects not exist
 
     """
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
     return _wait_objects(
         waiter_name="object_not_exists",
         paths=paths,
         delay=delay,
         max_attempts=max_attempts,
         use_threads=use_threads,
         parallelism=parallelism,
-        boto3_session=boto3_session,
+        s3_client=s3_client,
     )
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_write_excel.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_write_excel.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 
 import boto3
 import pandas as pd
 
 from awswrangler import _utils, exceptions
 from awswrangler.s3._fs import open_s3_object
 
+openpyxl = _utils.import_optional_dependency("openpyxl")
+
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
+@_utils.check_optional_dependency(openpyxl, "openpyxl")
 def to_excel(
     df: pd.DataFrame,
     path: str,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     use_threads: Union[bool, int] = True,
     **pandas_kwargs: Any,
@@ -26,15 +29,15 @@
     ----
     This function accepts any Pandas's read_excel() argument.
     https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_excel.html
 
     Note
     ----
     Depending on the file extension ('xlsx', 'xls', 'odf'...), an additional library
-    might have to be installed first (e.g. xlrd).
+    might have to be installed first.
 
     Note
     ----
     In case of `use_threads=True` the number of threads
     that will be spawned will be gotten from os.cpu_count().
 
     Parameters
@@ -75,18 +78,17 @@
     if "pandas_kwargs" in pandas_kwargs:
         raise exceptions.InvalidArgument(
             "You can NOT pass `pandas_kwargs` explicit, just add valid "
             "Pandas arguments in the function call and awswrangler will accept it."
             "e.g. wr.s3.to_excel(df, path, na_rep="
             ", index=False)"
         )
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
     with open_s3_object(
         path=path,
         mode="wb",
         use_threads=use_threads,
         s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=session,
+        boto3_session=boto3_session,
     ) as f:
         _logger.debug("pandas_kwargs: %s", pandas_kwargs)
         df.to_excel(f, **pandas_kwargs)
     return path
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/s3/_write_parquet.py` & `awswrangler-3.0.0rc3/awswrangler/s3/_write_text.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,453 +1,383 @@
-"""Amazon PARQUET S3 Parquet Write Module (PRIVATE)."""
+"""Amazon S3 Text Write Module (PRIVATE)."""
 
+import csv
 import logging
-import math
 import uuid
-from contextlib import contextmanager
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union, cast
 
 import boto3
 import pandas as pd
-import pyarrow as pa
-import pyarrow.lib
-import pyarrow.parquet
+from pandas.io.common import infer_compression
 
-from awswrangler import _data_types, _utils, catalog, exceptions, lakeformation
-from awswrangler._arrow import _df_to_table
+from awswrangler import _data_types, _utils, catalog, exceptions, lakeformation, typing
 from awswrangler._config import apply_configs
 from awswrangler._distributed import engine
+from awswrangler._utils import copy_df_shallow
 from awswrangler.s3._delete import delete_objects
 from awswrangler.s3._fs import open_s3_object
-from awswrangler.s3._read_parquet import _read_parquet_metadata
 from awswrangler.s3._write import _COMPRESSION_2_EXT, _apply_dtype, _sanitize, _validate_args
-from awswrangler.s3._write_concurrent import _WriteProxy
 from awswrangler.s3._write_dataset import _to_dataset
+from awswrangler.typing import BucketingInfoTuple, GlueTableSettings, _S3WriteDataReturnValue
+
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
 
-def _get_file_path(
-    path_root: Optional[str] = None,
+def _get_write_details(path: str, pandas_kwargs: Dict[str, Any]) -> Tuple[str, Optional[str], Optional[str]]:
+    if pandas_kwargs.get("compression", "infer") == "infer":
+        pandas_kwargs["compression"] = infer_compression(path, compression="infer")
+    mode: str = "w" if pandas_kwargs.get("compression") is None else "wb"
+    encoding: Optional[str] = pandas_kwargs.get("encoding", "utf-8")
+    newline: Optional[str] = pandas_kwargs.get("lineterminator", "")
+    return mode, encoding, newline
+
+
+@engine.dispatch_on_engine
+def _to_text(  # pylint: disable=unused-argument
+    df: pd.DataFrame,
+    file_format: str,
+    use_threads: Union[bool, int],
+    s3_client: Optional["S3Client"],
+    s3_additional_kwargs: Optional[Dict[str, str]],
     path: Optional[str] = None,
+    path_root: Optional[str] = None,
     filename_prefix: Optional[str] = None,
-    compression_ext: str = "",
-    bucket_id: Optional[int] = None,
-    extension: str = ".parquet",
-) -> str:
-    if bucket_id is not None:
-        filename_prefix = f"{filename_prefix}_bucket-{bucket_id:05d}"
+    bucketing: bool = False,
+    **pandas_kwargs: Any,
+) -> List[str]:
+    s3_client = s3_client if s3_client else _utils.client(service_name="s3")
+    if df.empty is True:
+        raise exceptions.EmptyDataFrame("DataFrame cannot be empty.")
     if path is None and path_root is not None:
-        file_path: str = f"{path_root}{filename_prefix}{compression_ext}{extension}"
+        file_path: str = (
+            f"{path_root}{filename_prefix}.{file_format}{_COMPRESSION_2_EXT.get(pandas_kwargs.get('compression'))}"
+        )
     elif path is not None and path_root is None:
         file_path = path
     else:
         raise RuntimeError("path and path_root received at the same time.")
-    return file_path
 
-
-def _get_chunk_file_path(file_counter: int, file_path: str) -> str:
-    slash_index: int = file_path.rfind("/")
-    dot_index: int = file_path.find(".", slash_index)
-    file_index: str = "_" + str(file_counter)
-    if dot_index == -1:
-        file_path = file_path + file_index
-    else:
-        file_path = file_path[:dot_index] + file_index + file_path[dot_index:]
-    return file_path
-
-
-@contextmanager
-def _new_writer(
-    file_path: str,
-    compression: Optional[str],
-    pyarrow_additional_kwargs: Dict[str, str],
-    schema: pa.Schema,
-    boto3_session: boto3.Session,
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    use_threads: Union[bool, int],
-) -> Iterator[pyarrow.parquet.ParquetWriter]:
-    writer: Optional[pyarrow.parquet.ParquetWriter] = None
+    mode, encoding, newline = _get_write_details(path=file_path, pandas_kwargs=pandas_kwargs)
     with open_s3_object(
         path=file_path,
-        mode="wb",
+        mode=mode,
         use_threads=use_threads,
+        s3_client=s3_client,
         s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=boto3_session,
+        encoding=encoding,
+        newline=newline,
     ) as f:
-        try:
-            writer = pyarrow.parquet.ParquetWriter(
-                where=f,
-                write_statistics=True,
-                use_dictionary=True,
-                compression="NONE" if compression is None else compression,
-                schema=schema,
-                **pyarrow_additional_kwargs,
-            )
-            yield writer
-        finally:
-            if writer is not None and writer.is_open is True:
-                writer.close()
-
-
-def _write_chunk(
-    file_path: str,
-    boto3_session: Optional[boto3.Session],
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    compression: Optional[str],
-    pyarrow_additional_kwargs: Dict[str, str],
-    table: pa.Table,
-    offset: int,
-    chunk_size: int,
-    use_threads: Union[bool, int],
-) -> List[str]:
-    with _new_writer(
-        file_path=file_path,
-        compression=compression,
-        pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-        schema=table.schema,
-        boto3_session=boto3_session,
-        s3_additional_kwargs=s3_additional_kwargs,
-        use_threads=use_threads,
-    ) as writer:
-        writer.write_table(table.slice(offset, chunk_size))
+        _logger.debug("pandas_kwargs: %s", pandas_kwargs)
+        if file_format == "csv":
+            df.to_csv(f, mode=mode, **pandas_kwargs)
+        elif file_format == "json":
+            df.to_json(f, **pandas_kwargs)
     return [file_path]
 
 
-def _to_parquet_chunked(
-    file_path: str,
-    boto3_session: Optional[boto3.Session],
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    compression: Optional[str],
-    pyarrow_additional_kwargs: Dict[str, Any],
-    table: pa.Table,
-    max_rows_by_file: int,
-    num_of_rows: int,
-    cpus: int,
-) -> List[str]:
-    chunks: int = math.ceil(num_of_rows / max_rows_by_file)
-    use_threads: Union[bool, int] = cpus > 1
-    proxy: _WriteProxy = _WriteProxy(use_threads=use_threads)
-    for chunk in range(chunks):
-        offset: int = chunk * max_rows_by_file
-        write_path: str = _get_chunk_file_path(chunk, file_path)
-        proxy.write(
-            func=_write_chunk,
-            file_path=write_path,
-            boto3_session=boto3_session,
-            s3_additional_kwargs=s3_additional_kwargs,
-            compression=compression,
-            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            table=table,
-            offset=offset,
-            chunk_size=max_rows_by_file,
-            use_threads=use_threads,
-        )
-    return proxy.close()  # blocking
-
-
-@engine.dispatch_on_engine
-def _to_parquet(
-    df: pd.DataFrame,
-    schema: pa.Schema,
-    index: bool,
-    compression: Optional[str],
-    compression_ext: str,
-    pyarrow_additional_kwargs: Dict[str, Any],
-    cpus: int,
-    dtype: Dict[str, str],
-    boto3_session: Optional[boto3.Session],
-    s3_additional_kwargs: Optional[Dict[str, str]],
-    use_threads: Union[bool, int],
-    path: Optional[str] = None,
-    path_root: Optional[str] = None,
-    filename_prefix: Optional[str] = None,
-    max_rows_by_file: Optional[int] = 0,
-) -> List[str]:
-    file_path = _get_file_path(
-        path_root=path_root, path=path, filename_prefix=filename_prefix, compression_ext=compression_ext
-    )
-    _logger.debug("file_path: %s", file_path)
-    table: pa.Table = _df_to_table(df, schema, index, dtype)
-    if max_rows_by_file is not None and max_rows_by_file > 0:
-        paths: List[str] = _to_parquet_chunked(
-            file_path=file_path,
-            boto3_session=boto3_session,
-            s3_additional_kwargs=s3_additional_kwargs,
-            compression=compression,
-            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            table=table,
-            max_rows_by_file=max_rows_by_file,
-            num_of_rows=df.shape[0],
-            cpus=cpus,
-        )
-    else:
-        with _new_writer(
-            file_path=file_path,
-            compression=compression,
-            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            schema=table.schema,
-            boto3_session=boto3_session,
-            s3_additional_kwargs=s3_additional_kwargs,
-            use_threads=use_threads,
-        ) as writer:
-            writer.write_table(table)
-        paths = [file_path]
-    return paths
-
-
 @apply_configs
-def to_parquet(  # pylint: disable=too-many-arguments,too-many-locals,too-many-branches,too-many-statements
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
+def to_csv(  # pylint: disable=too-many-arguments,too-many-locals,too-many-statements,too-many-branches
     df: pd.DataFrame,
     path: Optional[str] = None,
-    index: bool = False,
-    compression: Optional[str] = "snappy",
-    pyarrow_additional_kwargs: Optional[Dict[str, Any]] = None,
-    max_rows_by_file: Optional[int] = None,
+    sep: str = ",",
+    index: bool = True,
+    columns: Optional[List[str]] = None,
     use_threads: Union[bool, int] = True,
     boto3_session: Optional[boto3.Session] = None,
     s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     sanitize_columns: bool = False,
     dataset: bool = False,
     filename_prefix: Optional[str] = None,
     partition_cols: Optional[List[str]] = None,
-    bucketing_info: Optional[Tuple[List[str], int]] = None,
+    bucketing_info: Optional[BucketingInfoTuple] = None,
     concurrent_partitioning: bool = False,
     mode: Optional[str] = None,
     catalog_versioning: bool = False,
-    schema_evolution: bool = True,
+    schema_evolution: bool = False,
+    dtype: Optional[Dict[str, str]] = None,
     database: Optional[str] = None,
     table: Optional[str] = None,
-    table_type: Optional[str] = None,
-    transaction_id: Optional[str] = None,
-    dtype: Optional[Dict[str, str]] = None,
-    description: Optional[str] = None,
-    parameters: Optional[Dict[str, str]] = None,
-    columns_comments: Optional[Dict[str, str]] = None,
-    regular_partitions: bool = True,
-    projection_enabled: bool = False,
-    projection_types: Optional[Dict[str, str]] = None,
-    projection_ranges: Optional[Dict[str, str]] = None,
-    projection_values: Optional[Dict[str, str]] = None,
-    projection_intervals: Optional[Dict[str, str]] = None,
-    projection_digits: Optional[Dict[str, str]] = None,
-    projection_formats: Optional[Dict[str, str]] = None,
-    projection_storage_location_template: Optional[str] = None,
+    glue_table_settings: Optional[GlueTableSettings] = None,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
     catalog_id: Optional[str] = None,
-) -> Dict[str, Union[List[str], Dict[str, List[str]]]]:
-    """Write Parquet file or dataset on Amazon S3.
+    **pandas_kwargs: Any,
+) -> _S3WriteDataReturnValue:
+    """Write CSV file or dataset on Amazon S3.
 
     The concept of Dataset goes beyond the simple idea of ordinary files and enable more
     complex features like partitioning and catalog integration (Amazon Athena/AWS Glue Catalog).
 
     Note
     ----
-    This operation may mutate the original pandas dataframe in-place. To avoid this behaviour
-    please pass in a deep copy instead (i.e. `df.copy()`)
+    If database` and `table` arguments are passed, the table name and all column names
+    will be automatically sanitized using `wr.catalog.sanitize_table_name` and `wr.catalog.sanitize_column_name`.
+    Please, pass `sanitize_columns=True` to enforce this behaviour always.
 
     Note
     ----
-    If `database` and `table` arguments are passed, the table name and all column names
-    will be automatically sanitized using `wr.catalog.sanitize_table_name` and `wr.catalog.sanitize_column_name`.
-    Please, pass `sanitize_columns=True` to enforce this behaviour always.
+    If `table` and `database` arguments are passed, `pandas_kwargs` will be ignored due
+    restrictive quoting, date_format, escapechar and encoding required by Athena/Glue Catalog.
+
+    Note
+    ----
+    Compression: The minimum acceptable version to achieve it is Pandas 1.2.0 that requires Python >= 3.7.1.
 
     Note
     ----
     In case of `use_threads=True` the number of threads
     that will be spawned will be gotten from os.cpu_count().
 
     Parameters
     ----------
     df: pandas.DataFrame
         Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
     path : str, optional
-        S3 path (for file e.g. ``s3://bucket/prefix/filename.parquet``) (for dataset e.g. ``s3://bucket/prefix``).
-        Required if dataset=False or when dataset=True and creating a new dataset
+        Amazon S3 path (e.g. s3://bucket/prefix/filename.csv) (for dataset e.g. ``s3://bucket/prefix``).
+        Required if dataset=False or when creating a new dataset
+    sep : str
+        String of length 1. Field delimiter for the output file.
     index : bool
-        True to store the DataFrame index in file, otherwise False to ignore it.
-        Is not supported in conjunction with `max_rows_by_file` when running the library with Ray/Modin.
-    compression: str, optional
-        Compression style (``None``, ``snappy``, ``gzip``, ``zstd``).
-    pyarrow_additional_kwargs : Optional[Dict[str, Any]]
-        Additional parameters forwarded to pyarrow.
-        e.g. pyarrow_additional_kwargs={'coerce_timestamps': 'ns', 'use_deprecated_int96_timestamps': False,
-        'allow_truncated_timestamps'=False}
-    max_rows_by_file : int
-        Max number of rows in each file.
-        Default is None i.e. dont split the files.
-        (e.g. 33554432, 268435456)
-        Is not supported in conjuction with `index=True` when running the library with Ray/Modin.
+        Write row names (index).
+    columns : Optional[List[str]]
+        Columns to write.
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
     boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
+        Boto3 Session. The default boto3 Session will be used if boto3_session receive None.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'ServerSideEncryption': 'aws:kms', 'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'}
     sanitize_columns : bool
-        True to sanitize columns names (using `wr.catalog.sanitize_table_name` and `wr.catalog.sanitize_column_name`)
-        or False to keep it as is.
-        True value behaviour is enforced if `database` and `table` arguments are passed.
+        True to sanitize columns names or False to keep it as is.
+        True value is forced if `dataset=True`.
     dataset : bool
-        If True store a parquet dataset instead of a ordinary file(s)
+        If True store as a dataset instead of ordinary file(s)
         If True, enable all follow arguments:
         partition_cols, mode, database, table, description, parameters, columns_comments, concurrent_partitioning,
-        catalog_versioning, projection_enabled, projection_types, projection_ranges, projection_values,
-        projection_intervals, projection_digits, catalog_id, schema_evolution.
+        catalog_versioning, projection_params, catalog_id, schema_evolution.
     filename_prefix: str, optional
         If dataset=True, add a filename prefix to the output files.
     partition_cols: List[str], optional
         List of column names that will be used to create partitions. Only takes effect if dataset=True.
     bucketing_info: Tuple[List[str], int], optional
         Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
         second element.
         Only `str`, `int` and `bool` are supported as column data types for bucketing.
     concurrent_partitioning: bool
         If True will increase the parallelism level during the partitions writing. It will decrease the
         writing time and increase the memory usage.
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
-    mode: str, optional
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+    mode : str, optional
         ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
         For details check the related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/tutorials/004%20-%20Parquet%20Datasets.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
     catalog_versioning : bool
         If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
     schema_evolution : bool
-        If True allows schema evolution (new or missing columns), otherwise a exception will be raised. True by default.
-        (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
+        If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
+        (Only considered if dataset=True and mode in ("append", "overwrite_partitions")). False by default.
         Related tutorial:
-        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/tutorials/014%20-%20Schema%20Evolution.html
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/014%20-%20Schema%20Evolution.html
     database : str, optional
         Glue/Athena catalog: Database name.
     table : str, optional
         Glue/Athena catalog: Table name.
-    table_type: str, optional
-        The type of the Glue Table. Set to EXTERNAL_TABLE if None.
-    transaction_id: str, optional
-        The ID of the transaction when writing to a Governed Table.
+    glue_table_settings: dict (GlueTableSettings), optional
+        Settings for writing to the Glue table.
     dtype : Dict[str, str], optional
         Dictionary of columns names and Athena/Glue types to be casted.
         Useful when you have columns with undetermined or mixed data types.
         (e.g. {'col name': 'bigint', 'col2 name': 'int'})
-    description : str, optional
-        Glue/Athena catalog: Table description
-    parameters : Dict[str, str], optional
-        Glue/Athena catalog: Key/value pairs to tag the table.
-    columns_comments : Dict[str, str], optional
-        Glue/Athena catalog:
-        Columns names and the related comments (e.g. {'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}).
-    regular_partitions : bool
-        Create regular partitions (Non projected partitions) on Glue Catalog.
-        Disable when you will work only with Partition Projection.
-        Keep enabled even when working with projections is useful to keep
-        Redshift Spectrum working with the regular partitions.
-    projection_enabled : bool
-        Enable Partition Projection on Athena (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html)
-    projection_types : Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections types.
-        Valid types: "enum", "integer", "date", "injected"
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
-    projection_ranges: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections ranges.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
-    projection_values: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections values.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
-    projection_intervals: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections intervals.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '5'})
-    projection_digits: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections digits.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '2'})
-    projection_formats: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections formats.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
-    projection_storage_location_template: Optional[str]
-        Value which is allows Athena to properly map partition values if the S3 file locations do not follow
-        a typical `.../column=value/...` pattern.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
-        (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
     catalog_id : str, optional
         The ID of the Data Catalog from which to retrieve Databases.
         If none is provided, the AWS account ID is used by default.
+    pandas_kwargs :
+        KEYWORD arguments forwarded to pandas.DataFrame.to_csv(). You can NOT pass `pandas_kwargs` explicit, just add
+        valid Pandas arguments in the function call and awswrangler will accept it.
+        e.g. wr.s3.to_csv(df, path, sep='|', na_rep='NULL', decimal=',')
+        https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html
 
     Returns
     -------
-    Dict[str, Union[List[str], Dict[str, List[str]]]]
+    wr.typing._S3WriteDataReturnValue
         Dictionary with:
         'paths': List of all stored files paths on S3.
         'partitions_values': Dictionary of partitions added with keys as S3 path locations
         and values as a list of partitions values as str.
 
     Examples
     --------
     Writing single file
 
     >>> import awswrangler as wr
     >>> import pandas as pd
-    >>> wr.s3.to_parquet(
+    >>> wr.s3.to_csv(
     ...     df=pd.DataFrame({'col': [1, 2, 3]}),
-    ...     path='s3://bucket/prefix/my_file.parquet',
+    ...     path='s3://bucket/prefix/my_file.csv',
     ... )
     {
-        'paths': ['s3://bucket/prefix/my_file.parquet'],
+        'paths': ['s3://bucket/prefix/my_file.csv'],
+        'partitions_values': {}
+    }
+
+    Writing single file with pandas_kwargs
+
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> wr.s3.to_csv(
+    ...     df=pd.DataFrame({'col': [1, 2, 3]}),
+    ...     path='s3://bucket/prefix/my_file.csv',
+    ...     sep='|',
+    ...     na_rep='NULL',
+    ...     decimal=','
+    ... )
+    {
+        'paths': ['s3://bucket/prefix/my_file.csv'],
         'partitions_values': {}
     }
 
     Writing single file encrypted with a KMS key
 
     >>> import awswrangler as wr
     >>> import pandas as pd
-    >>> wr.s3.to_parquet(
+    >>> wr.s3.to_csv(
     ...     df=pd.DataFrame({'col': [1, 2, 3]}),
-    ...     path='s3://bucket/prefix/my_file.parquet',
+    ...     path='s3://bucket/prefix/my_file.csv',
     ...     s3_additional_kwargs={
     ...         'ServerSideEncryption': 'aws:kms',
     ...         'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'
     ...     }
     ... )
     {
-        'paths': ['s3://bucket/prefix/my_file.parquet'],
+        'paths': ['s3://bucket/prefix/my_file.csv'],
         'partitions_values': {}
     }
 
     Writing partitioned dataset
 
     >>> import awswrangler as wr
     >>> import pandas as pd
-    >>> wr.s3.to_parquet(
+    >>> wr.s3.to_csv(
     ...     df=pd.DataFrame({
     ...         'col': [1, 2, 3],
     ...         'col2': ['A', 'A', 'B']
     ...     }),
     ...     path='s3://bucket/prefix',
     ...     dataset=True,
     ...     partition_cols=['col2']
     ... )
     {
-        'paths': ['s3://.../col2=A/x.parquet', 's3://.../col2=B/y.parquet'],
+        'paths': ['s3://.../col2=A/x.csv', 's3://.../col2=B/y.csv'],
         'partitions_values: {
             's3://.../col2=A/': ['A'],
             's3://.../col2=B/': ['B']
         }
     }
 
+    Writing partitioned dataset with partition projection
+
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> from datetime import datetime
+    >>> dt = lambda x: datetime.strptime(x, "%Y-%m-%d").date()
+    >>> wr.s3.to_csv(
+    ...     df=pd.DataFrame({
+    ...         "id": [1, 2, 3],
+    ...         "value": [1000, 1001, 1002],
+    ...         "category": ['A', 'B', 'C'],
+    ...     }),
+    ...     path='s3://bucket/prefix',
+    ...     dataset=True,
+    ...     partition_cols=['value', 'category'],
+    ...     athena_partition_projection_settings={
+    ...        "projection_types": {
+    ...             "value": "integer",
+    ...             "category": "enum",
+    ...         },
+    ...         "projection_ranges": {
+    ...             "value": "1000,2000",
+    ...             "category": "A,B,C",
+    ...         },
+    ...     },
+    ... )
+    {
+        'paths': [
+            's3://.../value=1000/category=A/x.json', ...
+        ],
+        'partitions_values': {
+            's3://.../value=1000/category=A/': [
+                '1000',
+                'A',
+            ], ...
+        }
+    }
+
     Writing bucketed dataset
 
     >>> import awswrangler as wr
     >>> import pandas as pd
-    >>> wr.s3.to_parquet(
+    >>> wr.s3.to_csv(
     ...     df=pd.DataFrame({
     ...         'col': [1, 2, 3],
     ...         'col2': ['A', 'A', 'B']
     ...     }),
     ...     path='s3://bucket/prefix',
     ...     dataset=True,
     ...     bucketing_info=(["col2"], 2)
@@ -457,77 +387,98 @@
         'partitions_values: {}
     }
 
     Writing dataset to S3 with metadata on Athena/Glue Catalog.
 
     >>> import awswrangler as wr
     >>> import pandas as pd
-    >>> wr.s3.to_parquet(
+    >>> wr.s3.to_csv(
     ...     df=pd.DataFrame({
     ...         'col': [1, 2, 3],
     ...         'col2': ['A', 'A', 'B']
     ...     }),
     ...     path='s3://bucket/prefix',
     ...     dataset=True,
     ...     partition_cols=['col2'],
     ...     database='default',  # Athena/Glue database
     ...     table='my_table'  # Athena/Glue table
     ... )
     {
-        'paths': ['s3://.../col2=A/x.parquet', 's3://.../col2=B/y.parquet'],
+        'paths': ['s3://.../col2=A/x.csv', 's3://.../col2=B/y.csv'],
         'partitions_values: {
             's3://.../col2=A/': ['A'],
             's3://.../col2=B/': ['B']
         }
     }
 
     Writing dataset to Glue governed table
 
     >>> import awswrangler as wr
     >>> import pandas as pd
-    >>> wr.s3.to_parquet(
+    >>> wr.s3.to_csv(
     ...     df=pd.DataFrame({
     ...         'col': [1, 2, 3],
     ...         'col2': ['A', 'A', 'B'],
     ...         'col3': [None, None, None]
     ...     }),
     ...     dataset=True,
     ...     mode='append',
     ...     database='default',  # Athena/Glue database
     ...     table='my_table',  # Athena/Glue table
-    ...     table_type='GOVERNED',
-    ...     transaction_id="xxx",
+    ...     glue_table_settings=wr.typing.GlueTableSettings(
+    ...         table_type="GOVERNED",
+    ...         transaction_id="xxx",
+    ...     ),
     ... )
     {
-        'paths': ['s3://.../x.parquet'],
+        'paths': ['s3://.../x.csv'],
         'partitions_values: {}
     }
 
     Writing dataset casting empty column data type
 
     >>> import awswrangler as wr
     >>> import pandas as pd
-    >>> wr.s3.to_parquet(
+    >>> wr.s3.to_csv(
     ...     df=pd.DataFrame({
     ...         'col': [1, 2, 3],
     ...         'col2': ['A', 'A', 'B'],
     ...         'col3': [None, None, None]
     ...     }),
     ...     path='s3://bucket/prefix',
     ...     dataset=True,
     ...     database='default',  # Athena/Glue database
     ...     table='my_table'  # Athena/Glue table
     ...     dtype={'col3': 'date'}
     ... )
     {
-        'paths': ['s3://.../x.parquet'],
+        'paths': ['s3://.../x.csv'],
         'partitions_values: {}
     }
 
     """
+    if "pandas_kwargs" in pandas_kwargs:
+        raise exceptions.InvalidArgument(
+            "You can NOT pass `pandas_kwargs` explicit, just add valid "
+            "Pandas arguments in the function call and awswrangler will accept it."
+            "e.g. wr.s3.to_csv(df, path, sep='|', na_rep='NULL', decimal=',', compression='gzip')"
+        )
+
+    glue_table_settings = cast(
+        GlueTableSettings,
+        glue_table_settings if glue_table_settings else {},
+    )
+
+    table_type = glue_table_settings.get("table_type")
+    transaction_id = glue_table_settings.get("transaction_id")
+    description = glue_table_settings.get("description")
+    parameters = glue_table_settings.get("parameters")
+    columns_comments = glue_table_settings.get("columns_comments")
+    regular_partitions = glue_table_settings.get("regular_partitions", True)
+
     _validate_args(
         df=df,
         table=table,
         database=database,
         dataset=dataset,
         path=path,
         partition_cols=partition_cols,
@@ -535,408 +486,676 @@
         mode=mode,
         description=description,
         parameters=parameters,
         columns_comments=columns_comments,
         execution_engine=engine.get(),
     )
 
-    # Evaluating compression
-    if _COMPRESSION_2_EXT.get(compression, None) is None:
-        raise exceptions.InvalidCompression(f"{compression} is invalid, please use None, 'snappy', 'gzip' or 'zstd'.")
-    compression_ext: str = _COMPRESSION_2_EXT[compression]
-
     # Initializing defaults
     partition_cols = partition_cols if partition_cols else []
     dtype = dtype if dtype else {}
     partitions_values: Dict[str, List[str]] = {}
     mode = "append" if mode is None else mode
     commit_trans: bool = False
     if transaction_id:
         table_type = "GOVERNED"
+
     filename_prefix = filename_prefix + uuid.uuid4().hex if filename_prefix else uuid.uuid4().hex
-    cpus: int = _utils.ensure_cpu_count(use_threads=use_threads)
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    # Pyarrow defaults
-    if not pyarrow_additional_kwargs:
-        pyarrow_additional_kwargs = {}
-    if not pyarrow_additional_kwargs.get("coerce_timestamps"):
-        pyarrow_additional_kwargs["coerce_timestamps"] = "ms"
-    if "flavor" not in pyarrow_additional_kwargs:
-        pyarrow_additional_kwargs["flavor"] = "spark"
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
 
     # Sanitize table to respect Athena's standards
     if (sanitize_columns is True) or (database is not None and table is not None):
-        df, dtype, partition_cols = _sanitize(df=df, dtype=dtype, partition_cols=partition_cols)
+        df, dtype, partition_cols = _sanitize(
+            df=copy_df_shallow(df),
+            dtype=dtype,
+            partition_cols=partition_cols,
+        )
 
     # Evaluating dtype
     catalog_table_input: Optional[Dict[str, Any]] = None
-    if database is not None and table is not None:
+    if database and table:
         catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
-            database=database, table=table, boto3_session=session, transaction_id=transaction_id, catalog_id=catalog_id
+            database=database,
+            table=table,
+            boto3_session=boto3_session,
+            transaction_id=transaction_id,
+            catalog_id=catalog_id,
         )
+
         catalog_path: Optional[str] = None
         if catalog_table_input:
             table_type = catalog_table_input["TableType"]
-            catalog_path = catalog_table_input["StorageDescriptor"]["Location"]
+            catalog_path = catalog_table_input.get("StorageDescriptor", {}).get("Location")
         if path is None:
             if catalog_path:
                 path = catalog_path
             else:
                 raise exceptions.InvalidArgumentValue(
                     "Glue table does not exist in the catalog. Please pass the `path` argument to create it."
                 )
         elif path and catalog_path:
             if path.rstrip("/") != catalog_path.rstrip("/"):
                 raise exceptions.InvalidArgumentValue(
                     f"The specified path: {path}, does not match the existing Glue catalog table path: {catalog_path}"
                 )
+        if pandas_kwargs.get("compression") not in ("gzip", "bz2", None):
+            raise exceptions.InvalidArgumentCombination(
+                "If database and table are given, you must use one of these compressions: gzip, bz2 or None."
+            )
         if (table_type == "GOVERNED") and (not transaction_id):
             _logger.debug("`transaction_id` not specified for GOVERNED table, starting transaction")
-            transaction_id = lakeformation.start_transaction(read_only=False, boto3_session=boto3_session)
+            transaction_id = lakeformation.start_transaction(
+                read_only=False,
+                boto3_session=boto3_session,
+            )
             commit_trans = True
 
     df = _apply_dtype(df=df, dtype=dtype, catalog_table_input=catalog_table_input, mode=mode)
-    schema: pa.Schema = _data_types.pyarrow_schema_from_pandas(
-        df=df, index=index, ignore_cols=partition_cols, dtype=dtype
-    )
-    _logger.debug("schema: \n%s", schema)
 
+    paths: List[str] = []
     if dataset is False:
-        paths = _to_parquet(
+        pandas_kwargs["sep"] = sep
+        pandas_kwargs["index"] = index
+        pandas_kwargs["columns"] = columns
+        _to_text(
             df,
+            file_format="csv",
+            use_threads=use_threads,
             path=path,
-            filename_prefix=filename_prefix,
-            schema=schema,
-            index=index,
-            cpus=cpus,
-            compression=compression,
-            compression_ext=compression_ext,
-            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            boto3_session=session,
+            s3_client=s3_client,
             s3_additional_kwargs=s3_additional_kwargs,
-            dtype=dtype,
-            max_rows_by_file=max_rows_by_file,
-            use_threads=use_threads,
+            **pandas_kwargs,
         )
+        paths = [path]  # type: ignore[list-item]
     else:
+        compression: Optional[str] = pandas_kwargs.get("compression", None)
+        if database and table:
+            quoting: Optional[int] = csv.QUOTE_NONE
+            escapechar: Optional[str] = "\\"
+            header: Union[bool, List[str]] = pandas_kwargs.get("header", False)
+            date_format: Optional[str] = "%Y-%m-%d %H:%M:%S.%f"
+            pd_kwargs: Dict[str, Any] = {}
+        else:
+            quoting = pandas_kwargs.get("quoting", None)
+            escapechar = pandas_kwargs.get("escapechar", None)
+            header = pandas_kwargs.get("header", True)
+            date_format = pandas_kwargs.get("date_format", None)
+            pd_kwargs = pandas_kwargs.copy()
+            pd_kwargs.pop("quoting", None)
+            pd_kwargs.pop("escapechar", None)
+            pd_kwargs.pop("header", None)
+            pd_kwargs.pop("date_format", None)
+            pd_kwargs.pop("compression", None)
+
+        df = df[columns] if columns else df
+
         columns_types: Dict[str, str] = {}
         partitions_types: Dict[str, str] = {}
-        if (database is not None) and (table is not None):
+
+        if database and table:
             columns_types, partitions_types = _data_types.athena_types_from_pandas_partitioned(
-                df=df, index=index, partition_cols=partition_cols, dtype=dtype
+                df=df, index=index, partition_cols=partition_cols, dtype=dtype, index_left=True
             )
             if schema_evolution is False:
                 _utils.check_schema_changes(columns_types=columns_types, table_input=catalog_table_input, mode=mode)
 
             create_table_args: Dict[str, Any] = {
                 "database": database,
                 "table": table,
                 "path": path,
                 "columns_types": columns_types,
                 "table_type": table_type,
                 "partitions_types": partitions_types,
                 "bucketing_info": bucketing_info,
-                "compression": compression,
                 "description": description,
                 "parameters": parameters,
                 "columns_comments": columns_comments,
-                "boto3_session": session,
+                "boto3_session": boto3_session,
                 "mode": mode,
                 "transaction_id": transaction_id,
+                "schema_evolution": schema_evolution,
                 "catalog_versioning": catalog_versioning,
-                "projection_enabled": projection_enabled,
-                "projection_types": projection_types,
-                "projection_ranges": projection_ranges,
-                "projection_values": projection_values,
-                "projection_intervals": projection_intervals,
-                "projection_digits": projection_digits,
-                "projection_formats": projection_formats,
-                "projection_storage_location_template": projection_storage_location_template,
-                "catalog_id": catalog_id,
+                "sep": sep,
+                "athena_partition_projection_settings": athena_partition_projection_settings,
                 "catalog_table_input": catalog_table_input,
+                "catalog_id": catalog_id,
+                "compression": pandas_kwargs.get("compression"),
+                "skip_header_line_count": True if header else None,
+                "serde_library": None,
+                "serde_parameters": None,
             }
 
             if (catalog_table_input is None) and (table_type == "GOVERNED"):
-                catalog._create_parquet_table(**create_table_args)  # pylint: disable=protected-access
-                create_table_args["catalog_table_input"] = catalog._get_table_input(  # pylint: disable=protected-access
+                catalog._create_csv_table(**create_table_args)  # pylint: disable=protected-access
+                catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
                     database=database,
                     table=table,
-                    boto3_session=session,
+                    boto3_session=boto3_session,
                     transaction_id=transaction_id,
                     catalog_id=catalog_id,
                 )
+                create_table_args["catalog_table_input"] = catalog_table_input
 
         paths, partitions_values = _to_dataset(
-            func=_to_parquet,
+            func=_to_text,
             concurrent_partitioning=concurrent_partitioning,
             df=df,
-            path_root=path,  # type: ignore
-            filename_prefix=filename_prefix,
+            path_root=path,  # type: ignore[arg-type]
             index=index,
+            sep=sep,
             compression=compression,
-            compression_ext=compression_ext,
             catalog_id=catalog_id,
             database=database,
             table=table,
             table_type=table_type,
             transaction_id=transaction_id,
-            pyarrow_additional_kwargs=pyarrow_additional_kwargs,
-            cpus=cpus,
+            filename_prefix=filename_prefix,
             use_threads=use_threads,
             partition_cols=partition_cols,
             partitions_types=partitions_types,
             bucketing_info=bucketing_info,
-            dtype=dtype,
             mode=mode,
-            boto3_session=session,
+            boto3_session=boto3_session,
             s3_additional_kwargs=s3_additional_kwargs,
-            schema=schema,
-            max_rows_by_file=max_rows_by_file,
+            file_format="csv",
+            quoting=quoting,
+            escapechar=escapechar,
+            header=header,
+            date_format=date_format,
+            **pd_kwargs,
         )
-        if (database is not None) and (table is not None):
+        if database and table:
             try:
-                catalog._create_parquet_table(**create_table_args)  # pylint: disable=protected-access
+                serde_info: Dict[str, Any] = {}
+                if catalog_table_input:
+                    serde_info = catalog_table_input["StorageDescriptor"]["SerdeInfo"]
+                create_table_args["serde_library"] = serde_info.get("SerializationLibrary", None)
+                create_table_args["serde_parameters"] = serde_info.get("Parameters", None)
+                catalog._create_csv_table(**create_table_args)  # pylint: disable=protected-access
                 if partitions_values and (regular_partitions is True) and (table_type != "GOVERNED"):
                     _logger.debug("partitions_values:\n%s", partitions_values)
-                    catalog.add_parquet_partitions(
+                    catalog.add_csv_partitions(
                         database=database,
                         table=table,
                         partitions_values=partitions_values,
                         bucketing_info=bucketing_info,
-                        compression=compression,
-                        boto3_session=session,
+                        boto3_session=boto3_session,
+                        sep=sep,
+                        serde_library=create_table_args["serde_library"],
+                        serde_parameters=create_table_args["serde_parameters"],
                         catalog_id=catalog_id,
                         columns_types=columns_types,
+                        compression=pandas_kwargs.get("compression"),
                     )
                 if commit_trans:
                     lakeformation.commit_transaction(
-                        transaction_id=transaction_id, boto3_session=boto3_session  # type: ignore
+                        transaction_id=transaction_id,  # type: ignore[arg-type]
+                        boto3_session=boto3_session,
                     )
             except Exception:
-                _logger.debug("Catalog write failed, cleaning up S3 (paths: %s).", paths)
+                _logger.debug("Catalog write failed, cleaning up S3 objects (len(paths): %s).", len(paths))
                 delete_objects(
                     path=paths,
                     use_threads=use_threads,
-                    boto3_session=session,
+                    boto3_session=boto3_session,
                     s3_additional_kwargs=s3_additional_kwargs,
                 )
                 raise
     return {"paths": paths, "partitions_values": partitions_values}
 
 
 @apply_configs
-def store_parquet_metadata(  # pylint: disable=too-many-arguments,too-many-locals
-    path: str,
-    database: str,
-    table: str,
-    catalog_id: Optional[str] = None,
-    path_suffix: Optional[str] = None,
-    path_ignore_suffix: Optional[str] = None,
-    ignore_empty: bool = True,
-    dtype: Optional[Dict[str, str]] = None,
-    sampling: float = 1.0,
-    dataset: bool = False,
+@_utils.validate_distributed_kwargs(
+    unsupported_kwargs=["boto3_session"],
+)
+def to_json(  # pylint: disable=too-many-arguments,too-many-locals,too-many-statements,too-many-branches
+    df: pd.DataFrame,
+    path: Optional[str] = None,
+    index: bool = True,
+    columns: Optional[List[str]] = None,
     use_threads: Union[bool, int] = True,
-    description: Optional[str] = None,
-    parameters: Optional[Dict[str, str]] = None,
-    columns_comments: Optional[Dict[str, str]] = None,
-    compression: Optional[str] = None,
-    mode: str = "overwrite",
-    catalog_versioning: bool = False,
-    regular_partitions: bool = True,
-    projection_enabled: bool = False,
-    projection_types: Optional[Dict[str, str]] = None,
-    projection_ranges: Optional[Dict[str, str]] = None,
-    projection_values: Optional[Dict[str, str]] = None,
-    projection_intervals: Optional[Dict[str, str]] = None,
-    projection_digits: Optional[Dict[str, str]] = None,
-    projection_formats: Optional[Dict[str, str]] = None,
-    projection_storage_location_template: Optional[str] = None,
-    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
     boto3_session: Optional[boto3.Session] = None,
-) -> Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]:
-    """Infer and store parquet metadata on AWS Glue Catalog.
-
-    Infer Apache Parquet file(s) metadata from a received S3 prefix
-    And then stores it on AWS Glue Catalog including all inferred partitions
-    (No need for 'MSCK REPAIR TABLE')
-
-    The concept of Dataset goes beyond the simple idea of files and enables more
-    complex features like partitioning and catalog integration (AWS Glue Catalog).
-
-    This function accepts Unix shell-style wildcards in the path argument.
-    * (matches everything), ? (matches any single character),
-    [seq] (matches any character in seq), [!seq] (matches any character not in seq).
-    If you want to use a path which includes Unix shell-style wildcard characters (`*, ?, []`),
-    you can use `glob.escape(path)` before passing the path to this function.
+    s3_additional_kwargs: Optional[Dict[str, Any]] = None,
+    sanitize_columns: bool = False,
+    dataset: bool = False,
+    filename_prefix: Optional[str] = None,
+    partition_cols: Optional[List[str]] = None,
+    bucketing_info: Optional[BucketingInfoTuple] = None,
+    concurrent_partitioning: bool = False,
+    mode: Optional[str] = None,
+    catalog_versioning: bool = False,
+    schema_evolution: bool = True,
+    dtype: Optional[Dict[str, str]] = None,
+    database: Optional[str] = None,
+    table: Optional[str] = None,
+    glue_table_settings: Optional[GlueTableSettings] = None,
+    athena_partition_projection_settings: Optional[typing.AthenaPartitionProjectionSettings] = None,
+    catalog_id: Optional[str] = None,
+    **pandas_kwargs: Any,
+) -> _S3WriteDataReturnValue:
+    """Write JSON file on Amazon S3.
 
     Note
     ----
     In case of `use_threads=True` the number of threads
     that will be spawned will be gotten from os.cpu_count().
 
+    Note
+    ----
+    Compression: The minimum acceptable version to achive it is Pandas 1.2.0 that requires Python >= 3.7.1.
+
     Parameters
     ----------
+    df: pandas.DataFrame
+        Pandas DataFrame https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
     path : str
-        S3 prefix (accepts Unix shell-style wildcards) (e.g. s3://bucket/prefix).
-    table : str
-        Glue/Athena catalog: Table name.
-    database : str
-        AWS Glue Catalog database name.
-    catalog_id : str, optional
-        The ID of the Data Catalog from which to retrieve Databases.
-        If none is provided, the AWS account ID is used by default.
-    path_suffix: Union[str, List[str], None]
-        Suffix or List of suffixes for filtering S3 keys.
-    path_ignore_suffix: Union[str, List[str], None]
-        Suffix or List of suffixes for S3 keys to be ignored.
-    ignore_empty: bool
-        Ignore files with 0 bytes.
-    dtype : Dict[str, str], optional
-        Dictionary of columns names and Athena/Glue types to be casted.
-        Useful when you have columns with undetermined data types as partitions columns.
-        (e.g. {'col name': 'bigint', 'col2 name': 'int'})
-    sampling : float
-        Random sample ratio of files that will have the metadata inspected.
-        Must be `0.0 < sampling <= 1.0`.
-        The higher, the more accurate.
-        The lower, the faster.
-    dataset: bool
-        If True read a parquet dataset instead of simple file(s) loading all the related partitions as columns.
+        Amazon S3 path (e.g. s3://bucket/filename.json).
+    index : bool
+        Write row names (index).
+    columns : Optional[List[str]]
+        Columns to write.
     use_threads : bool, int
         True to enable concurrent requests, False to disable multiple threads.
         If enabled os.cpu_count() will be used as the max number of threads.
         If integer is provided, specified number is used.
-    description: str, optional
-        Glue/Athena catalog: Table description
-    parameters: Dict[str, str], optional
-        Glue/Athena catalog: Key/value pairs to tag the table.
-    columns_comments: Dict[str, str], optional
-        Glue/Athena catalog:
-        Columns names and the related comments (e.g. {'col0': 'Column 0.', 'col1': 'Column 1.', 'col2': 'Partition.'}).
-    compression: str, optional
-        Compression style (``None``, ``snappy``, ``gzip``, etc).
-    mode: str
-        'overwrite' to recreate any possible existing table or 'append' to keep any possible existing table.
-    catalog_versioning : bool
-        If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
-    regular_partitions : bool
-        Create regular partitions (Non projected partitions) on Glue Catalog.
-        Disable when you will work only with Partition Projection.
-        Keep enabled even when working with projections is useful to keep
-        Redshift Spectrum working with the regular partitions.
-    projection_enabled : bool
-        Enable Partition Projection on Athena (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html)
-    projection_types : Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections types.
-        Valid types: "enum", "integer", "date", "injected"
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
-    projection_ranges: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections ranges.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
-    projection_values: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections values.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
-    projection_intervals: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections intervals.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '5'})
-    projection_digits: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections digits.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_name': '1', 'col2_name': '2'})
-    projection_formats: Optional[Dict[str, str]]
-        Dictionary of partitions names and Athena projections formats.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
-        (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
-    projection_storage_location_template: Optional[str]
-        Value which is allows Athena to properly map partition values if the S3 file locations do not follow
-        a typical `.../column=value/...` pattern.
-        https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
-        (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    boto3_session : boto3.Session(), optional
+        Boto3 Session. The default boto3 Session will be used if boto3_session receive None.
     s3_additional_kwargs : Optional[Dict[str, Any]]
         Forwarded to botocore requests.
         e.g. s3_additional_kwargs={'ServerSideEncryption': 'aws:kms', 'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'}
-    boto3_session : boto3.Session(), optional
-        Boto3 Session. The default boto3 session will be used if boto3_session receive None.
+    sanitize_columns : bool
+        True to sanitize columns names or False to keep it as is.
+        True value is forced if `dataset=True`.
+    dataset : bool
+        If True store as a dataset instead of ordinary file(s)
+        If True, enable all follow arguments:
+        partition_cols, mode, database, table, description, parameters, columns_comments, concurrent_partitioning,
+        catalog_versioning, projection_params, catalog_id, schema_evolution.
+    filename_prefix: str, optional
+        If dataset=True, add a filename prefix to the output files.
+    partition_cols: List[str], optional
+        List of column names that will be used to create partitions. Only takes effect if dataset=True.
+    bucketing_info: Tuple[List[str], int], optional
+        Tuple consisting of the column names used for bucketing as the first element and the number of buckets as the
+        second element.
+        Only `str`, `int` and `bool` are supported as column data types for bucketing.
+    concurrent_partitioning: bool
+        If True will increase the parallelism level during the partitions writing. It will decrease the
+        writing time and increase the memory usage.
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/022%20-%20Writing%20Partitions%20Concurrently.html
+    mode : str, optional
+        ``append`` (Default), ``overwrite``, ``overwrite_partitions``. Only takes effect if dataset=True.
+        For details check the related tutorial:
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/stubs/awswrangler.s3.to_parquet.html#awswrangler.s3.to_parquet
+    catalog_versioning : bool
+        If True and `mode="overwrite"`, creates an archived version of the table catalog before updating it.
+    schema_evolution : bool
+        If True allows schema evolution (new or missing columns), otherwise a exception will be raised.
+        (Only considered if dataset=True and mode in ("append", "overwrite_partitions"))
+        Related tutorial:
+        https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/tutorials/014%20-%20Schema%20Evolution.html
+    database : str, optional
+        Glue/Athena catalog: Database name.
+    table : str, optional
+        Glue/Athena catalog: Table name.
+    glue_table_settings: dict (GlueTableSettings), optional
+        Settings for writing to the Glue table.
+    dtype : Dict[str, str], optional
+        Dictionary of columns names and Athena/Glue types to be casted.
+        Useful when you have columns with undetermined or mixed data types.
+        (e.g. {'col name': 'bigint', 'col2 name': 'int'})
+    athena_partition_projection_settings: typing.AthenaPartitionProjectionSettings, optional
+        Params of the Athena Partition Projection (https://docs.aws.amazon.com/athena/latest/ug/partition-projection.html).
+        AthenaPartitionProjectionSettings is a `TypedDict`, meaning the passed parameter can be instantiated either as an
+        instance of AthenaPartitionProjectionSettings or as a regular Python dict.
+
+        Following projection parameters are supported:
+
+        .. list-table:: Projection Parameters
+           :header-rows: 1
+
+           * - Name
+             - Type
+             - Description
+           * - projection_types
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections types.
+               Valid types: "enum", "integer", "date", "injected"
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'enum', 'col2_name': 'integer'})
+           * - projection_ranges
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections ranges.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '0,10', 'col2_name': '-1,8675309'})
+           * - projection_values
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections values.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': 'A,B,Unknown', 'col2_name': 'foo,boo,bar'})
+           * - projection_intervals
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections intervals.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '5'})
+           * - projection_digits
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections digits.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_name': '1', 'col2_name': '2'})
+           * - projection_formats
+             - Optional[Dict[str, str]]
+             - Dictionary of partitions names and Athena projections formats.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-supported-types.html
+               (e.g. {'col_date': 'yyyy-MM-dd', 'col2_timestamp': 'yyyy-MM-dd HH:mm:ss'})
+           * - projection_storage_location_template
+             - Optional[str]
+             - Value which is allows Athena to properly map partition values if the S3 file locations do not follow
+               a typical `.../column=value/...` pattern.
+               https://docs.aws.amazon.com/athena/latest/ug/partition-projection-setting-up.html
+               (e.g. s3://bucket/table_root/a=${a}/${b}/some_static_subdirectory/${c}/)
+    catalog_id : str, optional
+        The ID of the Data Catalog from which to retrieve Databases.
+        If none is provided, the AWS account ID is used by default.
+    pandas_kwargs:
+        KEYWORD arguments forwarded to pandas.DataFrame.to_json(). You can NOT pass `pandas_kwargs` explicit, just add
+        valid Pandas arguments in the function call and awswrangler will accept it.
+        e.g. wr.s3.to_json(df, path, lines=True, date_format='iso')
+        https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_json.html
 
     Returns
     -------
-    Tuple[Dict[str, str], Optional[Dict[str, str]], Optional[Dict[str, List[str]]]]
-        The metadata used to create the Glue Table.
-        columns_types: Dictionary with keys as column names and values as
-        data types (e.g. {'col0': 'bigint', 'col1': 'double'}). /
-        partitions_types: Dictionary with keys as partition names
-        and values as data types (e.g. {'col2': 'date'}). /
-        partitions_values: Dictionary with keys as S3 path locations and values as a
-        list of partitions values as str (e.g. {'s3://bucket/prefix/y=2020/m=10/': ['2020', '10']}).
+    wr.typing._S3WriteDataReturnValue
+        Dictionary with:
+        'paths': List of all stored files paths on S3.
+        'partitions_values': Dictionary of partitions added with keys as S3 path locations
+        and values as a list of partitions values as str.
 
     Examples
     --------
-    Reading all Parquet files metadata under a prefix
+    Writing JSON file
 
     >>> import awswrangler as wr
-    >>> columns_types, partitions_types, partitions_values = wr.s3.store_parquet_metadata(
-    ...     path='s3://bucket/prefix/',
-    ...     database='...',
-    ...     table='...',
-    ...     dataset=True
+    >>> import pandas as pd
+    >>> wr.s3.to_json(
+    ...     df=pd.DataFrame({'col': [1, 2, 3]}),
+    ...     path='s3://bucket/filename.json',
+    ... )
+
+    Writing JSON file using pandas_kwargs
+
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> wr.s3.to_json(
+    ...     df=pd.DataFrame({'col': [1, 2, 3]}),
+    ...     path='s3://bucket/filename.json',
+    ...     lines=True,
+    ...     date_format='iso'
     ... )
 
+    Writing CSV file encrypted with a KMS key
+
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> wr.s3.to_json(
+    ...     df=pd.DataFrame({'col': [1, 2, 3]}),
+    ...     path='s3://bucket/filename.json',
+    ...     s3_additional_kwargs={
+    ...         'ServerSideEncryption': 'aws:kms',
+    ...         'SSEKMSKeyId': 'YOUR_KMS_KEY_ARN'
+    ...     }
+    ... )
+
+    Writing partitioned dataset with partition projection
+
+    >>> import awswrangler as wr
+    >>> import pandas as pd
+    >>> from datetime import datetime
+    >>> dt = lambda x: datetime.strptime(x, "%Y-%m-%d").date()
+    >>> wr.s3.to_json(
+    ...     df=pd.DataFrame({
+    ...         "id": [1, 2, 3],
+    ...         "value": [1000, 1001, 1002],
+    ...         "category": ['A', 'B', 'C'],
+    ...     }),
+    ...     path='s3://bucket/prefix',
+    ...     dataset=True,
+    ...     partition_cols=['value', 'category'],
+    ...     athena_partition_projection_settings={
+    ...        "projection_types": {
+    ...             "value": "integer",
+    ...             "category": "enum",
+    ...         },
+    ...         "projection_ranges": {
+    ...             "value": "1000,2000",
+    ...             "category": "A,B,C",
+    ...         },
+    ...     },
+    ... )
+    {
+        'paths': [
+            's3://.../value=1000/category=A/x.json', ...
+        ],
+        'partitions_values': {
+            's3://.../value=1000/category=A/': [
+                '1000',
+                'A',
+            ], ...
+        }
+    }
+
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    columns_types: Dict[str, str]
-    partitions_types: Optional[Dict[str, str]]
-    partitions_values: Optional[Dict[str, List[str]]]
-    columns_types, partitions_types, partitions_values = _read_parquet_metadata(
-        path=path,
-        dtype=dtype,
-        sampling=sampling,
-        dataset=dataset,
-        path_suffix=path_suffix,
-        path_ignore_suffix=path_ignore_suffix,
-        ignore_empty=ignore_empty,
-        ignore_null=False,
-        use_threads=use_threads,
-        s3_additional_kwargs=s3_additional_kwargs,
-        boto3_session=session,
+    if "pandas_kwargs" in pandas_kwargs:
+        raise exceptions.InvalidArgument(
+            "You can NOT pass `pandas_kwargs` explicit, just add valid "
+            "Pandas arguments in the function call and awswrangler will accept it."
+            "e.g. wr.s3.to_json(df, path, lines=True, date_format='iso')"
+        )
+
+    glue_table_settings = cast(
+        GlueTableSettings,
+        glue_table_settings if glue_table_settings else {},
     )
-    _logger.debug("columns_types: %s", columns_types)
-    _logger.debug("partitions_types: %s", partitions_types)
-    _logger.debug("partitions_values: %s", partitions_values)
-    catalog.create_parquet_table(
-        database=database,
+
+    table_type = glue_table_settings.get("table_type")
+    transaction_id = glue_table_settings.get("transaction_id")
+    description = glue_table_settings.get("description")
+    parameters = glue_table_settings.get("parameters")
+    columns_comments = glue_table_settings.get("columns_comments")
+    regular_partitions = glue_table_settings.get("regular_partitions", True)
+
+    _validate_args(
+        df=df,
         table=table,
+        database=database,
+        dataset=dataset,
         path=path,
-        columns_types=columns_types,
-        partitions_types=partitions_types,
+        partition_cols=partition_cols,
+        bucketing_info=bucketing_info,
+        mode=mode,
         description=description,
         parameters=parameters,
         columns_comments=columns_comments,
-        mode=mode,
-        compression=compression,
-        catalog_versioning=catalog_versioning,
-        projection_enabled=projection_enabled,
-        projection_types=projection_types,
-        projection_ranges=projection_ranges,
-        projection_values=projection_values,
-        projection_intervals=projection_intervals,
-        projection_digits=projection_digits,
-        projection_formats=projection_formats,
-        projection_storage_location_template=projection_storage_location_template,
-        boto3_session=session,
-        catalog_id=catalog_id,
+        execution_engine=engine.get(),
     )
-    if (partitions_types is not None) and (partitions_values is not None) and (regular_partitions is True):
-        catalog.add_parquet_partitions(
+
+    # Initializing defaults
+    partition_cols = partition_cols if partition_cols else []
+    dtype = dtype if dtype else {}
+    partitions_values: Dict[str, List[str]] = {}
+    mode = "append" if mode is None else mode
+    commit_trans: bool = False
+    if transaction_id:
+        table_type = "GOVERNED"
+
+    filename_prefix = filename_prefix + uuid.uuid4().hex if filename_prefix else uuid.uuid4().hex
+    s3_client = _utils.client(service_name="s3", session=boto3_session)
+
+    # Sanitize table to respect Athena's standards
+    if (sanitize_columns is True) or (database is not None and table is not None):
+        df, dtype, partition_cols = _sanitize(
+            df=copy_df_shallow(df),
+            dtype=dtype,
+            partition_cols=partition_cols,
+        )
+
+    # Evaluating dtype
+    catalog_table_input: Optional[Dict[str, Any]] = None
+
+    if database and table:
+        catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
             database=database,
             table=table,
-            partitions_values=partitions_values,
-            compression=compression,
-            boto3_session=session,
+            boto3_session=boto3_session,
+            transaction_id=transaction_id,
             catalog_id=catalog_id,
-            columns_types=columns_types,
         )
-    return columns_types, partitions_types, partitions_values
+        catalog_path: Optional[str] = None
+        if catalog_table_input:
+            table_type = catalog_table_input["TableType"]
+            catalog_path = catalog_table_input.get("StorageDescriptor", {}).get("Location")
+        if path is None:
+            if catalog_path:
+                path = catalog_path
+            else:
+                raise exceptions.InvalidArgumentValue(
+                    "Glue table does not exist in the catalog. Please pass the `path` argument to create it."
+                )
+        elif path and catalog_path:
+            if path.rstrip("/") != catalog_path.rstrip("/"):
+                raise exceptions.InvalidArgumentValue(
+                    f"The specified path: {path}, does not match the existing Glue catalog table path: {catalog_path}"
+                )
+        if pandas_kwargs.get("compression") not in ("gzip", "bz2", None):
+            raise exceptions.InvalidArgumentCombination(
+                "If database and table are given, you must use one of these compressions: gzip, bz2 or None."
+            )
+        if (table_type == "GOVERNED") and (not transaction_id):
+            _logger.debug("`transaction_id` not specified for GOVERNED table, starting transaction")
+            transaction_id = lakeformation.start_transaction(
+                read_only=False,
+                boto3_session=boto3_session,
+            )
+            commit_trans = True
+
+    df = _apply_dtype(df=df, dtype=dtype, catalog_table_input=catalog_table_input, mode=mode)
+
+    if dataset is False:
+        output_paths = _to_text(
+            df,
+            file_format="json",
+            path=path,
+            use_threads=use_threads,
+            s3_client=s3_client,
+            s3_additional_kwargs=s3_additional_kwargs,
+            **pandas_kwargs,
+        )
+        return {"paths": output_paths, "partitions_values": {}}
+
+    compression: Optional[str] = pandas_kwargs.pop("compression", None)
+    df = df[columns] if columns else df
+
+    columns_types: Dict[str, str] = {}
+    partitions_types: Dict[str, str] = {}
+
+    if database and table:
+        columns_types, partitions_types = _data_types.athena_types_from_pandas_partitioned(
+            df=df, index=index, partition_cols=partition_cols, dtype=dtype
+        )
+        if schema_evolution is False:
+            _utils.check_schema_changes(columns_types=columns_types, table_input=catalog_table_input, mode=mode)
+
+        create_table_args: Dict[str, Any] = {
+            "database": database,
+            "table": table,
+            "path": path,
+            "columns_types": columns_types,
+            "table_type": table_type,
+            "partitions_types": partitions_types,
+            "bucketing_info": bucketing_info,
+            "description": description,
+            "parameters": parameters,
+            "columns_comments": columns_comments,
+            "boto3_session": boto3_session,
+            "mode": mode,
+            "transaction_id": transaction_id,
+            "catalog_versioning": catalog_versioning,
+            "schema_evolution": schema_evolution,
+            "athena_partition_projection_settings": athena_partition_projection_settings,
+            "catalog_table_input": catalog_table_input,
+            "catalog_id": catalog_id,
+            "compression": compression,
+            "serde_library": None,
+            "serde_parameters": None,
+        }
+
+        if (catalog_table_input is None) and (table_type == "GOVERNED"):
+            catalog._create_json_table(**create_table_args)  # pylint: disable=protected-access
+            catalog_table_input = catalog._get_table_input(  # pylint: disable=protected-access
+                database=database,
+                table=table,
+                boto3_session=boto3_session,
+                transaction_id=transaction_id,
+                catalog_id=catalog_id,
+            )
+            create_table_args["catalog_table_input"] = catalog_table_input
+
+    paths, partitions_values = _to_dataset(
+        func=_to_text,
+        concurrent_partitioning=concurrent_partitioning,
+        df=df,
+        path_root=path,  # type: ignore[arg-type]
+        filename_prefix=filename_prefix,
+        index=index,
+        compression=compression,
+        catalog_id=catalog_id,
+        database=database,
+        table=table,
+        table_type=table_type,
+        transaction_id=transaction_id,
+        use_threads=use_threads,
+        partition_cols=partition_cols,
+        partitions_types=partitions_types,
+        bucketing_info=bucketing_info,
+        mode=mode,
+        boto3_session=boto3_session,
+        s3_additional_kwargs=s3_additional_kwargs,
+        file_format="json",
+        **pandas_kwargs,
+    )
+    if database and table:
+        try:
+            serde_info: Dict[str, Any] = {}
+            if catalog_table_input:
+                serde_info = catalog_table_input["StorageDescriptor"]["SerdeInfo"]
+            create_table_args["serde_library"] = serde_info.get("SerializationLibrary", None)
+            create_table_args["serde_parameters"] = serde_info.get("Parameters", None)
+            catalog._create_json_table(**create_table_args)  # pylint: disable=protected-access
+            if partitions_values and (regular_partitions is True) and (table_type != "GOVERNED"):
+                _logger.debug("partitions_values:\n%s", partitions_values)
+                catalog.add_json_partitions(
+                    database=database,
+                    table=table,
+                    partitions_values=partitions_values,
+                    bucketing_info=bucketing_info,
+                    boto3_session=boto3_session,
+                    serde_library=create_table_args["serde_library"],
+                    serde_parameters=create_table_args["serde_parameters"],
+                    catalog_id=catalog_id,
+                    columns_types=columns_types,
+                    compression=compression,
+                )
+                if commit_trans:
+                    lakeformation.commit_transaction(
+                        transaction_id=transaction_id,  # type: ignore[arg-type]
+                        boto3_session=boto3_session,
+                    )
+        except Exception:
+            _logger.debug("Catalog write failed, cleaning up S3 (paths: %s).", paths)
+            delete_objects(
+                path=paths,
+                use_threads=use_threads,
+                boto3_session=boto3_session,
+                s3_additional_kwargs=s3_additional_kwargs,
+            )
+            raise
+    return {"paths": paths, "partitions_values": partitions_values}
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/secretsmanager.py` & `awswrangler-3.0.0rc3/awswrangler/secretsmanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,19 +30,18 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> value = wr.secretsmanager.get_secret("my-secret")
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    client: boto3.client = _utils.client(service_name="secretsmanager", session=session)
-    response: Dict[str, Any] = client.get_secret_value(SecretId=name)
+    client = _utils.client(service_name="secretsmanager", session=boto3_session)
+    response = client.get_secret_value(SecretId=name)
     if "SecretString" in response:
-        return cast(str, response["SecretString"])
+        return response["SecretString"]
     return base64.b64decode(response["SecretBinary"])
 
 
 def get_secret_json(name: str, boto3_session: Optional[boto3.Session] = None) -> Dict[str, Any]:
     """Get JSON secret value.
 
     Parameters
@@ -60,9 +59,9 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> value = wr.secretsmanager.get_secret_json("my-secret-with-json-content")
 
     """
-    value: Union[str, bytes] = get_secret(name=name, boto3_session=boto3_session)
+    value = get_secret(name=name, boto3_session=boto3_session)
     return cast(Dict[str, Any], json.loads(value))
```

### Comparing `awswrangler-3.0.0rc2/awswrangler/sts.py` & `awswrangler-3.0.0rc3/awswrangler/sts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """STS module."""
 
 import logging
-from typing import Optional, cast
+from typing import Optional
 
 import boto3
 
 from awswrangler import _utils
 
 _logger: logging.Logger = logging.getLogger(__name__)
 
@@ -25,16 +25,15 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> account_id = wr.sts.get_account_id()
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    return cast(str, _utils.client(service_name="sts", session=session).get_caller_identity().get("Account"))
+    return _utils.client(service_name="sts", session=boto3_session).get_caller_identity()["Account"]
 
 
 def get_current_identity_arn(boto3_session: Optional[boto3.Session] = None) -> str:
     """Get current user/role ARN.
 
     Parameters
     ----------
@@ -48,16 +47,15 @@
 
     Examples
     --------
     >>> import awswrangler as wr
     >>> arn = wr.sts.get_current_identity_arn()
 
     """
-    session: boto3.Session = _utils.ensure_session(session=boto3_session)
-    return cast(str, _utils.client(service_name="sts", session=session).get_caller_identity().get("Arn"))
+    return _utils.client(service_name="sts", session=boto3_session).get_caller_identity()["Arn"]
 
 
 def get_current_identity_name(boto3_session: Optional[boto3.Session] = None) -> str:
     """Get current user/role name.
 
     Parameters
     ----------
```

### Comparing `awswrangler-3.0.0rc2/setup.py` & `awswrangler-3.0.0rc3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,58 +2,62 @@
 from setuptools import setup
 
 packages = \
 ['awswrangler',
  'awswrangler.athena',
  'awswrangler.catalog',
  'awswrangler.data_api',
+ 'awswrangler.data_quality',
  'awswrangler.distributed',
  'awswrangler.distributed.ray',
  'awswrangler.distributed.ray.datasources',
  'awswrangler.distributed.ray.modin',
  'awswrangler.distributed.ray.modin.s3',
+ 'awswrangler.distributed.ray.s3',
  'awswrangler.dynamodb',
  'awswrangler.lakeformation',
  'awswrangler.neptune',
  'awswrangler.opensearch',
  'awswrangler.quicksight',
  'awswrangler.s3']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['backoff>=2.0.0,<3.0.0',
- 'boto3>=1.24.11,<2.0.0',
- 'botocore>=1.27.11,<2.0.0',
- 'gremlinpython>=3.5.2,<4.0.0',
- 'jsonpath-ng>=1.5.3,<2.0.0',
- 'numpy>=1.22.4,<2.0.0',
- 'openpyxl>=3.0.0,<3.1.0',
- 'opensearch-py>=2.0.0,<3.0.0',
- 'pandas>=1.2.0,<2.0.0,<=1.5.1,!=1.5.0',
- 'pg8000>=1.29.0,<2.0.0',
- 'progressbar2>=4.0.0,<5.0.0',
- 'pyarrow>=6.0.0,<8.1.0',
- 'pymysql>=1.0.0,<2.0.0',
- 'redshift-connector>=2.0.889,<2.1.0',
- 'requests-aws4auth>=1.1.1,<2.0.0']
+['boto3>=1.20.32,<2.0.0',
+ 'botocore>=1.23.32,<2.0.0',
+ 'numpy>=1.18,<2.0',
+ 'pandas>=1.0,<2.0',
+ 'pyarrow>=7.0.0',
+ 'typing-extensions>=4.4.0,<5.0.0']
 
 extras_require = \
-{'modin': ['modin>=0.16.0,<0.17.0'],
- 'oracle': ['oracledb>=1.0.0,<1.1.0'],
- 'ray': ['ray[data,default]>=2.0.0,<2.1.0'],
- 'sparql': ['SPARQLWrapper>=2.0.0,<3.0.0'],
- 'sqlserver': ['pyodbc>=4.0.32,<4.1.0']}
+{'deltalake': ['deltalake>=0.6.4,<0.7.0'],
+ 'gremlin': ['gremlinpython>=3.5.2,<4.0.0', 'requests>=2.0.0,<3.0.0'],
+ 'modin': ['modin>=0.18.0,<0.19.0'],
+ 'mysql': ['pymysql>=1.0.0,<2.0.0'],
+ 'opencypher': ['requests>=2.0.0,<3.0.0'],
+ 'openpyxl': ['openpyxl>=3.0.0,<4.0.0'],
+ 'opensearch': ['opensearch-py>=2.0.0,<3.0.0',
+                'requests-aws4auth>=1.1.1,<2.0.0',
+                'jsonpath-ng>=1.5.3,<2.0.0'],
+ 'oracle': ['oracledb>=1.0.0,<2.0.0'],
+ 'postgres': ['pg8000>=1.29.0,<2.0.0'],
+ 'progressbar': ['progressbar2>=4.0.0,<5.0.0'],
+ 'ray': ['ray[data,default]>=2.0.0,<2.4.0'],
+ 'redshift': ['redshift-connector>=2.0.0,<3.0.0'],
+ 'sparql': ['SPARQLWrapper>=2.0.0,<3.0.0', 'requests>=2.0.0,<3.0.0'],
+ 'sqlserver': ['pyodbc>=4.0.0,<5.0.0']}
 
 setup_kwargs = {
     'name': 'awswrangler',
-    'version': '3.0.0rc2',
+    'version': '3.0.0rc3',
     'description': 'Pandas on AWS.',
-    'long_description': '# AWS SDK for pandas (awswrangler)\n\nAWS Data Wrangler is now **AWS SDK for pandas (awswrangler)**.  We’re changing the name we use when we talk about the library, but everything else will stay the same.  You’ll still be able to install using `pip install awswrangler` and you won’t need to change any of your code.  As part of this change, we’ve moved the library from AWS Labs to the main AWS GitHub organisation but, thanks to the GitHub’s redirect feature, you’ll still be able to access the project by its old URLs until you update your bookmarks.  Our documentation has also moved to [aws-sdk-pandas.readthedocs.io](https://aws-sdk-pandas.readthedocs.io), but old bookmarks will redirect to the new site.\n\n*Pandas on AWS*\n\nEasy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).\n\n![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")\n![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)\n\n> An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com\n\n[![Release](https://img.shields.io/badge/release-3.0.0rc2-brightgreen.svg)](https://pypi.org/project/awswrangler/)\n[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Coverage](https://img.shields.io/badge/coverage-91%25-brightgreen.svg)](https://pypi.org/project/awswrangler/)\n![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)\n\n| Source | Downloads | Installation Command |\n|--------|-----------|----------------------|\n| **[PyPi](https://pypi.org/project/awswrangler/)**  | [![PyPI Downloads](https://pepy.tech/badge/awswrangler)](https://pypi.org/project/awswrangler/) | `pip install awswrangler` |\n| **[Conda](https://anaconda.org/conda-forge/awswrangler)** | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/awswrangler.svg)](https://anaconda.org/conda-forge/awswrangler) | `conda install -c conda-forge awswrangler` |\n\n> ⚠️ **For platforms without PyArrow 3 support (e.g. [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr-cluster), [Glue PySpark Job](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs), MWAA):**<br>\n➡️ `pip install pyarrow==2 awswrangler`\n\nPowered By [<img src="https://arrow.apache.org/img/arrow.png" width="200">](https://arrow.apache.org/powered_by/)\n\n## Table of contents\n\n- [Quick Start](#quick-start)\n- [At Scale](#at-scale)\n- [Read The Docs](#read-the-docs)\n- [Getting Help](#getting-help)\n- [Community Resources](#community-resources)\n- [Logging](#logging)\n- [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-pandas)\n\n## Quick Start\n\nInstallation command: `pip install awswrangler`\n\n> ⚠️ **For platforms without PyArrow 3 support (e.g. [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr-cluster), [Glue PySpark Job](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs), MWAA):**<br>\n➡️`pip install pyarrow==2 awswrangler`\n\n```py3\nimport awswrangler as wr\nimport pandas as pd\nfrom datetime import datetime\n\ndf = pd.DataFrame({"id": [1, 2], "value": ["foo", "boo"]})\n\n# Storing data on Data Lake\nwr.s3.to_parquet(\n    df=df,\n    path="s3://bucket/dataset/",\n    dataset=True,\n    database="my_db",\n    table="my_table"\n)\n\n# Retrieving the data directly from Amazon S3\ndf = wr.s3.read_parquet("s3://bucket/dataset/", dataset=True)\n\n# Retrieving the data from Amazon Athena\ndf = wr.athena.read_sql_query("SELECT * FROM my_table", database="my_db")\n\n# Get a Redshift connection from Glue Catalog and retrieving data from Redshift Spectrum\ncon = wr.redshift.connect("my-glue-connection")\ndf = wr.redshift.read_sql_query("SELECT * FROM external_schema.my_table", con=con)\ncon.close()\n\n# Amazon Timestream Write\ndf = pd.DataFrame({\n    "time": [datetime.now(), datetime.now()],   \n    "my_dimension": ["foo", "boo"],\n    "measure": [1.0, 1.1],\n})\nrejected_records = wr.timestream.write(df,\n    database="sampleDB",\n    table="sampleTable",\n    time_col="time",\n    measure_col="measure",\n    dimensions_cols=["my_dimension"],\n)\n\n# Amazon Timestream Query\nwr.timestream.query("""\nSELECT time, measure_value::double, my_dimension\nFROM "sampleDB"."sampleTable" ORDER BY time DESC LIMIT 3\n""")\n\n```\n\n## At scale\nAWS SDK for pandas can also run your workflows at scale by leveraging [modin](https://modin.readthedocs.io/en/stable/) and [ray](https://www.ray.io/). Both projects aim to speed up data workloads (pandas workloads in particular in the case of modin) by distributing processing over a cluster of workers.\n\n### Installation\n```\npip install "awswrangler[modin,ray]==3.0.0rc2"\n```\n\nAs a result existing scripts can run on significantly larger datasets with no code rewrite. Supported APIs are parallelized across cores on a single machine or across multiple nodes on a cluster in the cloud.\n\n### Supported APIs\n\n<p align="center">\n\n| Service     | API                                                           | Implementation |\n|-------------------|:------------------------------------------------------------------------------------:|:---------------:|\n|  `S3`    | `read_parquet`                                               | ✅ |\n|    | `read_csv`                                               | ✅ |\n|    | `read_json`                                               | ✅ |\n|    | `read_fwf`                                               | ✅ |\n|    | `to_parquet`                                               | ✅ |\n|    | `to_csv`                                               | ✅ |\n|    | `to_json`                                               | ✅ |\n|    | `select_query`                                               | ✅ |\n|    | `delete`                                               | ✅ |\n|    | `copy`                                               | ✅ |\n|    | `wait`                                               | ✅ |\n|  `Redshift`    | `copy`                                               | ✅ |\n|    | `unload`                                               | ✅ |\n|  `Athena`    | `read_sql_query`                                               | ✅ |\n|  `LakeFormation`    | `read_sql_query`                                               | ✅ |\n|  `Timestream`    | `write`                                               | ✅ |\n</p>\n\n## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)\n\n- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/what.html)\n- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html)\n  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#pypi-pip)\n  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#conda)\n  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-lambda-layer)\n  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-python-shell-jobs)\n  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs)\n  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#amazon-sagemaker-notebook)\n  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#amazon-sagemaker-notebook-lifecycle)\n  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr)\n  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#from-source)\n- [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)\n  - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)\n  - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)\n  - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)\n  - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)\n  - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)\n  - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)\n  - [007 - Databases (Redshift, MySQL, PostgreSQL, SQL Server and Oracle)](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/007%20-%20Redshift%2C%20MySQL%2C%20PostgreSQL%2C%20SQL%20Server%2C%20Oracle.ipynb)\n  - [008 - Redshift - Copy & Unload.ipynb](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/008%20-%20Redshift%20-%20Copy%20%26%20Unload.ipynb)\n  - [009 - Redshift - Append, Overwrite and Upsert](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/009%20-%20Redshift%20-%20Append%2C%20Overwrite%2C%20Upsert.ipynb)\n  - [010 - Parquet Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/010%20-%20Parquet%20Crawler.ipynb)\n  - [011 - CSV Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/011%20-%20CSV%20Datasets.ipynb)\n  - [012 - CSV Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/012%20-%20CSV%20Crawler.ipynb)\n  - [013 - Merging Datasets on S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/013%20-%20Merging%20Datasets%20on%20S3.ipynb)\n  - [014 - Schema Evolution](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/014%20-%20Schema%20Evolution.ipynb)\n  - [015 - EMR](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/015%20-%20EMR.ipynb)\n  - [016 - EMR & Docker](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/016%20-%20EMR%20%26%20Docker.ipynb)\n  - [017 - Partition Projection](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/017%20-%20Partition%20Projection.ipynb)\n  - [018 - QuickSight](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/018%20-%20QuickSight.ipynb)\n  - [019 - Athena Cache](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/019%20-%20Athena%20Cache.ipynb)\n  - [020 - Spark Table Interoperability](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/020%20-%20Spark%20Table%20Interoperability.ipynb)\n  - [021 - Global Configurations](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/021%20-%20Global%20Configurations.ipynb)\n  - [022 - Writing Partitions Concurrently](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/022%20-%20Writing%20Partitions%20Concurrently.ipynb)\n  - [023 - Flexible Partitions Filter](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/023%20-%20Flexible%20Partitions%20Filter.ipynb)\n  - [024 - Athena Query Metadata](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/024%20-%20Athena%20Query%20Metadata.ipynb)\n  - [025 - Redshift - Loading Parquet files with Spectrum](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/025%20-%20Redshift%20-%20Loading%20Parquet%20files%20with%20Spectrum.ipynb)\n  - [026 - Amazon Timestream](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/026%20-%20Amazon%20Timestream.ipynb)\n  - [027 - Amazon Timestream 2](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/027%20-%20Amazon%20Timestream%202.ipynb)\n  - [028 - Amazon DynamoDB](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/028%20-%20DynamoDB.ipynb)\n  - [029 - S3 Select](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/029%20-%20S3%20Select.ipynb)\n  - [030 - Data Api](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/030%20-%20Data%20Api.ipynb)\n  - [031 - OpenSearch](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/031%20-%20OpenSearch.ipynb)\n  - [032 - Lake Formation Governed Tables](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/032%20-%20Lake%20Formation%20Governed%20Tables.ipynb)\n  - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)\n  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0rc2/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)\n  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0rc2/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)\n- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html)\n  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-s3)\n  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-glue-catalog)\n  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-athena)\n  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-lake-formation)\n  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-redshift)\n  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#postgresql)\n  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#mysql)\n  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#sqlserver)\n  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#oracle)\n  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#data-api-redshift)\n  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#data-api-rds)\n  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#opensearch)\n  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-neptune)\n  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#dynamodb)\n  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-timestream)\n  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-emr)\n  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-cloudwatch-logs)\n  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-chime)\n  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-quicksight)\n  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-sts)\n  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-secrets-manager)\n  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#global-configurations)\n- [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)\n- [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)\n\n## Getting Help\n\nThe best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...\nYou may also find help on these community resources:\n* The #aws-sdk-pandas Slack [channel](https://join.slack.com/t/aws-sdk-pandas/shared_invite/zt-sxdx38sl-E0coRfAds8WdpxXD2Nzfrg)\n* Ask a question on [Stack Overflow](https://stackoverflow.com/questions/tagged/awswrangler)\n  and tag it with `awswrangler`\n\n## Community Resources\n\nPlease [send a Pull Request](https://github.com/aws/aws-sdk-pandas/edit/main/README.md) with your resource reference and @githubhandle.\n\n- [Optimize Python ETL by extending Pandas with AWS SDK for pandas](https://aws.amazon.com/blogs/big-data/optimize-python-etl-by-extending-pandas-with-aws-data-wrangler/) [[@igorborgest](https://github.com/igorborgest)]\n- [Reading Parquet Files With AWS Lambda](https://aprakash.wordpress.com/2020/04/14/reading-parquet-files-with-aws-lambda/) [[@anand086](https://github.com/anand086)]\n- [Transform AWS CloudTrail data using AWS SDK for pandas](https://aprakash.wordpress.com/2020/09/17/transform-aws-cloudtrail-data-using-aws-data-wrangler/) [[@anand086](https://github.com/anand086)]\n- [Rename Glue Tables using AWS SDK for pandas](https://ananddatastories.com/rename-glue-tables-using-aws-sdk-pandas/) [[@anand086](https://github.com/anand086)]\n- [Getting started on AWS SDK for pandas and Athena](https://medium.com/@dheerajsharmainampudi/getting-started-on-aws-sdk-pandas-and-athena-7b446c834076) [[@dheerajsharma21](https://github.com/dheerajsharma21)]\n- [Simplifying Pandas integration with AWS data related services](https://medium.com/@bv_subhash/aws-sdk-pandas-simplifying-pandas-integration-with-aws-data-related-services-2b3325c12188) [[@bvsubhash](https://github.com/bvsubhash)]\n- [Build an ETL pipeline using AWS S3, Glue and Athena](https://www.linkedin.com/pulse/build-etl-pipeline-using-aws-s3-glue-athena-data-wrangler-tom-reid/) [[@taupirho](https://github.com/taupirho)]\n\n## Logging\n\nEnabling internal logging examples:\n\n```py3\nimport logging\nlogging.basicConfig(level=logging.INFO, format="[%(name)s][%(funcName)s] %(message)s")\nlogging.getLogger("awswrangler").setLevel(logging.DEBUG)\nlogging.getLogger("botocore.credentials").setLevel(logging.CRITICAL)\n```\n\nInto AWS lambda:\n\n```py3\nimport logging\nlogging.getLogger("awswrangler").setLevel(logging.DEBUG)\n```\n\n## Who uses AWS SDK for pandas?\n\nKnowing which companies are using this library is important to help prioritize the project internally.\nIf you would like us to include your company’s name and/or logo in the README file to indicate that your company is using the AWS SDK for pandas, please raise a "Support Us" issue. If you would like us to display your company’s logo, please raise a linked pull request to provide an image file for the logo. Note that by raising a Support Us issue (and related pull request), you are granting AWS permission to use your company’s name (and logo) for the limited purpose described here and you are confirming that you have authority to grant such permission.\n\n- [Amazon](https://www.amazon.com/)\n- [AWS](https://aws.amazon.com/)\n- [Cepsa](https://cepsa.com) [[@alvaropc](https://github.com/alvaropc)]\n- [Cognitivo](https://www.cognitivo.ai/) [[@msantino](https://github.com/msantino)]\n- [Digio](https://www.digio.com.br/) [[@afonsomy](https://github.com/afonsomy)]\n- [DNX](https://www.dnx.solutions/) [[@DNXLabs](https://github.com/DNXLabs)]\n- [Fortescue Future Industries](https://ffi.com.au/) [[@spencervoorend](https://github.com/spencervoorend)]\n- [Funcional Health Tech](https://www.funcionalcorp.com.br/) [[@webysther](https://github.com/webysther)]\n- [Funding Circle](https://www.fundingcircle.com/) [[@pfig](https://github.com/pfig)]\n- [Infomach](https://www.infomach.com.br/)\n- [Informa Markets](https://www.informamarkets.com/en/home.html) [[@mateusmorato]](http://github.com/mateusmorato)\n- [LINE TV](https://www.linetv.tw/) [[@bryanyang0528](https://github.com/bryanyang0528)]\n- [Magnataur](https://magnataur.com) [[@brianmingus2](https://github.com/brianmingus2)]\n- [M4U](https://www.m4u.com.br/) [[@Thiago-Dantas](https://github.com/Thiago-Dantas)]\n- [NBCUniversal](https://www.nbcuniversal.com/) [[@vibe](https://github.com/vibe)]\n- [nrd.io](https://nrd.io/) [[@mrtns](https://github.com/mrtns)]\n- [OKRA Technologies](https://okra.ai) [[@JPFrancoia](https://github.com/JPFrancoia), [@schot](https://github.com/schot)]\n- [Pier](https://www.pier.digital/) [[@flaviomax](https://github.com/flaviomax)]\n- [Pismo](https://www.pismo.io/) [[@msantino](https://github.com/msantino)]\n- [ringDNA](https://www.ringdna.com/) [[@msropp](https://github.com/msropp)]\n- [Serasa Experian](https://www.serasaexperian.com.br/) [[@andre-marcos-perez](https://github.com/andre-marcos-perez)]\n- [Shipwell](https://shipwell.com/) [[@zacharycarter](https://github.com/zacharycarter)]\n- [strongDM](https://www.strongdm.com/) [[@mrtns](https://github.com/mrtns)]\n- [Thinkbumblebee](https://www.thinkbumblebee.com/) [[@dheerajsharma21]](https://github.com/dheerajsharma21)\n- [VTEX](https://vtex.com/us-en/) [[@igorborgest]](https://github.com/igorborgest)\n- [Zillow](https://www.zillow.com/) [[@nicholas-miles]](https://github.com/nicholas-miles)\n',
+    'long_description': '# AWS SDK for pandas (awswrangler)\n\nAWS Data Wrangler is now **AWS SDK for pandas (awswrangler)**.  We’re changing the name we use when we talk about the library, but everything else will stay the same.  You’ll still be able to install using `pip install awswrangler` and you won’t need to change any of your code.  As part of this change, we’ve moved the library from AWS Labs to the main AWS GitHub organisation but, thanks to the GitHub’s redirect feature, you’ll still be able to access the project by its old URLs until you update your bookmarks.  Our documentation has also moved to [aws-sdk-pandas.readthedocs.io](https://aws-sdk-pandas.readthedocs.io), but old bookmarks will redirect to the new site.\n\n*Pandas on AWS*\n\nEasy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).\n\n![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")\n![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)\n\n> An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com\n\n[![Release](https://img.shields.io/badge/release-3.0.0rc3-brightgreen.svg)](https://pypi.org/project/awswrangler/)\n[![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)\n\n[![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)\n[![Coverage](https://img.shields.io/badge/coverage-91%25-brightgreen.svg)](https://pypi.org/project/awswrangler/)\n![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)\n[![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)\n\n| Source | Downloads | Installation Command |\n|--------|-----------|----------------------|\n| **[PyPi](https://pypi.org/project/awswrangler/)**  | [![PyPI Downloads](https://pepy.tech/badge/awswrangler)](https://pypi.org/project/awswrangler/) | `pip install awswrangler` |\n| **[Conda](https://anaconda.org/conda-forge/awswrangler)** | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/awswrangler.svg)](https://anaconda.org/conda-forge/awswrangler) | `conda install -c conda-forge awswrangler` |\n\n> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>\n➡️`pip install \'awswrangler[redshift]\'`\n\nPowered By [<img src="https://arrow.apache.org/img/arrow.png" width="200">](https://arrow.apache.org/powered_by/)\n\n## Table of contents\n\n- [Quick Start](#quick-start)\n- [At Scale](#at-scale)\n- [Read The Docs](#read-the-docs)\n- [Getting Help](#getting-help)\n- [Community Resources](#community-resources)\n- [Logging](#logging)\n- [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-pandas)\n\n## Quick Start\n\nInstallation command: `pip install awswrangler`\n\n> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>\n➡️`pip install \'awswrangler[redshift]\'`\n\n```py3\nimport awswrangler as wr\nimport pandas as pd\nfrom datetime import datetime\n\ndf = pd.DataFrame({"id": [1, 2], "value": ["foo", "boo"]})\n\n# Storing data on Data Lake\nwr.s3.to_parquet(\n    df=df,\n    path="s3://bucket/dataset/",\n    dataset=True,\n    database="my_db",\n    table="my_table"\n)\n\n# Retrieving the data directly from Amazon S3\ndf = wr.s3.read_parquet("s3://bucket/dataset/", dataset=True)\n\n# Retrieving the data from Amazon Athena\ndf = wr.athena.read_sql_query("SELECT * FROM my_table", database="my_db")\n\n# Get a Redshift connection from Glue Catalog and retrieving data from Redshift Spectrum\ncon = wr.redshift.connect("my-glue-connection")\ndf = wr.redshift.read_sql_query("SELECT * FROM external_schema.my_table", con=con)\ncon.close()\n\n# Amazon Timestream Write\ndf = pd.DataFrame({\n    "time": [datetime.now(), datetime.now()],   \n    "my_dimension": ["foo", "boo"],\n    "measure": [1.0, 1.1],\n})\nrejected_records = wr.timestream.write(df,\n    database="sampleDB",\n    table="sampleTable",\n    time_col="time",\n    measure_col="measure",\n    dimensions_cols=["my_dimension"],\n)\n\n# Amazon Timestream Query\nwr.timestream.query("""\nSELECT time, measure_value::double, my_dimension\nFROM "sampleDB"."sampleTable" ORDER BY time DESC LIMIT 3\n""")\n\n```\n\n## At scale\nAWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.\n\nThe quickest way to get started is to use AWS Glue with Ray. Read our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/) to learn about it, then head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/release-3.0.0/tutorials) to discover even more features.\n\n### Installation\n```\npip install "awswrangler[modin,ray]==3.0.0rc3"\n```\n\nAs a result existing scripts can run on significantly larger datasets with no code rewrite. Supported APIs are parallelized across cores on a single machine or across multiple nodes on a cluster in the cloud.\n\n### Supported APIs\n\n<p align="center">\n\n| Service         | API                      | Implementation |\n|-----------------|--------------------------|:--------------:|\n| `S3`            | `read_parquet`           |       ✅        |\n|                 | `read_parquet_metadata`  |       ✅        |\n|                 | `read_parquet_table`     |       ✅        |\n|                 | `read_csv`               |       ✅        |\n|                 | `read_json`              |       ✅        |\n|                 | `read_fwf`               |       ✅        |\n|                 | `to_parquet`             |       ✅        |\n|                 | `to_csv`                 |       ✅        |\n|                 | `to_json`                |       ✅        |\n|                 | `select_query`           |       ✅        |\n|                 | `store_parquet_metadata` |       ✅        |\n|                 | `delete_objects`         |       ✅        |\n|                 | `describe_objects`       |       ✅        |\n|                 | `size_objects`           |       ✅        |\n|                 | `wait_objects_exist`     |       ✅        |\n|                 | `wait_objects_not_exist` |       ✅        |\n|                 | `merge_datasets`         |       ✅        |\n|                 | `copy_objects`           |       ✅        |\n| `Redshift`      | `copy`                   |       ✅        |\n|                 | `unload`                 |       ✅        |\n| `Athena`        | `read_sql_query`         |       ✅        |\n|                 | `read_sql_table`         |       ✅        |\n|                 | `describe_table`         |       ✅        |\n|                 | `get_query_results`      |       ✅        |\n|                 | `show_create_table`      |       ✅        |\n| `DynamoDB`      | `read_items`             |       ✅        |\n| `LakeFormation` | `read_sql_query`         |       ✅        |\n|                 | `read_sql_table`         |       ✅        |\n| `Timestream`    | `write`                  |       ✅        |\n</p>\n\n## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)\n\n- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/what.html)\n- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html)\n  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#pypi-pip)\n  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#conda)\n  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-lambda-layer)\n  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-python-shell-jobs)\n  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-pyspark-jobs)\n  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook)\n  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook-lifecycle)\n  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#emr)\n  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#from-source)\n- [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)\n  - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)\n  - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)\n  - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)\n  - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)\n  - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)\n  - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)\n  - [007 - Databases (Redshift, MySQL, PostgreSQL, SQL Server and Oracle)](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/007%20-%20Redshift%2C%20MySQL%2C%20PostgreSQL%2C%20SQL%20Server%2C%20Oracle.ipynb)\n  - [008 - Redshift - Copy & Unload.ipynb](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/008%20-%20Redshift%20-%20Copy%20%26%20Unload.ipynb)\n  - [009 - Redshift - Append, Overwrite and Upsert](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/009%20-%20Redshift%20-%20Append%2C%20Overwrite%2C%20Upsert.ipynb)\n  - [010 - Parquet Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/010%20-%20Parquet%20Crawler.ipynb)\n  - [011 - CSV Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/011%20-%20CSV%20Datasets.ipynb)\n  - [012 - CSV Crawler](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/012%20-%20CSV%20Crawler.ipynb)\n  - [013 - Merging Datasets on S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/013%20-%20Merging%20Datasets%20on%20S3.ipynb)\n  - [014 - Schema Evolution](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/014%20-%20Schema%20Evolution.ipynb)\n  - [015 - EMR](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/015%20-%20EMR.ipynb)\n  - [016 - EMR & Docker](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/016%20-%20EMR%20%26%20Docker.ipynb)\n  - [017 - Partition Projection](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/017%20-%20Partition%20Projection.ipynb)\n  - [018 - QuickSight](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/018%20-%20QuickSight.ipynb)\n  - [019 - Athena Cache](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/019%20-%20Athena%20Cache.ipynb)\n  - [020 - Spark Table Interoperability](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/020%20-%20Spark%20Table%20Interoperability.ipynb)\n  - [021 - Global Configurations](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/021%20-%20Global%20Configurations.ipynb)\n  - [022 - Writing Partitions Concurrently](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/022%20-%20Writing%20Partitions%20Concurrently.ipynb)\n  - [023 - Flexible Partitions Filter](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/023%20-%20Flexible%20Partitions%20Filter.ipynb)\n  - [024 - Athena Query Metadata](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/024%20-%20Athena%20Query%20Metadata.ipynb)\n  - [025 - Redshift - Loading Parquet files with Spectrum](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/025%20-%20Redshift%20-%20Loading%20Parquet%20files%20with%20Spectrum.ipynb)\n  - [026 - Amazon Timestream](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/026%20-%20Amazon%20Timestream.ipynb)\n  - [027 - Amazon Timestream 2](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/027%20-%20Amazon%20Timestream%202.ipynb)\n  - [028 - Amazon DynamoDB](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/028%20-%20DynamoDB.ipynb)\n  - [029 - S3 Select](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/029%20-%20S3%20Select.ipynb)\n  - [030 - Data Api](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/030%20-%20Data%20Api.ipynb)\n  - [031 - OpenSearch](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/031%20-%20OpenSearch.ipynb)\n  - [032 - Lake Formation Governed Tables](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/032%20-%20Lake%20Formation%20Governed%20Tables.ipynb)\n  - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)\n  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)\n  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)\n  - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)\n  - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)\n  - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)\n- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html)\n  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-s3)\n  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-glue-catalog)\n  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-athena)\n  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-lake-formation)\n  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-redshift)\n  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#postgresql)\n  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#mysql)\n  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#sqlserver)\n  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#oracle)\n  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-redshift)\n  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-rds)\n  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#opensearch)\n  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-neptune)\n  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#dynamodb)\n  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-timestream)\n  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-emr)\n  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-cloudwatch-logs)\n  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-chime)\n  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-quicksight)\n  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-sts)\n  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-secrets-manager)\n  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#global-configurations)\n- [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)\n- [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)\n\n## Getting Help\n\nThe best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...\nYou may also find help on these community resources:\n* The #aws-sdk-pandas Slack [channel](https://join.slack.com/t/aws-sdk-pandas/shared_invite/zt-sxdx38sl-E0coRfAds8WdpxXD2Nzfrg)\n* Ask a question on [Stack Overflow](https://stackoverflow.com/questions/tagged/awswrangler)\n  and tag it with `awswrangler`\n\n## Community Resources\n\nPlease [send a Pull Request](https://github.com/aws/aws-sdk-pandas/edit/main/README.md) with your resource reference and @githubhandle.\n\n- [Optimize Python ETL by extending Pandas with AWS SDK for pandas](https://aws.amazon.com/blogs/big-data/optimize-python-etl-by-extending-pandas-with-aws-data-wrangler/) [[@igorborgest](https://github.com/igorborgest)]\n- [Reading Parquet Files With AWS Lambda](https://aprakash.wordpress.com/2020/04/14/reading-parquet-files-with-aws-lambda/) [[@anand086](https://github.com/anand086)]\n- [Transform AWS CloudTrail data using AWS SDK for pandas](https://aprakash.wordpress.com/2020/09/17/transform-aws-cloudtrail-data-using-aws-data-wrangler/) [[@anand086](https://github.com/anand086)]\n- [Rename Glue Tables using AWS SDK for pandas](https://ananddatastories.com/rename-glue-tables-using-aws-sdk-pandas/) [[@anand086](https://github.com/anand086)]\n- [Getting started on AWS SDK for pandas and Athena](https://medium.com/@dheerajsharmainampudi/getting-started-on-aws-sdk-pandas-and-athena-7b446c834076) [[@dheerajsharma21](https://github.com/dheerajsharma21)]\n- [Simplifying Pandas integration with AWS data related services](https://medium.com/@bv_subhash/aws-sdk-pandas-simplifying-pandas-integration-with-aws-data-related-services-2b3325c12188) [[@bvsubhash](https://github.com/bvsubhash)]\n- [Build an ETL pipeline using AWS S3, Glue and Athena](https://www.linkedin.com/pulse/build-etl-pipeline-using-aws-s3-glue-athena-data-wrangler-tom-reid/) [[@taupirho](https://github.com/taupirho)]\n\n## Logging\n\nEnabling internal logging examples:\n\n```py3\nimport logging\nlogging.basicConfig(level=logging.INFO, format="[%(name)s][%(funcName)s] %(message)s")\nlogging.getLogger("awswrangler").setLevel(logging.DEBUG)\nlogging.getLogger("botocore.credentials").setLevel(logging.CRITICAL)\n```\n\nInto AWS lambda:\n\n```py3\nimport logging\nlogging.getLogger("awswrangler").setLevel(logging.DEBUG)\n```\n\n## Who uses AWS SDK for pandas?\n\nKnowing which companies are using this library is important to help prioritize the project internally.\nIf you would like us to include your company’s name and/or logo in the README file to indicate that your company is using the AWS SDK for pandas, please raise a "Support Us" issue. If you would like us to display your company’s logo, please raise a linked pull request to provide an image file for the logo. Note that by raising a Support Us issue (and related pull request), you are granting AWS permission to use your company’s name (and logo) for the limited purpose described here and you are confirming that you have authority to grant such permission.\n\n- [Amazon](https://www.amazon.com/)\n- [AWS](https://aws.amazon.com/)\n- [Cepsa](https://cepsa.com) [[@alvaropc](https://github.com/alvaropc)]\n- [Cognitivo](https://www.cognitivo.ai/) [[@msantino](https://github.com/msantino)]\n- [Digio](https://www.digio.com.br/) [[@afonsomy](https://github.com/afonsomy)]\n- [DNX](https://www.dnx.solutions/) [[@DNXLabs](https://github.com/DNXLabs)]\n- [Fortescue Future Industries](https://ffi.com.au/) [[@spencervoorend](https://github.com/spencervoorend)]\n- [Funcional Health Tech](https://www.funcionalcorp.com.br/) [[@webysther](https://github.com/webysther)]\n- [Funding Circle](https://www.fundingcircle.com/) [[@pfig](https://github.com/pfig)]\n- [Infomach](https://www.infomach.com.br/)\n- [Informa Markets](https://www.informamarkets.com/en/home.html) [[@mateusmorato]](http://github.com/mateusmorato)\n- [LINE TV](https://www.linetv.tw/) [[@bryanyang0528](https://github.com/bryanyang0528)]\n- [Magnataur](https://magnataur.com) [[@brianmingus2](https://github.com/brianmingus2)]\n- [M4U](https://www.m4u.com.br/) [[@Thiago-Dantas](https://github.com/Thiago-Dantas)]\n- [NBCUniversal](https://www.nbcuniversal.com/) [[@vibe](https://github.com/vibe)]\n- [nrd.io](https://nrd.io/) [[@mrtns](https://github.com/mrtns)]\n- [OKRA Technologies](https://okra.ai) [[@JPFrancoia](https://github.com/JPFrancoia), [@schot](https://github.com/schot)]\n- [Pier](https://www.pier.digital/) [[@flaviomax](https://github.com/flaviomax)]\n- [Pismo](https://www.pismo.io/) [[@msantino](https://github.com/msantino)]\n- [ringDNA](https://www.ringdna.com/) [[@msropp](https://github.com/msropp)]\n- [Serasa Experian](https://www.serasaexperian.com.br/) [[@andre-marcos-perez](https://github.com/andre-marcos-perez)]\n- [Shipwell](https://shipwell.com/) [[@zacharycarter](https://github.com/zacharycarter)]\n- [strongDM](https://www.strongdm.com/) [[@mrtns](https://github.com/mrtns)]\n- [Thinkbumblebee](https://www.thinkbumblebee.com/) [[@dheerajsharma21]](https://github.com/dheerajsharma21)\n- [VTEX](https://vtex.com/us-en/) [[@igorborgest]](https://github.com/igorborgest)\n- [Zillow](https://www.zillow.com/) [[@nicholas-miles]](https://github.com/nicholas-miles)\n',
     'author': 'Amazon Web Services',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aws-sdk-pandas.readthedocs.io/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `awswrangler-3.0.0rc2/PKG-INFO` & `awswrangler-3.0.0rc3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awswrangler
-Version: 3.0.0rc2
+Version: 3.0.0rc3
 Summary: Pandas on AWS.
 Home-page: https://aws-sdk-pandas.readthedocs.io/
 License: Apache-2.0
 Keywords: pandas,aws
 Author: Amazon Web Services
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,39 +12,50 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: deltalake
+Provides-Extra: gremlin
 Provides-Extra: modin
+Provides-Extra: mysql
+Provides-Extra: opencypher
+Provides-Extra: openpyxl
+Provides-Extra: opensearch
 Provides-Extra: oracle
+Provides-Extra: postgres
+Provides-Extra: progressbar
 Provides-Extra: ray
+Provides-Extra: redshift
 Provides-Extra: sparql
 Provides-Extra: sqlserver
 Requires-Dist: SPARQLWrapper (>=2.0.0,<3.0.0); extra == "sparql"
-Requires-Dist: backoff (>=2.0.0,<3.0.0)
-Requires-Dist: boto3 (>=1.24.11,<2.0.0)
-Requires-Dist: botocore (>=1.27.11,<2.0.0)
-Requires-Dist: gremlinpython (>=3.5.2,<4.0.0)
-Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
-Requires-Dist: modin (>=0.16.0,<0.17.0); extra == "modin"
-Requires-Dist: numpy (>=1.22.4,<2.0.0)
-Requires-Dist: openpyxl (>=3.0.0,<3.1.0)
-Requires-Dist: opensearch-py (>=2.0.0,<3.0.0)
-Requires-Dist: oracledb (>=1.0.0,<1.1.0); extra == "oracle"
-Requires-Dist: pandas (>=1.2.0,<2.0.0,<=1.5.1,!=1.5.0)
-Requires-Dist: pg8000 (>=1.29.0,<2.0.0)
-Requires-Dist: progressbar2 (>=4.0.0,<5.0.0)
-Requires-Dist: pyarrow (>=6.0.0,<8.1.0)
-Requires-Dist: pymysql (>=1.0.0,<2.0.0)
-Requires-Dist: pyodbc (>=4.0.32,<4.1.0); extra == "sqlserver"
-Requires-Dist: ray[data,default] (>=2.0.0,<2.1.0); extra == "ray"
-Requires-Dist: redshift-connector (>=2.0.889,<2.1.0)
-Requires-Dist: requests-aws4auth (>=1.1.1,<2.0.0)
+Requires-Dist: boto3 (>=1.20.32,<2.0.0)
+Requires-Dist: botocore (>=1.23.32,<2.0.0)
+Requires-Dist: deltalake (>=0.6.4,<0.7.0); extra == "deltalake"
+Requires-Dist: gremlinpython (>=3.5.2,<4.0.0); extra == "gremlin"
+Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0); extra == "opensearch"
+Requires-Dist: modin (>=0.18.0,<0.19.0); extra == "modin"
+Requires-Dist: numpy (>=1.18,<2.0)
+Requires-Dist: openpyxl (>=3.0.0,<4.0.0); extra == "openpyxl"
+Requires-Dist: opensearch-py (>=2.0.0,<3.0.0); extra == "opensearch"
+Requires-Dist: oracledb (>=1.0.0,<2.0.0); extra == "oracle"
+Requires-Dist: pandas (>=1.0,<2.0)
+Requires-Dist: pg8000 (>=1.29.0,<2.0.0); extra == "postgres"
+Requires-Dist: progressbar2 (>=4.0.0,<5.0.0); extra == "progressbar"
+Requires-Dist: pyarrow (>=7.0.0)
+Requires-Dist: pymysql (>=1.0.0,<2.0.0); extra == "mysql"
+Requires-Dist: pyodbc (>=4.0.0,<5.0.0); extra == "sqlserver"
+Requires-Dist: ray[data,default] (>=2.0.0,<2.4.0); extra == "ray"
+Requires-Dist: redshift-connector (>=2.0.0,<3.0.0); extra == "redshift"
+Requires-Dist: requests (>=2.0.0,<3.0.0); extra == "gremlin" or extra == "sparql" or extra == "opencypher"
+Requires-Dist: requests-aws4auth (>=1.1.1,<2.0.0); extra == "opensearch"
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://aws-sdk-pandas.readthedocs.io/
 Project-URL: Repository, https://github.com/aws/aws-sdk-pandas
 Description-Content-Type: text/markdown
 
 # AWS SDK for pandas (awswrangler)
 
 AWS Data Wrangler is now **AWS SDK for pandas (awswrangler)**.  We’re changing the name we use when we talk about the library, but everything else will stay the same.  You’ll still be able to install using `pip install awswrangler` and you won’t need to change any of your code.  As part of this change, we’ve moved the library from AWS Labs to the main AWS GitHub organisation but, thanks to the GitHub’s redirect feature, you’ll still be able to access the project by its old URLs until you update your bookmarks.  Our documentation has also moved to [aws-sdk-pandas.readthedocs.io](https://aws-sdk-pandas.readthedocs.io), but old bookmarks will redirect to the new site.
@@ -54,31 +65,31 @@
 Easy integration with Athena, Glue, Redshift, Timestream, OpenSearch, Neptune, QuickSight, Chime, CloudWatchLogs, DynamoDB, EMR, SecretManager, PostgreSQL, MySQL, SQLServer and S3 (Parquet, CSV, JSON and EXCEL).
 
 ![AWS SDK for pandas](docs/source/_static/logo2.png?raw=true "AWS SDK for pandas")
 ![tracker](https://d3tiqpr4kkkomd.cloudfront.net/img/pixel.png?asset=GVOYN2BOOQ573LTVIHEW)
 
 > An [AWS Professional Service](https://aws.amazon.com/professional-services/) open source initiative | aws-proserve-opensource@amazon.com
 
-[![Release](https://img.shields.io/badge/release-3.0.0rc2-brightgreen.svg)](https://pypi.org/project/awswrangler/)
+[![Release](https://img.shields.io/badge/release-3.0.0rc3-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 [![Python Version](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-brightgreen.svg)](https://anaconda.org/conda-forge/awswrangler)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Coverage](https://img.shields.io/badge/coverage-91%25-brightgreen.svg)](https://pypi.org/project/awswrangler/)
 ![Static Checking](https://github.com/aws/aws-sdk-pandas/workflows/Static%20Checking/badge.svg?branch=main)
 [![Documentation Status](https://readthedocs.org/projects/aws-sdk-pandas/badge/?version=latest)](https://aws-sdk-pandas.readthedocs.io/?badge=latest)
 
 | Source | Downloads | Installation Command |
 |--------|-----------|----------------------|
 | **[PyPi](https://pypi.org/project/awswrangler/)**  | [![PyPI Downloads](https://pepy.tech/badge/awswrangler)](https://pypi.org/project/awswrangler/) | `pip install awswrangler` |
 | **[Conda](https://anaconda.org/conda-forge/awswrangler)** | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/awswrangler.svg)](https://anaconda.org/conda-forge/awswrangler) | `conda install -c conda-forge awswrangler` |
 
-> ⚠️ **For platforms without PyArrow 3 support (e.g. [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr-cluster), [Glue PySpark Job](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs), MWAA):**<br>
-➡️ `pip install pyarrow==2 awswrangler`
+> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>
+➡️`pip install 'awswrangler[redshift]'`
 
 Powered By [<img src="https://arrow.apache.org/img/arrow.png" width="200">](https://arrow.apache.org/powered_by/)
 
 ## Table of contents
 
 - [Quick Start](#quick-start)
 - [At Scale](#at-scale)
@@ -88,16 +99,16 @@
 - [Logging](#logging)
 - [Who uses AWS SDK for pandas?](#who-uses-aws-sdk-pandas)
 
 ## Quick Start
 
 Installation command: `pip install awswrangler`
 
-> ⚠️ **For platforms without PyArrow 3 support (e.g. [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr-cluster), [Glue PySpark Job](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs), MWAA):**<br>
-➡️`pip install pyarrow==2 awswrangler`
+> ⚠️ **Starting version 3.0, optional modules must be installed explicitly:**<br>
+➡️`pip install 'awswrangler[redshift]'`
 
 ```py3
 import awswrangler as wr
 import pandas as pd
 from datetime import datetime
 
 df = pd.DataFrame({"id": [1, 2], "value": ["foo", "boo"]})
@@ -141,60 +152,75 @@
 SELECT time, measure_value::double, my_dimension
 FROM "sampleDB"."sampleTable" ORDER BY time DESC LIMIT 3
 """)
 
 ```
 
 ## At scale
-AWS SDK for pandas can also run your workflows at scale by leveraging [modin](https://modin.readthedocs.io/en/stable/) and [ray](https://www.ray.io/). Both projects aim to speed up data workloads (pandas workloads in particular in the case of modin) by distributing processing over a cluster of workers.
+AWS SDK for pandas can also run your workflows at scale by leveraging [Modin](https://modin.readthedocs.io/en/stable/) and [Ray](https://www.ray.io/). Both projects aim to speed up data workloads by distributing processing over a cluster of workers.
+
+The quickest way to get started is to use AWS Glue with Ray. Read our [blog](https://aws.amazon.com/blogs/big-data/scale-aws-sdk-for-pandas-workloads-with-aws-glue-for-ray/) to learn about it, then head to our latest [tutorials](https://github.com/aws/aws-sdk-pandas/tree/release-3.0.0/tutorials) to discover even more features.
 
 ### Installation
 ```
-pip install "awswrangler[modin,ray]==3.0.0rc2"
+pip install "awswrangler[modin,ray]==3.0.0rc3"
 ```
 
 As a result existing scripts can run on significantly larger datasets with no code rewrite. Supported APIs are parallelized across cores on a single machine or across multiple nodes on a cluster in the cloud.
 
 ### Supported APIs
 
 <p align="center">
 
-| Service     | API                                                           | Implementation |
-|-------------------|:------------------------------------------------------------------------------------:|:---------------:|
-|  `S3`    | `read_parquet`                                               | ✅ |
-|    | `read_csv`                                               | ✅ |
-|    | `read_json`                                               | ✅ |
-|    | `read_fwf`                                               | ✅ |
-|    | `to_parquet`                                               | ✅ |
-|    | `to_csv`                                               | ✅ |
-|    | `to_json`                                               | ✅ |
-|    | `select_query`                                               | ✅ |
-|    | `delete`                                               | ✅ |
-|    | `copy`                                               | ✅ |
-|    | `wait`                                               | ✅ |
-|  `Redshift`    | `copy`                                               | ✅ |
-|    | `unload`                                               | ✅ |
-|  `Athena`    | `read_sql_query`                                               | ✅ |
-|  `LakeFormation`    | `read_sql_query`                                               | ✅ |
-|  `Timestream`    | `write`                                               | ✅ |
+| Service         | API                      | Implementation |
+|-----------------|--------------------------|:--------------:|
+| `S3`            | `read_parquet`           |       ✅        |
+|                 | `read_parquet_metadata`  |       ✅        |
+|                 | `read_parquet_table`     |       ✅        |
+|                 | `read_csv`               |       ✅        |
+|                 | `read_json`              |       ✅        |
+|                 | `read_fwf`               |       ✅        |
+|                 | `to_parquet`             |       ✅        |
+|                 | `to_csv`                 |       ✅        |
+|                 | `to_json`                |       ✅        |
+|                 | `select_query`           |       ✅        |
+|                 | `store_parquet_metadata` |       ✅        |
+|                 | `delete_objects`         |       ✅        |
+|                 | `describe_objects`       |       ✅        |
+|                 | `size_objects`           |       ✅        |
+|                 | `wait_objects_exist`     |       ✅        |
+|                 | `wait_objects_not_exist` |       ✅        |
+|                 | `merge_datasets`         |       ✅        |
+|                 | `copy_objects`           |       ✅        |
+| `Redshift`      | `copy`                   |       ✅        |
+|                 | `unload`                 |       ✅        |
+| `Athena`        | `read_sql_query`         |       ✅        |
+|                 | `read_sql_table`         |       ✅        |
+|                 | `describe_table`         |       ✅        |
+|                 | `get_query_results`      |       ✅        |
+|                 | `show_create_table`      |       ✅        |
+| `DynamoDB`      | `read_items`             |       ✅        |
+| `LakeFormation` | `read_sql_query`         |       ✅        |
+|                 | `read_sql_table`         |       ✅        |
+| `Timestream`    | `write`                  |       ✅        |
 </p>
 
 ## [Read The Docs](https://aws-sdk-pandas.readthedocs.io/)
 
-- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/what.html)
-- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html)
-  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#pypi-pip)
-  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#conda)
-  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-lambda-layer)
-  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-python-shell-jobs)
-  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#aws-glue-pyspark-jobs)
-  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#amazon-sagemaker-notebook)
-  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#amazon-sagemaker-notebook-lifecycle)
-  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#emr)
-  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/install.html#from-source)
+- [**What is AWS SDK for pandas?**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/what.html)
+- [**Install**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html)
+  - [PyPi (pip)](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#pypi-pip)
+  - [Conda](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#conda)
+  - [AWS Lambda Layer](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-lambda-layer)
+  - [AWS Glue Python Shell Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-python-shell-jobs)
+  - [AWS Glue PySpark Jobs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#aws-glue-pyspark-jobs)
+  - [Amazon SageMaker Notebook](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook)
+  - [Amazon SageMaker Notebook Lifecycle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#amazon-sagemaker-notebook-lifecycle)
+  - [EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#emr)
+  - [From source](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/install.html#from-source)
 - [**Tutorials**](https://github.com/aws/aws-sdk-pandas/tree/main/tutorials)
   - [001 - Introduction](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/001%20-%20Introduction.ipynb)
   - [002 - Sessions](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/002%20-%20Sessions.ipynb)
   - [003 - Amazon S3](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/003%20-%20Amazon%20S3.ipynb)
   - [004 - Parquet Datasets](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/004%20-%20Parquet%20Datasets.ipynb)
   - [005 - Glue Catalog](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/005%20-%20Glue%20Catalog.ipynb)
   - [006 - Amazon Athena](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/006%20-%20Amazon%20Athena.ipynb)
@@ -221,39 +247,42 @@
   - [027 - Amazon Timestream 2](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/027%20-%20Amazon%20Timestream%202.ipynb)
   - [028 - Amazon DynamoDB](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/028%20-%20DynamoDB.ipynb)
   - [029 - S3 Select](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/029%20-%20S3%20Select.ipynb)
   - [030 - Data Api](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/030%20-%20Data%20Api.ipynb)
   - [031 - OpenSearch](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/031%20-%20OpenSearch.ipynb)
   - [032 - Lake Formation Governed Tables](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/032%20-%20Lake%20Formation%20Governed%20Tables.ipynb)
   - [033 - Amazon Neptune](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/033%20-%20Amazon%20Neptune.ipynb)
-  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0rc2/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
-  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0rc2/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
-- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html)
-  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-s3)
-  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-glue-catalog)
-  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-athena)
-  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-lake-formation)
-  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-redshift)
-  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#postgresql)
-  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#mysql)
-  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#sqlserver)
-  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#oracle)
-  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#data-api-redshift)
-  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#data-api-rds)
-  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#opensearch)
-  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-neptune)
-  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#dynamodb)
-  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-timestream)
-  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-emr)
-  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-cloudwatch-logs)
-  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-chime)
-  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#amazon-quicksight)
-  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-sts)
-  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#aws-secrets-manager)
-  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc2/api.html#global-configurations)
+  - [034 - Distributing Calls Using Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/034%20-%20Distributing%20Calls%20using%20Ray.ipynb)
+  - [035 - Distributing Calls on Ray Remote Cluster](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/035%20-%20Distributing%20Calls%20on%20Ray%20Remote%20Cluster.ipynb)
+  - [036 - Distributing Calls with Glue Interactive Sessions on Ray](https://github.com/aws/aws-sdk-pandas/blob/release-3.0.0/tutorials/036%20-%20Distributing%20Calls%20with%20Glue%20Interactive%20Sessions%20on%20Ray.ipynb)
+  - [037 - Glue Data Quality](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/037%20-%20Glue%20Data%20Quality.ipynb)
+  - [038 - OpenSearch Serverless](https://github.com/aws/aws-sdk-pandas/blob/main/tutorials/038%20-%20OpenSearch%20Serverless.ipynb)
+- [**API Reference**](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html)
+  - [Amazon S3](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-s3)
+  - [AWS Glue Catalog](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-glue-catalog)
+  - [Amazon Athena](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-athena)
+  - [AWS Lake Formation](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-lake-formation)
+  - [Amazon Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-redshift)
+  - [PostgreSQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#postgresql)
+  - [MySQL](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#mysql)
+  - [SQL Server](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#sqlserver)
+  - [Oracle](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#oracle)
+  - [Data API Redshift](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-redshift)
+  - [Data API RDS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#data-api-rds)
+  - [OpenSearch](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#opensearch)
+  - [Amazon Neptune](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-neptune)
+  - [DynamoDB](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#dynamodb)
+  - [Amazon Timestream](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-timestream)
+  - [Amazon EMR](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-emr)
+  - [Amazon CloudWatch Logs](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-cloudwatch-logs)
+  - [Amazon Chime](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-chime)
+  - [Amazon QuickSight](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#amazon-quicksight)
+  - [AWS STS](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-sts)
+  - [AWS Secrets Manager](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#aws-secrets-manager)
+  - [Global Configurations](https://aws-sdk-pandas.readthedocs.io/en/3.0.0rc3/api.html#global-configurations)
 - [**License**](https://github.com/aws/aws-sdk-pandas/blob/main/LICENSE.txt)
 - [**Contributing**](https://github.com/aws/aws-sdk-pandas/blob/main/CONTRIBUTING.md)
 
 ## Getting Help
 
 The best way to interact with our team is through GitHub. You can open an [issue](https://github.com/aws/aws-sdk-pandas/issues/new/choose) and choose from one of our templates for bug reports, feature requests...
 You may also find help on these community resources:
```

