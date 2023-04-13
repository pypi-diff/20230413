# Comparing `tmp/recon_lw-2.0.0.dev4665720729.tar.gz` & `tmp/recon_lw-2.0.0.dev4688544420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev4665720729.tar", last modified: Tue Apr 11 08:58:40 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev4688544420.tar", last modified: Thu Apr 13 11:11:09 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev4665720729.tar` & `recon_lw-2.0.0.dev4688544420.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-11 08:58:23.000000 recon_lw-2.0.0.dev4665720729/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    13342 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/recon_lw/recon_ob.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 08:58:40.000000 recon_lw-2.0.0.dev4665720729/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-11 08:57:57.000000 recon_lw-2.0.0.dev4665720729/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-04-13 11:10:50.000000 recon_lw-2.0.0.dev4688544420/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12849 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13351 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/recon_lw/recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 11:11:09.000000 recon_lw-2.0.0.dev4688544420/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-13 11:10:43.000000 recon_lw-2.0.0.dev4688544420/setup.py
```

### Comparing `recon_lw-2.0.0.dev4665720729/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev4688544420/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev4665720729/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev4688544420/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,8 +318,8 @@
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
     order_book["bid_real_qty"] = bid_real_qty
     order_book["bid_impl_qty"] = bid_impl_qty
     order_book["bid_real_n_orders"] = bid_real_n_orders
     order_book["bid_impl_n_orders"] = bid_impl_n_orders
 
-    
+    return {}
```

### Comparing `recon_lw-2.0.0.dev4665720729/setup.py` & `recon_lw-2.0.0.dev4688544420/setup.py`

 * *Files identical despite different names*

