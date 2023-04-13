# Comparing `tmp/selcol-0.0.4.tar.gz` & `tmp/selcol-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selcol-0.0.4.tar", last modified: Mon Apr 10 21:15:23 2023, max compression
+gzip compressed data, was "selcol-0.0.4.1.tar", last modified: Thu Apr 13 07:54:18 2023, max compression
```

## Comparing `selcol-0.0.4.tar` & `selcol-0.0.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.696110 selcol-0.0.4/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-01-11 08:30:47.000000 selcol-0.0.4/MANIFEST.in
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      197 2023-04-10 21:15:23.696110 selcol-0.0.4/PKG-INFO
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      550 2023-01-01 17:29:44.000000 selcol-0.0.4/README.md
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       63 2022-12-28 18:19:34.000000 selcol-0.0.4/pyproject.toml
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 18:57:10.000000 selcol-0.0.4/selcol/__init__.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      824 2023-01-15 03:02:13.000000 selcol-0.0.4/selcol/file.py
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol/pretrained/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       13 2023-01-11 08:28:54.000000 selcol-0.0.4/selcol/pretrained/.gitignore
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)     1020 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/metadata.json
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-1.onnx
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355007 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-128.onnx
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-16.onnx
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-32.onnx
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-64.onnx
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-8.onnx
--rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   354164 2023-04-10 21:04:13.000000 selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/numpy_layers.pkl
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.692110 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      529 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332605 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   331764 2023-01-01 19:38:20.000000 selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.692110 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      726 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338205 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   337364 2023-01-01 15:51:31.000000 selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.696110 selcol-0.0.4/selcol/runtime/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      168 2023-01-01 18:50:35.000000 selcol-0.0.4/selcol/runtime/__init__.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3327 2023-04-09 19:21:17.000000 selcol-0.0.4/selcol/runtime/interface.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3658 2023-01-11 07:41:04.000000 selcol-0.0.4/selcol/runtime/jax_model.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     4128 2023-01-11 07:41:04.000000 selcol-0.0.4/selcol/runtime/ort_model.py
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.696110 selcol-0.0.4/selcol/traintime/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 16:59:41.000000 selcol-0.0.4/selcol/traintime/__init__.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     8395 2023-04-09 14:41:30.000000 selcol-0.0.4/selcol/traintime/dataset.py
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     9915 2023-04-09 15:36:33.000000 selcol-0.0.4/selcol/traintime/neural.py
-drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-10 21:15:23.680110 selcol-0.0.4/selcol.egg-info/
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      197 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/PKG-INFO
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3338 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/SOURCES.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        1 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/dependency_links.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       49 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/requires.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        7 2023-04-10 21:15:23.000000 selcol-0.0.4/selcol.egg-info/top_level.txt
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-04-10 21:15:23.696110 selcol-0.0.4/setup.cfg
--rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      553 2023-04-10 21:14:53.000000 selcol-0.0.4/setup.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.426335 selcol-0.0.4.1/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-01-11 08:30:47.000000 selcol-0.0.4.1/MANIFEST.in
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      199 2023-04-13 07:54:18.426335 selcol-0.0.4.1/PKG-INFO
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      550 2023-01-01 17:29:44.000000 selcol-0.0.4.1/README.md
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       63 2022-12-28 18:19:34.000000 selcol-0.0.4.1/pyproject.toml
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.422335 selcol-0.0.4.1/selcol/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 18:57:10.000000 selcol-0.0.4.1/selcol/__init__.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      824 2023-01-15 03:02:13.000000 selcol-0.0.4.1/selcol/file.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.422335 selcol-0.0.4.1/selcol/pretrained/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       13 2023-01-11 08:28:54.000000 selcol-0.0.4.1/selcol/pretrained/.gitignore
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.422335 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)     1020 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/metadata.json
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-1.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355007 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-128.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-16.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-32.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-64.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   355005 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-8.onnx
+-rw-r--r--   0 h-ishida  (1000) h-ishida  (1000)   354164 2023-04-13 07:52:57.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/numpy_layers.pkl
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.422335 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      529 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332605 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   332603 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   331764 2023-01-01 19:38:20.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.426335 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      726 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338205 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   338203 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)   337364 2023-01-01 15:51:31.000000 selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.426335 selcol-0.0.4.1/selcol/runtime/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      168 2023-01-01 18:50:35.000000 selcol-0.0.4.1/selcol/runtime/__init__.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3327 2023-04-09 19:21:17.000000 selcol-0.0.4.1/selcol/runtime/interface.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3658 2023-01-11 07:41:04.000000 selcol-0.0.4.1/selcol/runtime/jax_model.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     4128 2023-01-11 07:41:04.000000 selcol-0.0.4.1/selcol/runtime/ort_model.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.426335 selcol-0.0.4.1/selcol/traintime/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        0 2022-12-29 16:59:41.000000 selcol-0.0.4.1/selcol/traintime/__init__.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     8395 2023-04-09 14:41:30.000000 selcol-0.0.4.1/selcol/traintime/dataset.py
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     9915 2023-04-09 15:36:33.000000 selcol-0.0.4.1/selcol/traintime/neural.py
+drwxrwxr-x   0 h-ishida  (1000) h-ishida  (1000)        0 2023-04-13 07:54:18.422335 selcol-0.0.4.1/selcol.egg-info/
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      199 2023-04-13 07:54:18.000000 selcol-0.0.4.1/selcol.egg-info/PKG-INFO
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)     3338 2023-04-13 07:54:18.000000 selcol-0.0.4.1/selcol.egg-info/SOURCES.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        1 2023-04-13 07:54:18.000000 selcol-0.0.4.1/selcol.egg-info/dependency_links.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       49 2023-04-13 07:54:18.000000 selcol-0.0.4.1/selcol.egg-info/requires.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)        7 2023-04-13 07:54:18.000000 selcol-0.0.4.1/selcol.egg-info/top_level.txt
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)       38 2023-04-13 07:54:18.426335 selcol-0.0.4.1/setup.cfg
+-rw-rw-r--   0 h-ishida  (1000) h-ishida  (1000)      555 2023-04-13 07:53:39.000000 selcol-0.0.4.1/setup.py
```

### Comparing `selcol-0.0.4/README.md` & `selcol-0.0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/file.py` & `selcol-0.0.4.1/selcol/file.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/metadata.json` & `selcol-0.0.4.1/selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/metadata.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'time_stamp'": '1681258356.730166', "'valid_loss'": '0.009082690371817304'}*

