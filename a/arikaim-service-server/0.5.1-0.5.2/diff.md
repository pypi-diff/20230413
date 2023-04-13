# Comparing `tmp/arikaim service server-0.5.1.tar.gz` & `tmp/arikaim_service_server-0.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arikaim service server-0.5.1.tar", last modified: Wed Feb 15 12:32:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

