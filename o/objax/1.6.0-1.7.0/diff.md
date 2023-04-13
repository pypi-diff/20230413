# Comparing `tmp/objax-1.6.0.tar.gz` & `tmp/objax-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objax-1.6.0.tar", last modified: Mon Jan 31 23:16:51 2022, max compression
+gzip compressed data, was "objax-1.7.0.tar", last modified: Sun Apr  9 04:21:27 2023, max compression
```

## Comparing `objax-1.6.0.tar` & `objax-1.7.0.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.116581 objax-1.6.0/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)    11358 2022-01-05 23:01:33.000000 objax-1.6.0/LICENSE
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)       25 2022-01-05 23:01:33.000000 objax-1.6.0/MANIFEST.in
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     3897 2022-01-31 23:16:51.116581 objax-1.6.0/PKG-INFO
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     3072 2022-01-05 23:01:33.000000 objax-1.6.0/README.md
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.108581 objax-1.6.0/objax/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1016 2022-01-05 23:01:33.000000 objax-1.6.0/objax/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1394 2022-01-05 23:01:33.000000 objax-1.6.0/objax/_patch_jax.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      598 2022-01-31 23:13:39.000000 objax-1.6.0/objax/_version.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1135 2022-01-05 23:01:33.000000 objax-1.6.0/objax/constants.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.112581 objax-1.6.0/objax/functional/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      663 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/__init__.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.112581 objax-1.6.0/objax/functional/core/
--rwxr-xr-x   0 kurakin  (189798) primarygroup (89939)      644 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/core/__init__.py
--rwxr-xr-x   0 kurakin  (189798) primarygroup (89939)     1433 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/core/activation.py
--rwxr-xr-x   0 kurakin  (189798) primarygroup (89939)     4671 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/core/ops.py
--rwxr-xr-x   0 kurakin  (189798) primarygroup (89939)     5299 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/core/pooling.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      852 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/divergence.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     5665 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/loss.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1493 2022-01-05 23:01:33.000000 objax-1.6.0/objax/functional/parallel.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     5246 2022-01-05 23:01:33.000000 objax-1.6.0/objax/gradient.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.112581 objax-1.6.0/objax/io/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      621 2022-01-05 23:01:33.000000 objax-1.6.0/objax/io/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     4997 2022-01-05 23:01:33.000000 objax-1.6.0/objax/io/checkpoint.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     4451 2022-01-05 23:01:33.000000 objax-1.6.0/objax/io/ops.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     4637 2022-01-05 23:01:33.000000 objax-1.6.0/objax/jaxboard.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)    17078 2022-01-05 23:01:33.000000 objax-1.6.0/objax/module.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.112581 objax-1.6.0/objax/nn/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      617 2022-01-05 23:01:33.000000 objax-1.6.0/objax/nn/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     8244 2022-01-05 23:01:33.000000 objax-1.6.0/objax/nn/init.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)    26039 2022-01-07 22:29:41.000000 objax-1.6.0/objax/nn/layers.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.112581 objax-1.6.0/objax/optimizer/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      701 2022-01-05 23:01:33.000000 objax-1.6.0/objax/optimizer/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2898 2022-01-05 23:01:33.000000 objax-1.6.0/objax/optimizer/adam.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     5027 2022-01-05 23:01:33.000000 objax-1.6.0/objax/optimizer/ema.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2914 2022-01-05 23:01:33.000000 objax-1.6.0/objax/optimizer/lars.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2439 2022-01-05 23:01:33.000000 objax-1.6.0/objax/optimizer/momentum.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     3624 2022-01-05 23:01:33.000000 objax-1.6.0/objax/optimizer/scheduler.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1578 2022-01-05 23:01:33.000000 objax-1.6.0/objax/optimizer/sgd.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.112581 objax-1.6.0/objax/privacy/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      596 2022-01-05 23:01:33.000000 objax-1.6.0/objax/privacy/__init__.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.116581 objax-1.6.0/objax/privacy/dpsgd/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      633 2022-01-05 23:01:33.000000 objax-1.6.0/objax/privacy/dpsgd/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     8283 2022-01-05 23:01:33.000000 objax-1.6.0/objax/privacy/dpsgd/gradient.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)    22737 2022-01-31 23:11:50.000000 objax-1.6.0/objax/privacy/dpsgd/privacyaccountant.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.116581 objax-1.6.0/objax/random/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      598 2022-01-05 23:01:33.000000 objax-1.6.0/objax/random/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     4124 2022-01-05 23:01:33.000000 objax-1.6.0/objax/random/random.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1218 2022-01-05 23:01:33.000000 objax-1.6.0/objax/typing.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.116581 objax-1.6.0/objax/util/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      707 2022-01-05 23:01:33.000000 objax-1.6.0/objax/util/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2313 2022-01-05 23:01:33.000000 objax-1.6.0/objax/util/check.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     3050 2022-01-05 23:01:33.000000 objax-1.6.0/objax/util/image.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2581 2022-01-06 00:34:57.000000 objax-1.6.0/objax/util/objax2tf.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     6973 2022-01-05 23:01:33.000000 objax-1.6.0/objax/util/tracing.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     8335 2022-01-05 23:01:33.000000 objax-1.6.0/objax/util/util.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)    18012 2022-01-06 18:39:56.000000 objax-1.6.0/objax/variable.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.116581 objax-1.6.0/objax/zoo/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)      575 2022-01-05 23:01:33.000000 objax-1.6.0/objax/zoo/__init__.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2030 2022-01-06 18:39:56.000000 objax-1.6.0/objax/zoo/convnet.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1222 2022-01-05 23:01:33.000000 objax-1.6.0/objax/zoo/dnnet.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)    20090 2022-01-05 23:01:33.000000 objax-1.6.0/objax/zoo/resnet_v2.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2913 2022-01-05 23:01:33.000000 objax-1.6.0/objax/zoo/rnn.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     6021 2022-01-05 23:01:33.000000 objax-1.6.0/objax/zoo/vgg.py
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     5255 2022-01-05 23:01:33.000000 objax-1.6.0/objax/zoo/wide_resnet.py
-drwxr-xr-x   0 kurakin  (189798) primarygroup (89939)        0 2022-01-31 23:16:51.108581 objax-1.6.0/objax.egg-info/
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     3897 2022-01-31 23:16:50.000000 objax-1.6.0/objax.egg-info/PKG-INFO
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     1352 2022-01-31 23:16:50.000000 objax-1.6.0/objax.egg-info/SOURCES.txt
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)        1 2022-01-31 23:16:50.000000 objax-1.6.0/objax.egg-info/dependency_links.txt
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)       79 2022-01-31 23:16:50.000000 objax-1.6.0/objax.egg-info/requires.txt
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)        6 2022-01-31 23:16:50.000000 objax-1.6.0/objax.egg-info/top_level.txt
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)       79 2022-01-05 23:01:33.000000 objax-1.6.0/requirements.txt
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)       38 2022-01-31 23:16:51.116581 objax-1.6.0/setup.cfg
--rw-r--r--   0 kurakin  (189798) primarygroup (89939)     2079 2022-01-05 23:01:33.000000 objax-1.6.0/setup.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.479338 objax-1.7.0/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)    11358 2023-04-08 00:40:41.000000 objax-1.7.0/LICENSE
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)       25 2023-04-08 00:40:41.000000 objax-1.7.0/MANIFEST.in
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     3954 2023-04-09 04:21:27.479338 objax-1.7.0/PKG-INFO
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     3216 2023-04-08 00:40:41.000000 objax-1.7.0/README.md
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.471337 objax-1.7.0/objax/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1016 2023-04-08 00:40:41.000000 objax-1.7.0/objax/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1394 2023-04-08 00:40:41.000000 objax-1.7.0/objax/_patch_jax.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      598 2023-04-09 04:18:26.000000 objax-1.7.0/objax/_version.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1135 2023-04-08 00:40:41.000000 objax-1.7.0/objax/constants.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax/functional/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      663 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/__init__.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax/functional/core/
+-rwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)      644 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/core/__init__.py
+-rwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)     1433 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/core/activation.py
+-rwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)     4671 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/core/ops.py
+-rwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)     5299 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/core/pooling.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      852 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/divergence.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     5665 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/loss.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1369 2023-04-08 00:40:41.000000 objax-1.7.0/objax/functional/parallel.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     8816 2023-04-08 00:40:41.000000 objax-1.7.0/objax/gradient.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax/io/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      621 2023-04-08 00:40:41.000000 objax-1.7.0/objax/io/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     4997 2023-04-08 00:40:41.000000 objax-1.7.0/objax/io/checkpoint.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     4526 2023-04-08 00:40:41.000000 objax-1.7.0/objax/io/ops.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     4637 2023-04-08 00:40:41.000000 objax-1.7.0/objax/jaxboard.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)    16998 2023-04-08 00:40:41.000000 objax-1.7.0/objax/module.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax/nn/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      617 2023-04-08 00:40:41.000000 objax-1.7.0/objax/nn/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     8244 2023-04-08 00:40:41.000000 objax-1.7.0/objax/nn/init.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)    26039 2023-04-08 00:40:41.000000 objax-1.7.0/objax/nn/layers.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax/optimizer/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      701 2023-04-08 00:40:41.000000 objax-1.7.0/objax/optimizer/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2898 2023-04-08 00:40:41.000000 objax-1.7.0/objax/optimizer/adam.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     5027 2023-04-08 00:40:41.000000 objax-1.7.0/objax/optimizer/ema.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2914 2023-04-08 00:40:41.000000 objax-1.7.0/objax/optimizer/lars.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2439 2023-04-08 00:40:41.000000 objax-1.7.0/objax/optimizer/momentum.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     3624 2023-04-08 00:40:41.000000 objax-1.7.0/objax/optimizer/scheduler.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1578 2023-04-08 00:40:41.000000 objax-1.7.0/objax/optimizer/sgd.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax/privacy/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      596 2023-04-08 00:40:41.000000 objax-1.7.0/objax/privacy/__init__.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax/privacy/dpsgd/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      633 2023-04-08 00:40:41.000000 objax-1.7.0/objax/privacy/dpsgd/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     8303 2023-04-08 00:40:41.000000 objax-1.7.0/objax/privacy/dpsgd/gradient.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)    22737 2023-04-08 00:40:41.000000 objax-1.7.0/objax/privacy/dpsgd/privacyaccountant.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.479338 objax-1.7.0/objax/random/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      598 2023-04-08 00:40:41.000000 objax-1.7.0/objax/random/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     4124 2023-04-08 00:40:41.000000 objax-1.7.0/objax/random/random.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1132 2023-04-08 00:40:41.000000 objax-1.7.0/objax/typing.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.479338 objax-1.7.0/objax/util/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      707 2023-04-08 00:40:41.000000 objax-1.7.0/objax/util/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2341 2023-04-08 00:40:41.000000 objax-1.7.0/objax/util/check.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     3050 2023-04-08 00:40:41.000000 objax-1.7.0/objax/util/image.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2581 2023-04-08 00:40:41.000000 objax-1.7.0/objax/util/objax2tf.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     6973 2023-04-08 00:40:41.000000 objax-1.7.0/objax/util/tracing.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     8274 2023-04-08 00:40:41.000000 objax-1.7.0/objax/util/util.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)    18012 2023-04-08 00:40:41.000000 objax-1.7.0/objax/variable.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.479338 objax-1.7.0/objax/zoo/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)      575 2023-04-08 00:40:41.000000 objax-1.7.0/objax/zoo/__init__.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2030 2023-04-08 00:40:41.000000 objax-1.7.0/objax/zoo/convnet.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1222 2023-04-08 00:40:41.000000 objax-1.7.0/objax/zoo/dnnet.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)    20090 2023-04-08 00:40:41.000000 objax-1.7.0/objax/zoo/resnet_v2.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2913 2023-04-08 00:40:41.000000 objax-1.7.0/objax/zoo/rnn.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     6021 2023-04-08 00:40:41.000000 objax-1.7.0/objax/zoo/vgg.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     5255 2023-04-08 00:40:41.000000 objax-1.7.0/objax/zoo/wide_resnet.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.475337 objax-1.7.0/objax.egg-info/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     3954 2023-04-09 04:21:27.000000 objax-1.7.0/objax.egg-info/PKG-INFO
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     1388 2023-04-09 04:21:27.000000 objax-1.7.0/objax.egg-info/SOURCES.txt
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)        1 2023-04-09 04:21:27.000000 objax-1.7.0/objax.egg-info/dependency_links.txt
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)       79 2023-04-09 04:21:27.000000 objax-1.7.0/objax.egg-info/requires.txt
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)        6 2023-04-09 04:21:27.000000 objax-1.7.0/objax.egg-info/top_level.txt
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)       79 2023-04-08 00:40:41.000000 objax-1.7.0/requirements.txt
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)       38 2023-04-09 04:21:27.479338 objax-1.7.0/setup.cfg
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     2030 2023-04-08 00:40:41.000000 objax-1.7.0/setup.py
+drwxrwxr-x   0 shuangsong  (1001) shuangsong  (1002)        0 2023-04-09 04:21:27.479338 objax-1.7.0/tests/
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     6121 2023-04-08 00:40:41.000000 objax-1.7.0/tests/testio.py
+-rw-rw-r--   0 shuangsong  (1001) shuangsong  (1002)     5786 2023-04-08 00:40:41.000000 objax-1.7.0/tests/testrandom.py
```

### Comparing `objax-1.6.0/LICENSE` & `objax-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/PKG-INFO` & `objax-1.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: objax
-Version: 1.6.0
+Version: 1.7.0
 Summary: Objax is a machine learning framework that provides an Object Oriented layer for JAX.
 Home-page: https://github.com/google/objax
 Author: Objax team
 Author-email: objax-dev@google.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,22 +46,26 @@
 You install Objax using `pip` as follows:
 
 ```bash
 pip install --upgrade objax
 ```
 
 Objax supports GPUs but assumes that you already have some version of CUDA
