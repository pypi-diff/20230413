# Comparing `tmp/sunyata-0.0.32.tar.gz` & `tmp/sunyata-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.32.tar", last modified: Thu Apr 13 03:22:56 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.33.tar", last modified: Thu Apr 13 05:55:48 2023, max compression
```

## Comparing `sunyata-0.0.32.tar` & `sunyata-0.0.33.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 03:22:56.000000 sunyata-0.0.32/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 03:22:56.000000 sunyata-0.0.32/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1382 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)       52 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       19 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       63 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata/
--rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/db.py
--rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/log.py
--rw-r--r--   0 root         (0) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/util.py
--rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/orm.py
--rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/eventloop.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata/cli/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/cli/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/cli/cli.py
--rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/cli/entry.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata/algorithm/
--rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.32/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.32/sunyata/algorithm/rbtree.py
--rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.32/sunyata/algorithm/avltree.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/algorithm/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.32/sunyata/algorithm/bplustree.py
--rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.32/sunyata/algorithm/btree.py
--rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.32/sunyata/algorithm/bintree.py
--rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/algorithm/lru.py
--rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/algorithm/trie.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/algorithm/hashtable.py
--rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.32/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/redislock.py
--rw-r--r--   0 root         (0) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/consul.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata/http/
--rw-r--r--   0 root         (0) staff       (20)     2751 2023-04-13 03:14:27.000000 sunyata-0.0.32/sunyata/http/server.py
--rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.32/sunyata/http/request_stream.py
--rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.32/sunyata/http/transport.py
--rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.32/sunyata/http/request.py
--rw-r--r--   0 root         (0) staff       (20)       68 2023-04-12 02:59:45.000000 sunyata-0.0.32/sunyata/http/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      892 2023-04-13 03:14:18.000000 sunyata-0.0.32/sunyata/http/response.py
--rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.32/sunyata/http/factory.py
--rw-r--r--   0 root         (0) staff       (20)     3001 2023-04-13 03:15:16.000000 sunyata-0.0.32/sunyata/http/uvserver.py
--rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.32/sunyata/http/router.py
--rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.32/sunyata/http/status.py
--rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/cache_wrap.py
--rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/compress.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 03:22:56.000000 sunyata-0.0.32/sunyata/rpc/
--rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/rpc/encrypt.py
--rw-r--r--   0 root         (0) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/rpc/serialize.py
--rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/rpc/exception.py
--rw-r--r--   0 root         (0) staff       (20)    11596 2023-04-12 02:59:15.000000 sunyata-0.0.32/sunyata/rpc/server.py
--rw-r--r--   0 root         (0) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/rpc/discovery.py
--rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.32/sunyata/rpc/transport.py
--rw-r--r--   0 root         (0) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/rpc/client.py
--rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/rpc/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/rpc/compress.py
--rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/rpc/method.py
--rw-r--r--   0 root         (0) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/rpc/protocal.py
--rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/rpc/const.py
--rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.32/sunyata/table_writer.py
--rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.32/sunyata/wrap.py
--rw-r--r--   0 root         (0) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.32/README.md
--rwxr-xr-x   0 root         (0) staff       (20)      963 2023-04-13 03:22:51.000000 sunyata-0.0.32/setup.py
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-13 03:22:56.000000 sunyata-0.0.32/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 05:55:48.000000 sunyata-0.0.33/PKG-INFO
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      486 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1382 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)       52 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       63 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-04-13 05:55:47.000000 sunyata-0.0.33/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/
+-rw-r--r--   0 root         (0) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/db.py
+-rwxr-xr-x   0 root         (0) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/log.py
+-rw-r--r--   0 root         (0) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/util.py
+-rw-r--r--   0 root         (0) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/orm.py
+-rwxr-xr-x   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/eventloop.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/cli/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/cli/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/cli/cli.py
+-rw-r--r--   0 root         (0) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/cli/entry.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/algorithm/
+-rw-r--r--   0 root         (0) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.33/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.33/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 root         (0) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.33/sunyata/algorithm/avltree.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.33/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 root         (0) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.33/sunyata/algorithm/btree.py
+-rw-r--r--   0 root         (0) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.33/sunyata/algorithm/bintree.py
+-rw-r--r--   0 root         (0) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/lru.py
+-rw-r--r--   0 root         (0) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/algorithm/trie.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 root         (0) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.33/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 root         (0) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/redislock.py
+-rw-r--r--   0 root         (0) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/consul.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/http/
+-rw-r--r--   0 root         (0) staff       (20)     2823 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/http/server.py
+-rw-r--r--   0 root         (0) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.33/sunyata/http/request_stream.py
+-rw-r--r--   0 root         (0) staff       (20)     2375 2023-04-13 03:14:33.000000 sunyata-0.0.33/sunyata/http/transport.py
+-rw-r--r--   0 root         (0) staff       (20)      538 2023-04-13 02:26:49.000000 sunyata-0.0.33/sunyata/http/request.py
+-rw-r--r--   0 root         (0) staff       (20)       68 2023-04-12 02:59:45.000000 sunyata-0.0.33/sunyata/http/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      892 2023-04-13 03:14:18.000000 sunyata-0.0.33/sunyata/http/response.py
+-rw-r--r--   0 root         (0) staff       (20)     2817 2023-04-13 03:13:06.000000 sunyata-0.0.33/sunyata/http/factory.py
+-rw-r--r--   0 root         (0) staff       (20)     3094 2023-04-13 05:54:25.000000 sunyata-0.0.33/sunyata/http/uvserver.py
+-rw-r--r--   0 root         (0) staff       (20)      255 2023-04-13 03:14:24.000000 sunyata-0.0.33/sunyata/http/router.py
+-rw-r--r--   0 root         (0) staff       (20)      663 2023-04-13 03:14:30.000000 sunyata-0.0.33/sunyata/http/status.py
+-rw-r--r--   0 root         (0) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/cache_wrap.py
+-rw-r--r--   0 root         (0) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/compress.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-13 05:55:48.000000 sunyata-0.0.33/sunyata/rpc/
+-rw-r--r--   0 root         (0) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/encrypt.py
+-rw-r--r--   0 root         (0) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/rpc/serialize.py
+-rw-r--r--   0 root         (0) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/rpc/exception.py
+-rw-r--r--   0 root         (0) staff       (20)    11621 2023-04-13 05:52:50.000000 sunyata-0.0.33/sunyata/rpc/server.py
+-rw-r--r--   0 root         (0) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/discovery.py
+-rw-r--r--   0 root         (0) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.33/sunyata/rpc/transport.py
+-rw-r--r--   0 root         (0) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/client.py
+-rw-r--r--   0 root         (0) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/compress.py
+-rw-r--r--   0 root         (0) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/method.py
+-rw-r--r--   0 root         (0) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/rpc/protocal.py
+-rw-r--r--   0 root         (0) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/rpc/const.py
+-rw-r--r--   0 root         (0) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.33/sunyata/table_writer.py
+-rw-r--r--   0 root         (0) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.33/sunyata/wrap.py
+-rw-r--r--   0 root         (0) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.33/README.md
+-rwxr-xr-x   0 root         (0) staff       (20)      962 2023-04-13 05:50:20.000000 sunyata-0.0.33/setup.py
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-04-13 05:55:48.000000 sunyata-0.0.33/setup.cfg
```

### Comparing `sunyata-0.0.32/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.33/sunyata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/db.py` & `sunyata-0.0.33/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/log.py` & `sunyata-0.0.33/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/orm.py` & `sunyata-0.0.33/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/cli/cli.py` & `sunyata-0.0.33/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.33/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/algorithm/lru.py` & `sunyata-0.0.33/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/algorithm/trie.py` & `sunyata-0.0.33/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/algorithm/hashtable.py` & `sunyata-0.0.33/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/redislock.py` & `sunyata-0.0.33/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/consul.py` & `sunyata-0.0.33/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/http/server.py` & `sunyata-0.0.33/sunyata/http/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         tasklist = []
         server = await asyncio.start_server(self.acceptStream, self.bind, self.port)
         tasklist.append(server.serve_forever())
         for task in tasklist:
             await task
 
     def serve(self):
