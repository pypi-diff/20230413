# Comparing `tmp/griptape_tools-0.5.0.tar.gz` & `tmp/griptape_tools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.5.0.tar", max compression
+gzip compressed data, was "griptape_tools-0.5.1.tar", max compression
```

## Comparing `griptape_tools-0.5.0.tar` & `griptape_tools-0.5.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.0/LICENSE
--rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.0/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.0/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.0/griptape/tools/__init__.py
--rw-r--r--   0        0        0      499 2023-04-13 16:44:18.759766 griptape_tools-0.5.0/griptape/tools/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      161 2023-04-13 16:44:18.862164 griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1729 2023-04-13 17:32:12.692546 griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     1790 2023-04-13 17:00:19.874640 griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.0/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       78 2023-04-13 17:30:17.934482 griptape_tools-0.5.0/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.0/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      164 2023-04-07 15:56:04.337980 griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1782 2023-04-11 19:13:20.365906 griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     1052 2023-04-13 16:51:04.094631 griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.0/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 17:01:17.168803 griptape_tools-0.5.0/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.0/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      166 2023-04-12 21:41:15.550396 griptape_tools-0.5.0/griptape/tools/email_client/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2195 2023-04-13 16:44:18.859633 griptape_tools-0.5.0/griptape/tools/email_client/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.0/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 17:01:17.163490 griptape_tools-0.5.0/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     2354 2023-04-13 16:12:25.314046 griptape_tools-0.5.0/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.0/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      164 2023-04-12 20:32:26.158552 griptape_tools-0.5.0/griptape/tools/sql_client/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1895 2023-04-13 16:51:04.196419 griptape_tools-0.5.0/griptape/tools/sql_client/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.0/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       33 2023-04-13 17:01:17.166413 griptape_tools-0.5.0/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.0/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.0/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      165 2023-04-12 16:01:57.738417 griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3883 2023-04-12 22:07:30.759928 griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     3994 2023-04-13 15:56:54.679897 griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.0/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       53 2023-04-13 17:01:17.164930 griptape_tools-0.5.0/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     4506 2023-04-13 15:55:25.582021 griptape_tools-0.5.0/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.0/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      167 2023-04-07 15:56:04.338570 griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2374 2023-04-10 14:23:53.062035 griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/tool.cpython-310.pyc
--rw-r--r--   0        0        0     2423 2023-04-12 19:48:43.940734 griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/tool.cpython-39.pyc
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.0/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       29 2023-04-13 17:01:17.161796 griptape_tools-0.5.0/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.0/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      526 2023-04-13 17:50:25.659660 griptape_tools-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.1/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.1/griptape/tools/__init__.py
+-rw-r--r--   0        0        0      499 2023-04-13 16:44:18.759766 griptape_tools-0.5.1/griptape/tools/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      161 2023-04-13 16:44:18.862164 griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1729 2023-04-13 17:32:12.692546 griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1790 2023-04-13 17:00:19.874640 griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.1/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       78 2023-04-13 21:55:09.487715 griptape_tools-0.5.1/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.1/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-07 15:56:04.337980 griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1782 2023-04-11 19:13:20.365906 griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1052 2023-04-13 16:51:04.094631 griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.1/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 21:55:09.483314 griptape_tools-0.5.1/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.1/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      166 2023-04-12 21:41:15.550396 griptape_tools-0.5.1/griptape/tools/email_client/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2195 2023-04-13 16:44:18.859633 griptape_tools-0.5.1/griptape/tools/email_client/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.1/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 21:55:09.481296 griptape_tools-0.5.1/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     2354 2023-04-13 16:12:25.314046 griptape_tools-0.5.1/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.1/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      164 2023-04-12 20:32:26.158552 griptape_tools-0.5.1/griptape/tools/sql_client/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1895 2023-04-13 16:51:04.196419 griptape_tools-0.5.1/griptape/tools/sql_client/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.1/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       33 2023-04-13 21:55:09.486224 griptape_tools-0.5.1/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.1/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.1/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      165 2023-04-12 16:01:57.738417 griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3931 2023-04-13 20:35:47.051663 griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     3994 2023-04-13 15:56:54.679897 griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.1/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       53 2023-04-13 21:55:09.484886 griptape_tools-0.5.1/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     4506 2023-04-13 15:55:25.582021 griptape_tools-0.5.1/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.1/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-07 15:56:04.338570 griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2374 2023-04-10 14:23:53.062035 griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/tool.cpython-310.pyc
+-rw-r--r--   0        0        0     2423 2023-04-12 19:48:43.940734 griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/tool.cpython-39.pyc
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.1/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       29 2023-04-13 21:55:09.489187 griptape_tools-0.5.1/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.1/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      526 2023-04-13 21:56:28.623300 griptape_tools-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.1/PKG-INFO
```

### Comparing `griptape_tools-0.5.0/LICENSE` & `griptape_tools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/README.md` & `griptape_tools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/tool.cpython-310.pyc` & `griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/aws_cli/__pycache__/tool.cpython-39.pyc` & `griptape_tools-0.5.1/griptape/tools/aws_cli/__pycache__/tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/aws_cli/tool.py` & `griptape_tools-0.5.1/griptape/tools/aws_cli/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/tool.cpython-310.pyc` & `griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/calculator/__pycache__/tool.cpython-39.pyc` & `griptape_tools-0.5.1/griptape/tools/calculator/__pycache__/tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/calculator/tool.py` & `griptape_tools-0.5.1/griptape/tools/calculator/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/email_client/__pycache__/tool.cpython-39.pyc` & `griptape_tools-0.5.1/griptape/tools/email_client/__pycache__/tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/email_client/tool.py` & `griptape_tools-0.5.1/griptape/tools/email_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/sql_client/__pycache__/tool.cpython-39.pyc` & `griptape_tools-0.5.1/griptape/tools/sql_client/__pycache__/tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/sql_client/tool.py` & `griptape_tools-0.5.1/griptape/tools/sql_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/tool.cpython-310.pyc` & `griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/tool.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Apr 12 22:07:09 2023 UTC, .py size: 4516 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8d2b 3764 a411 0000  o........+7d....
+00000000: 6f0d 0d0a 0000 0000 ed25 3864 9a11 0000  o........%8d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 8400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 5a05 6400 6404 6c02 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 6d0c 5a0c 0100 6400  d.l.m.Z.m.Z...d.
@@ -20,32 +20,32 @@
 00000130: 0000 0000 0000 0b00 0000 4000 0001 736e  ..........@...sn
 00000140: 0100 0065 005a 0164 005a 0255 0065 0364  ...e.Z.d.Z.U.e.d
 00000150: 0164 0264 0364 0469 0164 058d 035a 0464  .d.d.d.i.d...Z.d
 00000160: 0665 0564 073c 0065 0364 0264 0264 0364  .e.d.<.e.d.d.d.d
 00000170: 0869 0164 058d 035a 0664 0965 0564 0a3c  .i.d...Z.d.e.d.<
 00000180: 0065 0764 0b64 0c65 0865 0964 0d64 0e64  .e.d.d.e.e.d.d.d
 00000190: 0f8d 0265 0a69 0183 0164 109c 0364 118d  ...e.i...d...d..
