# Comparing `tmp/sunyata-0.0.30.tar.gz` & `tmp/sunyata-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sunyata-0.0.30.tar", last modified: Wed Apr 12 05:35:53 2023, max compression
+gzip compressed data, was "dist/sunyata-0.0.31.tar", last modified: Wed Apr 12 06:52:49 2023, max compression
```

## Comparing `sunyata-0.0.30.tar` & `sunyata-0.0.31.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/
--rw-r--r--   0 admin      (501) staff       (20)      636 2023-04-12 05:35:53.000000 sunyata-0.0.30/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)      636 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     1357 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)       52 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)       57 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       63 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata.egg-info/dependency_links.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/
--rw-r--r--   0 admin      (501) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/db.py
--rwxr-xr-x   0 admin      (501) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/log.py
--rw-r--r--   0 admin      (501) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/util.py
--rw-r--r--   0 admin      (501) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/orm.py
--rwxr-xr-x   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/eventloop.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/cli/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/cli/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/cli/cli.py
--rw-r--r--   0 admin      (501) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/cli/entry.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/algorithm/
--rw-r--r--   0 admin      (501) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/bloomfilter.py
--rw-r--r--   0 admin      (501) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.30/sunyata/algorithm/binsearchtree.py
--rw-r--r--   0 admin      (501) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.30/sunyata/algorithm/rbtree.py
--rw-r--r--   0 admin      (501) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.30/sunyata/algorithm/avltree.py
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.30/sunyata/algorithm/bplustree.py
--rw-r--r--   0 admin      (501) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.30/sunyata/algorithm/btree.py
--rw-r--r--   0 admin      (501) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.30/sunyata/algorithm/bintree.py
--rw-r--r--   0 admin      (501) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/lru.py
--rw-r--r--   0 admin      (501) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/algorithm/trie.py
--rw-r--r--   0 admin      (501) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/algorithm/hashtable.py
--rw-r--r--   0 admin      (501) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.30/sunyata/algorithm/avlsearchtree.py
--rw-r--r--   0 admin      (501) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/redislock.py
--rw-r--r--   0 admin      (501) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/consul.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/http/
--rw-r--r--   0 admin      (501) staff       (20)     3333 2023-04-12 02:46:43.000000 sunyata-0.0.30/sunyata/http/server.py
--rw-r--r--   0 admin      (501) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.30/sunyata/http/request_stream.py
--rw-r--r--   0 admin      (501) staff       (20)     2375 2023-04-12 01:46:57.000000 sunyata-0.0.30/sunyata/http/transport.py
--rw-r--r--   0 admin      (501) staff       (20)      368 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/http/request.py
--rw-r--r--   0 admin      (501) staff       (20)       68 2023-04-12 02:59:45.000000 sunyata-0.0.30/sunyata/http/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      938 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/http/response.py
--rw-r--r--   0 admin      (501) staff       (20)     3738 2023-04-12 02:47:40.000000 sunyata-0.0.30/sunyata/http/factory.py
--rw-r--r--   0 admin      (501) staff       (20)      256 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/http/router.py
--rw-r--r--   0 admin      (501) staff       (20)      663 2023-04-11 12:55:36.000000 sunyata-0.0.30/sunyata/http/status.py
--rw-r--r--   0 admin      (501) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/cache_wrap.py
--rw-r--r--   0 admin      (501) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/compress.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 05:35:53.000000 sunyata-0.0.30/sunyata/rpc/
--rw-r--r--   0 admin      (501) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/encrypt.py
--rw-r--r--   0 admin      (501) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/rpc/serialize.py
--rw-r--r--   0 admin      (501) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/rpc/exception.py
--rw-r--r--   0 admin      (501) staff       (20)    11596 2023-04-12 02:59:15.000000 sunyata-0.0.30/sunyata/rpc/server.py
--rw-r--r--   0 admin      (501) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/discovery.py
--rw-r--r--   0 admin      (501) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.30/sunyata/rpc/transport.py
--rw-r--r--   0 admin      (501) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/client.py
--rw-r--r--   0 admin      (501) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/compress.py
--rw-r--r--   0 admin      (501) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/method.py
--rw-r--r--   0 admin      (501) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/rpc/protocal.py
--rw-r--r--   0 admin      (501) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/rpc/const.py
--rw-r--r--   0 admin      (501) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.30/sunyata/table_writer.py
--rw-r--r--   0 admin      (501) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.30/sunyata/wrap.py
--rw-r--r--   0 admin      (501) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.30/README.md
--rwxr-xr-x   0 admin      (501) staff       (20)     1110 2023-04-12 03:00:11.000000 sunyata-0.0.30/setup.py
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-12 05:35:53.000000 sunyata-0.0.30/setup.cfg
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 06:52:49.000000 sunyata-0.0.31/
+-rw-r--r--   0 admin      (501) staff       (20)      486 2023-04-12 06:52:49.000000 sunyata-0.0.31/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      486 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1357 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)       52 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)       57 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       63 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata.egg-info/dependency_links.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata/
+-rw-r--r--   0 admin      (501) staff       (20)    13810 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/db.py
+-rwxr-xr-x   0 admin      (501) staff       (20)     3069 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/log.py
+-rw-r--r--   0 admin      (501) staff       (20)      265 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/util.py
+-rw-r--r--   0 admin      (501) staff       (20)     4302 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/orm.py
+-rwxr-xr-x   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      354 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/eventloop.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata/cli/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/cli/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1164 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/cli/cli.py
+-rw-r--r--   0 admin      (501) staff       (20)      140 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/cli/entry.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata/algorithm/
+-rw-r--r--   0 admin      (501) staff       (20)     1083 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/algorithm/bloomfilter.py
+-rw-r--r--   0 admin      (501) staff       (20)      100 2023-03-03 07:53:20.000000 sunyata-0.0.31/sunyata/algorithm/binsearchtree.py
+-rw-r--r--   0 admin      (501) staff       (20)       93 2023-03-03 08:19:20.000000 sunyata-0.0.31/sunyata/algorithm/rbtree.py
+-rw-r--r--   0 admin      (501) staff       (20)       94 2023-03-03 07:53:31.000000 sunyata-0.0.31/sunyata/algorithm/avltree.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/algorithm/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)       90 2023-03-03 07:58:15.000000 sunyata-0.0.31/sunyata/algorithm/bplustree.py
+-rw-r--r--   0 admin      (501) staff       (20)      110 2023-03-03 07:55:58.000000 sunyata-0.0.31/sunyata/algorithm/btree.py
+-rw-r--r--   0 admin      (501) staff       (20)       46 2023-03-03 07:53:11.000000 sunyata-0.0.31/sunyata/algorithm/bintree.py
+-rw-r--r--   0 admin      (501) staff       (20)     3484 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/algorithm/lru.py
+-rw-r--r--   0 admin      (501) staff       (20)     3875 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/algorithm/trie.py
+-rw-r--r--   0 admin      (501) staff       (20)     1466 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/algorithm/hashtable.py
+-rw-r--r--   0 admin      (501) staff       (20)       99 2023-03-03 07:53:38.000000 sunyata-0.0.31/sunyata/algorithm/avlsearchtree.py
+-rw-r--r--   0 admin      (501) staff       (20)     1352 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/redislock.py
+-rw-r--r--   0 admin      (501) staff       (20)     3903 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/consul.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata/http/
+-rw-r--r--   0 admin      (501) staff       (20)     3333 2023-04-12 06:52:01.000000 sunyata-0.0.31/sunyata/http/server.py
+-rw-r--r--   0 admin      (501) staff       (20)      182 2023-04-12 02:31:22.000000 sunyata-0.0.31/sunyata/http/request_stream.py
+-rw-r--r--   0 admin      (501) staff       (20)     2375 2023-04-12 01:46:57.000000 sunyata-0.0.31/sunyata/http/transport.py
+-rw-r--r--   0 admin      (501) staff       (20)      368 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/http/request.py
+-rw-r--r--   0 admin      (501) staff       (20)       68 2023-04-12 02:59:45.000000 sunyata-0.0.31/sunyata/http/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      938 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/http/response.py
+-rw-r--r--   0 admin      (501) staff       (20)     3738 2023-04-12 02:47:40.000000 sunyata-0.0.31/sunyata/http/factory.py
+-rw-r--r--   0 admin      (501) staff       (20)      256 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/http/router.py
+-rw-r--r--   0 admin      (501) staff       (20)      663 2023-04-11 12:55:36.000000 sunyata-0.0.31/sunyata/http/status.py
+-rw-r--r--   0 admin      (501) staff       (20)     1466 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/cache_wrap.py
+-rw-r--r--   0 admin      (501) staff       (20)      505 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/compress.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-04-12 06:52:49.000000 sunyata-0.0.31/sunyata/rpc/
+-rw-r--r--   0 admin      (501) staff       (20)      447 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/rpc/encrypt.py
+-rw-r--r--   0 admin      (501) staff       (20)      699 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/rpc/serialize.py
+-rw-r--r--   0 admin      (501) staff       (20)      100 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/rpc/exception.py
+-rw-r--r--   0 admin      (501) staff       (20)    11596 2023-04-12 02:59:15.000000 sunyata-0.0.31/sunyata/rpc/server.py
+-rw-r--r--   0 admin      (501) staff       (20)     2177 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/rpc/discovery.py
+-rw-r--r--   0 admin      (501) staff       (20)     8307 2023-04-12 02:48:07.000000 sunyata-0.0.31/sunyata/rpc/transport.py
+-rw-r--r--   0 admin      (501) staff       (20)     8370 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/rpc/client.py
+-rw-r--r--   0 admin      (501) staff       (20)       61 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/rpc/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      132 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/rpc/compress.py
+-rw-r--r--   0 admin      (501) staff       (20)     1845 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/rpc/method.py
+-rw-r--r--   0 admin      (501) staff       (20)     2840 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/rpc/protocal.py
+-rw-r--r--   0 admin      (501) staff       (20)       19 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/rpc/const.py
+-rw-r--r--   0 admin      (501) staff       (20)     3129 2023-02-28 12:29:05.000000 sunyata-0.0.31/sunyata/table_writer.py
+-rw-r--r--   0 admin      (501) staff       (20)     2657 2023-03-01 03:10:44.000000 sunyata-0.0.31/sunyata/wrap.py
+-rw-r--r--   0 admin      (501) staff       (20)     9004 2023-03-01 03:14:12.000000 sunyata-0.0.31/README.md
+-rwxr-xr-x   0 admin      (501) staff       (20)      963 2023-04-12 06:52:39.000000 sunyata-0.0.31/setup.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-04-12 06:52:49.000000 sunyata-0.0.31/setup.cfg
```

### Comparing `sunyata-0.0.30/sunyata.egg-info/SOURCES.txt` & `sunyata-0.0.31/sunyata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/db.py` & `sunyata-0.0.31/sunyata/db.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/log.py` & `sunyata-0.0.31/sunyata/log.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/orm.py` & `sunyata-0.0.31/sunyata/orm.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/cli/cli.py` & `sunyata-0.0.31/sunyata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/algorithm/bloomfilter.py` & `sunyata-0.0.31/sunyata/algorithm/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/algorithm/lru.py` & `sunyata-0.0.31/sunyata/algorithm/lru.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/algorithm/trie.py` & `sunyata-0.0.31/sunyata/algorithm/trie.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/algorithm/hashtable.py` & `sunyata-0.0.31/sunyata/algorithm/hashtable.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/redislock.py` & `sunyata-0.0.31/sunyata/redislock.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/consul.py` & `sunyata-0.0.31/sunyata/consul.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/http/server.py` & `sunyata-0.0.31/sunyata/http/server.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/http/transport.py` & `sunyata-0.0.31/sunyata/http/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/http/response.py` & `sunyata-0.0.31/sunyata/http/response.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/http/factory.py` & `sunyata-0.0.31/sunyata/http/factory.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/http/status.py` & `sunyata-0.0.31/sunyata/http/status.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/cache_wrap.py` & `sunyata-0.0.31/sunyata/cache_wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/rpc/serialize.py` & `sunyata-0.0.31/sunyata/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/rpc/server.py` & `sunyata-0.0.31/sunyata/rpc/server.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/rpc/discovery.py` & `sunyata-0.0.31/sunyata/rpc/discovery.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/rpc/transport.py` & `sunyata-0.0.31/sunyata/rpc/transport.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/rpc/client.py` & `sunyata-0.0.31/sunyata/rpc/client.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/rpc/method.py` & `sunyata-0.0.31/sunyata/rpc/method.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/rpc/protocal.py` & `sunyata-0.0.31/sunyata/rpc/protocal.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/table_writer.py` & `sunyata-0.0.31/sunyata/table_writer.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/sunyata/wrap.py` & `sunyata-0.0.31/sunyata/wrap.py`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/README.md` & `sunyata-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `sunyata-0.0.30/setup.py` & `sunyata-0.0.31/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-DEFINE_VERSION = '0.0.30'
+DEFINE_VERSION = '0.0.31'
 from setuptools import setup
 
 requireList = [
     'lz4==3.1.3',
     'requests==2.25.1',
     'PyMySQL==0.10.1',
     'DBUtils==1.3',
@@ -13,17 +13,14 @@
     version=DEFINE_VERSION,
     description='Light, simple, asynchronous RPC framework for Python',
     author='tank',
     license='MIT',
     platforms="any",
     install_requires=requireList,
     classifiers=[
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='sunyata',
```