+        print('http running on http://%s:%s' % (self.bind, self.port) )
         asyncio.run(self.listenAndServe())
 
     @classmethod
     def route(cls, path, methods = None):
         def wrapper(func):
             cls.addRoute(path, func, methods)
             return func
```

### Comparing `sunyata-0.0.32/sunyata/http/transport.py` & `sunyata-0.0.33/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/http/request.py` & `sunyata-0.0.33/sunyata/http/request.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/http/response.py` & `sunyata-0.0.33/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/http/factory.py` & `sunyata-0.0.33/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/http/uvserver.py` & `sunyata-0.0.33/sunyata/http/uvserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 import traceback
 
 
 class UvHttpServer(HttpServer):
 
     routerMap = {}
 
-    def __init__(self, bind = '0.0.0.0', port=9989):
+    def __init__(self, bind = '0.0.0.0', port=9989, log_level='error'):
         HttpServer.__init__(self, bind=bind, port=port)
-        self.config = uvicorn.Config("sunyata.http.uvserver:UvHttpServer", host=self.bind, port=self.port, log_level="debug")
+        self.config = uvicorn.Config("sunyata.http.uvserver:UvHttpServer", host=self.bind, port=self.port, log_level=log_level)
 
     def serve(self):
         server = uvicorn.Server(self.config)
