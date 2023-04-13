# Comparing `tmp/pm4pyminimal-2.7.2.tar.gz` & `tmp/pm4pyminimal-2.7.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm4pyminimal-2.7.2.tar", last modified: Mon Apr  3 09:39:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

