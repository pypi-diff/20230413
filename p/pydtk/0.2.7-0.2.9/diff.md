# Comparing `tmp/pydtk-0.2.7.tar.gz` & `tmp/pydtk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydtk-0.2.7.tar", max compression
+gzip compressed data, was "pydtk-0.2.9.tar", max compression
```

## Comparing `pydtk-0.2.7.tar` & `pydtk-0.2.9.tar`

### file list

```diff
@@ -1,116 +1,120 @@
--rw-r--r--   0        0        0    11340 2022-12-26 04:31:29.178282 pydtk-0.2.7/LICENSE
--rw-r--r--   0        0        0     2574 2022-12-26 04:31:29.178282 pydtk-0.2.7/README.md
--rw-r--r--   0        0        0      103 2022-12-26 04:31:46.538392 pydtk-0.2.7/pydtk/__init__.py
--rw-r--r--   0        0        0       44 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/__init__.py
--rwxr-xr-x   0        0        0     2184 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/cli.py
--rwxr-xr-x   0        0        0     3679 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/make_meta.py
--rw-r--r--   0        0        0     2631 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/oas.py
--rw-r--r--   0        0        0       28 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/sub_commands/__init__.py
--rw-r--r--   0        0        0    14604 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/sub_commands/db.py
--rw-r--r--   0        0        0      585 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/sub_commands/io.py
--rw-r--r--   0        0        0     4246 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/sub_commands/model.py
--rw-r--r--   0        0        0     1501 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/bin/sub_commands/status.py
--rw-r--r--   0        0        0       44 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/__init__.py
--rwxr-xr-x   0        0        0     1578 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/concat_df.py
--rw-r--r--   0        0        0       44 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/dbdb/__init__.py
--rwxr-xr-x   0        0        0     5177 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/dbdb/file_info.py
--rwxr-xr-x   0        0        0     6453 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/df_list.py
--rwxr-xr-x   0        0        0     1696 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/df_path.py
--rwxr-xr-x   0        0        0     3473 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/meta_db.py
--rwxr-xr-x   0        0        0     6572 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/builder/statistic_db.py
--rw-r--r--   0        0        0      697 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/conf/v1.yaml
--rw-r--r--   0        0        0     1477 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/conf/v2.yaml
--rw-r--r--   0        0        0     2553 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/conf/v3.yaml
--rw-r--r--   0        0        0     2185 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/conf/v4.yaml
--rw-r--r--   0        0        0     1093 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/__init__.py
--rw-r--r--   0        0        0      305 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/exceptions.py
--rw-r--r--   0        0        0     2965 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/__init__.py
--rw-r--r--   0        0        0      504 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation.py
--rw-r--r--   0        0        0     1123 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_pixel.py
--rw-r--r--   0        0        0     1387 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_rectangular_area.py
--rw-r--r--   0        0        0      903 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_point.py
--rw-r--r--   0        0        0      512 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py
--rw-r--r--   0        0        0      399 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/record.py
--rw-r--r--   0        0        0        0 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha2/__init__.py
--rw-r--r--   0        0        0      697 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha2/file.py
--rw-r--r--   0        0        0      584 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py
--rw-r--r--   0        0        0      193 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/v1/__init__.py
--rw-r--r--   0        0        0     6508 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/v1/handlers/__init__.py
--rw-r--r--   0        0        0     4913 2022-12-26 04:31:29.182282 pydtk-0.2.7/pydtk/db/v1/handlers/meta.py
--rw-r--r--   0        0        0      360 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v2/__init__.py
--rw-r--r--   0        0        0    18710 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v2/handlers/__init__.py
--rw-r--r--   0        0        0     4519 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v2/handlers/meta.py
--rw-r--r--   0        0        0     1494 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v2/search_engines/__init__.py
--rw-r--r--   0        0        0     1813 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v2/search_engines/time_series.py
--rw-r--r--   0        0        0      562 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v3/__init__.py
--rw-r--r--   0        0        0    22454 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v3/handlers/__init__.py
--rw-r--r--   0        0        0    10185 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v3/handlers/meta.py
--rw-r--r--   0        0        0     4960 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v3/handlers/statistics.py
--rw-r--r--   0        0        0    12075 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v3/handlers/time_series.py
--rw-r--r--   0        0        0     4376 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v3/search_engines/__init__.py
--rw-r--r--   0        0        0     2409 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v3/search_engines/time_series.py
--rw-r--r--   0        0        0      288 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/__init__.py
--rw-r--r--   0        0        0      271 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/deps/__init__.py
--rw-r--r--   0        0        0       66 2022-12-26 04:31:29.830286 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/.git
--rw-r--r--   0        0        0       61 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/.gitignore
--rw-r--r--   0        0        0     1496 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/LICENSE
--rw-r--r--   0        0        0     7682 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/README.md
--rw-r--r--   0        0        0     5531 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/aggregation_tests.py
--rw-r--r--   0        0        0     7885 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/find_tests.py
--rw-r--r--   0        0        0     3066 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/pql/__init__.py
--rw-r--r--   0        0        0     4848 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/pql/aggregation.py
--rw-r--r--   0        0        0    14159 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/pql/matching.py
--rw-r--r--   0        0        0      929 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/setup.py
--rw-r--r--   0        0        0       64 2022-12-26 04:31:31.682297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/tox.ini
--rw-r--r--   0        0        0       66 2022-12-26 04:31:30.398289 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/.git
--rw-r--r--   0        0        0       61 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/.gitignore
--rw-r--r--   0        0        0     1496 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/LICENSE
--rw-r--r--   0        0        0     7682 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/README.md
--rw-r--r--   0        0        0     5531 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/aggregation_tests.py
--rw-r--r--   0        0        0     8389 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/find_tests.py
--rw-r--r--   0        0        0     3066 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/pql/__init__.py
--rw-r--r--   0        0        0     4848 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/pql/aggregation.py
--rw-r--r--   0        0        0    15543 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/pql/matching.py
--rw-r--r--   0        0        0     1116 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/setup.py
--rw-r--r--   0        0        0      112 2022-12-26 04:31:31.694297 pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/tox.ini
--rw-r--r--   0        0        0      954 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/engines/__init__.py
--rw-r--r--   0        0        0     6354 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/engines/mongodb.py
--rw-r--r--   0        0        0     5491 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/engines/montydb.py
--rw-r--r--   0        0        0     2854 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/engines/tinydb.py
--rw-r--r--   0        0        0     5716 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/engines/tinymongo.py
--rw-r--r--   0        0        0    26613 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/handlers/__init__.py
--rw-r--r--   0        0        0     3169 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/handlers/annotation.py
--rw-r--r--   0        0        0    16709 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/db/v4/handlers/meta.py
--rwxr-xr-x   0        0        0     1456 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/frontend.py
--rw-r--r--   0        0        0      256 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/io/__init__.py
--rw-r--r--   0        0        0      187 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/io/errors.py
--rw-r--r--   0        0        0     4732 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/io/reader.py
--rw-r--r--   0        0        0     2459 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/io/writer.py
--rw-r--r--   0        0        0    18983 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/__init__.py
--rw-r--r--   0        0        0       67 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/autoware/__init__.py
--rw-r--r--   0        0        0     2402 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/autoware/can_packet.py
--rw-r--r--   0        0        0     6969 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/csv.py
--rw-r--r--   0        0        0     1991 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/image.py
--rw-r--r--   0        0        0     2308 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/json_model.py
--rw-r--r--   0        0        0    11798 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/movie.py
--rw-r--r--   0        0        0       58 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/pointcloud/__init__.py
--rw-r--r--   0        0        0     3413 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/pointcloud/pcd.py
--rw-r--r--   0        0        0    11181 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/rosbag.py
--rw-r--r--   0        0        0    15066 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/rosbag2.py
--rw-r--r--   0        0        0       65 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/zstd/__init__.py
--rw-r--r--   0        0        0     4374 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/models/zstd/rosbag.py
--rw-r--r--   0        0        0      131 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/preprocesses/__init__.py
--rwxr-xr-x   0        0        0     2527 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/preprocesses/downsampling.py
--rwxr-xr-x   0        0        0      929 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/preprocesses/passthrough.py
--rwxr-xr-x   0        0        0      352 2022-12-26 04:31:29.186282 pydtk-0.2.7/pydtk/preprocesses/preprocess.py
--rw-r--r--   0        0        0     3648 2022-12-26 04:31:29.190282 pydtk-0.2.7/pydtk/statistics/__init__.py
--rwxr-xr-x   0        0        0     8688 2022-12-26 04:31:29.190282 pydtk-0.2.7/pydtk/statistics/calculator.py
--rw-r--r--   0        0        0       44 2022-12-26 04:31:29.190282 pydtk-0.2.7/pydtk/utils/__init__.py
--rw-r--r--   0        0        0    18150 2022-12-26 04:31:29.190282 pydtk-0.2.7/pydtk/utils/can_decoder.py
--rwxr-xr-x   0        0        0     2728 2022-12-26 04:31:29.190282 pydtk-0.2.7/pydtk/utils/fileutils.py
--rwxr-xr-x   0        0        0     7034 2022-12-26 04:31:29.190282 pydtk-0.2.7/pydtk/utils/utils.py
--rwxr-xr-x   0        0        0     2560 2022-12-26 04:31:46.530392 pydtk-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5459 2022-12-26 04:31:47.923086 pydtk-0.2.7/setup.py
--rw-r--r--   0        0        0     4664 2022-12-26 04:31:47.924049 pydtk-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-02-09 04:26:45.614931 pydtk-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2574 2023-02-09 04:26:45.614931 pydtk-0.2.9/README.md
+-rw-r--r--   0        0        0      103 2023-02-09 04:27:01.803170 pydtk-0.2.9/pydtk/__init__.py
+-rw-r--r--   0        0        0       44 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/__init__.py
+-rwxr-xr-x   0        0        0     2184 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/cli.py
+-rwxr-xr-x   0        0        0     3679 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/make_meta.py
+-rw-r--r--   0        0        0     2631 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/oas.py
+-rw-r--r--   0        0        0       28 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/__init__.py
+-rw-r--r--   0        0        0    14844 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/db.py
+-rw-r--r--   0        0        0      585 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/io.py
+-rw-r--r--   0        0        0     4310 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/model.py
+-rw-r--r--   0        0        0     1501 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/bin/sub_commands/status.py
+-rw-r--r--   0        0        0       44 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/__init__.py
+-rwxr-xr-x   0        0        0     1578 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/concat_df.py
+-rw-r--r--   0        0        0       44 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/dbdb/__init__.py
+-rwxr-xr-x   0        0        0     5177 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/dbdb/file_info.py
+-rwxr-xr-x   0        0        0     6453 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/df_list.py
+-rwxr-xr-x   0        0        0     1696 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/df_path.py
+-rwxr-xr-x   0        0        0     3473 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/meta_db.py
+-rwxr-xr-x   0        0        0     6572 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/builder/statistic_db.py
+-rw-r--r--   0        0        0      697 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v1.yaml
+-rw-r--r--   0        0        0     1477 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v2.yaml
+-rw-r--r--   0        0        0     2553 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v3.yaml
+-rw-r--r--   0        0        0     2185 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/conf/v4.yaml
+-rw-r--r--   0        0        0     1093 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/__init__.py
+-rw-r--r--   0        0        0      305 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/exceptions.py
+-rw-r--r--   0        0        0     4114 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/__init__.py
+-rw-r--r--   0        0        0      504 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation.py
+-rw-r--r--   0        0        0     1123 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_pixel.py
+-rw-r--r--   0        0        0     1387 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_rectangular_area.py
+-rw-r--r--   0        0        0      903 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_point.py
+-rw-r--r--   0        0        0      512 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py
+-rw-r--r--   0        0        0      399 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/record.py
+-rw-r--r--   0        0        0        0 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/__init__.py
+-rw-r--r--   0        0        0      540 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation.py
+-rw-r--r--   0        0        0     1123 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_pixel.py
+-rw-r--r--   0        0        0     1387 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_image_rectangular_area.py
+-rw-r--r--   0        0        0      903 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation_commented_point.py
+-rw-r--r--   0        0        0      891 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/file.py
+-rw-r--r--   0        0        0      780 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py
+-rw-r--r--   0        0        0      193 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v1/__init__.py
+-rw-r--r--   0        0        0     6508 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v1/handlers/__init__.py
+-rw-r--r--   0        0        0     4913 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v1/handlers/meta.py
+-rw-r--r--   0        0        0      360 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/__init__.py
+-rw-r--r--   0        0        0    18716 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/handlers/__init__.py
+-rw-r--r--   0        0        0     4519 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/handlers/meta.py
+-rw-r--r--   0        0        0     1494 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/search_engines/__init__.py
+-rw-r--r--   0        0        0     1813 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v2/search_engines/time_series.py
+-rw-r--r--   0        0        0      562 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/__init__.py
+-rw-r--r--   0        0        0    22454 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/__init__.py
+-rw-r--r--   0        0        0    10185 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/meta.py
+-rw-r--r--   0        0        0     4960 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/statistics.py
+-rw-r--r--   0        0        0    12075 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/handlers/time_series.py
+-rw-r--r--   0        0        0     4376 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/search_engines/__init__.py
+-rw-r--r--   0        0        0     2409 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v3/search_engines/time_series.py
+-rw-r--r--   0        0        0      288 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/__init__.py
+-rw-r--r--   0        0        0      271 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/deps/__init__.py
+-rw-r--r--   0        0        0       66 2023-02-09 04:26:46.118938 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/.git
+-rw-r--r--   0        0        0       61 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/.gitignore
+-rw-r--r--   0        0        0     1496 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/LICENSE
+-rw-r--r--   0        0        0     7682 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/README.md
+-rw-r--r--   0        0        0     5531 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/aggregation_tests.py
+-rw-r--r--   0        0        0     7885 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/find_tests.py
+-rw-r--r--   0        0        0     3066 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/__init__.py
+-rw-r--r--   0        0        0     4848 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/aggregation.py
+-rw-r--r--   0        0        0    14159 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/matching.py
+-rw-r--r--   0        0        0      929 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/setup.py
+-rw-r--r--   0        0        0       64 2023-02-09 04:26:47.534959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/tox.ini
+-rw-r--r--   0        0        0       66 2023-02-09 04:26:46.522944 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/.git
+-rw-r--r--   0        0        0       61 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/.gitignore
+-rw-r--r--   0        0        0     1496 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/LICENSE
+-rw-r--r--   0        0        0     7682 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/README.md
+-rw-r--r--   0        0        0     5531 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/aggregation_tests.py
+-rw-r--r--   0        0        0     8389 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/find_tests.py
+-rw-r--r--   0        0        0     3066 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/__init__.py
+-rw-r--r--   0        0        0     4848 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/aggregation.py
+-rw-r--r--   0        0        0    15543 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/matching.py
+-rw-r--r--   0        0        0     1116 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/setup.py
+-rw-r--r--   0        0        0      112 2023-02-09 04:26:47.542959 pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/tox.ini
+-rw-r--r--   0        0        0      954 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/__init__.py
+-rw-r--r--   0        0        0     6354 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/mongodb.py
+-rw-r--r--   0        0        0     5543 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/montydb.py
+-rw-r--r--   0        0        0     2854 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/tinydb.py
+-rw-r--r--   0        0        0     5716 2023-02-09 04:26:45.618931 pydtk-0.2.9/pydtk/db/v4/engines/tinymongo.py
+-rw-r--r--   0        0        0    26623 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/db/v4/handlers/__init__.py
+-rw-r--r--   0        0        0     3169 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/db/v4/handlers/annotation.py
+-rw-r--r--   0        0        0    16709 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/db/v4/handlers/meta.py
+-rwxr-xr-x   0        0        0     1456 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/frontend.py
+-rw-r--r--   0        0        0      256 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/__init__.py
+-rw-r--r--   0        0        0      187 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/errors.py
+-rw-r--r--   0        0        0     4732 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/reader.py
+-rw-r--r--   0        0        0     2459 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/io/writer.py
+-rw-r--r--   0        0        0    18983 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/__init__.py
+-rw-r--r--   0        0        0       67 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/autoware/__init__.py
+-rw-r--r--   0        0        0     2402 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/autoware/can_packet.py
+-rw-r--r--   0        0        0     6971 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/csv.py
+-rw-r--r--   0        0        0     1991 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/image.py
+-rw-r--r--   0        0        0     2308 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/json_model.py
+-rw-r--r--   0        0        0    11798 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/movie.py
+-rw-r--r--   0        0        0       58 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/pointcloud/__init__.py
+-rw-r--r--   0        0        0     3413 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/pointcloud/pcd.py
+-rw-r--r--   0        0        0    11181 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/rosbag.py
+-rw-r--r--   0        0        0    14704 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/rosbag2.py
+-rw-r--r--   0        0        0       65 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/zstd/__init__.py
+-rw-r--r--   0        0        0     4374 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/models/zstd/rosbag.py
+-rw-r--r--   0        0        0      131 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/__init__.py
+-rwxr-xr-x   0        0        0     2527 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/downsampling.py
+-rwxr-xr-x   0        0        0      929 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/passthrough.py
+-rwxr-xr-x   0        0        0      352 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/preprocesses/preprocess.py
+-rw-r--r--   0        0        0     3648 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/statistics/__init__.py
+-rwxr-xr-x   0        0        0     8688 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/statistics/calculator.py
+-rw-r--r--   0        0        0       44 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/__init__.py
+-rw-r--r--   0        0        0    18150 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/can_decoder.py
+-rwxr-xr-x   0        0        0     2728 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/fileutils.py
+-rwxr-xr-x   0        0        0     7478 2023-02-09 04:26:45.622931 pydtk-0.2.9/pydtk/utils/utils.py
+-rwxr-xr-x   0        0        0     2591 2023-02-09 04:27:01.799170 pydtk-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5489 2023-02-09 04:27:03.137252 pydtk-0.2.9/setup.py
+-rw-r--r--   0        0        0     4661 2023-02-09 04:27:03.137844 pydtk-0.2.9/PKG-INFO
```

### Comparing `pydtk-0.2.7/LICENSE` & `pydtk-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/README.md` & `pydtk-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/bin/cli.py` & `pydtk-0.2.9/pydtk/bin/cli.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/bin/make_meta.py` & `pydtk-0.2.9/pydtk/bin/make_meta.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/bin/oas.py` & `pydtk-0.2.9/pydtk/bin/oas.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/bin/sub_commands/db.py` & `pydtk-0.2.9/pydtk/bin/sub_commands/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 import os
 import sys
 
 import pandas
 
 from pydtk.db import DBHandler
 from pydtk.models import MetaDataModel