+        print('http running on http://%s:%s' % (self.bind, self.port) )
         server.run()
     
     async def genHttpRequest(self, scheme, httpVersion, method, path, queryString, headers, body, clientTuple):
         httpRequest = HttpRequest()
         httpRequest.scheme = scheme
         httpRequest.httpVersion = httpVersion
         httpRequest.method = method
```

### Comparing `sunyata-0.0.32/sunyata/http/status.py` & `sunyata-0.0.33/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/cache_wrap.py` & `sunyata-0.0.33/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/rpc/serialize.py` & `sunyata-0.0.33/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/rpc/server.py` & `sunyata-0.0.33/sunyata/rpc/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         return resp
 
     def serve(self):
         tRegist = None
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         self.printLogo()
-        print(' HTTP rpc serving on %s:%s' % (self.host, self.port) )
+        print(' http rpc running on http://%s:%s' % (self.host, self.port) )
         self.app.serve()
 
 
 class TcpRpcServer(BlockTcpRpcServer):
 
     def __init__(self, host, port):
         BlockTcpRpcServer.__init__(self, host, port)
@@ -215,15 +215,15 @@
                 writer.close()
                 return
 
     async def main(self):
         loop = asyncio.get_event_loop()
         coro = asyncio.start_server(self.handle, self.host, self.port, loop=loop)
         server = loop.run_until_complete(coro)
-        print('TCP rpc serving on %s:%s' % (self.host, self.port))
+        print('tcp rpc running on tcp://%s:%s' % (self.host, self.port))
         try:
             loop.run_forever()
         except KeyboardInterrupt:
             pass
         # Close the server
         server.close()
         loop.run_until_complete(server.wait_closed())
@@ -250,15 +250,15 @@
         if self.discovery and self.discoveryConfig:
             tRegist = self.discovery.asyncRegist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
             tasks.append(tRegist)
         coro = asyncio.start_server(self.handle, self.host, self.port, loop=loop)
         tasks.append(coro)
         rs = loop.run_until_complete(asyncio.gather(*tasks))
         self.printLogo()
-        print('TCP rpc serving on %s:%s' % (self.host, self.port) )
+        print('tcp rpc running on tcp://%s:%s' % (self.host, self.port) )
         try:
             loop.run_forever()
         except KeyboardInterrupt:
             pass
         server = rs[-1]
         # Close the server
         server.close()
@@ -295,15 +295,15 @@
             except Exception as ex:
                 print('UDP handler exception:', ex)
     
     def serve(self):
         self.startWorkers()
         self.protocal.transport.bind()
         self.printLogo()
-        print(' UDP rpc serving on %s:%s' % (self.host, self.port))
+        print(' udp rpc running on udp://%s:%s' % (self.host, self.port))
         if self.discovery and self.discoveryConfig:
             self.discovery.regist(self.discoveryConfig.serviceName, self.discoveryConfig.serviceHost, self.discoveryConfig.servicePort, ttlHeartBeat=True)
         while 1:
             try:
                 msg, cliAddr = self.protocal.transport.recv()
                 self.queue.put({'msg' : msg, 'addr' : cliAddr})
             except socket.timeout:
```

### Comparing `sunyata-0.0.32/sunyata/rpc/discovery.py` & `sunyata-0.0.33/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/rpc/transport.py` & `sunyata-0.0.33/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/rpc/client.py` & `sunyata-0.0.33/sunyata/rpc/client.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/rpc/method.py` & `sunyata-0.0.33/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/rpc/protocal.py` & `sunyata-0.0.33/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/table_writer.py` & `sunyata-0.0.33/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/sunyata/wrap.py` & `sunyata-0.0.33/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/README.md` & `sunyata-0.0.33/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.32/setup.py` & `sunyata-0.0.33/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFINE_VERSION = '0.0.32'
+DEFINE_VERSION = '0.0.33'
 from setuptools import setup
 
 requireList = [
     'lz4',
     'requests',
     'ujson',
     #'PyMySQL==0.10.1',
@@ -34,8 +34,8 @@
     ],
     include_package_data=True,
     entry_points = {
         'console_scripts' : [
             'sunyata=sunyata.cli.entry:main'
         ]
     }
-)
+)
```

