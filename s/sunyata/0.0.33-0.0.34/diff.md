# Comparing `tmp/sunyata-0.0.33.tar.gz` & `tmp/sunyata-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.33.tar", last modified: Thu Apr 13 05:55:48 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.34.tar", last modified: Thu Apr 13 06:19:54 2023, max compression
```

## Comparing `sunyata-0.0.33.tar` & `sunyata-0.0.34.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 05:55:48.000000 sunyata-0.0.33/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1382 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       19 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/db.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.33/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.33/sunyata/algorithm/rbtree.py
--rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.33/sunyata/algorithm/avltree.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.33/sunyata/algorithm/bplustree.py
--rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.33/sunyata/algorithm/btree.py
--rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.33/sunyata/algorithm/bintree.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.33/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     2823 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.33/sunyata/http/request_stream.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.33/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.33/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-04-12 02:59:45.000000 sunyata-0.0.33/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      892 2023-04-13 03:14:18.000000 sunyata-0.0.33/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.33/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)     3094 2023-04-13 05:54:25.000000 sunyata-0.0.33/sunyata/http/uvserver.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.33/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.33/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    11621 2023-04-13 05:52:50.000000 sunyata-0.0.33/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.33/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.33/README.md
--rwxr-xr-x   0 root         (0) staff       (20)      962 2023-04-13 05:50:20.000000 sunyata-0.0.33/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-13 05:55:48.000000 sunyata-0.0.33/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 06:19:54.000000 sunyata-0.0.34/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 06:19:54.000000 sunyata-0.0.34/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1383 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)       52 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata/
+-rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/db.py
+-rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/log.py
+-rw-r--r--   0 root         (0) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/orm.py
+-rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/eventloop.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata/cli/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/cli/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/cli/cli.py
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/cli/entry.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata/algorithm/
+-rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.34/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.34/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.34/sunyata/algorithm/avltree.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/algorithm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.34/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.34/sunyata/algorithm/btree.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.34/sunyata/algorithm/bintree.py
+-rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/algorithm/lru.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/algorithm/trie.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.34/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/redislock.py
+-rw-r--r--   0 root         (0) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/consul.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata/http/
+-rw-r--r--   0 root         (0) staff       (20)     3103 2023-04-13 06:19:16.000000 sunyata-0.0.34/sunyata/http/server.py
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.34/sunyata/http/request_stream.py
+-rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.34/sunyata/http/transport.py
+-rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.34/sunyata/http/request.py
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-04-12 02:59:45.000000 sunyata-0.0.34/sunyata/http/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1050 2023-04-13 06:14:32.000000 sunyata-0.0.34/sunyata/http/response.py
+-rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.34/sunyata/http/factory.py
+-rw-r--r--   0 root         (0) staff       (20)     2829 2023-04-13 05:58:51.000000 sunyata-0.0.34/sunyata/http/rawserver.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.34/sunyata/http/router.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.34/sunyata/http/status.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/cache_wrap.py
+-rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/compress.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 06:19:54.000000 sunyata-0.0.34/sunyata/rpc/
+-rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/rpc/encrypt.py
+-rw-r--r--   0 root         (0) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/rpc/serialize.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/rpc/exception.py
+-rw-r--r--   0 root         (0) staff       (20)    11622 2023-04-13 06:17:35.000000 sunyata-0.0.34/sunyata/rpc/server.py
+-rw-r--r--   0 root         (0) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/rpc/discovery.py
+-rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.34/sunyata/rpc/transport.py
+-rw-r--r--   0 root         (0) staff       (20)     8110 2023-04-13 06:16:39.000000 sunyata-0.0.34/sunyata/rpc/client.py
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/rpc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/rpc/compress.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/rpc/method.py
+-rw-r--r--   0 root         (0) staff       (20)     2840 2023-04-13 06:02:14.000000 sunyata-0.0.34/sunyata/rpc/protocal.py
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/rpc/const.py
+-rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.34/sunyata/table_writer.py
+-rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.34/sunyata/wrap.py
+-rw-r--r--   0 root         (0) staff       (20)     9004 2023-04-13 06:19:43.000000 sunyata-0.0.34/README.md
+-rwxr-xr-x   0 root         (0) staff       (20)      962 2023-04-13 05:57:53.000000 sunyata-0.0.34/setup.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-13 06:19:54.000000 sunyata-0.0.34/setup.cfg
```

### Comparing `sunyata-0.0.33/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.34/sunyata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 sunyata/algorithm/rbtree.py
 sunyata/algorithm/trie.py
 sunyata/cli/__init__.py
 sunyata/cli/cli.py
 sunyata/cli/entry.py
 sunyata/http/__init__.py
 sunyata/http/factory.py
