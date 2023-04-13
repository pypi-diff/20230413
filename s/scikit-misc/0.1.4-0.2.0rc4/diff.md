# Comparing `tmp/scikit-misc-0.1.4.tar.gz` & `tmp/scikit_misc-0.2.0rc4-cp39-cp39-macosx_12_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-misc-0.1.4.tar", last modified: Thu May  6 13:42:05 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

