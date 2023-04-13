# Comparing `tmp/ezQgd-0.0.0.2.tar.gz` & `tmp/ezQgd-0.0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezQgd-0.0.0.2.tar", last modified: Tue Mar 14 11:37:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

