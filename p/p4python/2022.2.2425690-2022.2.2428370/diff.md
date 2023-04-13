# Comparing `tmp/p4python-2022.2.2425690.tar.gz` & `tmp/p4python-2022.2.2428370-cp38-cp38-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\p4python-2022.2.2425690.tar", last modified: Tue Apr  4 14:52:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

