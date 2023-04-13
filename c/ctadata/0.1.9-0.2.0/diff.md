# Comparing `tmp/ctadata-0.1.9.tar.gz` & `tmp/ctadata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctadata-0.1.9.tar", max compression
+gzip compressed data, was "ctadata-0.2.0.tar", max compression
```

## Comparing `ctadata-0.1.9.tar` & `ctadata-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,7 @@
--rw-r--r--   0        0        0        0 2023-03-21 20:23:26.963551 ctadata-0.1.9/README.md
--rw-r--r--   0        0        0     1235 2023-03-21 21:17:36.697942 ctadata-0.1.9/ctadata/__init__.py
--rw-r--r--   0        0        0      348 2023-03-21 21:17:41.269990 ctadata-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 ctadata-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1976 2023-04-12 15:32:43.928799 ctadata-0.2.0/README.md
+-rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.0/ctadata/__init__.py
+-rw-r--r--   0        0        0     3220 2023-04-13 11:56:04.865225 ctadata-0.2.0/ctadata/api.py
+-rw-r--r--   0        0        0      850 2023-04-13 12:12:59.548331 ctadata-0.2.0/ctadata/cli.py
+-rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.0/ctadata/util.py
+-rw-r--r--   0        0        0      369 2023-04-13 12:26:44.425929 ctadata-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 ctadata-0.2.0/PKG-INFO
```

