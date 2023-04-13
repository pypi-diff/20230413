# Comparing `tmp/scylla-driver-3.25.9.tar.gz` & `tmp/scylla-driver-3.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scylla-driver-3.25.9.tar", last modified: Mon Nov 28 17:23:41 2022, max compression
+gzip compressed data, was "scylla-driver-3.26.0.tar", last modified: Thu Apr 13 14:29:15 2023, max compression
```

## Comparing `scylla-driver-3.25.9.tar` & `scylla-driver-3.26.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/
--rw-r--r--   0 runner    (1001) docker     (122)    17478 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     5220 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8596 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/ez_setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     7259 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/
--rw-r--r--   0 runner    (1001) docker     (122)    43701 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/cqlengine/
--rw-r--r--   0 runner    (1001) docker     (122)    38850 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2535 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/operators.py
--rw-r--r--   0 runner    (1001) docker     (122)    14372 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)      973 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22838 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/management.py
--rw-r--r--   0 runner    (1001) docker     (122)    56369 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/query.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/functions.py
--rw-r--r--   0 runner    (1001) docker     (122)    29542 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/statements.py
--rw-r--r--   0 runner    (1001) docker     (122)     7432 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/usertype.py
--rw-r--r--   0 runner    (1001) docker     (122)     4717 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/named.py
--rw-r--r--   0 runner    (1001) docker     (122)    33173 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqlengine/columns.py
--rw-r--r--   0 runner    (1001) docker     (122)     1683 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/deserializers.pxd
--rw-r--r--   0 runner    (1001) docker     (122)       80 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cython_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    10777 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     6516 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cmurmur3.c
--rw-r--r--   0 runner    (1001) docker     (122)     2002 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/row_parser.pyx
--rw-r--r--   0 runner    (1001) docker     (122)   231991 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     1951 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/type_codes.py
--rw-r--r--   0 runner    (1001) docker     (122)      743 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/bytesio.pxd
--rw-r--r--   0 runner    (1001) docker     (122)    48183 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/protocol.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cython_deps.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/deserializers.pyx
--rw-r--r--   0 runner    (1001) docker     (122)      967 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/type_codes.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     4927 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/marshal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2984 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/obj_parser.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2551 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/murmur3.py
--rw-r--r--   0 runner    (1001) docker     (122)    69867 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/connection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2440 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cython_marshal.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2919 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/c_shard_info.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    10059 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (122)    19687 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8719 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/datastax/
--rw-r--r--   0 runner    (1001) docker     (122)      569 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/datastax/insights/
--rw-r--r--   0 runner    (1001) docker     (122)     4369 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/insights/registry.py
--rw-r--r--   0 runner    (1001) docker     (122)    10159 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/insights/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/insights/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     9149 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/insights/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/datastax/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6432 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/datastax/graph/
--rw-r--r--   0 runner    (1001) docker     (122)      983 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11751 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/
--rw-r--r--   0 runner    (1001) docker     (122)     8469 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/_serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      731 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)    12811 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/query.py
--rw-r--r--   0 runner    (1001) docker     (122)     7820 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/_query.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/predicates.py
--rw-r--r--   0 runner    (1001) docker     (122)     6100 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/fluent/_predicates.py
--rw-r--r--   0 runner    (1001) docker     (122)    35798 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/graphson.py
--rw-r--r--   0 runner    (1001) docker     (122)     5798 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/datastax/graph/types.py
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    42069 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/query.py
--rw-r--r--   0 runner    (1001) docker     (122)     6576 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      684 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     3917 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/timestamps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/io/
--rw-r--r--   0 runner    (1001) docker     (122)     4305 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/geventreactor.py
--rw-r--r--   0 runner    (1001) docker     (122)      570 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12826 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/libevreactor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6835 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/eventletreactor.py
--rw-r--r--   0 runner    (1001) docker     (122)    22348 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/libevwrapper.c
--rw-r--r--   0 runner    (1001) docker     (122)     7755 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/asyncioreactor.py
--rw-r--r--   0 runner    (1001) docker     (122)    10333 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/twistedreactor.py
--rw-r--r--   0 runner    (1001) docker     (122)    14375 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/io/asyncorereactor.py
--rw-r--r--   0 runner    (1001) docker     (122)   136705 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/segment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2972 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/shard_info.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/scylla/
--rw-r--r--   0 runner    (1001) docker     (122)     6254 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/scylla/cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/scylla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5855 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/numpy_parser.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     2052 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cython_utils.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1701 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/bytesio.pyx
--rw-r--r--   0 runner    (1001) docker     (122)    47427 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/cqltypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (122)       50 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/numpyFlags.h
--rw-r--r--   0 runner    (1001) docker     (122)    49865 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/pool.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/parsing.pyx
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/tuple.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/parsing.pxd
--rw-r--r--   0 runner    (1001) docker     (122)     1638 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/ioutils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/cassandra/graph/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/graph/query.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/graph/graphson.py
--rw-r--r--   0 runner    (1001) docker     (122)      689 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/cassandra/graph/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/scylla_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/scylla_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/scylla_driver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2646 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/scylla_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7259 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/scylla_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       75 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/scylla_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)      195 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2022-11-28 17:23:37.000000 scylla-driver-3.25.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 17:23:41.000000 scylla-driver-3.25.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.790249 scylla-driver-3.26.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/
+-rw-r--r--   0 runner    (1001) docker     (123)    19691 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/bytesio.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/bytesio.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/c_shard_info.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   239424 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cmurmur3.c
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69867 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/cqlengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33173 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38850 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56369 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29542 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqlengine/usertype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cqltypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_marshal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/cython_utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/datastax/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.782249 scylla-driver-3.26.0/cassandra/datastax/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/datastax/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/
+-rw-r--r--   0 runner    (1001) docker     (123)    12811 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/fluent/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35798 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/graphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/graph/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/datastax/insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/datastax/insights/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/deserializers.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/deserializers.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/graphson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/graph/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/asyncioreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/asyncorereactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/eventletreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/geventreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/libevreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22348 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/libevwrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/io/twistedreactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/ioutils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/marshal.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136904 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/murmur3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/numpyFlags.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/numpy_parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/obj_parser.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/parsing.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/parsing.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    43701 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42069 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/row_parser.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/cassandra/scylla/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/scylla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/scylla/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/shard_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/tuple.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/type_codes.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/type_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65131 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/cassandra/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/ez_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:29:15.786249 scylla-driver-3.26.0/scylla_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 14:29:15.000000 scylla-driver-3.26.0/scylla_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:29:15.790249 scylla-driver-3.26.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    17231 2023-04-13 14:29:09.000000 scylla-driver-3.26.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scylla-driver-3.25.9/setup.py` & `scylla-driver-3.26.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 from setuptools import setup
 from distutils.command.build_ext import build_ext
 from distutils.core import Extension
 from distutils.errors import (CCompilerError, DistutilsPlatformError,
                               DistutilsExecError)
 from distutils.cmd import Command
 
-PY3 = sys.version_info[0] == 3
-
 try:
     import subprocess
     has_subprocess = True
 except ImportError:
     has_subprocess = False
 
 from cassandra import __version__
@@ -403,17 +401,14 @@
         else:
             sys.stderr.write("Bypassing Cython setup requirement\n")
 
     dependencies = ['six >=1.9',
                     'geomet>=0.1,<0.3',
                     'pyyaml > 5.0']
 