-000001a0: 0164 3464 1564 1684 0483 015a 0b65 0764  .d4d.d.....Z.e.d
+000001a0: 0164 3664 1564 1684 0483 015a 0b65 0764  .d6d.d.....Z.e.d
 000001b0: 1764 1865 0865 0964 0d64 0e64 0f8d 0265  .d.e.e.d.d.d...e
-000001c0: 0a69 0183 0164 109c 0364 118d 0164 3464  .i...d...d...d4d
-000001d0: 1964 1a84 0483 015a 0c65 0764 1764 1865  .d.....Z.e.d.d.e
-000001e0: 0864 0d65 0964 1b64 0e64 0f8d 0265 0a65  .d.e.d.d.d...e.e
-000001f0: 0964 1c64 1d64 0f8d 0265 0a69 0269 0183  .d.d.d...e.i.i..
-00000200: 0164 109c 0364 118d 0164 3464 1e64 1f84  .d...d...d4d.d..
-00000210: 0483 015a 0d65 0764 2064 2165 0865 0964  ...Z.e.d d!e.e.d
+000001c0: 0a69 0183 0164 109c 0364 118d 0164 3664  .i...d...d...d6d
+000001d0: 1964 1a84 0483 015a 0c65 0764 1b64 1c65  .d.....Z.e.d.d.e
+000001e0: 0864 0d65 0964 1d64 0e64 0f8d 0265 0a65  .d.e.d.d.d...e.e
+000001f0: 0964 1e64 1f64 0f8d 0265 0a69 0269 0183  .d.d.d...e.i.i..
+00000200: 0164 109c 0364 118d 0164 3664 2064 2184  .d...d...d6d d!.
+00000210: 0483 015a 0d65 0764 2264 2365 0865 0964  ...Z.e.d"d#e.e.d
 00000220: 0d64 0e64 0f8d 0265 0a69 0183 0164 109c  .d.d...e.i...d..
-00000230: 0364 118d 0164 3564 2364 2484 0483 015a  .d...d5d#d$....Z
-00000240: 0e65 0764 2564 2665 0865 0964 0d64 0e64  .e.d%d&e.e.d.d.d
+00000230: 0364 118d 0164 3764 2564 2684 0483 015a  .d...d7d%d&....Z
+00000240: 0e65 0764 2764 2865 0865 0964 0d64 0e64  .e.d'd(e.e.d.d.d
 00000250: 0f8d 0265 0a69 0183 0164 109c 0364 118d  ...e.i...d...d..
-00000260: 0164 3564 2764 2884 0483 015a 0f65 0764  .d5d'd(....Z.e.d
-00000270: 2964 2a65 0865 0964 0d64 0e64 0f8d 0265  )d*e.e.d.d.d...e
-00000280: 0a69 0183 0164 109c 0364 118d 0164 3464  .i...d...d...d4d
-00000290: 2b64 2c84 0483 015a 1064 3664 2f64 3084  +d,....Z.d6d/d0.
-000002a0: 045a 1164 3764 3264 3384 045a 1264 0153  .Z.d7d2d3..Z.d.S
-000002b0: 0029 38da 0a57 6562 5363 7261 7065 724e  .)8..WebScraperN
+00000260: 0164 3764 2964 2a84 0483 015a 0f65 0764  .d7d)d*....Z.e.d
+00000270: 2b64 2c65 0865 0964 0d64 0e64 0f8d 0265  +d,e.e.d.d.d...e
+00000280: 0a69 0183 0164 109c 0364 118d 0164 3664  .i...d...d...d6d
+00000290: 2d64 2e84 0483 015a 1064 3864 3164 3284  -d.....Z.d8d1d2.
+000002a0: 045a 1164 3964 3464 3584 045a 1264 0153  .Z.d9d4d5..Z.d.S
+000002b0: 0029 3ada 0a57 6562 5363 7261 7065 724e  .):..WebScraperN
 000002c0: 54da 0365 6e76 5a0e 4f50 454e 4149 5f41  T..envZ.OPENAI_A
 000002d0: 5049 5f4b 4559 2903 da07 6465 6661 756c  PI_KEY)...defaul
 000002e0: 745a 076b 775f 6f6e 6c79 5a08 6d65 7461  tZ.kw_onlyZ.meta
 000002f0: 6461 7461 7a0d 4f70 7469 6f6e 616c 5b73  dataz.Optional[s
 00000300: 7472 5dda 0e6f 7065 6e61 695f 6170 695f  tr]..openai_api_
 00000310: 6b65 79da 0d49 4e43 4c55 4445 5f4c 494e  key..INCLUDE_LIN
 00000320: 4b53 da04 626f 6f6c da0d 696e 636c 7564  KS..bool..includ