+sunyata/http/rawserver.py
 sunyata/http/request.py
 sunyata/http/request_stream.py
 sunyata/http/response.py
 sunyata/http/router.py
 sunyata/http/server.py
 sunyata/http/status.py
 sunyata/http/transport.py
-sunyata/http/uvserver.py
 sunyata/rpc/__init__.py
 sunyata/rpc/client.py
 sunyata/rpc/compress.py
 sunyata/rpc/const.py
 sunyata/rpc/discovery.py
 sunyata/rpc/encrypt.py
 sunyata/rpc/exception.py
```

### Comparing `sunyata-0.0.33/sunyata/db.py` & `sunyata-0.0.34/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/log.py` & `sunyata-0.0.34/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/orm.py` & `sunyata-0.0.34/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/cli/cli.py` & `sunyata-0.0.34/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.34/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/algorithm/lru.py` & `sunyata-0.0.34/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/algorithm/trie.py` & `sunyata-0.0.34/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/algorithm/hashtable.py` & `sunyata-0.0.34/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/redislock.py` & `sunyata-0.0.34/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/consul.py` & `sunyata-0.0.34/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/http/server.py` & `sunyata-0.0.34/sunyata/http/rawserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sunyata.http.request_stream import RequestStream
 from traceback import format_exc
 from types import MethodType,FunctionType
 import asyncio
 import inspect
 
 
-class HttpServer(object):
+class RawHttpServer(object):
 
     routerMap = {}
 
     def __init__(self, bind = '0.0.0.0', port=9989):
         super().__init__()
         self.bind = bind
         self.port = port
@@ -68,8 +68,8 @@
     @classmethod
     def route(cls, path, methods = None):
         def wrapper(func):
             cls.addRoute(path, func, methods)
             return func
         return wrapper
 
-route = HttpServer.route
+route = RawHttpServer.route
```

### Comparing `sunyata-0.0.33/sunyata/http/transport.py` & `sunyata-0.0.34/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/http/request.py` & `sunyata-0.0.34/sunyata/http/request.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/http/response.py` & `sunyata-0.0.34/sunyata/http/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,14 @@
         for k, v in self.headers.items():
             resHeaders += f"{k}: {v}\r\n"
         resHeaders += "\r\n"
         resBody = self.body
         if type(resBody) == str:
             resBody = str2bytes(resBody)
         res = str2bytes(resLine + resHeaders) + resBody
-        return res
+        return res
+    
+    def responseBody(self):
+        resBody = self.body
+        if type(resBody) == str:
+            resBody = str2bytes(resBody)
+        return resBody
```

### Comparing `sunyata-0.0.33/sunyata/http/factory.py` & `sunyata-0.0.34/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/http/uvserver.py` & `sunyata-0.0.34/sunyata/http/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from sunyata.http.factory import HttpFactory
 from sunyata.http.status import *
 import uvicorn
-from sunyata.http.server import HttpServer
+from sunyata.http.rawserver import RawHttpServer
 from sunyata.http.request import HttpRequest
 import sunyata.util as util
 import traceback
 
 
-class UvHttpServer(HttpServer):
+class HttpServer(RawHttpServer):
 
     routerMap = {}
 
     def __init__(self, bind = '0.0.0.0', port=9989, log_level='error'):