-    if not PY3:
-        dependencies.append('futures')
-
     _EXTRAS_REQUIRE = {
         'graph': ['gremlinpython==3.4.6']
     }
 
     setup(
         name='scylla-driver',
         version=__version__,
@@ -440,17 +435,14 @@
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Intended Audience :: Developers',
             'License :: OSI Approved :: Apache Software License',
             'Natural Language :: English',
             'Operating System :: OS Independent',
             'Programming Language :: Python',
-            'Programming Language :: Python :: 2.7',
-            'Programming Language :: Python :: 3.5',
-            'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: Implementation :: CPython',
             'Programming Language :: Python :: Implementation :: PyPy',
             'Topic :: Software Development :: Libraries :: Python Modules'
         ],
         **kw)
```

### Comparing `scylla-driver-3.25.9/README.rst` & `scylla-driver-3.26.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 
 .. image:: https://github.com/scylladb/python-driver/workflows/Build%20and%20upload%20to%20PyPi/badge.svg?tag=*-scylla
    :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22Build+and+upload+to+PyPi%22+event%3Apush+branch%3A*-scylla
 
 .. image:: https://github.com/scylladb/python-driver/workflows/CI%20Docs/badge.svg?tag=*-scylla
    :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22CI+Docs%22+event%3Apush+branch%3A*-scylla
 
-The driver supports Python versions 2.7, 3.4, 3.5, 3.6, 3.7 and 3.8.
+The driver supports Python versions 3.6-3.11.
 
 .. **Note:** This driver does not support big-endian systems.
 
 Features
 --------
 * `Synchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute>`_ and `Asynchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute_async>`_ APIs
 * `Simple, Prepared, and Batch statements <http://python-driver.docs.scylladb.com/stable/api/cassandra/query.html#cassandra.query.Statement>`_
 * Asynchronous IO, parallel execution, request pipelining
 * `Connection pooling <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Cluster.get_core_connections_per_host>`_
 * Automatic node discovery
 * `Automatic reconnection <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#reconnecting-to-dead-hosts>`_
 * Configurable `load balancing <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#load-balancing>`_ and `retry policies <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#retrying-failed-operations>`_
 * `Concurrent execution utilities <http://python-driver.docs.scylladb.com/stable/api/cassandra/concurrent.html>`_
-* `Object mapper <http://python-driver.docs.scylladb.com/stable/object_mapper.html>`_
-* `Shard awareness <http://python-driver.docs.scylladb.com/stable/scylla_specific.html#shard-awareness>`_
+* `Object mapper <http://python-driver.docs.scylladb.com/stable/object-mapper.html>`_
+* `Shard awareness <http://python-driver.docs.scylladb.com/stable/scylla-specific.html#shard-awareness>`_
 
 Installation
 ------------
 Installation through pip is recommended::
 
     $ pip install scylla-driver
 
@@ -39,15 +39,15 @@
 Documentation
 -------------
 The documentation can be found online `here <http://python-driver.docs.scylladb.com/stable/index.html>`_.
 
 Information includes: 
 
 * `Installation <http://python-driver.docs.scylladb.com/stable/installation.html>`_
-* `Getting started guide <http://python-driver.docs.scylladb.com/stable/getting_started.html>`_
+* `Getting started guide <http://python-driver.docs.scylladb.com/stable/getting-started.html>`_
 * `API docs <http://python-driver.docs.scylladb.com/stable/api/index.html>`_
 * `Performance tips <http://python-driver.docs.scylladb.com/stable/performance.html>`_
 
 Training
 --------
 The course `Using Scylla Drivers <https://university.scylladb.com/courses/using-scylla-drivers/lessons/coding-with-python/>`_ in `Scylla University <https://university.scylladb.com>`_  explains how to use drivers in different languages to interact with a Scylla cluster. 
 The lesson, Coding with Python (link), goes over a sample application that, using the Python driver, interacts with a three-node Scylla cluster.
@@ -55,15 +55,15 @@
 `Scylla University <https://university.scylladb.com>`_ includes other training material and online courses which will help you become a Scylla NoSQL database expert.
 
 
 Object Mapper
 -------------
 cqlengine (originally developed by Blake Eggleston and Jon Haddad, with contributions from the
 community) is now maintained as an integral part of this package. Refer to
-`documentation here <http://python-driver.docs.scylladb.com/stable/object_mapper.html>`_.
+`documentation here <http://python-driver.docs.scylladb.com/stable/object-mapper.html>`_.
 
 Contributing
 ------------
 See `CONTRIBUTING <https://github.com/scylladb/python-driver/blob/master/CONTRIBUTING.rst>`_.
 
 Reporting Problems
 ------------------
```

### Comparing `scylla-driver-3.25.9/ez_setup.py` & `scylla-driver-3.26.0/ez_setup.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/PKG-INFO` & `scylla-driver-3.26.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,120 @@
 Metadata-Version: 2.1
 Name: scylla-driver
-Version: 3.25.9
+Version: 3.26.0
 Summary: Scylla Driver for Apache Cassandra
 Home-page: https://github.com/scylladb/python-driver
 Author: ScyllaDB
-License: UNKNOWN
-Project-URL: Source, https://github.com/scylladb/python-driver/
 Project-URL: Documentation, https://scylladb.github.io/python-driver/
+Project-URL: Source, https://github.com/scylladb/python-driver/
 Project-URL: Issues, https://github.com/scylladb/python-driver/issues
