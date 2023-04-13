# Comparing `tmp/sienna-0.1.5.tar.gz` & `tmp/sienna-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sienna-0.1.5.tar", max compression
+gzip compressed data, was "sienna-0.2.0.tar", max compression
```

## Comparing `sienna-0.1.5.tar` & `sienna-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      380 2022-06-10 10:02:21.420705 sienna-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       57 2022-04-05 09:20:12.345236 sienna-0.1.5/sienna/__init__.py
--rw-r--r--   0        0        0     1047 2022-05-03 12:58:47.856797 sienna-0.1.5/sienna/core.py
--rw-r--r--   0        0        0      501 2022-06-10 10:02:39.261509 sienna-0.1.5/setup.py
--rw-r--r--   0        0        0      351 2022-06-10 10:02:39.261923 sienna-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      380 2023-04-13 10:11:35.652110 sienna-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-04-13 10:11:35.652403 sienna-0.2.0/sienna/__init__.py
+-rw-r--r--   0        0        0     1378 2023-04-13 10:11:35.652653 sienna-0.2.0/sienna/core.py
+-rw-r--r--   0        0        0      509 1970-01-01 00:00:00.000000 sienna-0.2.0/setup.py
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 sienna-0.2.0/PKG-INFO
```

