# Comparing `tmp/p-ttauto-crawler-0.0.2.tar.gz` & `tmp/p_ttauto_crawler-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.0.2.tar", last modified: Tue Apr 11 08:11:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