-Description: Scylla Python Driver
-        ====================
-        
-        A modern, feature-rich and highly-tunable Python client library for Scylla Open Source (2.1+) and Apache Cassandra (2.1+) and
-        Scylla Enterprise (2018.1.x+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
-        
-        .. image:: https://github.com/scylladb/python-driver/workflows/Build%20and%20upload%20to%20PyPi/badge.svg?tag=*-scylla
-           :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22Build+and+upload+to+PyPi%22+event%3Apush+branch%3A*-scylla
-        
-        .. image:: https://github.com/scylladb/python-driver/workflows/CI%20Docs/badge.svg?tag=*-scylla
-           :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22CI+Docs%22+event%3Apush+branch%3A*-scylla
-        
-        The driver supports Python versions 2.7, 3.4, 3.5, 3.6, 3.7 and 3.8.
-        
-        .. **Note:** This driver does not support big-endian systems.
-        
-        Features
-        --------
-        * `Synchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute>`_ and `Asynchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute_async>`_ APIs
-        * `Simple, Prepared, and Batch statements <http://python-driver.docs.scylladb.com/stable/api/cassandra/query.html#cassandra.query.Statement>`_
-        * Asynchronous IO, parallel execution, request pipelining
-        * `Connection pooling <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Cluster.get_core_connections_per_host>`_
-        * Automatic node discovery
-        * `Automatic reconnection <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#reconnecting-to-dead-hosts>`_
-        * Configurable `load balancing <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#load-balancing>`_ and `retry policies <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#retrying-failed-operations>`_
-        * `Concurrent execution utilities <http://python-driver.docs.scylladb.com/stable/api/cassandra/concurrent.html>`_
-        * `Object mapper <http://python-driver.docs.scylladb.com/stable/object_mapper.html>`_
-        * `Shard awareness <http://python-driver.docs.scylladb.com/stable/scylla_specific.html#shard-awareness>`_
-        
-        Installation
-        ------------
-        Installation through pip is recommended::
-        
-            $ pip install scylla-driver
-        
-        For more complete installation instructions, see the
-        `installation guide <http://python-driver.docs.scylladb.com/stable/installation.html>`_.
-        
-        Documentation
-        -------------
-        The documentation can be found online `here <http://python-driver.docs.scylladb.com/stable/index.html>`_.
-        
-        Information includes: 
-        
-        * `Installation <http://python-driver.docs.scylladb.com/stable/installation.html>`_
-        * `Getting started guide <http://python-driver.docs.scylladb.com/stable/getting_started.html>`_
-        * `API docs <http://python-driver.docs.scylladb.com/stable/api/index.html>`_
-        * `Performance tips <http://python-driver.docs.scylladb.com/stable/performance.html>`_
-        
-        Training
-        --------
-        The course `Using Scylla Drivers <https://university.scylladb.com/courses/using-scylla-drivers/lessons/coding-with-python/>`_ in `Scylla University <https://university.scylladb.com>`_  explains how to use drivers in different languages to interact with a Scylla cluster. 
-        The lesson, Coding with Python (link), goes over a sample application that, using the Python driver, interacts with a three-node Scylla cluster.
-        It connects to a Scylla cluster, displays the contents of a  table, inserts and deletes data, and shows the contents of the table after each action.
-        `Scylla University <https://university.scylladb.com>`_ includes other training material and online courses which will help you become a Scylla NoSQL database expert.
-        
-        
-        Object Mapper
-        -------------
-        cqlengine (originally developed by Blake Eggleston and Jon Haddad, with contributions from the
-        community) is now maintained as an integral part of this package. Refer to
-        `documentation here <http://python-driver.docs.scylladb.com/stable/object_mapper.html>`_.
-        
-        Contributing
-        ------------
-        See `CONTRIBUTING <https://github.com/scylladb/python-driver/blob/master/CONTRIBUTING.rst>`_.
-        
-        Reporting Problems
-        ------------------
-        Please report any bugs and make any feature requests by clicking the New Issue button in 
-        `Github <https://github.com/scylladb/python-driver/issues>`_.
-        
-        If you would like to contribute, please feel free to send a pull request.
-        
-        Getting Help
-        ------------
-        Your best options for getting help with the driver are the
-        `mailing list <https://groups.google.com/forum/#!forum/scylladb-users>`_
-        and the Scylla Users `Slack channel <https://scylladb-users.slack.com>`_.
-        
-        License
-        -------
-        Copyright DataStax, Inc.
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
 Keywords: cassandra,cql,orm,dse,graph
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: graph
+License-File: LICENSE
+
+Scylla Python Driver
+====================
+
+A modern, feature-rich and highly-tunable Python client library for Scylla Open Source (2.1+) and Apache Cassandra (2.1+) and
+Scylla Enterprise (2018.1.x+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
+
+.. image:: https://github.com/scylladb/python-driver/workflows/Build%20and%20upload%20to%20PyPi/badge.svg?tag=*-scylla
+   :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22Build+and+upload+to+PyPi%22+event%3Apush+branch%3A*-scylla
+
+.. image:: https://github.com/scylladb/python-driver/workflows/CI%20Docs/badge.svg?tag=*-scylla
+   :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22CI+Docs%22+event%3Apush+branch%3A*-scylla
+
+The driver supports Python versions 3.6-3.11.
+
+.. **Note:** This driver does not support big-endian systems.
+
+Features
+--------
+* `Synchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute>`_ and `Asynchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute_async>`_ APIs
+* `Simple, Prepared, and Batch statements <http://python-driver.docs.scylladb.com/stable/api/cassandra/query.html#cassandra.query.Statement>`_
+* Asynchronous IO, parallel execution, request pipelining
+* `Connection pooling <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Cluster.get_core_connections_per_host>`_
+* Automatic node discovery
+* `Automatic reconnection <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#reconnecting-to-dead-hosts>`_
+* Configurable `load balancing <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#load-balancing>`_ and `retry policies <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#retrying-failed-operations>`_
+* `Concurrent execution utilities <http://python-driver.docs.scylladb.com/stable/api/cassandra/concurrent.html>`_
+* `Object mapper <http://python-driver.docs.scylladb.com/stable/object-mapper.html>`_
+* `Shard awareness <http://python-driver.docs.scylladb.com/stable/scylla-specific.html#shard-awareness>`_
+
+Installation
+------------
+Installation through pip is recommended::
+
+    $ pip install scylla-driver
+
+For more complete installation instructions, see the
+`installation guide <http://python-driver.docs.scylladb.com/stable/installation.html>`_.
+
+Documentation
+-------------
+The documentation can be found online `here <http://python-driver.docs.scylladb.com/stable/index.html>`_.
+
+Information includes: 
+
+* `Installation <http://python-driver.docs.scylladb.com/stable/installation.html>`_
+* `Getting started guide <http://python-driver.docs.scylladb.com/stable/getting-started.html>`_
+* `API docs <http://python-driver.docs.scylladb.com/stable/api/index.html>`_
+* `Performance tips <http://python-driver.docs.scylladb.com/stable/performance.html>`_
+
+Training
+--------
+The course `Using Scylla Drivers <https://university.scylladb.com/courses/using-scylla-drivers/lessons/coding-with-python/>`_ in `Scylla University <https://university.scylladb.com>`_  explains how to use drivers in different languages to interact with a Scylla cluster. 
+The lesson, Coding with Python (link), goes over a sample application that, using the Python driver, interacts with a three-node Scylla cluster.
+It connects to a Scylla cluster, displays the contents of a  table, inserts and deletes data, and shows the contents of the table after each action.
+`Scylla University <https://university.scylladb.com>`_ includes other training material and online courses which will help you become a Scylla NoSQL database expert.
+
+
+Object Mapper
+-------------
+cqlengine (originally developed by Blake Eggleston and Jon Haddad, with contributions from the
+community) is now maintained as an integral part of this package. Refer to
+`documentation here <http://python-driver.docs.scylladb.com/stable/object-mapper.html>`_.
+
+Contributing
+------------
+See `CONTRIBUTING <https://github.com/scylladb/python-driver/blob/master/CONTRIBUTING.rst>`_.
+
+Reporting Problems
+------------------
+Please report any bugs and make any feature requests by clicking the New Issue button in 
+`Github <https://github.com/scylladb/python-driver/issues>`_.
+
+If you would like to contribute, please feel free to send a pull request.
+
+Getting Help
+------------
+Your best options for getting help with the driver are the
+`mailing list <https://groups.google.com/forum/#!forum/scylladb-users>`_
+and the Scylla Users `Slack channel <https://scylladb-users.slack.com>`_.
+
+License
+-------
+Copyright DataStax, Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `scylla-driver-3.25.9/cassandra/policies.py` & `scylla-driver-3.26.0/cassandra/policies.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/models.py` & `scylla-driver-3.26.0/cassandra/cqlengine/models.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/operators.py` & `scylla-driver-3.26.0/cassandra/cqlengine/operators.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/connection.py` & `scylla-driver-3.26.0/cassandra/cqlengine/connection.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/__init__.py` & `scylla-driver-3.26.0/cassandra/cqlengine/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/management.py` & `scylla-driver-3.26.0/cassandra/cqlengine/management.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,17 +479,25 @@
             raise KeyError(msg % (name, existing_options.keys()))
         if isinstance(existing_value, six.string_types):
             if value != existing_value:
                 update_options[name] = value
         else:
             try:
                 for k, v in value.items():
-                    if existing_value[k] != v:
-                        update_options[name] = value
-                        break
+                    # When creating table with compaction 'class': 'org.apache.cassandra.db.compaction.LeveledCompactionStrategy' in Scylla,
+                    # it will be silently changed to 'class': 'LeveledCompactionStrategy' - same for at least SizeTieredCompactionStrategy,
+                    # probably others too. We need to handle this case here.
+                    if k == 'class' and name == 'compaction':
+                        if existing_value[k] != v and existing_value[k] != v.split('.')[-1]:
+                            update_options[name] = value
+                            break
+                    else:
+                        if existing_value[k] != v:
+                            update_options[name] = value
+                            break
             except KeyError:
                 update_options[name] = value
 
     if update_options:
         options = ' AND '.join(metadata.TableMetadataV3._make_option_strings(update_options))
         query = "ALTER TABLE {0} WITH {1}".format(model.column_family_name(), options)
         execute(query, connection=connection)
```

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/query.py` & `scylla-driver-3.26.0/cassandra/cqlengine/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/functions.py` & `scylla-driver-3.26.0/cassandra/cqlengine/functions.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/statements.py` & `scylla-driver-3.26.0/cassandra/cqlengine/statements.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/usertype.py` & `scylla-driver-3.26.0/cassandra/cqlengine/usertype.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/named.py` & `scylla-driver-3.26.0/cassandra/cqlengine/named.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqlengine/columns.py` & `scylla-driver-3.26.0/cassandra/cqlengine/columns.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/deserializers.pxd` & `scylla-driver-3.26.0/cassandra/deserializers.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/auth.py` & `scylla-driver-3.26.0/cassandra/auth.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cmurmur3.c` & `scylla-driver-3.26.0/cassandra/cmurmur3.c`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/row_parser.pyx` & `scylla-driver-3.26.0/cassandra/row_parser.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cluster.py` & `scylla-driver-3.26.0/cassandra/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from copy import copy
 from functools import partial, wraps
 from itertools import groupby, count, chain
 import json
 import logging
 from warnings import warn
 from random import random
+import re
 import six
 from six.moves import filter, range, queue as Queue
 import socket
 import sys
 import time
 from threading import Lock, RLock, Thread, Event
 import uuid
@@ -529,15 +530,15 @@
 """
 
 EXEC_PROFILE_GRAPH_DEFAULT = object()
 """
 Key for the default graph execution profile, used when no other profile is selected in
 ``Session.execute_graph(execution_profile)``.
 
-Use this as the key in :doc:`Cluster(execution_profiles) </execution_profiles>`
+Use this as the key in :doc:`Cluster(execution_profiles) </execution-profiles>`
 to override the default graph profile.
 """
 
 EXEC_PROFILE_GRAPH_SYSTEM_DEFAULT = object()
 """
 Key for the default graph system execution profile. This can be used for graph statements using the DSE graph
 system API.
@@ -2110,15 +2111,15 @@
         for session in tuple(self.sessions):
             session.update_created_pools()
 
     def on_remove(self, host):
         if self.is_shutdown:
             return
 
-        log.debug("Removing host %s", host)
+        log.debug("[cluster] Removing host %s", host)
         host.set_down()
         self.profile_manager.on_remove(host)
         for session in tuple(self.sessions):
             session.on_remove(host)
         for listener in self.listeners:
             listener.on_remove(host)
         self.control_connection.on_remove(host)
@@ -3778,14 +3779,146 @@
         if not agreed:
             log.debug("Skipping schema refresh due to lack of schema agreement")
             return False
 
         self._cluster.metadata.refresh(connection, self._timeout, fetch_size=self._schema_meta_page_size, **kwargs)
 
         return True
+    
+    # Three functions below (_refresh_schema_async, _refresh_schema_async_inner, _wait_for_schema_agreement_async) are async
+    # versions of the functions without _async in name - instead of blocking and returning result, their first argument
+    # is a callback that will receive either a result or an exception.
+    # Purpose of those functions is to avoid filling whole thread pool and deadlocking.
+    def _refresh_schema_async(self, callback, force=False, **kwargs):
+        def new_callback(e):
+            if isinstance(e, ReferenceError):
+                # our weak reference to the Cluster is no good
+                callback(False)
+                return
+            elif isinstance(e, Exception):
+                log.debug("[control connection] Error refreshing schema", exc_info=True)
+                self._signal_error()
+                callback(False)
+                return
+            else:
+                callback(e)
+        if self._connection:
+            self._refresh_schema_async_inner(new_callback, self._connection, force=force, **kwargs)
+        else:
+            callback(False)
+
+    def _refresh_schema_async_inner(self, callback, connection, preloaded_results=None, schema_agreement_wait=None, force=False, **kwargs):
+        if self._cluster.is_shutdown:
+            callback(False)
+            return
+        
+        def new_callback(e):
+            if not self._schema_meta_enabled and not force:
+                log.debug("[control connection] Skipping schema refresh because schema metadata is disabled")
+                callback(False)
+                return
+
+            if not e:
+                log.debug("Skipping schema refresh due to lack of schema agreement")
+                callback(False)
+                return
+            self._cluster.metadata.refresh(connection, self._timeout, fetch_size=self._schema_meta_page_size, **kwargs)
+        
+        self._wait_for_schema_agreement_async(new_callback,
+                                                connection=self._connection,
+                                                preloaded_results=preloaded_results,
+                                                wait_time=schema_agreement_wait)
+
+    # INTENDED ONLY FOR INTERNAL USE
+    def _wait_for_schema_agreement_async(self, callback, connection=None, preloaded_results=None, wait_time=None):
+        total_timeout = wait_time if wait_time is not None else self._cluster.max_schema_agreement_wait
+        if total_timeout <= 0:
+            callback(True)
+            return
+
+        # Each schema change typically generates two schema refreshes, one
+        # from the response type and one from the pushed notification. Holding
+        # a lock is just a simple way to cut down on the number of schema queries
+        # we'll make.
+        if not self._schema_agreement_lock.acquire(blocking=False):
+            self._cluster.scheduler.schedule_unique(0.2, self._wait_for_schema_agreement_async, callback, connection, preloaded_results, wait_time)
+            return
+        
+        try:
+            if self._is_shutdown:
+                self._schema_agreement_lock.release()
+                callback(None)
+                return
+
+            if not connection:
+                connection = self._connection
+
+            if preloaded_results:
+                log.debug("[control connection] Attempting to use preloaded results for schema agreement")
+
+                peers_result = preloaded_results[0]
+                local_result = preloaded_results[1]
+                schema_mismatches = self._get_schema_mismatches(peers_result, local_result, connection.endpoint)
+                if schema_mismatches is None:
+                    self._schema_agreement_lock.release()
+                    callback(True)
+                    return
+
+            log.debug("[control connection] Waiting for schema agreement")
+            start = self._time.time()
+            elapsed = 0
+            cl = ConsistencyLevel.ONE
+            schema_mismatches = None
+            select_peers_query = self._get_peers_query(self.PeersQueryType.PEERS_SCHEMA, connection)
+        except Exception as e:
+            self._schema_agreement_lock.release()
+            callback(e)
+            return
+
+        def inner(first_iter):
+            try:
+                elapsed = self._time.time() - start
+                if elapsed < total_timeout or first_iter:
+                    peers_query = QueryMessage(query=select_peers_query, consistency_level=cl)
+                    local_query = QueryMessage(query=self._SELECT_SCHEMA_LOCAL, consistency_level=cl)
+                    try:
+                        timeout = min(self._timeout, total_timeout - elapsed)
+                        peers_result, local_result = connection.wait_for_responses(
+                            peers_query, local_query, timeout=timeout)
+                    except OperationTimedOut as timeout:
+                        log.debug("[control connection] Timed out waiting for "
+                                    "response during schema agreement check: %s", timeout)
+                        self._cluster.scheduler.schedule_unique(0.2, inner, False)
+                        return
+                    except ConnectionShutdown as e:
+                        if self._is_shutdown:
+                            log.debug("[control connection] Aborting wait for schema match due to shutdown")
+                            self._schema_agreement_lock.release()
+                            callback(None)
+                            return
+                        else:
+                            raise
+
+                    schema_mismatches = self._get_schema_mismatches(peers_result, local_result, connection.endpoint)
+                    if schema_mismatches is None:
+                        self._schema_agreement_lock.release()
+                        callback(True)
+                        return
+
+                    log.debug("[control connection] Schemas mismatched, trying again")
+                    self._cluster.scheduler.schedule_unique(0.2, inner, False)
+                else:
+                    log.warning("Node %s is reporting a schema disagreement: %s",
+                                connection.endpoint, schema_mismatches)
+                    self._schema_agreement_lock.release()
+                    callback(False)
+            except Exception as e:
+                self._schema_agreement_lock.release()
+                callback(e)
+        inner(True)
 
     def refresh_node_list_and_token_map(self, force_token_rebuild=False):
         try:
             if self._connection:
                 self._refresh_node_list_and_token_map(self._connection, force_token_rebuild=force_token_rebuild)
                 return True
         except ReferenceError:
@@ -3915,14 +4048,26 @@
             found_host_ids.add(host_id)
             found_endpoints.add(endpoint)
             host = self._cluster.metadata.get_host(endpoint)
             datacenter = row.get("data_center")
             rack = row.get("rack")
 
             if host is None:
+                host = self._cluster.metadata.get_host_by_host_id(host_id)
+                if host and host.endpoint != endpoint:
+                    log.debug("[control connection] Updating host ip from %s to %s for (%s)", host.endpoint, endpoint, host_id)
+                    old_endpoint = host.endpoint
+                    host.endpoint = endpoint
+                    self._cluster.metadata.update_host(host, old_endpoint)
+                    reconnector = host.get_and_set_reconnection_handler(None)
+                    if reconnector:
+                        reconnector.cancel()
+                    self._cluster.on_down(host, is_host_addition=False, expect_host_to_be_down=True)
+
+            if host is None:
                 log.debug("[control connection] Found new host to connect to: %s", endpoint)
                 host, _ = self._cluster.add_host(endpoint, datacenter=datacenter, rack=rack, signal=True, refresh_nodes=False, host_id=host_id)
                 should_rebuild_token_map = True
             else:
                 should_rebuild_token_map |= self._update_location_info(host, datacenter, rack)
 
             host.host_id = host_id
@@ -4022,15 +4167,15 @@
                 # this will be run by the scheduler
                 self._cluster.on_down(host, is_host_addition=False)
 
     def _handle_schema_change(self, event):
         if self._schema_event_refresh_window < 0:
             return
         delay = self._delay_for_event_type('schema_change', self._schema_event_refresh_window)
-        self._cluster.scheduler.schedule_unique(delay, self.refresh_schema, **event)
+        self._cluster.scheduler.schedule_unique(delay, self._refresh_schema_async, lambda *a, **k: None, **event)
 
     def wait_for_schema_agreement(self, connection=None, preloaded_results=None, wait_time=None):
 
         total_timeout = wait_time if wait_time is not None else self._cluster.max_schema_agreement_wait
         if total_timeout <= 0:
             return True
 
@@ -5249,15 +5394,14 @@
                 if not self._list_mode:
                     self._current_rows = []
                 raise
 
         if not self.response_future._continuous_paging_session:
             self.fetch_next_page()
             self._page_iter = iter(self._current_rows)
-            return self.next()
 
             # Some servers can return empty pages in this case; Scylla is known to do
             # so in some circumstances.  Guard against this by recursing to handle
             # the next(iter) call.  If we have an empty page in that case it will
             # get handled by the StopIteration handler when we recurse.
             return self.next()
 
@@ -5334,29 +5478,32 @@
 
     def cancel_continuous_paging(self):
         try:
             self.response_future._continuous_paging_session.cancel()
         except AttributeError:
             raise DriverException("Attempted to cancel paging with no active session. This is only for requests with ContinuousdPagingOptions.")
 
+    batch_regex = re.compile('^\s*BEGIN\s+[a-zA-Z]*\s*BATCH')
+
     @property
     def was_applied(self):
         """
         For LWT results, returns whether the transaction was applied.
 
         Result is indeterminate if called on a result that was not an LWT request or on
         a :class:`.query.BatchStatement` containing LWT. In the latter case either all the batch
         succeeds or fails.
 
         Only valid when one of the of the internal row factories is in use.
         """
         if self.response_future.row_factory not in (named_tuple_factory, dict_factory, tuple_factory):
             raise RuntimeError("Cannot determine LWT result with row factory %s" % (self.response_future.row_factory,))
 
-        is_batch_statement = isinstance(self.response_future.query, BatchStatement)
+        is_batch_statement = isinstance(self.response_future.query, BatchStatement) \
+                            or (isinstance(self.response_future.query, SimpleStatement) and self.batch_regex.match(self.response_future.query.query_string))
         if is_batch_statement and (not self.column_names or self.column_names[0] != "[applied]"):
             raise RuntimeError("No LWT were present in the BatchStatement")
 
         if not is_batch_statement and len(self.current_rows) != 1:
             raise RuntimeError("LWT result should have exactly one row. This has %d." % (len(self.current_rows)))
 
         row = self.current_rows[0]
```

### Comparing `scylla-driver-3.25.9/cassandra/type_codes.py` & `scylla-driver-3.26.0/cassandra/type_codes.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/bytesio.pxd` & `scylla-driver-3.26.0/cassandra/bytesio.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/protocol.py` & `scylla-driver-3.26.0/cassandra/protocol.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/deserializers.pyx` & `scylla-driver-3.26.0/cassandra/deserializers.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/type_codes.pxd` & `scylla-driver-3.26.0/cassandra/type_codes.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/marshal.py` & `scylla-driver-3.26.0/cassandra/marshal.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/obj_parser.pyx` & `scylla-driver-3.26.0/cassandra/obj_parser.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/murmur3.py` & `scylla-driver-3.26.0/cassandra/murmur3.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/connection.py` & `scylla-driver-3.26.0/cassandra/connection.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cython_marshal.pyx` & `scylla-driver-3.26.0/cassandra/cython_marshal.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/c_shard_info.pyx` & `scylla-driver-3.26.0/cassandra/c_shard_info.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/concurrent.py` & `scylla-driver-3.26.0/cassandra/concurrent.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/__init__.py` & `scylla-driver-3.26.0/cassandra/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class NullHandler(logging.Handler):
 
     def emit(self, record):
         pass
 
 logging.getLogger('cassandra').addHandler(NullHandler())
 
-__version_info__ = (3, 25, 9)
+__version_info__ = (3, 26, 0)
 __version__ = '.'.join(map(str, __version_info__))
 
 
 class ConsistencyLevel(object):
     """
     Spcifies how many replicas must respond for an operation to be considered
     a success.  By default, ``ONE`` is used for all operations.
@@ -51,15 +51,15 @@
     THREE = 3
     """
     Three replicas must respond to consider the operation a success
     """
 
     QUORUM = 4
     """
-    ``ceil(RF/2)`` replicas must respond to consider the operation a success
+    ``ceil(RF/2) + 1`` replicas must respond to consider the operation a success
     """
 
     ALL = 5
     """
     All replicas must respond to consider the operation a success
     """
```

### Comparing `scylla-driver-3.25.9/cassandra/encoder.py` & `scylla-driver-3.26.0/cassandra/encoder.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/__init__.py` & `scylla-driver-3.26.0/cassandra/datastax/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/insights/registry.py` & `scylla-driver-3.26.0/cassandra/datastax/insights/registry.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/insights/serializers.py` & `scylla-driver-3.26.0/cassandra/datastax/insights/serializers.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/insights/__init__.py` & `scylla-driver-3.26.0/cassandra/datastax/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/insights/util.py` & `scylla-driver-3.26.0/cassandra/datastax/insights/util.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/insights/reporter.py` & `scylla-driver-3.26.0/cassandra/datastax/insights/reporter.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/cloud/__init__.py` & `scylla-driver-3.26.0/cassandra/datastax/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/__init__.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/query.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/fluent/_serializers.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_serializers.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/fluent/serializers.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/serializers.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/fluent/__init__.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/fluent/query.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/fluent/_query.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/fluent/predicates.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/predicates.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/fluent/_predicates.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/fluent/_predicates.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/graphson.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/graphson.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/datastax/graph/types.py` & `scylla-driver-3.26.0/cassandra/datastax/graph/types.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/util.py` & `scylla-driver-3.26.0/cassandra/util.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/query.py` & `scylla-driver-3.26.0/cassandra/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/metrics.py` & `scylla-driver-3.26.0/cassandra/metrics.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/compat.py` & `scylla-driver-3.26.0/cassandra/compat.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/timestamps.py` & `scylla-driver-3.26.0/cassandra/timestamps.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/geventreactor.py` & `scylla-driver-3.26.0/cassandra/io/geventreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/__init__.py` & `scylla-driver-3.26.0/cassandra/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/libevreactor.py` & `scylla-driver-3.26.0/cassandra/io/libevreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/eventletreactor.py` & `scylla-driver-3.26.0/cassandra/io/eventletreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/libevwrapper.c` & `scylla-driver-3.26.0/cassandra/io/libevwrapper.c`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/asyncioreactor.py` & `scylla-driver-3.26.0/cassandra/io/asyncioreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/twistedreactor.py` & `scylla-driver-3.26.0/cassandra/io/twistedreactor.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/io/asyncorereactor.py` & `scylla-driver-3.26.0/cassandra/io/asyncorereactor.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,26 +245,29 @@
     def _run_loop(self):
         log.debug("Starting asyncore event loop")
         with self._loop_lock:
             while not self._shutdown:
                 try:
                     self._loop_dispatcher.loop(self.timer_resolution)
                     self._timers.service_timeouts()
-                except Exception:
-                    try:
-                        log.debug("Asyncore event loop stopped unexpectedly", exc_info=True)
-                    except Exception:
-                        # TODO: Remove when Python 2 support is removed
-                        # PYTHON-1266. If our logger has disappeared, there's nothing we
-                        # can do, so just log nothing.
-                        pass
+                except Exception as exc:
+                    self._maybe_log_debug("Asyncore event loop stopped unexpectedly", exc_info=exc)
                     break
             self._started = False
 
-        log.debug("Asyncore event loop ended")
+        self._maybe_log_debug("Asyncore event loop ended")
+
+    def _maybe_log_debug(self, *args, **kwargs):
+        try:
+            log.debug(*args, **kwargs)
+        except Exception:
+            # TODO: Remove when Python 2 support is removed
+            # PYTHON-1266. If our logger has disappeared, there's nothing we
+            # can do, so just log nothing.
+            pass
 
     def add_timer(self, timer):
         self._timers.add_timer(timer)
 
         # This function is called from a different thread than the event loop
         # thread, so for this call to be thread safe, we must wake up the loop
         # in case it's stuck at a select
```

### Comparing `scylla-driver-3.25.9/cassandra/metadata.py` & `scylla-driver-3.26.0/cassandra/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,21 @@
         with self._hosts_lock:
             if not isinstance(endpoint_or_address, EndPoint):
                 return self._get_host_by_address(endpoint_or_address, port)
 
             host_id = self._host_id_by_endpoint.get(endpoint_or_address)
             return self._hosts.get(host_id)
 
+    def get_host_by_host_id(self, host_id):
+        """
+        Same as get_host() but use host_id for lookup.
+        """
+        with self._hosts_lock:
+            return self._hosts.get(host_id)
+
     def _get_host_by_address(self, address, port=None):
         for host in six.itervalues(self._hosts):
             if (host.broadcast_rpc_address == address and
                     (port is None or host.broadcast_rpc_port is None or host.broadcast_rpc_port == port)):
                 return host
 
         return None
```

### Comparing `scylla-driver-3.25.9/cassandra/segment.py` & `scylla-driver-3.26.0/cassandra/segment.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/shard_info.py` & `scylla-driver-3.26.0/cassandra/shard_info.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/scylla/cloud.py` & `scylla-driver-3.26.0/cassandra/scylla/cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,22 +48,20 @@
 
 def nth(iterable, n, default=None):
     "Returns the nth item or a default value"
     return next(islice(iterable, n, None), default)
 
 
 class CloudConfiguration:
-    # Commented out because this syntax doesn't work with Python2
-    # Can be restores after dropping support for Python2
-    # endpoint_factory: SniEndPointFactory
-    # contact_points: list
-    # auth_provider: AuthProvider = None
-    # ssl_options: dict
-    # ssl_context: SSLContext
-    # skip_tls_verify: bool
+    endpoint_factory: SniEndPointFactory
+    contact_points: list
+    auth_provider: AuthProvider = None
+    ssl_options: dict
+    ssl_context: SSLContext
+    skip_tls_verify: bool
 
     def __init__(self, configuration_file, pyopenssl=False, endpoint_factory=None):
         cloud_config = yaml.safe_load(open(configuration_file))
 
         self.current_context = cloud_config['contexts'][cloud_config['currentContext']]
         self.data_centers = cloud_config['datacenters']
         self.current_data_center = self.data_centers[self.current_context['datacenterName']]
```

### Comparing `scylla-driver-3.25.9/cassandra/numpy_parser.pyx` & `scylla-driver-3.26.0/cassandra/numpy_parser.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cython_utils.pyx` & `scylla-driver-3.26.0/cassandra/cython_utils.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/bytesio.pyx` & `scylla-driver-3.26.0/cassandra/bytesio.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/cqltypes.py` & `scylla-driver-3.26.0/cassandra/cqltypes.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/buffer.pxd` & `scylla-driver-3.26.0/cassandra/buffer.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/pool.py` & `scylla-driver-3.26.0/cassandra/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Connection pooling and host management.
 """
-from __future__ import absolute_import
-
 from concurrent.futures import Future
 from functools import total_ordering
 import logging
 import socket
 import time
 import random
 import copy
@@ -735,14 +733,17 @@
                     log.debug(
                         "Replacing overloaded connection (%s) with (%s) for shard %i for host %s",
                         id(old_conn),
                         id(conn),
                         conn.shard_id,
                         self.host
                     )
+                if self._keyspace:
+                    conn.set_keyspace_blocking(self._keyspace)
+
                 self._connections[conn.shard_id] = conn
             if old_conn is not None:
                 remaining = old_conn.in_flight - len(old_conn.orphaned_request_ids)
                 if remaining == 0:
                     log.debug(
                         "Immediately closing the old connection (%s) for shard %i on host %s",
                         id(old_conn),
@@ -759,21 +760,14 @@
                         remaining,
                     )
                     with self._lock:
                         if self.is_shutdown:
                             old_conn.close()
                         else:
                             self._trash.add(old_conn)
-            if self._keyspace:
-                with self._lock:
-                    if self.is_shutdown:
-                        conn.close()
-                    old_conn = self._connections.get(conn.shard_id)
-                    if old_conn:
-                        old_conn.set_keyspace_blocking(self._keyspace)
             num_missing_or_needing_replacement = self.num_missing_or_needing_replacement
             log.debug(
                 "Connected to %s/%i shards on host %s (%i missing or needs replacement)",
                 len(self._connections.keys()),
                 self.host.sharding_info.shards_count,
                 self.host,
                 num_missing_or_needing_replacement
@@ -875,15 +869,17 @@
 
     def get_connections(self):
         connections = self._connections
         return list(connections.values()) if connections else []
 
     def get_state(self):
         in_flights = [c.in_flight for c in list(self._connections.values())]
-        return {'shutdown': self.is_shutdown, 'open_count': self.open_count, 'in_flights': in_flights}
+        orphan_requests = [c.orphaned_request_ids for c in list(self._connections.values())]
+        return {'shutdown': self.is_shutdown, 'open_count': self.open_count, \
+                'in_flights': in_flights, 'orphan_requests': orphan_requests}
 
     @property
     def num_missing_or_needing_replacement(self):
         return self.host.sharding_info.shards_count \
             - sum(1 for c in self._connections.values() if not c.orphaned_threshold_reached)
 
     @property
@@ -1198,17 +1194,15 @@
 
         self._signal_all_available_conn()
 
         connections_to_close = []
         with self._lock:
             connections_to_close.extend(self._connections)
             self.open_count -= len(self._connections)
-            # After dropping support for Python 2 we can again use list.clear()
-            # self._connections.clear()
-            del self._connections[:]
+            self._connections.clear()
             connections_to_close.extend(self._trash)
             self._trash.clear()
 
         for conn in connections_to_close:
             conn.close()
 
     def ensure_core_connections(self):
@@ -1249,8 +1243,10 @@
             conn.set_keyspace_async(keyspace, connection_finished_setting_keyspace)
 
     def get_connections(self):
         return self._connections
 
     def get_state(self):
         in_flights = [c.in_flight for c in self._connections]
-        return {'shutdown': self.is_shutdown, 'open_count': self.open_count, 'in_flights': in_flights}
+        orphan_requests = [c.orphaned_request_ids for c in self._connections]
+        return {'shutdown': self.is_shutdown, 'open_count': self.open_count, \
+            'in_flights': in_flights, 'orphan_requests': orphan_requests}
```

### Comparing `scylla-driver-3.25.9/cassandra/parsing.pyx` & `scylla-driver-3.26.0/cassandra/parsing.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/tuple.pxd` & `scylla-driver-3.26.0/cassandra/tuple.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/parsing.pxd` & `scylla-driver-3.26.0/cassandra/parsing.pxd`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/ioutils.pyx` & `scylla-driver-3.26.0/cassandra/ioutils.pyx`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/graph/__init__.py` & `scylla-driver-3.26.0/cassandra/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/graph/query.py` & `scylla-driver-3.26.0/cassandra/graph/query.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/graph/graphson.py` & `scylla-driver-3.26.0/cassandra/graph/graphson.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/cassandra/graph/types.py` & `scylla-driver-3.26.0/cassandra/graph/types.py`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/scylla_driver.egg-info/SOURCES.txt` & `scylla-driver-3.26.0/scylla_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scylla-driver-3.25.9/scylla_driver.egg-info/PKG-INFO` & `scylla-driver-3.26.0/scylla_driver.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,124 +1,120 @@
 Metadata-Version: 2.1
 Name: scylla-driver
-Version: 3.25.9
+Version: 3.26.0
 Summary: Scylla Driver for Apache Cassandra
 Home-page: https://github.com/scylladb/python-driver
 Author: ScyllaDB
-License: UNKNOWN
-Project-URL: Source, https://github.com/scylladb/python-driver/
 Project-URL: Documentation, https://scylladb.github.io/python-driver/
+Project-URL: Source, https://github.com/scylladb/python-driver/
 Project-URL: Issues, https://github.com/scylladb/python-driver/issues
-Description: Scylla Python Driver
-        ====================
-        
-        A modern, feature-rich and highly-tunable Python client library for Scylla Open Source (2.1+) and Apache Cassandra (2.1+) and
-        Scylla Enterprise (2018.1.x+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
-        
-        .. image:: https://github.com/scylladb/python-driver/workflows/Build%20and%20upload%20to%20PyPi/badge.svg?tag=*-scylla
-           :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22Build+and+upload+to+PyPi%22+event%3Apush+branch%3A*-scylla
-        
-        .. image:: https://github.com/scylladb/python-driver/workflows/CI%20Docs/badge.svg?tag=*-scylla
-           :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22CI+Docs%22+event%3Apush+branch%3A*-scylla
-        
-        The driver supports Python versions 2.7, 3.4, 3.5, 3.6, 3.7 and 3.8.
-        
-        .. **Note:** This driver does not support big-endian systems.
-        
-        Features
-        --------
-        * `Synchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute>`_ and `Asynchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute_async>`_ APIs
-        * `Simple, Prepared, and Batch statements <http://python-driver.docs.scylladb.com/stable/api/cassandra/query.html#cassandra.query.Statement>`_
-        * Asynchronous IO, parallel execution, request pipelining
-        * `Connection pooling <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Cluster.get_core_connections_per_host>`_
-        * Automatic node discovery
-        * `Automatic reconnection <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#reconnecting-to-dead-hosts>`_
-        * Configurable `load balancing <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#load-balancing>`_ and `retry policies <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#retrying-failed-operations>`_
-        * `Concurrent execution utilities <http://python-driver.docs.scylladb.com/stable/api/cassandra/concurrent.html>`_
-        * `Object mapper <http://python-driver.docs.scylladb.com/stable/object_mapper.html>`_
-        * `Shard awareness <http://python-driver.docs.scylladb.com/stable/scylla_specific.html#shard-awareness>`_
-        
-        Installation
-        ------------
-        Installation through pip is recommended::
-        
-            $ pip install scylla-driver
-        
-        For more complete installation instructions, see the
-        `installation guide <http://python-driver.docs.scylladb.com/stable/installation.html>`_.
-        
-        Documentation
-        -------------
-        The documentation can be found online `here <http://python-driver.docs.scylladb.com/stable/index.html>`_.
-        
-        Information includes: 
-        
-        * `Installation <http://python-driver.docs.scylladb.com/stable/installation.html>`_
-        * `Getting started guide <http://python-driver.docs.scylladb.com/stable/getting_started.html>`_
-        * `API docs <http://python-driver.docs.scylladb.com/stable/api/index.html>`_
-        * `Performance tips <http://python-driver.docs.scylladb.com/stable/performance.html>`_
-        
-        Training
-        --------
-        The course `Using Scylla Drivers <https://university.scylladb.com/courses/using-scylla-drivers/lessons/coding-with-python/>`_ in `Scylla University <https://university.scylladb.com>`_  explains how to use drivers in different languages to interact with a Scylla cluster. 
-        The lesson, Coding with Python (link), goes over a sample application that, using the Python driver, interacts with a three-node Scylla cluster.
-        It connects to a Scylla cluster, displays the contents of a  table, inserts and deletes data, and shows the contents of the table after each action.
-        `Scylla University <https://university.scylladb.com>`_ includes other training material and online courses which will help you become a Scylla NoSQL database expert.
-        
-        
-        Object Mapper
-        -------------
-        cqlengine (originally developed by Blake Eggleston and Jon Haddad, with contributions from the
-        community) is now maintained as an integral part of this package. Refer to
-        `documentation here <http://python-driver.docs.scylladb.com/stable/object_mapper.html>`_.
-        
-        Contributing
-        ------------
-        See `CONTRIBUTING <https://github.com/scylladb/python-driver/blob/master/CONTRIBUTING.rst>`_.
-        
-        Reporting Problems
-        ------------------
-        Please report any bugs and make any feature requests by clicking the New Issue button in 
-        `Github <https://github.com/scylladb/python-driver/issues>`_.
-        
-        If you would like to contribute, please feel free to send a pull request.
-        
-        Getting Help
-        ------------
-        Your best options for getting help with the driver are the
-        `mailing list <https://groups.google.com/forum/#!forum/scylladb-users>`_
-        and the Scylla Users `Slack channel <https://scylladb-users.slack.com>`_.
-        
-        License
-        -------
-        Copyright DataStax, Inc.
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
 Keywords: cassandra,cql,orm,dse,graph
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
 Provides-Extra: graph
+License-File: LICENSE
+
+Scylla Python Driver
+====================
+
+A modern, feature-rich and highly-tunable Python client library for Scylla Open Source (2.1+) and Apache Cassandra (2.1+) and
+Scylla Enterprise (2018.1.x+) using exclusively Cassandra's binary protocol and Cassandra Query Language v3.
+
+.. image:: https://github.com/scylladb/python-driver/workflows/Build%20and%20upload%20to%20PyPi/badge.svg?tag=*-scylla
+   :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22Build+and+upload+to+PyPi%22+event%3Apush+branch%3A*-scylla
+
+.. image:: https://github.com/scylladb/python-driver/workflows/CI%20Docs/badge.svg?tag=*-scylla
+   :target: https://github.com/scylladb/python-driver/actions?query=workflow%3A%22CI+Docs%22+event%3Apush+branch%3A*-scylla
+
+The driver supports Python versions 3.6-3.11.
+
+.. **Note:** This driver does not support big-endian systems.
+
+Features
+--------
+* `Synchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute>`_ and `Asynchronous <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Session.execute_async>`_ APIs
+* `Simple, Prepared, and Batch statements <http://python-driver.docs.scylladb.com/stable/api/cassandra/query.html#cassandra.query.Statement>`_
+* Asynchronous IO, parallel execution, request pipelining
+* `Connection pooling <http://python-driver.docs.scylladb.com/stable/api/cassandra/cluster.html#cassandra.cluster.Cluster.get_core_connections_per_host>`_
+* Automatic node discovery
+* `Automatic reconnection <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#reconnecting-to-dead-hosts>`_
+* Configurable `load balancing <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#load-balancing>`_ and `retry policies <http://python-driver.docs.scylladb.com/stable/api/cassandra/policies.html#retrying-failed-operations>`_
+* `Concurrent execution utilities <http://python-driver.docs.scylladb.com/stable/api/cassandra/concurrent.html>`_
+* `Object mapper <http://python-driver.docs.scylladb.com/stable/object-mapper.html>`_
+* `Shard awareness <http://python-driver.docs.scylladb.com/stable/scylla-specific.html#shard-awareness>`_
+
+Installation
+------------
+Installation through pip is recommended::
+
+    $ pip install scylla-driver
+
+For more complete installation instructions, see the
+`installation guide <http://python-driver.docs.scylladb.com/stable/installation.html>`_.
+
+Documentation
+-------------
+The documentation can be found online `here <http://python-driver.docs.scylladb.com/stable/index.html>`_.
+
+Information includes: 
+
+* `Installation <http://python-driver.docs.scylladb.com/stable/installation.html>`_
+* `Getting started guide <http://python-driver.docs.scylladb.com/stable/getting-started.html>`_
+* `API docs <http://python-driver.docs.scylladb.com/stable/api/index.html>`_
+* `Performance tips <http://python-driver.docs.scylladb.com/stable/performance.html>`_
+
+Training
+--------
+The course `Using Scylla Drivers <https://university.scylladb.com/courses/using-scylla-drivers/lessons/coding-with-python/>`_ in `Scylla University <https://university.scylladb.com>`_  explains how to use drivers in different languages to interact with a Scylla cluster. 
+The lesson, Coding with Python (link), goes over a sample application that, using the Python driver, interacts with a three-node Scylla cluster.
+It connects to a Scylla cluster, displays the contents of a  table, inserts and deletes data, and shows the contents of the table after each action.
+`Scylla University <https://university.scylladb.com>`_ includes other training material and online courses which will help you become a Scylla NoSQL database expert.
+
+
+Object Mapper
+-------------
+cqlengine (originally developed by Blake Eggleston and Jon Haddad, with contributions from the
+community) is now maintained as an integral part of this package. Refer to
+`documentation here <http://python-driver.docs.scylladb.com/stable/object-mapper.html>`_.
+
+Contributing
+------------
+See `CONTRIBUTING <https://github.com/scylladb/python-driver/blob/master/CONTRIBUTING.rst>`_.
+
+Reporting Problems
+------------------
+Please report any bugs and make any feature requests by clicking the New Issue button in 
+`Github <https://github.com/scylladb/python-driver/issues>`_.
+
+If you would like to contribute, please feel free to send a pull request.
+
+Getting Help
+------------
+Your best options for getting help with the driver are the
+`mailing list <https://groups.google.com/forum/#!forum/scylladb-users>`_
+and the Scylla Users `Slack channel <https://scylladb-users.slack.com>`_.
+
+License
+-------
+Copyright DataStax, Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `scylla-driver-3.25.9/LICENSE` & `scylla-driver-3.26.0/LICENSE`

 * *Files identical despite different names*