+from pydtk.utils.utils import fix_args_type
 
 pandas.set_option("display.max_columns", None)
 pandas.set_option("display.width", None)
 
 
 class EmptySTDINError(Exception):
     """Exception for the case that STDIN is empty."""
 
     pass
 
 
 def _get_db_handler(target: str, database_id: str = "default", base_dir: str = "/"):
+    if not isinstance(database_id, str):
+        raise ValueError(f"database_id must be str, not {type(database_id)}")
+
     if target in ["databases", "database"]:
         handler = DBHandler(db_class="database_id")
         group_by = None
     elif target in ["records", "record"]:
         handler = DBHandler(
             db_class="meta",
             database_id=database_id,
@@ -99,14 +103,15 @@
 
 
 class DB(object):
     """DB."""
 
     _handler = None
 
+    @fix_args_type
     def list(
         self,
         target: str,
         database_id: str = "default",
         pql: str = None,
         offset: int = 0,
         limit: int = 20,
@@ -180,14 +185,15 @@
                 "Tags",
             ],
             **kwargs,
         )
 
         self._handler = handler
 
+    @fix_args_type
     def get(
         self,
         target: str,
         database_id: str = "default",
         record_id: str = None,
         path: str = None,
         content: str = None,
@@ -234,14 +240,15 @@
         handler.read(pql=pql, group_by=group_by)
 
         # Display
         _display(handler, **kwargs)
 
         self._handler = handler
 
+    @fix_args_type
     def add(
         self,
         target: str,
         content: str = None,
         database_id: str = "default",
         base_dir: str = "/",
         overwrite: bool = False,
@@ -338,14 +345,15 @@
         if num_updated > 0:
             print("Updated: {} items.".format(num_updated))
         if num_added > 0:
             print("Added: {} items.".format(num_added))
 
         self._handler = handler
 
+    @fix_args_type
     def delete(
         self,
         target: str,
         database_id: str = "default",
         record_id: str = None,
         path: str = None,
         content: str = None,
```

### Comparing `pydtk-0.2.7/pydtk/bin/sub_commands/io.py` & `pydtk-0.2.9/pydtk/bin/sub_commands/io.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/bin/sub_commands/model.py` & `pydtk-0.2.9/pydtk/bin/sub_commands/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # Copyright Toolkit Authors
 
 import importlib
 import json
 import os
 import pprint
 
+from pydtk.utils.utils import fix_args_type
+
 
 class Model(object):
     """Model related operations."""
 
     @staticmethod
     def list(**kwargs):
         """List models."""
@@ -37,14 +39,15 @@
         try:
             _ = reader.read(path=file, contents=content, as_ndarray=False)
             print("True")
         except NoModelMatchedError:
             print("False")
 
     @staticmethod
+    @fix_args_type
     def generate(
         target: str,
         model: str = None,
         from_file: str = None,
         template: str = None,
         database_id: str = "default",
         record_id: str = None,
```

### Comparing `pydtk-0.2.7/pydtk/bin/sub_commands/status.py` & `pydtk-0.2.9/pydtk/bin/sub_commands/status.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/builder/concat_df.py` & `pydtk-0.2.9/pydtk/builder/concat_df.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/builder/dbdb/file_info.py` & `pydtk-0.2.9/pydtk/builder/dbdb/file_info.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/builder/df_list.py` & `pydtk-0.2.9/pydtk/builder/df_list.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/builder/df_path.py` & `pydtk-0.2.9/pydtk/builder/df_path.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/builder/meta_db.py` & `pydtk-0.2.9/pydtk/builder/meta_db.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/builder/statistic_db.py` & `pydtk-0.2.9/pydtk/builder/statistic_db.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/conf/v1.yaml` & `pydtk-0.2.9/pydtk/conf/v1.yaml`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/conf/v2.yaml` & `pydtk-0.2.9/pydtk/conf/v2.yaml`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/conf/v3.yaml` & `pydtk-0.2.9/pydtk/conf/v3.yaml`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/conf/v4.yaml` & `pydtk-0.2.9/pydtk/conf/v4.yaml`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/__init__.py` & `pydtk-0.2.9/pydtk/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_pixel.py` & `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_pixel.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_rectangular_area.py` & `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_image_rectangular_area.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_point.py` & `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/annotation_commented_point.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py` & `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha1/file.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha2/file.py` & `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/annotation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-from typing import Optional
-
-from pydantic import Field, constr, Extra
+from pydantic import Field, constr
+from typing import Union
 
 from pydtk.db.schemas import BaseSchema, register_schema
 
 
 @register_schema
-class File(BaseSchema):
-    """Schema for files."""
+class Annotation(BaseSchema):
+    """Schema for annotation."""
 
     _api_version = "dataware-tools.com/v1alpha2"
-    _kind = "File"
-    description: Optional[constr()] = Field(None, description="")
+    _kind = "Annotation"
+    annotation_id: constr(min_length=1) = Field(..., description="")
+    generation: int
     record_id: constr(min_length=1) = Field(..., description="")
-    path: constr(min_length=1) = Field(..., description="")
-    contents: Optional[dict] = Field(None, description="")
-
-    # Allow additional properties
-    class Config:
-        """Config."""
-
-        extra = Extra.allow
-        schema_extra = {
-            "additionalProperties": {}
-        }
+    timestamp_from: Union[float, None]
+    timestamp_to: Union[float, None]
+    created_at: Union[float, None]
```

### Comparing `pydtk-0.2.7/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py` & `pydtk-0.2.9/pydtk/db/schemas/dataware-tools.com/v1alpha2/record.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Optional, Dict, Any, Type
 
 from pydantic import Field, constr, Extra
 
 from pydtk.db.schemas import BaseSchema, register_schema
 
 
 @register_schema
@@ -11,14 +11,17 @@
 
     _api_version = "dataware-tools.com/v1alpha2"
     _kind = "Record"
     description: Optional[constr()] = Field(None, description="")
     record_id: constr(min_length=1) = Field(..., description="")
 
     # Allow additional properties
-    class Config:
+    class Config(BaseSchema.Config):
         """Config."""
 
         extra = Extra.allow
-        schema_extra = {
-            "additionalProperties": {}
-        }
+
+        @staticmethod
+        def schema_extra(schema: Dict[str, Any], model: Type['Record']):
+            """Extra schema."""
+            BaseSchema.Config.schema_extra(schema, model)
+            schema["additionalProperties"] = {}
```

### Comparing `pydtk-0.2.7/pydtk/db/v1/handlers/__init__.py` & `pydtk-0.2.9/pydtk/db/v1/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v1/handlers/meta.py` & `pydtk-0.2.9/pydtk/db/v1/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v2/handlers/__init__.py` & `pydtk-0.2.9/pydtk/db/v2/handlers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import logging
 from copy import deepcopy
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
 import sqlalchemy
-from attrdict import AttrDict
+from addict import Dict as AttrDict
 from sqlalchemy import sql
 from sqlalchemy.orm import scoped_session, sessionmaker
 from tqdm import tqdm
 
 from pydtk.utils.utils import (
     deserialize_dict_1d,
     dicts_to_listed_dict_2d,
```

### Comparing `pydtk-0.2.7/pydtk/db/v2/handlers/meta.py` & `pydtk-0.2.9/pydtk/db/v2/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v2/search_engines/__init__.py` & `pydtk-0.2.9/pydtk/db/v2/search_engines/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v2/search_engines/time_series.py` & `pydtk-0.2.9/pydtk/db/v2/search_engines/time_series.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v3/__init__.py` & `pydtk-0.2.9/pydtk/db/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v3/handlers/__init__.py` & `pydtk-0.2.9/pydtk/db/v3/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v3/handlers/meta.py` & `pydtk-0.2.9/pydtk/db/v3/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v3/handlers/statistics.py` & `pydtk-0.2.9/pydtk/db/v3/handlers/statistics.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v3/handlers/time_series.py` & `pydtk-0.2.9/pydtk/db/v3/handlers/time_series.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v3/search_engines/__init__.py` & `pydtk-0.2.9/pydtk/db/v3/search_engines/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v3/search_engines/time_series.py` & `pydtk-0.2.9/pydtk/db/v3/search_engines/time_series.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/LICENSE` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/LICENSE`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/README.md` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/README.md`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/aggregation_tests.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/aggregation_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/find_tests.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/find_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/pql/__init__.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/pql/aggregation.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/aggregation.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/pql/matching.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/pql/matching.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python37/setup.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python37/setup.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/LICENSE` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/LICENSE`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/README.md` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/README.md`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/aggregation_tests.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/aggregation_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/find_tests.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/find_tests.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/pql/__init__.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/pql/aggregation.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/aggregation.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/pql/matching.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/pql/matching.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/deps/pql_python38/setup.py` & `pydtk-0.2.9/pydtk/db/v4/deps/pql_python38/setup.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/engines/__init__.py` & `pydtk-0.2.9/pydtk/db/v4/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/engines/mongodb.py` & `pydtk-0.2.9/pydtk/db/v4/engines/mongodb.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/engines/montydb.py` & `pydtk-0.2.9/pydtk/db/v4/engines/montydb.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         db_name = DEFAULT_DB_NAME
     if collection_name is None:
         collection_name = DEFAULT_COLLECTION_NAME
 
     set_storage(
         # general settings
         repository=db_host,  # dir path for database to live on disk, default is {cwd}
-        storage="lightning",  # storage name, default "flatfile"
+        # NOTE(kan-bayashi): flatfile cannot pass test
+        storage="sqlite",  # storage name, default "flatfile"
         use_bson=None,  # default None, and will import pymongo's bson if None or True
         # any other kwargs are storage engine settings.
         cache_modified=0,  # the only setting that flat-file have
     )
 
     collection = getattr(getattr(MontyClient(db_host), db_name), collection_name)
     return collection
```

### Comparing `pydtk-0.2.7/pydtk/db/v4/engines/tinydb.py` & `pydtk-0.2.9/pydtk/db/v4/engines/tinydb.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/engines/tinymongo.py` & `pydtk-0.2.9/pydtk/db/v4/engines/tinymongo.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/handlers/__init__.py` & `pydtk-0.2.9/pydtk/db/v4/handlers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 """V4DBHandler."""
 
 import hashlib
 import importlib
 import inspect
 import logging
 import os
-from collections import MutableMapping
+from collections.abc import MutableMapping
 from copy import deepcopy
 from datetime import datetime
 
 import pandas as pd
-from attrdict import AttrDict
+from addict import Dict as AttrDict
 from deepmerge import Merger
 
 from pydtk.db.exceptions import DatabaseNotInitializedError, InvalidDatabaseConfigError
 from pydtk.db.schemas import get_schema
 from pydtk.db.v4.engines import DB_ENGINES
 from pydtk.utils.utils import (
     _deepmerge_append_list_unique,
```

### Comparing `pydtk-0.2.7/pydtk/db/v4/handlers/annotation.py` & `pydtk-0.2.9/pydtk/db/v4/handlers/annotation.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/db/v4/handlers/meta.py` & `pydtk-0.2.9/pydtk/db/v4/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/frontend.py` & `pydtk-0.2.9/pydtk/frontend.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/io/reader.py` & `pydtk-0.2.9/pydtk/io/reader.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/io/writer.py` & `pydtk-0.2.9/pydtk/io/writer.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/__init__.py` & `pydtk-0.2.9/pydtk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/autoware/can_packet.py` & `pydtk-0.2.9/pydtk/models/autoware/can_packet.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/csv.py` & `pydtk-0.2.9/pydtk/models/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             end_timestamp * 1000,
         )  # sec. -> msec.
         data = self.data
         data = data[np.logical_and(data[:, 0] >= start_msec, data[:, 0] <= end_msec), 0]
 
         # Convert unit (msec. -> sec.)
         # Note: CSV file timestamps in "Driving behavior DB" is recorded in msec.
-        data = data.astype(np.float) * pow(10, -3)
+        data = data.astype(np.float64) * pow(10, -3)
 
         self.data = data
 
     def to_ndarray(self):
         """Return data as ndarray."""
         return self.data
```

### Comparing `pydtk-0.2.7/pydtk/models/image.py` & `pydtk-0.2.9/pydtk/models/image.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/json_model.py` & `pydtk-0.2.9/pydtk/models/json_model.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/movie.py` & `pydtk-0.2.9/pydtk/models/movie.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/pointcloud/pcd.py` & `pydtk-0.2.9/pydtk/models/pointcloud/pcd.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/rosbag.py` & `pydtk-0.2.9/pydtk/models/rosbag.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/models/rosbag2.py` & `pydtk-0.2.9/pydtk/models/rosbag2.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 from rclpy.serialization import deserialize_message
 from rosidl_runtime_py.utilities import get_message
 
 from pydtk.models import BaseModel, register_model
 
 # check python version
 python_version = ".".join(platform.python_version_tuple()[:2])
-if version.parse(python_version) != version.parse("3.8"):
+if version.parse(python_version) != version.parse("3.10"):
     raise ImportError(
-        "Rosbag2 libraries support only Python 3.8, but your Python is"
-        f" {python_version}"
+        f"ROS2 (Humble) supports only Python 3.10, but your Python is {python_version}"
     )
 
 
 def get_rosbag_options(
     path,
     storage_id,
     serialization_format="cdr",
@@ -90,28 +89,27 @@
         if isinstance(contents, str):
             topic = contents
         if isinstance(contents, dict):
             topic = next(iter(contents))
         if topic is None:
             raise ValueError('Topic name must be specified by the argument "contents"')
 
-        # NOTE(kan-bayashi): seek() is not available in current version (2022/12/08) with apt,
-        #   and therefore, we do not use start_timestamp temporary.
-        if start_timestamp is not None:
+        # NOTE(kan-bayashi): Seek with mcap does not work well in 2022/12/27
+        # TODO(kan-bayashi): May next ROS2 support seek with mcap format
+        #   https://github.com/ros2/rosbag2/pull/1205
+        if start_timestamp is not None and self._get_storage_id(path) == "mcap":
             self.logger.warning("start_timestamp is not supported. ignored.")
             start_timestamp = None
 
         # Load rosbag2
         reader = rosbag2_py.SequentialReader()
         reader.open(*get_rosbag_options(path, self._get_storage_id(path)))
 
         # Seek timestamp if needed
         if start_timestamp is not None:
-            # NOTE(kan-bayashi): seek() is not available in current version (2022/12/08) with apt
-            raise NotImplementedError()
             # TODO(kan-bayashi): What happened when start timestamp if exceed end timestamp?
             reader.seek(int(start_timestamp * 10**9))
 
         # Create mapping dict of topic name and type
         topic_types = reader.get_all_topics_and_types()
         type_map = {
             topic_types[i].name: topic_types[i].type for i in range(len(topic_types))
@@ -130,16 +128,14 @@
                 timestamp_in_nsec = reader.read_next()[2]
                 timestamp = float(timestamp_in_nsec) / (10**9)
                 if end_timestamp is not None and timestamp > end_timestamp:
                     break
                 timestamps.append(timestamp)
             timestamps = self.downsample_timestamps(timestamps, target_frame_rate)
             if start_timestamp is not None:
-                # TODO(kan-bayashi): seek() is not available in current version (2022/12/08)
-                raise NotImplementedError()
                 reader.seek(int(start_timestamp * 10**9))
             else:
                 # TODO(kan-bayashi): Replace with seek()
                 del reader
                 reader = rosbag2_py.SequentialReader()
                 reader.open(*get_rosbag_options(path, self._get_storage_id(path)))
             timestamp_idx = 0
@@ -195,30 +191,29 @@
         if isinstance(contents, str):
             topic = contents
         if isinstance(contents, dict):
             topic = next(iter(contents))
         if topic is None:
             raise ValueError('Topic name must be specified by the argument "contents"')
 
-        # NOTE(kan-bayashi): seek() is not available in current version (2022/12/08) with apt,
-        #   and therefore, we do not use start_timestamp temporary.
-        if start_timestamp is not None:
+        # NOTE(kan-bayashi): Seek with mcap does not work well in 2022/12/27
+        # TODO(kan-bayashi): May next ROS2 support seek with mcap format
+        #   https://github.com/ros2/rosbag2/pull/1205
+        if start_timestamp is not None and self._get_storage_id(path) == "mcap":
             self.logger.warning("start_timestamp is not supported. ignored.")
             start_timestamp = None
 
         # Load rosbag2
         reader = rosbag2_py.SequentialReader()
         reader.open(*get_rosbag_options(path, self._get_storage_id(path)))
 
         # Seek timestamp if needed
         if start_timestamp is not None:
-            # NOTE(kan-bayashi): seek() is not available in current version (2022/12/08)
-            raise NotImplementedError()
             # TODO(kan-bayashi): What happened when start timestamp if exceed end timestamp?
-            reader.seek(start_timestamp)
+            reader.seek(int(start_timestamp * 10**9))
 
         # Create mapping dict of topic name and type
         topic_types = reader.get_all_topics_and_types()
         type_map = {
             topic_types[i].name: topic_types[i].type for i in range(len(topic_types))
         }
         assert topic in type_map, f"topic {topic} is not included in rosbag."
@@ -235,17 +230,15 @@
                 timestamp_in_nsec = reader.read_next()[2]
                 timestamp = float(timestamp_in_nsec) / (10**9)
                 if end_timestamp is not None and timestamp > end_timestamp:
                     break
                 timestamps.append(timestamp)
             timestamps = self.downsample_timestamps(timestamps, target_frame_rate)
             if start_timestamp is not None:
-                # TODO(kan-bayashi): seek() is not available in current version (2022/12/08)
-                raise NotImplementedError()
-                reader.seek(start_timestamp)
+                reader.seek(int(start_timestamp * 10**9))
             else:
                 # TODO(kan-bayashi): Replace with seek()
                 del reader
                 reader = rosbag2_py.SequentialReader()
                 reader.open(*get_rosbag_options(path, self._get_storage_id(path)))
             timestamp_idx = 0
             while True:
@@ -332,28 +325,24 @@
             path (str): Path of rosbag2 file
             content_key (str): Not used
 
         Returns:
             dict: Contents metadata
 
         """
-        # Load file
-        reader = rosbag2_py.SequentialReader()
-        reader.open(*get_rosbag_options(path, cls._get_storage_id(path)))
-        topics = reader.get_all_topics_and_types()
-
-        # Generate metadata
+        info_reader = rosbag2_py.Info()
+        info = info_reader.read_metadata(path, cls._get_storage_id(path))
         contents = {}
-        for topic in topics:
-            contents[topic.name] = {}
-            contents[topic.name]["type"] = topic.type
-            contents[topic.name]["serialization_format"] = topic.serialization_format
-            contents[topic.name]["offered_qos_profiles"] = topic.offered_qos_profiles
-
-        del reader
+        for topic in info.topics_with_message_count:
+            meta = topic.topic_metadata
+            contents[meta.name] = {}
+            contents[meta.name]["message_count"] = topic.message_count
+            contents[meta.name]["type"] = meta.type
+            contents[meta.name]["serialization_format"] = meta.serialization_format
+            contents[meta.name]["offered_qos_profiles"] = meta.offered_qos_profiles
 
         return contents
 
     @classmethod
     def generate_timestamp_meta(cls, path):
         """Generate timestamps metadata.
```

### Comparing `pydtk-0.2.7/pydtk/models/zstd/rosbag.py` & `pydtk-0.2.9/pydtk/models/zstd/rosbag.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/preprocesses/downsampling.py` & `pydtk-0.2.9/pydtk/preprocesses/downsampling.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/preprocesses/passthrough.py` & `pydtk-0.2.9/pydtk/preprocesses/passthrough.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/statistics/__init__.py` & `pydtk-0.2.9/pydtk/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/statistics/calculator.py` & `pydtk-0.2.9/pydtk/statistics/calculator.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/utils/can_decoder.py` & `pydtk-0.2.9/pydtk/utils/can_decoder.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/utils/fileutils.py` & `pydtk-0.2.9/pydtk/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `pydtk-0.2.7/pydtk/utils/utils.py` & `pydtk-0.2.9/pydtk/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # Copyright Toolkit Authors (Yusuke Adachi, Daiki Hayashi)
 
 import contextlib
 import os
 import re
 import sys
 
-import attrdict
 import yaml
+from addict import Dict as AttrDict
 from tqdm import tqdm
 
 DTYPE_MAP = {
     "string[]": str,
     "string": str,
     "str": str,
     "text": str,
@@ -42,15 +42,15 @@
     with open(
         os.path.join(
             os.path.dirname(os.path.dirname(__file__)), "conf", name + ".yaml"
         ),
         "r",
     ) as f:
         config = yaml.load(f, Loader=yaml.SafeLoader)
-    return attrdict.AttrDict(config)
+    return AttrDict(config)
 
 
 def tag_filter(tag_list, base_df):
     """Search with tags.
 
     Args:
         base_df (DataFrame): Search target.
@@ -298,7 +298,26 @@
         yield fh
     finally:
         if close:
             try:
                 fh.close()
             except AttributeError:
                 pass
+
+
+def fix_args_type(func):
+    """Decorator to fix function arguments type.
+
+    Args:
+        func (function): a function whose arguments should be checked
+
+    Returns:
+        function: decorated function
+
+    """
+    def fix(*args, **kwargs):
+        """Fix arguments type."""
+        if "database_id" in kwargs.keys():
+            kwargs["database_id"] = str(kwargs["database_id"])
+        func(*args, **kwargs)
+
+    return fix
```

### Comparing `pydtk-0.2.7/pyproject.toml` & `pydtk-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 [build-system]
 requires = ["poetry >= 1.0.0", "setuptools >= 50.3.0", "wheel >= 0.35.1", "pip >= 21.0.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pydtk"
-version = "0.2.7"
+version = "0.2.9"
 description = "A Python toolkit for managing, retrieving and processing data."
 license = "Apache-2.0"
 authors = [
     "Yusuke Adachi <adachi.yusuke@hdwlab.co.jp>",
     "Daiki Hayashi <hayashi.daiki@hdwlab.co.jp>",
     "Toshimitsu Watanabe <watanabe.toshimitsu@hdwlab.co.jp>"
 ]
 readme = 'README.md'
 repository = "https://github.com/dataware-tools/python-toolkit.git"
 homepage = "https://github.com/dataware-tools/python-toolkit.git"
 keywords = ['toolkit', 'data', 'dataware', 'metadata']
 classifiers = [
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Operating System :: POSIX :: Linux",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4"
-numpy = "^1.16.6"
+python = ">=3.8,<3.11"
+numpy = "<1.24.0"
 pandas = "^1.0.3"
 six = "^1.15.0"
 pyyaml = "*"
 pycryptodomex = { version = "*", optional = true }
 gnupg = { version = "*", optional = true }
 rospkg = { version = "*", optional = true }
 pyntcloud = { version = "*", optional = true }
-attrdict = "*"
 tqdm = "^4.46.1"
 fire = "^0.3.1"
 sqlalchemy = "^1.3.17"
 sqlalchemy-migrate = "*"
 opencv-python = "^4.2.0.34"
 bitstring = "^3.1.7"
 tinydb = ">=3.2.1,<4.0.0"
 pymongo = "^3.11.3"
 deepmerge = "^0.1.1"
 tinymongo = "^0.2.0"
 flatten-dict = "^0.3.0"
 python-dateutil = "^2.8.1"
-montydb = {extras = ["bson", "lmdb"], version = "^2.3.12"}
+montydb = {extras = ["bson", "lmdb"], version = "^2.4.0"}
 flatdict = { version = "^4.0.1", optional = true }
 pyzstd = { version = "^0.15.0", optional = true }
 pydantic = "^1.10.2"
 lark =  { version = "^1.1.5", optional = true }
+scipy = "^1.8.0"
+addict = "^2.4.0"
 
 [tool.poetry.dev-dependencies]
 importlib-resources = "<2.0.0"
 importlib-metadata = "<2.0.0"
 pytest = "^6.0.0"
 flake8-docstrings = "^1.5.0"
 tox = "<=3.17.0"
@@ -76,8 +77,8 @@
 analyze_statistics = "pydtk.builder.statistic_db:script"
 batch_analyze_statistics = "pydtk.builder.statistic_db:batch_script"
 make_meta = "pydtk.bin.make_meta:main"
 pydtk = "pydtk.bin.cli:script"
 oas_dump = "pydtk.bin.oas:script"
 
 [tool.pytest.ini_options]
-markers = ["extra", "ros", "ros2", "cassandra", "pointcloud"]
+markers = ["extra", "ros", "ros2", "cassandra", "pointcloud", "zstd"]
```

### Comparing `pydtk-0.2.7/setup.py` & `pydtk-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,28 @@
  'pydtk.statistics',
  'pydtk.utils']
 
 package_data = \
 {'': ['*'], 'pydtk': ['conf/*']}
 
 install_requires = \
-['attrdict',
+['addict>=2.4.0,<3.0.0',
  'bitstring>=3.1.7,<4.0.0',
  'deepmerge>=0.1.1,<0.2.0',
  'fire>=0.3.1,<0.4.0',
  'flatten-dict>=0.3.0,<0.4.0',
- 'montydb[bson,lmdb]>=2.3.12,<3.0.0',
- 'numpy>=1.16.6,<2.0.0',
+ 'montydb[lmdb,bson]>=2.4.0,<3.0.0',
+ 'numpy<1.24.0',
  'opencv-python>=4.2.0.34,<5.0.0.0',
  'pandas>=1.0.3,<2.0.0',
  'pydantic>=1.10.2,<2.0.0',
  'pymongo>=3.11.3,<4.0.0',
  'python-dateutil>=2.8.1,<3.0.0',
  'pyyaml',
+ 'scipy>=1.8.0,<2.0.0',
  'six>=1.15.0,<2.0.0',
  'sqlalchemy-migrate',
  'sqlalchemy>=1.3.17,<2.0.0',
  'tinydb>=3.2.1,<4.0.0',
  'tinymongo>=0.2.0,<0.3.0',
  'tqdm>=4.46.1,<5.0.0']
 
@@ -74,25 +75,25 @@
                      'create_meta_db = pydtk.builder.meta_db:script',
                      'make_meta = pydtk.bin.make_meta:main',
                      'oas_dump = pydtk.bin.oas:script',
                      'pydtk = pydtk.bin.cli:script']}
 
 setup_kwargs = {
     'name': 'pydtk',
-    'version': '0.2.7',
+    'version': '0.2.9',
     'description': 'A Python toolkit for managing, retrieving and processing data.',
     'long_description': '# Python Dataware Toolkit\n\nA Python toolkit for managing, retrieving, and processing data.\n\n## Installation\nYou can install the toolkit with:\n```bash\n$ pip3 install pydtk\n\n```\n\nIf you want to install the toolkit with extra feature (e.g. support for PointCloud and ROS), \nyou can install it with extra dependencies as follows:\n```bash\n$ pip3 install pydtk[pointcloud,ros]\n\n```\n\nSome PyDTK models require additional packages.  \nPlease refer the following table and install them manually with command `pip install ...`.  \n\n| PyDTK model | Required packages |\n| --- | --- |\n| rosbag.* | ros_numpy (https://github.com/eric-wieser/ros_numpy.git) |\n| pointcloud.PCDModel | pypcd (https://github.com/klintan/pypcd.git) |\n\n\n## Usage\n\nBy using Pydtk, you can load a variety of types of data with a unified interface as shown below.\n\n1. Load DBHandler for retrieving metadata\n```python\nfrom pydtk.db import DBHandler\n\n# Initialize handler (This will read all the metadata from DB on initialization)\nhandler = DBHandler(\n    db_class=\'meta\',\n    db_host=\'./examples/example_db\',\n    base_dir_path=\'./test\'\n)\n\n```\n\n2. Read metadata from db with data selection.\n```python\n# Select by timestamp\nhandler.read(pql=\'start_timestamp > 1420000000 and end_timestamp < 1500000000\')\nprint(handler.data)\n\n# Select by record-id\nhandler.read(pql=\'record_id == regex("test.*")\')\nprint(handler.data)\n\n```\n\n3. Load data from files based on metadata.\n```python\nfrom pydtk.io import BaseFileReader, NoModelMatchedError\n\nreader = BaseFileReader()\n\ntry:\n    for sample in handler:\n        print(\'loading content "{0}" from file "{1}"\'.format(sample[\'contents\'], sample[\'path\']))\n        try:\n            timestamps, data, columns = reader.read(sample)\n            assert print(data)\n        except NoModelMatchedError as e:\n            print(str(e))\n            continue\nexcept EOFError:\n    pass\n```\n\n\n## Documentation\nFor more information about this toolkit, please refer the [document](https://dataware-tools.github.io/pydtk/).\n\n\n## Setup for contribution\nTo improve this toolkit, firstly clone this repository and then \nrun the following command to prepare the environment. \n\n```bash\n$ git clone git@github.com:dataware-tools/pydtk.git --recurse-submodules\n$ poetry install\n\n```\n\nMake sure that [poetry](https://python-poetry.org/) is installed before executing the command.\n\nIf you want to install the toolkit with extra feature (e.g. support for ROS), \nplease specify it with `-E` option.  \nExample (installation with `pointcloud` and `ros` extras):\n```bash\n$ poetry install -E pointcloud -E ros\n\n```\n',
     'author': 'Yusuke Adachi',
     'author_email': 'adachi.yusuke@hdwlab.co.jp',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/dataware-tools/python-toolkit.git',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4',
+    'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pydtk-0.2.7/PKG-INFO` & `pydtk-0.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: pydtk
-Version: 0.2.7
+Version: 0.2.9
 Summary: A Python toolkit for managing, retrieving and processing data.
 Home-page: https://github.com/dataware-tools/python-toolkit.git
 License: Apache-2.0
 Keywords: toolkit,data,dataware,metadata
 Author: Yusuke Adachi
 Author-email: adachi.yusuke@hdwlab.co.jp
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: pointcloud
 Provides-Extra: ros
 Provides-Extra: ros2
 Provides-Extra: zstd
-Requires-Dist: attrdict
+Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: bitstring (>=3.1.7,<4.0.0)
 Requires-Dist: deepmerge (>=0.1.1,<0.2.0)
 Requires-Dist: fire (>=0.3.1,<0.4.0)
 Requires-Dist: flatdict (>=4.0.1,<5.0.0); extra == "ros" or extra == "ros2"
 Requires-Dist: flatten-dict (>=0.3.0,<0.4.0)
 Requires-Dist: gnupg; extra == "ros"
 Requires-Dist: lark (>=1.1.5,<2.0.0); extra == "ros2"
-Requires-Dist: montydb[bson,lmdb] (>=2.3.12,<3.0.0)
-Requires-Dist: numpy (>=1.16.6,<2.0.0)
+Requires-Dist: montydb[lmdb,bson] (>=2.4.0,<3.0.0)
+Requires-Dist: numpy (<1.24.0)
 Requires-Dist: opencv-python (>=4.2.0.34,<5.0.0.0)
 Requires-Dist: pandas (>=1.0.3,<2.0.0)
 Requires-Dist: pycryptodomex; extra == "ros"
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pymongo (>=3.11.3,<4.0.0)
 Requires-Dist: pyntcloud; extra == "pointcloud"
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: pyyaml
 Requires-Dist: pyzstd (>=0.15.0,<0.16.0); extra == "zstd"
 Requires-Dist: rospkg; extra == "ros"
+Requires-Dist: scipy (>=1.8.0,<2.0.0)
 Requires-Dist: six (>=1.15.0,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.3.17,<2.0.0)
 Requires-Dist: sqlalchemy-migrate
 Requires-Dist: tinydb (>=3.2.1,<4.0.0)
 Requires-Dist: tinymongo (>=0.2.0,<0.3.0)
 Requires-Dist: tqdm (>=4.46.1,<5.0.0)
 Project-URL: Repository, https://github.com/dataware-tools/python-toolkit.git
```