@@ -75,169 +75,172 @@
 000004a0: 7420 6f66 2061 2077 6562 2070 6167 6563  t of a web pagec
 000004b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
 000004c0: 0400 0000 4300 0001 721b 0000 0029 024e  ....C...r....).N
 000004d0: da04 7465 7874 721d 0000 0072 2100 0000  ..textr....r!...
 000004e0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
 000004f0: 2600 0000 1f00 0000 7225 0000 007a 1857  &.......r%...z.W
 00000500: 6562 5363 7261 7065 722e 6765 745f 6675  ebScraper.get_fu
-00000510: 6c6c 5f70 6167 65da 0375 726c da05 7175  ll_page..url..qu
-00000520: 6572 797a 0c53 6561 7263 6820 7175 6572  eryz.Search quer
-00000530: 7963 0200 0000 0000 0000 0000 0000 0400  yc..............
-00000540: 0000 0600 0000 4300 0001 733e 0000 0074  ......C...s>...t
-00000550: 00a0 017c 01a0 02a1 00a1 017d 027c 00a0  ...|.......}.|..
-00000560: 037c 00a0 047c 0264 0119 00a1 01a0 0564  .|...|.d.......d
-00000570: 02a1 01a1 017d 0374 067c 03a0 077c 0264  .....}.t.|...|.d
-00000580: 0319 00a1 0183 01a0 08a1 0053 0029 044e  ...........S.).N
-00000590: 7228 0000 0072 2700 0000 7229 0000 0029  r(...r'...r)...)
-000005a0: 09da 046a 736f 6eda 056c 6f61 6473 721f  ...json..loadsr.
-000005b0: 0000 00da 105f 746f 5f76 6563 746f 725f  ....._to_vector_
-000005c0: 696e 6465 7872 1e00 0000 7220 0000 0072  indexr....r ...r
-000005d0: 1a00 0000 7229 0000 00da 0573 7472 6970  ....r).....strip
-000005e0: 2904 7222 0000 0072 1400 0000 da06 7061  ).r"...r......pa
-000005f0: 7261 6d73 da05 696e 6465 7872 2300 0000  rams..indexr#...
-00000600: 7223 0000 0072 2400 0000 da0b 7365 6172  r#...r$.....sear
-00000610: 6368 5f70 6167 652c 0000 0073 0600 0000  ch_page,...s....
-00000620: 0e11 1a01 1602 7a16 5765 6253 6372 6170  ......z.WebScrap
-00000630: 6572 2e73 6561 7263 685f 7061 6765 da0b  er.search_page..
-00000640: 6765 745f 6175 7468 6f72 737a 2d43 616e  get_authorsz-Can
-00000650: 2062 6520 7573 6564 2074 6f20 6765 7420   be used to get 
-00000660: 6120 6c69 7374 206f 6620 7765 6220 7061  a list of web pa
-00000670: 6765 2061 7574 686f 7273 fa09 6c69 7374  ge authors..list
-00000680: 5b73 7472 5d63 0200 0000 0000 0000 0000  [str]c..........
-00000690: 0000 0200 0000 0400 0000 4300 0001 7316  ..........C...s.
-000006a0: 0000 007c 00a0 007c 01a0 01a1 00a1 01a0  ...|...|........
-000006b0: 0264 01a1 0167 0153 0029 024e 5a06 6175  .d...g.S.).NZ.au
-000006c0: 7468 6f72 721d 0000 0072 2100 0000 7223  thorr....r!...r#
-000006d0: 0000 0072 2300 0000 7224 0000 0072 3100  ...r#...r$...r1.
-000006e0: 0000 4200 0000 7304 0000 0012 0c04 ff7a  ..B...s........z
-000006f0: 1657 6562 5363 7261 7065 722e 6765 745f  .WebScraper.get_
-00000700: 6175 7468 6f72 73da 0c67 6574 5f6b 6579  authors..get_key
-00000710: 776f 7264 737a 3943 616e 2062 6520 7573  wordsz9Can be us
-00000720: 6564 2074 6f20 6765 6e65 7261 7465 2061  ed to generate a
-00000730: 206c 6973 7420 6f66 206b 6579 776f 7264   list of keyword
-00000740: 7320 666f 7220 6120 7765 6220 7061 6765  s for a web page
-00000750: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00000760: 0006 0000 0043 0000 0173 3c00 0000 7c00  .....C...s<...|.
-00000770: a000 7c00 a001 7c01 a002 a100 a101 a003  ..|...|.........
-00000780: 6401 a101 a101 7d02 7404 7c02 a005 6402  d.....}.t.|...d.
-00000790: a101 8301 7d03 6403 6404 8400 7c03 a006  ....}.d.d...|...
-000007a0: 6405 a101 4400 8301 5300 2906 4e72 2700  d...D...S.).Nr'.
-000007b0: 0000 7a42 4765 6e65 7261 7465 2061 2063  ..zBGenerate a c
-000007c0: 6f6d 6d61 2d73 6570 6172 6174 6564 206c  omma-separated l
-000007d0: 6973 7420 6f66 206b 6579 776f 7264 7320  ist of keywords 
-000007e0: 666f 7220 7468 6520 666f 6c6c 6f77 696e  for the followin
-000007f0: 6720 7465 7874 6301 0000 0000 0000 0000  g textc.........
-00000800: 0000 0002 0000 0004 0000 0053 0000 0173  ...........S...s
-00000810: 1400 0000 6700 7c00 5d06 7d01 7c01 a000  ....g.|.].}.|...
-00000820: a100 9102 7102 5300 7223 0000 0029 0172  ....q.S.r#...).r
-00000830: 2d00 0000 2902 da02 2e30 da01 7772 2300  -...)....0..wr#.
-00000840: 0000 7223 0000 0072 2400 0000 da0a 3c6c  ..r#...r$.....<l
-00000850: 6973 7463 6f6d 703e 5f00 0000 7302 0000  istcomp>_...s...
-00000860: 0014 007a 2b57 6562 5363 7261 7065 722e  ...z+WebScraper.
-00000870: 6765 745f 6b65 7977 6f72 6473 2e3c 6c6f  get_keywords.<lo
-00000880: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000890: fa01 2c29 0772 2c00 0000 721e 0000 0072  ..,).r,...r....r
-000008a0: 1f00 0000 7220 0000 0072 1a00 0000 7229  ....r ...r....r)
-000008b0: 0000 00da 0573 706c 6974 2904 7222 0000  .....split).r"..
-000008c0: 0072 1400 0000 722f 0000 00da 086b 6579  .r....r/.....key
-000008d0: 776f 7264 7372 2300 0000 7223 0000 0072  wordsr#...r#...r
-000008e0: 2400 0000 7233 0000 0051 0000 0073 0600  $...r3...Q...s..
-000008f0: 0000 1a0b 0e01 1402 7a17 5765 6253 6372  ........z.WebScr
-00000900: 6170 6572 2e67 6574 5f6b 6579 776f 7264  aper.get_keyword
-00000910: 73da 0e73 756d 6d61 7269 7a65 5f70 6167  s..summarize_pag
-00000920: 657a 2a43 616e 2062 6520 7573 6564 2074  ez*Can be used t
-00000930: 6f20 6765 6e65 7261 7465 2061 2077 6562  o generate a web
-00000940: 2070 6167 6520 7375 6d6d 6172 7963 0200   page summaryc..
-00000950: 0000 0000 0000 0000 0000 0300 0000 0600  ................
-00000960: 0000 4300 0001 732c 0000 007c 00a0 007c  ..C...s,...|...|
-00000970: 00a0 017c 01a0 02a1 00a1 01a0 0364 01a1  ...|.........d..
-00000980: 01a1 017d 0274 047c 02a0 0564 02a1 0183  ...}.t.|...d....
-00000990: 01a0 06a1 0053 0029 034e 7227 0000 007a  .....S.).Nr'...z
-000009a0: 1247 656e 6572 6174 6520 6120 7375 6d6d  .Generate a summ
-000009b0: 6172 7929 0772 2c00 0000 721e 0000 0072  ary).r,...r....r
-000009c0: 1f00 0000 7220 0000 0072 1a00 0000 7229  ....r ...r....r)
-000009d0: 0000 0072 2d00 0000 2903 7222 0000 0072  ...r-...).r"...r
-000009e0: 1400 0000 722f 0000 0072 2300 0000 7223  ....r/...r#...r#
-000009f0: 0000 0072 2400 0000 723a 0000 0061 0000  ...r$...r:...a..
-00000a00: 0073 0400 0000 1a0b 1202 7a19 5765 6253  .s........z.WebS
-00000a10: 6372 6170 6572 2e73 756d 6d61 7269 7a65  craper.summarize
-00000a20: 5f70 6167 6572 2700 0000 da14 4750 5453  _pager'.....GPTS
-00000a30: 696d 706c 6556 6563 746f 7249 6e64 6578  impleVectorIndex
-00000a40: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
-00000a50: 0003 0000 0043 0000 0173 1e00 0000 6401  .....C...s....d.
-00000a60: 6402 6c00 6d01 7d02 6d02 7d03 0100 7c02  d.l.m.}.m.}...|.
-00000a70: 7c03 7c01 8301 6701 8301 5300 2903 4e72  |.|...g...S.).Nr
-00000a80: 0100 0000 2902 723b 0000 00da 0844 6f63  ....).r;.....Doc
-00000a90: 756d 656e 7429 035a 0b6c 6c61 6d61 5f69  ument).Z.llama_i
-00000aa0: 6e64 6578 723b 0000 0072 3c00 0000 2904  ndexr;...r<...).
-00000ab0: 7222 0000 0072 2700 0000 723b 0000 0072  r"...r'...r;...r
-00000ac0: 3c00 0000 7223 0000 0072 2300 0000 7224  <...r#...r#...r$
-00000ad0: 0000 0072 2c00 0000 7000 0000 7308 0000  ...r,...p...s...
-00000ae0: 0010 0102 0206 0106 ff7a 1b57 6562 5363  .........z.WebSc
-00000af0: 7261 7065 722e 5f74 6f5f 7665 6374 6f72  raper._to_vector
-00000b00: 5f69 6e64 6578 fa10 556e 696f 6e5b 6469  _index..Union[di
-00000b10: 6374 2c20 7374 725d 6302 0000 0000 0000  ct, str]c.......
-00000b20: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
-00000b30: 0173 5c00 0000 6401 6400 6c00 7d02 6401  .s\...d.d.l.}.d.
-00000b40: 6402 6c01 6d02 7d03 0100 7c03 8300 7d04  d.l.m.}...|...}.
-00000b50: 7c02 a003 7c01 a101 7d05 7c04 a004 6403  |...|...}.|...d.
-00000b60: 6404 6405 a103 0100 7c05 6400 7500 721f  d.d.....|.d.u.r.
-00000b70: 6406 5300 7405 a006 7c02 6a07 7c05 7c00  d.S.t...|.j.|.|.
-00000b80: a008 6407 a101 6408 7c04 6409 8d04 a101  ..d...d.|.d.....
-00000b90: 5300 290a 4e72 0100 0000 2901 da0a 7573  S.).Nr....)...us
-00000ba0: 655f 636f 6e66 6967 5a07 4445 4641 554c  e_configZ.DEFAUL
-00000bb0: 545a 1245 5854 5241 4354 494f 4e5f 5449  TZ.EXTRACTION_TI
-00000bc0: 4d45 4f55 54da 0130 7a17 6572 726f 723a  MEOUT..0z.error:
-00000bd0: 2063 616e 2774 2061 6363 6573 7320 5552   can't access UR
-00000be0: 4c72 1000 0000 722a 0000 0029 0372 1200  Lr....r*...).r..
-00000bf0: 0000 5a0d 6f75 7470 7574 5f66 6f72 6d61  ..Z.output_forma
-00000c00: 7472 1700 0000 2909 da0b 7472 6166 696c  tr....)...trafil
-00000c10: 6174 7572 615a 1474 7261 6669 6c61 7475  aturaZ.trafilatu
-00000c20: 7261 2e73 6574 7469 6e67 7372 3e00 0000  ra.settingsr>...
-00000c30: 5a09 6665 7463 685f 7572 6cda 0373 6574  Z.fetch_url..set
-00000c40: 722a 0000 0072 2b00 0000 5a07 6578 7472  r*...r+...Z.extr
-00000c50: 6163 745a 0965 6e76 5f76 616c 7565 2906  actZ.env_value).
-00000c60: 7222 0000 0072 2800 0000 7240 0000 0072  r"...r(...r@...r
-00000c70: 3e00 0000 7217 0000 005a 0470 6167 6572  >...r....Z.pager
-00000c80: 2300 0000 7223 0000 0072 2400 0000 721e  #...r#...r$...r.
-00000c90: 0000 0077 0000 0073 1e00 0000 0801 0c01  ...w...s........
-00000ca0: 0602 0a01 0e04 0802 0401 0402 0401 0201  ................
-00000cb0: 0801 0201 0201 04fc 04ff 7a15 5765 6253  ..........z.WebS
-00000cc0: 6372 6170 6572 2e5f 6c6f 6164 5f70 6167  craper._load_pag
-00000cd0: 6529 0472 1400 0000 7218 0000 0072 1900  e).r....r....r..
-00000ce0: 0000 721a 0000 0029 0472 1400 0000 7218  ..r....).r....r.
-00000cf0: 0000 0072 1900 0000 7232 0000 0029 0472  ...r....r2...).r
-00000d00: 2700 0000 721a 0000 0072 1900 0000 723b  '...r....r....r;
-00000d10: 0000 0029 0472 2800 0000 721a 0000 0072  ...).r(...r....r
-00000d20: 1900 0000 723d 0000 0029 13da 085f 5f6e  ....r=...)...__n
-00000d30: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000d40: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000d50: 0700 0000 720f 0000 00da 0f5f 5f61 6e6e  ....r......__ann
-00000d60: 6f74 6174 696f 6e73 5f5f 7212 0000 0072  otations__r....r
-00000d70: 0b00 0000 7208 0000 0072 0900 0000 721a  ....r....r....r.
-00000d80: 0000 0072 1300 0000 7226 0000 0072 3000  ...r....r&...r0.
-00000d90: 0000 7231 0000 0072 3300 0000 723a 0000  ..r1...r3...r:..
-00000da0: 0072 2c00 0000 721e 0000 0072 2300 0000  .r,...r....r#...
-00000db0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
-00000dc0: 0c00 0000 0d00 0000 73a8 0000 000a 001a  ........s.......
-00000dd0: 021a 0102 0202 0102 0102 0102 0102 0102  ................
-00000de0: 0104 fe02 0304 fc08 fd0c 0a02 0302 0102  ................
-00000df0: 0102 0102 0102 0102 0104 fe02 0304 fc08  ................
-00000e00: fd0c 0a02 0302 0102 0102 0102 0102 0102  ................
-00000e10: 0102 0104 fe02 0302 0102 0102 0104 fe02  ................
-00000e20: 0302 f804 ff08 fd0c 1002 0602 0102 0102  ................
-00000e30: 0102 0102 0102 0104 fe02 0304 fc08 fd0c  ................
-00000e40: 0a02 0502 0102 0102 0102 0102 0102 0104  ................
-00000e50: fe02 0304 fc08 fd0c 0a02 0602 0102 0102  ................
+00000510: 6c6c 5f70 6167 65da 0b73 6561 7263 685f  ll_page..search_
+00000520: 7061 6765 7a29 4361 6e20 6265 2075 7365  pagez)Can be use
+00000530: 6420 746f 2073 6561 7263 6820 6120 7370  d to search a sp
+00000540: 6563 6966 6963 2077 6562 2070 6167 65da  ecific web page.
+00000550: 0375 726c da05 7175 6572 797a 0c53 6561  .url..queryz.Sea
+00000560: 7263 6820 7175 6572 7963 0200 0000 0000  rch queryc......
+00000570: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
+00000580: 0001 733e 0000 0074 00a0 017c 01a0 02a1  ..s>...t...|....
+00000590: 00a1 017d 027c 00a0 037c 00a0 047c 0264  ...}.|...|...|.d
+000005a0: 0119 00a1 01a0 0564 02a1 01a1 017d 0374  .......d.....}.t
+000005b0: 067c 03a0 077c 0264 0319 00a1 0183 01a0  .|...|.d........
+000005c0: 08a1 0053 0029 044e 7229 0000 0072 2700  ...S.).Nr)...r'.
+000005d0: 0000 722a 0000 0029 09da 046a 736f 6eda  ..r*...)...json.
+000005e0: 056c 6f61 6473 721f 0000 00da 105f 746f  .loadsr......_to
+000005f0: 5f76 6563 746f 725f 696e 6465 7872 1e00  _vector_indexr..
+00000600: 0000 7220 0000 0072 1a00 0000 722a 0000  ..r ...r....r*..
+00000610: 00da 0573 7472 6970 2904 7222 0000 0072  ...strip).r"...r
+00000620: 1400 0000 da06 7061 7261 6d73 da05 696e  ......params..in
+00000630: 6465 7872 2300 0000 7223 0000 0072 2400  dexr#...r#...r$.
+00000640: 0000 7228 0000 002c 0000 0073 0600 0000  ..r(...,...s....
+00000650: 0e11 1a01 1602 7a16 5765 6253 6372 6170  ......z.WebScrap
+00000660: 6572 2e73 6561 7263 685f 7061 6765 da0b  er.search_page..
+00000670: 6765 745f 6175 7468 6f72 737a 2d43 616e  get_authorsz-Can
+00000680: 2062 6520 7573 6564 2074 6f20 6765 7420   be used to get 
+00000690: 6120 6c69 7374 206f 6620 7765 6220 7061  a list of web pa
+000006a0: 6765 2061 7574 686f 7273 fa09 6c69 7374  ge authors..list
+000006b0: 5b73 7472 5d63 0200 0000 0000 0000 0000  [str]c..........
+000006c0: 0000 0200 0000 0400 0000 4300 0001 7316  ..........C...s.
+000006d0: 0000 007c 00a0 007c 01a0 01a1 00a1 01a0  ...|...|........
+000006e0: 0264 01a1 0167 0153 0029 024e 5a06 6175  .d...g.S.).NZ.au
+000006f0: 7468 6f72 721d 0000 0072 2100 0000 7223  thorr....r!...r#
+00000700: 0000 0072 2300 0000 7224 0000 0072 3100  ...r#...r$...r1.
+00000710: 0000 4200 0000 7304 0000 0012 0c04 ff7a  ..B...s........z
+00000720: 1657 6562 5363 7261 7065 722e 6765 745f  .WebScraper.get_
+00000730: 6175 7468 6f72 73da 0c67 6574 5f6b 6579  authors..get_key
+00000740: 776f 7264 737a 3943 616e 2062 6520 7573  wordsz9Can be us
+00000750: 6564 2074 6f20 6765 6e65 7261 7465 2061  ed to generate a
+00000760: 206c 6973 7420 6f66 206b 6579 776f 7264   list of keyword
+00000770: 7320 666f 7220 6120 7765 6220 7061 6765  s for a web page
+00000780: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00000790: 0006 0000 0043 0000 0173 3c00 0000 7c00  .....C...s<...|.
+000007a0: a000 7c00 a001 7c01 a002 a100 a101 a003  ..|...|.........
+000007b0: 6401 a101 a101 7d02 7404 7c02 a005 6402  d.....}.t.|...d.
+000007c0: a101 8301 7d03 6403 6404 8400 7c03 a006  ....}.d.d...|...
+000007d0: 6405 a101 4400 8301 5300 2906 4e72 2700  d...D...S.).Nr'.
+000007e0: 0000 7a42 4765 6e65 7261 7465 2061 2063  ..zBGenerate a c
+000007f0: 6f6d 6d61 2d73 6570 6172 6174 6564 206c  omma-separated l
+00000800: 6973 7420 6f66 206b 6579 776f 7264 7320  ist of keywords 
+00000810: 666f 7220 7468 6520 666f 6c6c 6f77 696e  for the followin
+00000820: 6720 7465 7874 6301 0000 0000 0000 0000  g textc.........
+00000830: 0000 0002 0000 0004 0000 0053 0000 0173  ...........S...s
+00000840: 1400 0000 6700 7c00 5d06 7d01 7c01 a000  ....g.|.].}.|...
+00000850: a100 9102 7102 5300 7223 0000 0029 0172  ....q.S.r#...).r
+00000860: 2e00 0000 2902 da02 2e30 da01 7772 2300  ....)....0..wr#.
+00000870: 0000 7223 0000 0072 2400 0000 da0a 3c6c  ..r#...r$.....<l
+00000880: 6973 7463 6f6d 703e 5f00 0000 7302 0000  istcomp>_...s...
+00000890: 0014 007a 2b57 6562 5363 7261 7065 722e  ...z+WebScraper.
+000008a0: 6765 745f 6b65 7977 6f72 6473 2e3c 6c6f  get_keywords.<lo
+000008b0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000008c0: fa01 2c29 0772 2d00 0000 721e 0000 0072  ..,).r-...r....r
+000008d0: 1f00 0000 7220 0000 0072 1a00 0000 722a  ....r ...r....r*
+000008e0: 0000 00da 0573 706c 6974 2904 7222 0000  .....split).r"..
+000008f0: 0072 1400 0000 7230 0000 00da 086b 6579  .r....r0.....key
+00000900: 776f 7264 7372 2300 0000 7223 0000 0072  wordsr#...r#...r
+00000910: 2400 0000 7233 0000 0051 0000 0073 0600  $...r3...Q...s..
+00000920: 0000 1a0b 0e01 1402 7a17 5765 6253 6372  ........z.WebScr
+00000930: 6170 6572 2e67 6574 5f6b 6579 776f 7264  aper.get_keyword
+00000940: 73da 0e73 756d 6d61 7269 7a65 5f70 6167  s..summarize_pag
+00000950: 657a 2a43 616e 2062 6520 7573 6564 2074  ez*Can be used t
+00000960: 6f20 6765 6e65 7261 7465 2061 2077 6562  o generate a web
+00000970: 2070 6167 6520 7375 6d6d 6172 7963 0200   page summaryc..
+00000980: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00000990: 0000 4300 0001 732c 0000 007c 00a0 007c  ..C...s,...|...|
+000009a0: 00a0 017c 01a0 02a1 00a1 01a0 0364 01a1  ...|.........d..
+000009b0: 01a1 017d 0274 047c 02a0 0564 02a1 0183  ...}.t.|...d....
+000009c0: 01a0 06a1 0053 0029 034e 7227 0000 007a  .....S.).Nr'...z
+000009d0: 1247 656e 6572 6174 6520 6120 7375 6d6d  .Generate a summ
+000009e0: 6172 7929 0772 2d00 0000 721e 0000 0072  ary).r-...r....r
+000009f0: 1f00 0000 7220 0000 0072 1a00 0000 722a  ....r ...r....r*
+00000a00: 0000 0072 2e00 0000 2903 7222 0000 0072  ...r....).r"...r
+00000a10: 1400 0000 7230 0000 0072 2300 0000 7223  ....r0...r#...r#
+00000a20: 0000 0072 2400 0000 723a 0000 0061 0000  ...r$...r:...a..
+00000a30: 0073 0400 0000 1a0b 1202 7a19 5765 6253  .s........z.WebS
+00000a40: 6372 6170 6572 2e73 756d 6d61 7269 7a65  craper.summarize
+00000a50: 5f70 6167 6572 2700 0000 da14 4750 5453  _pager'.....GPTS
+00000a60: 696d 706c 6556 6563 746f 7249 6e64 6578  impleVectorIndex
+00000a70: 6302 0000 0000 0000 0000 0000 0004 0000  c...............
+00000a80: 0003 0000 0043 0000 0173 1e00 0000 6401  .....C...s....d.
+00000a90: 6402 6c00 6d01 7d02 6d02 7d03 0100 7c02  d.l.m.}.m.}...|.
+00000aa0: 7c03 7c01 8301 6701 8301 5300 2903 4e72  |.|...g...S.).Nr
+00000ab0: 0100 0000 2902 723b 0000 00da 0844 6f63  ....).r;.....Doc
+00000ac0: 756d 656e 7429 035a 0b6c 6c61 6d61 5f69  ument).Z.llama_i
+00000ad0: 6e64 6578 723b 0000 0072 3c00 0000 2904  ndexr;...r<...).
+00000ae0: 7222 0000 0072 2700 0000 723b 0000 0072  r"...r'...r;...r
+00000af0: 3c00 0000 7223 0000 0072 2300 0000 7224  <...r#...r#...r$
+00000b00: 0000 0072 2d00 0000 7000 0000 7308 0000  ...r-...p...s...
+00000b10: 0010 0102 0206 0106 ff7a 1b57 6562 5363  .........z.WebSc
+00000b20: 7261 7065 722e 5f74 6f5f 7665 6374 6f72  raper._to_vector
+00000b30: 5f69 6e64 6578 fa10 556e 696f 6e5b 6469  _index..Union[di
+00000b40: 6374 2c20 7374 725d 6302 0000 0000 0000  ct, str]c.......
+00000b50: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
+00000b60: 0173 5c00 0000 6401 6400 6c00 7d02 6401  .s\...d.d.l.}.d.
+00000b70: 6402 6c01 6d02 7d03 0100 7c03 8300 7d04  d.l.m.}...|...}.
+00000b80: 7c02 a003 7c01 a101 7d05 7c04 a004 6403  |...|...}.|...d.
+00000b90: 6404 6405 a103 0100 7c05 6400 7500 721f  d.d.....|.d.u.r.
+00000ba0: 6406 5300 7405 a006 7c02 6a07 7c05 7c00  d.S.t...|.j.|.|.
+00000bb0: a008 6407 a101 6408 7c04 6409 8d04 a101  ..d...d.|.d.....
+00000bc0: 5300 290a 4e72 0100 0000 2901 da0a 7573  S.).Nr....)...us
+00000bd0: 655f 636f 6e66 6967 5a07 4445 4641 554c  e_configZ.DEFAUL
+00000be0: 545a 1245 5854 5241 4354 494f 4e5f 5449  TZ.EXTRACTION_TI
+00000bf0: 4d45 4f55 54da 0130 7a17 6572 726f 723a  MEOUT..0z.error:
+00000c00: 2063 616e 2774 2061 6363 6573 7320 5552   can't access UR
+00000c10: 4c72 1000 0000 722b 0000 0029 0372 1200  Lr....r+...).r..
+00000c20: 0000 5a0d 6f75 7470 7574 5f66 6f72 6d61  ..Z.output_forma
+00000c30: 7472 1700 0000 2909 da0b 7472 6166 696c  tr....)...trafil
+00000c40: 6174 7572 615a 1474 7261 6669 6c61 7475  aturaZ.trafilatu
+00000c50: 7261 2e73 6574 7469 6e67 7372 3e00 0000  ra.settingsr>...
+00000c60: 5a09 6665 7463 685f 7572 6cda 0373 6574  Z.fetch_url..set
+00000c70: 722b 0000 0072 2c00 0000 5a07 6578 7472  r+...r,...Z.extr
+00000c80: 6163 745a 0965 6e76 5f76 616c 7565 2906  actZ.env_value).
+00000c90: 7222 0000 0072 2900 0000 7240 0000 0072  r"...r)...r@...r
+00000ca0: 3e00 0000 7217 0000 005a 0470 6167 6572  >...r....Z.pager
+00000cb0: 2300 0000 7223 0000 0072 2400 0000 721e  #...r#...r$...r.
+00000cc0: 0000 0077 0000 0073 1e00 0000 0801 0c01  ...w...s........
+00000cd0: 0602 0a01 0e04 0802 0401 0402 0401 0201  ................
+00000ce0: 0801 0201 0201 04fc 04ff 7a15 5765 6253  ..........z.WebS
+00000cf0: 6372 6170 6572 2e5f 6c6f 6164 5f70 6167  craper._load_pag
+00000d00: 6529 0472 1400 0000 7218 0000 0072 1900  e).r....r....r..
+00000d10: 0000 721a 0000 0029 0472 1400 0000 7218  ..r....).r....r.
+00000d20: 0000 0072 1900 0000 7232 0000 0029 0472  ...r....r2...).r
+00000d30: 2700 0000 721a 0000 0072 1900 0000 723b  '...r....r....r;
+00000d40: 0000 0029 0472 2900 0000 721a 0000 0072  ...).r)...r....r
+00000d50: 1900 0000 723d 0000 0029 13da 085f 5f6e  ....r=...)...__n
+00000d60: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000d70: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+00000d80: 0700 0000 720f 0000 00da 0f5f 5f61 6e6e  ....r......__ann
+00000d90: 6f74 6174 696f 6e73 5f5f 7212 0000 0072  otations__r....r
+00000da0: 0b00 0000 7208 0000 0072 0900 0000 721a  ....r....r....r.
+00000db0: 0000 0072 1300 0000 7226 0000 0072 2800  ...r....r&...r(.
+00000dc0: 0000 7231 0000 0072 3300 0000 723a 0000  ..r1...r3...r:..
+00000dd0: 0072 2d00 0000 721e 0000 0072 2300 0000  .r-...r....r#...
+00000de0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
+00000df0: 0c00 0000 0d00 0000 73a8 0000 000a 001a  ........s.......
+00000e00: 021a 0102 0202 0102 0102 0102 0102 0102  ................
+00000e10: 0104 fe02 0304 fc08 fd0c 0a02 0302 0102  ................
+00000e20: 0102 0102 0102 0102 0104 fe02 0304 fc08  ................
+00000e30: fd0c 0a02 0302 0102 0102 0102 0102 0102  ................
+00000e40: 0102 0104 fe02 0302 0102 0102 0104 fe02  ................
+00000e50: 0302 f804 ff08 fd0c 1002 0602 0102 0102  ................
 00000e60: 0102 0102 0102 0104 fe02 0304 fc08 fd0c  ................
-00000e70: 0a0a 050e 0772 0c00 0000 2912 5a0a 5f5f  .....r....).Z.__
-00000e80: 6675 7475 7265 5f5f 7202 0000 00da 0674  future__r......t
-00000e90: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
-00000ea0: 2a00 0000 7205 0000 00da 0461 7474 7272  *...r......attrr
-00000eb0: 0600 0000 7207 0000 005a 0673 6368 656d  ....r....Z.schem
-00000ec0: 6172 0800 0000 7209 0000 005a 0d67 7269  ar....r....Z.gri
-00000ed0: 7074 6170 652e 636f 7265 720a 0000 0072  ptape.corer....r
-00000ee0: 0b00 0000 723b 0000 0072 0c00 0000 7223  ....r;...r....r#
-00000ef0: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00000f00: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000f10: 7316 0000 000c 0010 0108 010c 0110 0110  s...............
-00000f20: 0110 0104 0208 0102 0316 01              ...........
+00000e70: 0a02 0502 0102 0102 0102 0102 0102 0104  ................
+00000e80: fe02 0304 fc08 fd0c 0a02 0602 0102 0102  ................
+00000e90: 0102 0102 0102 0104 fe02 0304 fc08 fd0c  ................
+00000ea0: 0a0a 050e 0772 0c00 0000 2912 5a0a 5f5f  .....r....).Z.__
+00000eb0: 6675 7475 7265 5f5f 7202 0000 00da 0674  future__r......t
+00000ec0: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
+00000ed0: 2b00 0000 7205 0000 00da 0461 7474 7272  +...r......attrr
+00000ee0: 0600 0000 7207 0000 005a 0673 6368 656d  ....r....Z.schem
+00000ef0: 6172 0800 0000 7209 0000 005a 0d67 7269  ar....r....Z.gri
+00000f00: 7074 6170 652e 636f 7265 720a 0000 0072  ptape.corer....r
+00000f10: 0b00 0000 723b 0000 0072 0c00 0000 7223  ....r;...r....r#
+00000f20: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
+00000f30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000f40: 7316 0000 000c 0010 0108 010c 0110 0110  s...............
+00000f50: 0110 0104 0208 0102 0316 01              ...........
```

### Comparing `griptape_tools-0.5.0/griptape/tools/web_scraper/__pycache__/tool.cpython-39.pyc` & `griptape_tools-0.5.1/griptape/tools/web_scraper/__pycache__/tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/web_scraper/tool.py` & `griptape_tools-0.5.1/griptape/tools/web_scraper/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/tool.cpython-310.pyc` & `griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/web_search/__pycache__/tool.cpython-39.pyc` & `griptape_tools-0.5.1/griptape/tools/web_search/__pycache__/tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/griptape/tools/web_search/tool.py` & `griptape_tools-0.5.1/griptape/tools/web_search/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.0/pyproject.toml` & `griptape_tools-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.5.0"
+version = "0.5.1"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape-core = ">=0.6.0"
+griptape-core = ">=0.7.2"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
```

### Comparing `griptape_tools-0.5.0/PKG-INFO` & `griptape_tools-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape-core (>=0.6.0)
+Requires-Dist: griptape-core (>=0.7.2)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # Griptape Tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
```

