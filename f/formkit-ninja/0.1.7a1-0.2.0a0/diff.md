# Comparing `tmp/formkit_ninja-0.1.7a1.tar.gz` & `tmp/formkit_ninja-0.2.0a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.1.7a1.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

