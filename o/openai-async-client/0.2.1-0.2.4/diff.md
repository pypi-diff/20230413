# Comparing `tmp/openai-async-client-0.2.1.tar.gz` & `tmp/openai_async_client-0.2.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openai-async-client-0.2.1.tar", last modified: Fri Mar 24 21:03:06 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

