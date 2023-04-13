# Comparing `tmp/seurat-0.0.2.tar.gz` & `tmp/seurat-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seurat-0.0.2.tar", max compression
+gzip compressed data, was "seurat-0.1.0.tar", max compression
```

## Comparing `seurat-0.0.2.tar` & `seurat-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,4 @@
--rw-r--r--   0        0        0      460 2023-04-13 15:49:18.207221 seurat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      159 2023-04-13 11:25:34.139438 seurat-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-08 23:26:41.176937 seurat-0.0.2/seurat/__init__.py
--rw-r--r--   0        0        0     2372 2023-04-13 11:58:45.035525 seurat-0.0.2/seurat/mphands.py
--rw-r--r--   0        0        0      590 2023-04-13 15:15:44.676799 seurat-0.0.2/seurat/tracker_abc.py
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 seurat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      272 2023-04-08 23:26:41.181935 seurat-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      164 2023-04-08 23:30:42.263589 seurat-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-08 23:26:41.176937 seurat-0.1.0/seurat/__init__.py
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 seurat-0.1.0/PKG-INFO
```

