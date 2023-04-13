# Comparing `tmp/mnnllzz-1.4.1.tar.gz` & `tmp/mnnllzz-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnnllzz-1.4.1.tar", last modified: Thu Apr 13 07:30:12 2023, max compression
+gzip compressed data, was "mnnllzz-1.4.2.tar", last modified: Thu Apr 13 07:41:42 2023, max compression
```

## Comparing `mnnllzz-1.4.1.tar` & `mnnllzz-1.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 07:30:12.017768 mnnllzz-1.4.1/
--rw-rw-rw-   0        0        0      517 2023-04-13 07:30:12.017768 mnnllzz-1.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 07:30:12.016768 mnnllzz-1.4.1/mnnllzz/
--rw-rw-rw-   0        0        0        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.1/mnnllzz/__init__.py
--rw-rw-rw-   0        0        0      537 2023-02-20 17:34:38.000000 mnnllzz-1.4.1/mnnllzz/__main__.py
--rw-rw-rw-   0        0        0    24950 2023-04-13 07:22:25.556788 mnnllzz-1.4.1/mnnllzz/mnnllzz.py
--rw-rw-rw-   0        0        0       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-04-13 07:27:45.738307 mnnllzz-1.4.1/setup.py
+drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 07:41:42.013728 mnnllzz-1.4.2/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      391 2023-04-13 07:41:42.013728 mnnllzz-1.4.2/PKG-INFO
+drwxr-xr-x   0 andrea    (1000) andrea    (1000)        0 2023-04-13 07:41:42.012730 mnnllzz-1.4.2/mnnllzz/
+-rw-r--r--   0 andrea    (1000) andrea    (1000)        0 2022-02-07 08:57:12.000000 mnnllzz-1.4.2/mnnllzz/__init__.py
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      537 2023-02-20 17:34:38.000000 mnnllzz-1.4.2/mnnllzz/__main__.py
+-rw-r--r--   0 andrea    (1000) andrea    (1000)    24950 2023-04-13 07:22:25.556788 mnnllzz-1.4.2/mnnllzz/mnnllzz.py
+-rw-r--r--   0 andrea    (1000) andrea    (1000)       42 2022-02-14 09:41:48.000000 mnnllzz-1.4.2/setup.cfg
+-rw-r--r--   0 andrea    (1000) andrea    (1000)      450 2023-04-13 07:39:49.219107 mnnllzz-1.4.2/setup.py
```

### Comparing `mnnllzz-1.4.1/mnnllzz/__main__.py` & `mnnllzz-1.4.2/mnnllzz/__main__.py`

 * *Files identical despite different names*

### Comparing `mnnllzz-1.4.1/mnnllzz/mnnllzz.py` & `mnnllzz-1.4.2/mnnllzz/mnnllzz.py`

 * *Files identical despite different names*