-installed. Here are the extra steps:
+installed. Here are the extra steps required to install CUDA-enabled jaxlib
+(jaxlib releases require CUDA 11.2 or newer):
 
 ```bash
-# Update accordingly to your installed CUDA version
-CUDA_VERSION=11.0
-pip install -f https://storage.googleapis.com/jax-releases/jax_releases.html jaxlib==`python3 -c 'import jaxlib; print(jaxlib.__version__)'`+cuda`echo $CUDA_VERSION | sed s:\\\.::g`
+RELEASE_URL="https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
+JAX_VERSION=`python3 -c 'import jax; print(jax.__version__)'`
+pip uninstall -y jaxlib
+pip install -f $RELEASE_URL jax[cuda]==$JAX_VERSION
 ```
 
+For more installation options, see https://github.com/google/jax#pip-installation-gpu-cuda
+
 ### Useful environment configurations
 
 Here are a few useful options:
 
 ```bash
 # Prevent JAX from taking the whole GPU memory
 # (useful if you want to run several programs on a single GPU)
@@ -117,9 +118,7 @@
 ```
 
 ## Developer documentation
 
 Here is information about
 [development setup](https://objax.readthedocs.io/en/latest/dev/setup.html)
 and a [guide on adding new code](https://objax.readthedocs.io/en/latest/dev/adding_module.html).
-
-
```

### Comparing `objax-1.6.0/README.md` & `objax-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,26 @@
 You install Objax using `pip` as follows:
 
 ```bash
 pip install --upgrade objax
 ```
 
 Objax supports GPUs but assumes that you already have some version of CUDA
-installed. Here are the extra steps:
+installed. Here are the extra steps required to install CUDA-enabled jaxlib
+(jaxlib releases require CUDA 11.2 or newer):
 
 ```bash
-# Update accordingly to your installed CUDA version
-CUDA_VERSION=11.0
-pip install -f https://storage.googleapis.com/jax-releases/jax_releases.html jaxlib==`python3 -c 'import jaxlib; print(jaxlib.__version__)'`+cuda`echo $CUDA_VERSION | sed s:\\\.::g`
+RELEASE_URL="https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
+JAX_VERSION=`python3 -c 'import jax; print(jax.__version__)'`
+pip uninstall -y jaxlib
+pip install -f $RELEASE_URL jax[cuda]==$JAX_VERSION
 ```
 
+For more installation options, see https://github.com/google/jax#pip-installation-gpu-cuda
+
 ### Useful environment configurations
 
 Here are a few useful options:
 
 ```bash
 # Prevent JAX from taking the whole GPU memory
 # (useful if you want to run several programs on a single GPU)
```

### Comparing `objax-1.6.0/objax/__init__.py` & `objax-1.7.0/objax/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/_patch_jax.py` & `objax-1.7.0/objax/_patch_jax.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/_version.py` & `objax-1.7.0/objax/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = '1.6.0'
+__version__ = '1.7.0'
```

### Comparing `objax-1.6.0/objax/constants.py` & `objax-1.7.0/objax/constants.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/functional/__init__.py` & `objax-1.7.0/objax/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/functional/core/__init__.py` & `objax-1.7.0/objax/functional/core/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/functional/core/activation.py` & `objax-1.7.0/objax/functional/core/activation.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/functional/core/ops.py` & `objax-1.7.0/objax/functional/core/ops.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/functional/core/pooling.py` & `objax-1.7.0/objax/functional/core/pooling.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/functional/divergence.py` & `objax-1.7.0/objax/functional/divergence.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/functional/loss.py` & `objax-1.7.0/objax/functional/loss.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/gradient.py` & `objax-1.7.0/objax/io/checkpoint.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,114 +8,109 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__all__ = ['Grad', 'GradValues']
+__all__ = ['Checkpoint']
 
-import inspect
-from typing import List, Optional, Callable, Tuple, Dict, Union
+import glob
+import os
+from typing import Callable, Optional
 
-import jax
+from objax.io.ops import load_var_collection, save_var_collection
+from objax.typing import FileOrStr
+from objax.variable import VarCollection
 
-from objax.module import Function, Module
-from objax.typing import JaxArray
-from objax.util import repr_function, class_name
-from objax.variable import BaseState, TrainVar, VarCollection
 
+class Checkpoint:
+    """Helper class which performs saving and restoring of the variables.
 
-class GradValues(Module):
-    """The GradValues module is used to compute the gradients of a function."""
+    Variables are stored in the checkpoint files. One checkpoint file stores a single snapshot of the variables.
+    Different checkpoint files store different snapshots of the variables (for example at different training step).
+    Each checkpoint has associated index, which is used to identify time when snapshot of the variables was made.
+    Typically training step or training epoch are used as an index.
+    """
 
-    def __init__(self, f: Union[Module, Callable],
-                 variables: Optional[VarCollection],
-                 input_argnums: Optional[Tuple[int, ...]] = None):
-        """Constructs an instance to compute the gradient of f w.r.t. variables.
+    DIR_NAME: str = 'ckpt'
+    """Name of the subdirectory of model directory where checkpoints will be saved."""
+
+    FILE_MATCH: str = '*.npz'
+    """File pattern which is used to search for checkpoint files."""
+
+    FILE_FORMAT: str = '%010d.npz'
+    """Format of the filename of one checkpoint file."""
+
+    LOAD_FN: Callable[[FileOrStr, VarCollection], None] = staticmethod(load_var_collection)
+    """Load function, which loads variables collection from given file."""
+
+    SAVE_FN: Callable[[FileOrStr, VarCollection], None] = staticmethod(save_var_collection)
+    """Save function, which saves variables collection into given file."""
+
+    def __init__(self, logdir: str, keep_ckpts: int, makedir: bool = True, verbose: bool = True):
+        """Creates instance of the Checkpoint class.
 
         Args:
-            f: the function for which to compute gradients.
-            variables: the variables for which to compute gradients.
-            input_argnums: input indexes, if any, on which to compute gradients.
+            logdir: model directory. Checkpoints will be saved in the subdirectory of model directory.
+            keep_ckpts: maximum number of checkpoints to keep.
+            makedir: if True then directory for checkpoints will be created,
+                otherwise it's expected that directory already exists.
+            verbose: if True then print when data is restored from checkpoint.
         """
-        self.f = f
-        self.vc = variables = VarCollection(variables or ())
-        if not isinstance(f, Module):
-            f = Function(f, self.vc)
-
-        def f_func(inputs_and_train_tensors: List[JaxArray],
-                   state_tensors: List[JaxArray],
-                   list_args: List,
-                   kwargs: Dict):
-            inputs = inputs_and_train_tensors[:len(self.input_argnums)]
-            train_tensors = inputs_and_train_tensors[len(self.input_argnums):]
-            original_vc = self.vc.tensors()
-            try:
-                self.vc.subset(TrainVar).assign(train_tensors)
-                self.vc.subset(BaseState).assign(state_tensors)
-                for i, arg in zip(self.input_argnums, inputs):
-                    list_args[i] = arg
-                outputs = f(*list_args, **kwargs)
-                if not isinstance(outputs, (list, tuple)):
-                    outputs = [outputs]
-                return outputs[0], (outputs, variables.tensors())
-            finally:
-                self.vc.assign(original_vc)
-
-        assert isinstance(input_argnums, tuple) or input_argnums is None, \
-            f'Must pass a tuple of indices to input_argnums; received {input_argnums}.'
-        self.input_argnums = input_argnums or tuple()
-
-        signature = inspect.signature(f)
-        self.__wrapped__ = f
-        self.__signature__ = signature.replace(return_annotation=Tuple[List[JaxArray],
-                                                                       signature.return_annotation])
-        self._call = jax.grad(f_func, has_aux=True)
+        self.logdir = logdir
+        self.keep_ckpts = keep_ckpts
+        self.verbose = verbose
+        if makedir:
+            os.makedirs(os.path.join(logdir, self.DIR_NAME), exist_ok=True)
+
+    @staticmethod
+    def checkpoint_idx(filename: str):
+        """Returns index of checkpoint from given checkpoint filename.
 
-    def __call__(self, *args, **kwargs):
-        """Returns the computed gradients for the first value returned by `f` and the values returned by `f`.
+        Args:
+            filename: checkpoint filename.
 
         Returns:
-            A tuple (gradients , values of f]), where gradients is a list containing
-                the input gradients, if any, followed by the variable gradients."""
-        inputs = [args[i] for i in self.input_argnums]
-        g, (outputs, changes) = self._call(inputs + self.vc.subset(TrainVar).tensors(),
-                                           self.vc.subset(BaseState).tensors(),
-                                           list(args), kwargs)
-        self.vc.assign(changes)
-        return g, outputs
-
-    def vars(self, scope: str = '') -> VarCollection:
-        """Return the VarCollection of the variables used."""
-        if scope:
-            return VarCollection((scope + k, v) for k, v in self.vc.items())
-        return VarCollection(self.vc)
-
-    def __repr__(self):
-        f = repr(self.f) if isinstance(self.f, Module) else repr_function(self.f)
-        return f'{class_name(self)}(f={f}, input_argnums={self.input_argnums or None})'
-
-
-class Grad(GradValues):
-    """The Grad module is used to compute the gradients of a function."""
-
-    def __init__(self, f: Callable,
-                 variables: Optional[VarCollection],
-                 input_argnums: Optional[Tuple[int, ...]] = None):
-        """Constructs an instance to compute the gradient of f w.r.t. variables.
+            checkpoint index.
+        """
+        return int(os.path.basename(filename).split('.')[0])
+
+    def restore(self, vc: VarCollection, idx: Optional[int] = None):
+        """Restores values of all variables of given variables collection from the checkpoint.
+
+        Old values from the variables collection will be replaced with the new values read from checkpoint.
+        If variable does not exist in the variables collection, it won't be restored from checkpoint.
 
         Args:
-            f: the function for which to compute gradients.
-            variables: the variables for which to compute gradients.
-            input_argnums: input indexes, if any, on which to compute gradients.
+            vc: variables collection to restore.
+            idx: if provided then checkpoint index to use, if None then latest checkpoint will be restored.
+
+        Returns:
+            idx: index of the restored checkpoint.
+            ckpt: full path to the restored checkpoint.
         """
-        super().__init__(f, variables, input_argnums)
-        signature = inspect.signature(self.__wrapped__)
-        self.__signature__ = signature.replace(return_annotation=List[JaxArray])
+        assert isinstance(vc, VarCollection), f'Must pass a VarCollection to restore; received type {type(vc)}.'
+        if idx is None:
+            all_ckpts = glob.glob(os.path.join(self.logdir, self.DIR_NAME, self.FILE_MATCH))
+            if not all_ckpts:
+                if self.verbose:
+                    print('No checkpoints found. Skipping restoring variables.')
+                return 0, ''
+            idx = self.checkpoint_idx(max(all_ckpts))
+        ckpt = os.path.join(self.logdir, self.DIR_NAME, self.FILE_FORMAT % idx)
+        if self.verbose:
+            print('Resuming from', ckpt)
+        self.LOAD_FN(ckpt, vc)
+        return idx, ckpt
 
-    def __call__(self, *args, **kwargs):
-        """Returns the computed gradients for the first value returned by `f`.
+    def save(self, vc: VarCollection, idx: int):
+        """Saves variables collection to checkpoint with given index.
 
-        Returns:
-            A list of input gradients, if any, followed by the variable gradients."""
-        return super().__call__(*args, **kwargs)[0]
+        Args:
+            vc: variables collection to save.
+            idx: index of the new checkpoint where variables should be saved.
+        """
+        assert isinstance(vc, VarCollection), f'Must pass a VarCollection to save; received type {type(vc)}.'
+        self.SAVE_FN(os.path.join(self.logdir, self.DIR_NAME, self.FILE_FORMAT % idx), vc)
+        for ckpt in sorted(glob.glob(os.path.join(self.logdir, self.DIR_NAME, self.FILE_MATCH)))[:-self.keep_ckpts]:
+            os.remove(ckpt)
```

### Comparing `objax-1.6.0/objax/io/__init__.py` & `objax-1.7.0/objax/io/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/io/ops.py` & `objax-1.7.0/objax/io/ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 import collections
 import os
 from typing import IO, BinaryIO, Union, Optional
 
 import jax.numpy as jn
 import numpy as np
-from jax.interpreters.pxla import ShardedDeviceArray
 
 from objax.util import Renamer
 from objax.variable import TrainRef, VarCollection
 
 
 def load_var_collection(file: Union[str, IO[BinaryIO]],
                         vc: VarCollection,
@@ -94,17 +93,21 @@
     for k, v in vc.items():
         if isinstance(v, TrainRef):
             v = v.ref
         if id(v) not in seen:
             names.append(k)
             data[str(len(data))] = v.value
             seen.add(id(v))
-        if isinstance(v.value, ShardedDeviceArray):
-            replicated.append(k)
     if replicated:
         print('Warning: When saving VarCollection, some variables were replicated on multiple devices.')
         print('         While it is valid, in most use cases it is more disk efficient to save variables outside of ')
         print('         vars().replicate().')
+
+    def _disabled_seek(*_):
+        raise AttributeError('seek() is disabled on this object.')
+    _old_seek = getattr(file, 'seek')
+    setattr(file, 'seek', _disabled_seek)
     np.savez(file, names=np.array(names), **data)
+    setattr(file, 'seek', _old_seek)
     if do_close:
         file.close()
         os.rename(filename + '.tmp', filename)  # Atomic rename to avoid broken file (when killed while saving).
```

### Comparing `objax-1.6.0/objax/jaxboard.py` & `objax-1.7.0/objax/jaxboard.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/module.py` & `objax-1.7.0/objax/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from collections import namedtuple
 from typing import Optional, List, Union, Callable, Tuple
 
 import jax
 import jax.numpy as jn
 import numpy as np
-from jax.interpreters.pxla import ShardedDeviceArray
 
 from objax.typing import JaxArray
 from objax.util import class_name, override_args_kwargs, positional_args_names, repr_function
 from objax.variable import BaseVar, RandomState, VarCollection
 
 
 class Module:
@@ -283,15 +282,15 @@
                 A new graph is compiled for each different combination of values for such inputs.
         """
         if not isinstance(f, Module):
             if vc is None:
                 raise ValueError('You must supply the VarCollection used by the function f.')
             f = Function(f, vc)
 
-        def pmap(tensor_list: List[ShardedDeviceArray], random_list: List[ShardedDeviceArray], *args):
+        def pmap(tensor_list: List[jax.Array], random_list: List[jax.Array], *args):
             original_values = self.vc.tensors()
             try:
                 self.vc.assign(tensor_list)
                 self.vc.subset(RandomState).assign(random_list)
                 return f(*args), self.vc.tensors()
             finally:
                 self.vc.assign(original_values)
@@ -316,15 +315,15 @@
         return x.reshape((self.ndevices, x.shape[0] // self.ndevices) + x.shape[1:])
 
     def __call__(self, *args):
         """Call the compiled function or module on multiple devices in parallel.
         Important: Make sure you call this function within the scope of VarCollection.replicate() statement.
         """
         unreplicated = [k for k, v in self.vc.items()
-                        if not isinstance(v.value, (ShardedDeviceArray,
+                        if not isinstance(v.value, (jax.Array,
                                                     jax.interpreters.partial_eval.JaxprTracer,
                                                     jax.interpreters.partial_eval.DynamicJaxprTracer))]
         assert not unreplicated, \
             f'Some variables were not replicated: {unreplicated}.' \
             'did you forget to call VarCollection.replicate on them?'
 
         args = [x if i in self.static_argnums
```

### Comparing `objax-1.6.0/objax/nn/__init__.py` & `objax-1.7.0/objax/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/nn/init.py` & `objax-1.7.0/objax/nn/init.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/nn/layers.py` & `objax-1.7.0/objax/nn/layers.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/optimizer/__init__.py` & `objax-1.7.0/objax/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/optimizer/adam.py` & `objax-1.7.0/objax/optimizer/adam.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/optimizer/ema.py` & `objax-1.7.0/objax/optimizer/ema.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/optimizer/lars.py` & `objax-1.7.0/objax/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/optimizer/momentum.py` & `objax-1.7.0/objax/optimizer/momentum.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/optimizer/scheduler.py` & `objax-1.7.0/objax/optimizer/scheduler.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/optimizer/sgd.py` & `objax-1.7.0/objax/optimizer/sgd.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/privacy/__init__.py` & `objax-1.7.0/objax/privacy/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/privacy/dpsgd/__init__.py` & `objax-1.7.0/objax/privacy/dpsgd/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/privacy/dpsgd/gradient.py` & `objax-1.7.0/objax/privacy/dpsgd/gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         Returns:
           clipped_grad: the function computing the average of gradients clipped per-sample.
         """
         @Function.with_vars(gv.vars())
         def clipped_grad_single_example(*args):
             grads, values = gv(*args)
-            total_grad_norm = jn.linalg.norm([jn.linalg.norm(g) for g in grads])
+            total_grad_norm = jn.linalg.norm(jn.array([jn.linalg.norm(g) for g in grads]))
             idivisor = 1 / jn.maximum(total_grad_norm / self.l2_norm_clip, 1.)
             return [g * idivisor for g in grads], values
 
         clipped_grad_vectorized = Vectorize(clipped_grad_single_example,
                                             batch_axis=self.batch_axis)
 
         def clipped_grad(*args):
@@ -119,15 +119,15 @@
 
         Returns:
           clipped_grad: the function computing the average of gradients clipped per-sample.
         """
         @Function.with_vars(gv.vars())
         def grad_norm_fn(*args):
             grads, values = gv(*args)
-            total_grad_norm = jn.linalg.norm([jn.linalg.norm(g) for g in grads])
+            total_grad_norm = jn.linalg.norm(jn.array([jn.linalg.norm(g) for g in grads]))
             return total_grad_norm, values
 
         grad_norm_fn_vectorized = Vectorize(grad_norm_fn, batch_axis=self.batch_axis)
         loss_fn_vectorized = Vectorize(Function.with_vars(gv.vars())(f), batch_axis=self.batch_axis)
 
         def weighted_loss_fn(weights, *args):
             returned = loss_fn_vectorized(*args)
```

### Comparing `objax-1.6.0/objax/privacy/dpsgd/privacyaccountant.py` & `objax-1.7.0/objax/privacy/dpsgd/privacyaccountant.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/random/__init__.py` & `objax-1.7.0/objax/random/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/random/random.py` & `objax-1.7.0/objax/random/random.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/typing.py` & `objax-1.7.0/objax/typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 """This module contains type declarations for Objax."""
 
 __all__ = ['FileOrStr', 'JaxArray', 'JaxDType']
 
 from typing import Union, IO, BinaryIO, Sequence, Tuple
 
+import jax
 import jax.numpy as jn
-from jax.interpreters.pxla import ShardedDeviceArray
 
 ConvPaddingInt = Union[Sequence[Tuple[int, int]], Tuple[int, int], int]
 FileOrStr = Union[str, IO[BinaryIO]]
-JaxArray = Union[jn.ndarray, jn.DeviceArray, ShardedDeviceArray]
+JaxArray = jax.Array
 JaxDType = Union[jn.complex64, jn.complex128, jn.bfloat16,
                  jn.float16, jn.float32, jn.float64,
                  jn.int8, jn.int16, jn.int32, jn.int64,
                  jn.uint8, jn.uint16, jn.uint32, jn.uint64]
```

### Comparing `objax-1.6.0/objax/util/__init__.py` & `objax-1.7.0/objax/util/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/util/check.py` & `objax-1.7.0/objax/util/check.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,30 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __all__ = ['assert_assigned_type_and_shape_match']
 
 import jax
 
-from objax.typing import JaxArray
-
 
 TRACER_TYPES = (jax.interpreters.partial_eval.JaxprTracer,
                 jax.interpreters.partial_eval.DynamicJaxprTracer)
 
 
 def split_shape_and_device(array):
-    if isinstance(array, jax.interpreters.pxla.ShardedDeviceArray):
+    if isinstance(array, jax.Array) and hasattr(array, 'sharding') and isinstance(
+            array.sharding, jax.sharding.PmapSharding):
         return array.shape[0], array.shape[1:]
     else:
         return None, array.shape
 
 
 def assert_assigned_type_and_shape_match(existing_tensor, new_tensor):
-    assert isinstance(new_tensor, JaxArray.__args__), \
+    assert isinstance(new_tensor, jax.Array), \
         f'Assignments to variable must be an instance of JaxArray, but received f{type(new_tensor)}.'
 
     new_tensor_device, new_tensor_shape = split_shape_and_device(new_tensor)
     self_device, self_shape = split_shape_and_device(existing_tensor)
 
     device_mismatch_error = f'Can not replicate a variable that is currently on ' \
                             f'{self_device} devices to {new_tensor_device} devices.'
```

### Comparing `objax-1.6.0/objax/util/image.py` & `objax-1.7.0/objax/util/image.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/util/objax2tf.py` & `objax-1.7.0/objax/util/objax2tf.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/util/tracing.py` & `objax-1.7.0/objax/util/tracing.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/util/util.py` & `objax-1.7.0/objax/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import re
 from numbers import Number
 from typing import Callable, List, Union, Tuple, Iterable, Dict, Pattern, Optional, Sequence
 
 import jax
 import jax.numpy as jn
 import numpy as np
-from jax.interpreters.pxla import ShardedDeviceArray
 
 from objax.constants import ConvPadding, Interpolate
 from objax.typing import ConvPaddingInt
 
 CLASS_MODULES = {
     'objax.dpsgd.gradient': 'objax.dpsgd',
     'objax.gradient': 'objax',
@@ -134,15 +133,15 @@
     if next(reversed(p.values())).kind == inspect.Parameter.VAR_KEYWORD:
         return kwargs
     if len(kwargs) < len(p):
         return {k: v for k, v in kwargs.items() if k in p}
     return {k: kwargs[k] for k in p.keys() if k in kwargs}
 
 
-map_to_device: Callable[[List[jn.ndarray]], List[ShardedDeviceArray]] = jax.pmap(lambda x: x, axis_name='device')
+map_to_device: Callable[[List[jn.ndarray]], List[jn.ndarray]] = jax.pmap(lambda x: x, axis_name='device')
 
 
 def multi_host_barrier():
     """Barrier op for multi-host setup."""
     jax.random.normal(jax.random.PRNGKey(0), ()).block_until_ready()
```

### Comparing `objax-1.6.0/objax/variable.py` & `objax-1.7.0/objax/variable.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/zoo/__init__.py` & `objax-1.7.0/objax/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/zoo/convnet.py` & `objax-1.7.0/objax/zoo/convnet.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/zoo/dnnet.py` & `objax-1.7.0/objax/zoo/dnnet.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/zoo/resnet_v2.py` & `objax-1.7.0/objax/zoo/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/zoo/rnn.py` & `objax-1.7.0/objax/zoo/rnn.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/zoo/vgg.py` & `objax-1.7.0/objax/zoo/vgg.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax/zoo/wide_resnet.py` & `objax-1.7.0/objax/zoo/wide_resnet.py`

 * *Files identical despite different names*

### Comparing `objax-1.6.0/objax.egg-info/PKG-INFO` & `objax-1.7.0/objax.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: objax
-Version: 1.6.0
+Version: 1.7.0
 Summary: Objax is a machine learning framework that provides an Object Oriented layer for JAX.
 Home-page: https://github.com/google/objax
 Author: Objax team
 Author-email: objax-dev@google.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,22 +46,26 @@
 You install Objax using `pip` as follows:
 
 ```bash
 pip install --upgrade objax
 ```
 
 Objax supports GPUs but assumes that you already have some version of CUDA
-installed. Here are the extra steps:
+installed. Here are the extra steps required to install CUDA-enabled jaxlib
+(jaxlib releases require CUDA 11.2 or newer):
 
 ```bash
-# Update accordingly to your installed CUDA version
-CUDA_VERSION=11.0
-pip install -f https://storage.googleapis.com/jax-releases/jax_releases.html jaxlib==`python3 -c 'import jaxlib; print(jaxlib.__version__)'`+cuda`echo $CUDA_VERSION | sed s:\\\.::g`
+RELEASE_URL="https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
+JAX_VERSION=`python3 -c 'import jax; print(jax.__version__)'`
+pip uninstall -y jaxlib
+pip install -f $RELEASE_URL jax[cuda]==$JAX_VERSION
 ```
 
+For more installation options, see https://github.com/google/jax#pip-installation-gpu-cuda
+
 ### Useful environment configurations
 
 Here are a few useful options:
 
 ```bash
 # Prevent JAX from taking the whole GPU memory
 # (useful if you want to run several programs on a single GPU)
@@ -117,9 +118,7 @@
 ```
 
 ## Developer documentation
 
 Here is information about
 [development setup](https://objax.readthedocs.io/en/latest/dev/setup.html)
 and a [guide on adding new code](https://objax.readthedocs.io/en/latest/dev/adding_module.html).
-
-
```

### Comparing `objax-1.6.0/objax.egg-info/SOURCES.txt` & `objax-1.7.0/objax.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -52,8 +52,10 @@
 objax/util/util.py
 objax/zoo/__init__.py
 objax/zoo/convnet.py
 objax/zoo/dnnet.py
 objax/zoo/resnet_v2.py
 objax/zoo/rnn.py
 objax/zoo/vgg.py
-objax/zoo/wide_resnet.py
+objax/zoo/wide_resnet.py
+tests/testio.py
+tests/testrandom.py
```

### Comparing `objax-1.6.0/setup.py` & `objax-1.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     url='https://github.com/google/objax',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
     ],
     install_requires=install_requires,
 )
```