-        HttpServer.__init__(self, bind=bind, port=port)
-        self.config = uvicorn.Config("sunyata.http.uvserver:UvHttpServer", host=self.bind, port=self.port, log_level=log_level)
+        RawHttpServer.__init__(self, bind=bind, port=port)
+        self.config = uvicorn.Config("sunyata.http.server:HttpServer", host=self.bind, port=self.port, log_level=log_level)
 
     def serve(self):
         server = uvicorn.Server(self.config)
         print('http running on http://%s:%s' % (self.bind, self.port) )
         server.run()
     
     async def genHttpRequest(self, scheme, httpVersion, method, path, queryString, headers, body, clientTuple):
@@ -77,13 +77,13 @@
                 "status": httpResponse.status.code,
                 "headers": [[b"content-type", b"text/plain"]],
             }
         )
         await send(
             {
                 "type": "http.response.body", 
-                "body": httpResponse.toBytes(),
+                "body": httpResponse.responseBody(),
             }
         )
 
 
-route = UvHttpServer.route
+route = HttpServer.route
```

### Comparing `sunyata-0.0.33/sunyata/http/status.py` & `sunyata-0.0.34/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/cache_wrap.py` & `sunyata-0.0.34/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/rpc/serialize.py` & `sunyata-0.0.34/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/rpc/server.py` & `sunyata-0.0.34/sunyata/rpc/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from sunyata.rpc.discovery import DiscoveryConfig, ConsulRpcDiscovery
 import struct
 from sunyata.rpc.compress import RpcCompress
 from types import FunctionType
 from sunyata.rpc.method import RpcMethod
 import asyncio
 import inspect
-from sunyata.http.server import HttpServer
+from sunyata.http.rawserver import HttpServer
 import traceback
 
 class RpcServer(object):
 
     __slots__ = ('discoveryConfig', 'discovery', 'protocal')
 
     funcMap = {}
@@ -160,15 +160,15 @@
         return resp
 
     def serve(self):
         tRegist = None
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         self.printLogo()
-        print(' http rpc running on http://%s:%s' % (self.host, self.port) )
+        print('http rpc running on http://%s:%s' % (self.host, self.port) )
         self.app.serve()
 
 
 class TcpRpcServer(BlockTcpRpcServer):
 
     def __init__(self, host, port):
         BlockTcpRpcServer.__init__(self, host, port)
@@ -295,15 +295,15 @@
             except Exception as ex:
                 print('UDP handler exception:', ex)
     
     def serve(self):
         self.startWorkers()
         self.protocal.transport.bind()
         self.printLogo()
-        print(' udp rpc running on udp://%s:%s' % (self.host, self.port))
+        print('udp rpc running on udp://%s:%s' % (self.host, self.port))
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         while 1:
             try:
                 msg, cliAddr = self.protocal.transport.recv()
                 self.queue.put({'msg' : msg, 'addr' : cliAddr})
             except socket.timeout:
```

### Comparing `sunyata-0.0.33/sunyata/rpc/discovery.py` & `sunyata-0.0.34/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/rpc/transport.py` & `sunyata-0.0.34/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/rpc/client.py` & `sunyata-0.0.34/sunyata/rpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,19 +91,14 @@
         return self.lastServer
 
     @retryTimes(retryTimes=3)
     def call(self, func, *args, **kwargs):
         pass
 
     def __getattr__(self, key):
-        #def remote_attr(*args, **kwargs):
-        #    print(f'{key}方法不存在, 参数为:{args}, {kwargs}')
-        #    return self.call(f'{key}', *args, **kwargs)
-        #def remote_attr(*args, **kwargs):
-        #    return Callable(self, f"{key}")
         if key in dir(self):
             return getattr(self, key)
         return Callable(self, f"{key}")
 
 
 class TcpRpcClient(RpcClient):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sunyata-0.0.33/sunyata/rpc/method.py` & `sunyata-0.0.34/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/rpc/protocal.py` & `sunyata-0.0.34/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/table_writer.py` & `sunyata-0.0.34/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/sunyata/wrap.py` & `sunyata-0.0.34/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/README.md` & `sunyata-0.0.34/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.33/setup.py` & `sunyata-0.0.34/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFINE_VERSION = '0.0.33'
+DEFINE_VERSION = '0.0.34'
 from setuptools import setup
 
 requireList = [
     'lz4',
     'requests',
     'ujson',
     #'PyMySQL==0.10.1',
```