```diff
@@ -42,11 +42,11 @@
     ],
     "model_config": {
         "n_depth": 3,
         "n_dof": 38,
         "n_width": 200
     },
     "robot_name": "JAXON_JVRC",
-    "time_stamp": 1681098151.601409,
+    "time_stamp": 1681258356.730166,
     "urdf_md5sum": "0cc17003e5f01cd6157233f92877ddc8",
-    "valid_loss": 0.011621874798516523
+    "valid_loss": 0.009082690371817304
 }
```

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl` & `selcol-0.0.4.1/selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/numpy_layers.pkl`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/metadata.json`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-1.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-128.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-16.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-32.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-64.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/model-8.onnx`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl` & `selcol-0.0.4.1/selcol/pretrained/pretrained-pr2-a29f30bd85e6752168a29b0e19e7b9ef-feef89ef-cc97-4946-901e-4cfc5d608ec6/numpy_layers.pkl`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/runtime/interface.py` & `selcol-0.0.4.1/selcol/runtime/interface.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/runtime/jax_model.py` & `selcol-0.0.4.1/selcol/runtime/jax_model.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/runtime/ort_model.py` & `selcol-0.0.4.1/selcol/runtime/ort_model.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/traintime/dataset.py` & `selcol-0.0.4.1/selcol/traintime/dataset.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol/traintime/neural.py` & `selcol-0.0.4.1/selcol/traintime/neural.py`

 * *Files identical despite different names*

### Comparing `selcol-0.0.4/selcol.egg-info/SOURCES.txt` & `selcol-0.0.4.1/selcol.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 selcol/file.py
 selcol.egg-info/PKG-INFO
 selcol.egg-info/SOURCES.txt
 selcol.egg-info/dependency_links.txt
 selcol.egg-info/requires.txt
 selcol.egg-info/top_level.txt
 selcol/pretrained/.gitignore
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/metadata.json
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-1.onnx
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-128.onnx
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-16.onnx
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-32.onnx
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-64.onnx
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/model-8.onnx
-selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-5e2ba177-8798-42bd-b48a-3d8ac057e580/numpy_layers.pkl
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/metadata.json
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-1.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-128.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-16.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-32.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-64.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/model-8.onnx
+selcol/pretrained/pretrained-JAXON_JVRC-0cc17003e5f01cd6157233f92877ddc8-19cd5b6d-7026-41a5-b0ed-944ff9b7d6c9/numpy_layers.pkl
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/metadata.json
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-1.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-128.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-16.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-32.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-64.onnx
 selcol/pretrained/pretrained-fetch-338459c27088a928a7a3b08023474fbb-ab64c329-13bf-442f-b331-20eb21250e3b/model-8.onnx
```

### Comparing `selcol-0.0.4/setup.py` & `selcol-0.0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 install_requires = ["numpy", "onnxruntime"]
 dev_requires = ["torch", "scikit-robot", "tqdm"]
 
 setup(
     name="selcol",
-    version="0.0.4",
+    version="0.0.4.1",
     description="yet another percol implementation",
     author="Hirokazu Ishida",
     author_email="h-ishida@jsk.imi.i.u-tokyo.ac.jp",
     license="MIT",
     install_requires=install_requires,
     extras_require={"dev": dev_requires},
     packages=find_packages(exclude=("tests", "docs")),
```

