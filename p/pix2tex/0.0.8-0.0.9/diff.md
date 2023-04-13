# Comparing `tmp/pix2tex-0.0.8.tar.gz` & `tmp/pix2tex-0.0.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pix2tex-0.0.8.tar", last modified: Wed Apr 13 19:32:28 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

