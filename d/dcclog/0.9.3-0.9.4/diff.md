# Comparing `tmp/dcclog-0.9.3-py3-none-any.whl.zip` & `tmp/dcclog-0.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 11544 bytes, number of entries: 18
+Zip file size: 12236 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      773 b- defN 23-Mar-05 14:41 dcclog/__init__.py
 -rw-r--r--  2.0 unx      349 b- defN 23-Jan-22 15:25 dcclog/colors.py
 -rw-r--r--  2.0 unx     2590 b- defN 23-Feb-08 21:27 dcclog/formatters.py
 -rw-r--r--  2.0 unx     2212 b- defN 23-Feb-03 15:45 dcclog/handlers.py
 -rw-r--r--  2.0 unx     1791 b- defN 23-Mar-05 14:40 dcclog/logger.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-18 19:46 dcclog/py.typed
--rw-r--r--  2.0 unx      527 b- defN 23-Jan-28 16:14 dcclog/reader.py
+-rw-r--r--  2.0 unx     1668 b- defN 23-Mar-16 23:19 dcclog/reader.py
 -rw-r--r--  2.0 unx      806 b- defN 23-Jan-26 11:21 dcclog/utils.py
 -rw-r--r--  2.0 unx     3294 b- defN 23-Feb-08 21:27 dcclog/wrapper.py
 -rw-r--r--  2.0 unx     1780 b- defN 23-Jan-31 12:55 dcclog/cipher/__init__.py
 -rw-r--r--  2.0 unx     2030 b- defN 23-Feb-03 20:06 dcclog/cipher/aes.py
 -rw-r--r--  2.0 unx     2168 b- defN 23-Jan-31 12:56 dcclog/cipher/chacha.py
 -rw-r--r--  2.0 unx     2114 b- defN 23-Feb-04 21:07 dcclog/cipher/rsa.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Mar-12 15:39 dcclog-0.9.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2388 b- defN 23-Mar-12 15:39 dcclog-0.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-12 15:39 dcclog-0.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-12 15:39 dcclog-0.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1353 b- defN 23-Mar-12 15:39 dcclog-0.9.3.dist-info/RECORD
-18 files, 25346 bytes uncompressed, 9368 bytes compressed:  63.0%
+-rw-r--r--  2.0 unx     1072 b- defN 23-Mar-16 23:21 dcclog-0.9.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2388 b- defN 23-Mar-16 23:21 dcclog-0.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-16 23:21 dcclog-0.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Mar-16 23:21 dcclog-0.9.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Mar-16 23:21 dcclog-0.9.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1448 b- defN 23-Mar-16 23:21 dcclog-0.9.4.dist-info/RECORD
+19 files, 26641 bytes uncompressed, 9906 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -33,23 +33,26 @@
 
 Filename: dcclog/cipher/chacha.py
 Comment: 
 
 Filename: dcclog/cipher/rsa.py
 Comment: 
 
-Filename: dcclog-0.9.3.dist-info/LICENSE
+Filename: dcclog-0.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: dcclog-0.9.3.dist-info/METADATA
+Filename: dcclog-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: dcclog-0.9.3.dist-info/WHEEL
+Filename: dcclog-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: dcclog-0.9.3.dist-info/top_level.txt
+Filename: dcclog-0.9.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: dcclog-0.9.3.dist-info/RECORD
+Filename: dcclog-0.9.4.dist-info/top_level.txt
+Comment: 
+
+Filename: dcclog-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dcclog/reader.py

```diff
@@ -11,7 +11,42 @@
                 if cipher:
                     try:
                         yield cipher.decrypt(message)
                     except ValueError:
                         pass
                 else:
                     yield message
+
+
+def main() -> int:
+    import argparse
+    from pathlib import Path
+
+    def _parse_log_files(
+        keyfile: Path, logs_dir: Path, filter_: str, expand: bool
+    ) -> None:
+        from dcclog.cipher.rsa import RSAEncryption
+
+        cipher = RSAEncryption(keyfile.as_posix())
+        for file in logs_dir.glob("*.log*"):
+            print(f"\n============ LOG FILE {file.name} ============\n")
+            for log in read_log(file.as_posix(), cipher):
+                if filter_ in log:
+                    print(log.replace("\\n\t", "\n") if expand else log)
+
+    arg_parser = argparse.ArgumentParser()
+    arg_parser.add_argument("-k", "--key", required=True, type=Path)
+    arg_parser.add_argument("-l", "--logs-dir", required=True, type=Path)
+    arg_parser.add_argument("-f", "--filter", default="", type=str)
+    arg_parser.add_argument(
+        "--expand", default=True, action=argparse.BooleanOptionalAction
+    )
+    args = arg_parser.parse_args()
+    _parse_log_files(
+        args.key.resolve(), args.logs_dir.resolve(), args.filter, args.expand
+    )
+
+    return 0
+
+
+if __name__ == "__main__":
+    raise SystemExit(main())
```

## Comparing `dcclog-0.9.3.dist-info/LICENSE` & `dcclog-0.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dcclog-0.9.3.dist-info/METADATA` & `dcclog-0.9.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcclog
-Version: 0.9.3
+Version: 0.9.4
 Summary: Logging package with color and encryption support
 Author-email: jamazi <jamazi@tutanota.com>
 Project-URL: Homepage, https://github.com/jamazi/dcclog
 Project-URL: Bug Tracker, https://github.com/jamazi/dcclog/issues
 Keywords: log
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `dcclog-0.9.3.dist-info/RECORD` & `dcclog-0.9.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 dcclog/__init__.py,sha256=UGl_bbyyjTuwmw9R6p4kO2Jy5m84SH4yiWLQLg0B5J0,773
 dcclog/colors.py,sha256=jvuFtizdHF4u0O7jMJ9QN--vmE5xy37J3Cb2BwCyhTc,349
 dcclog/formatters.py,sha256=wLZls2LpO7uX0Jdl2AnPXAV41TM-cxG9nmUBv_3-ruQ,2590
 dcclog/handlers.py,sha256=WcEK91uNXiXUPWobs8JdwH0VNgH5PZiDOE_j3cLFsts,2212
 dcclog/logger.py,sha256=epVFTkg9Twe9MQTXTIhxJ_f5TEt_TXT4lW4_LcQekxM,1791
 dcclog/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dcclog/reader.py,sha256=eKLGJdGFnpnFW_HtQG30IEekVz0TICDB_XfdMolObac,527
+dcclog/reader.py,sha256=UlYrCG6yCRW6sklSHGc1yozJ8IqXJ6nI9k1PJV9WqZM,1668
 dcclog/utils.py,sha256=h0rF361wsQM8J07mzicfMHWXK8PWzn1zFSjjubDuKio,806
 dcclog/wrapper.py,sha256=F4XiYUwQ6TjkbcVFPeiQZBLfB_Pizwlvd-cDKH0xA4E,3294
 dcclog/cipher/__init__.py,sha256=CrxEn7mviGOrRR2xXBbH3GZuDV6NrSeM-GYvfWxxpnM,1780
 dcclog/cipher/aes.py,sha256=YbvLBfndukqFp18EXFkLxITZTkPmM7TLYR04zT7ff7Y,2030
 dcclog/cipher/chacha.py,sha256=B2AaspZ8LY38nZVKVVIFctwA4d7XPtoPGlt5qQvSoWM,2168
 dcclog/cipher/rsa.py,sha256=c9nfE_hUWTvFQwXqobd5WI8uOW9odadMOu6jvP-3Pls,2114
-dcclog-0.9.3.dist-info/LICENSE,sha256=td_TlLS2jUN5g6N7TjnV8ubpI0K3ibe7-C0q2J-Bb-4,1072
-dcclog-0.9.3.dist-info/METADATA,sha256=hKbf5PE1OA6urEwKBH_CtxHxZAEuB7OU_TST2MQaub8,2388
-dcclog-0.9.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dcclog-0.9.3.dist-info/top_level.txt,sha256=QfeSnKmDAjqvNGhKBYUfxJcwG03knJAffrYt6M8PJM4,7
-dcclog-0.9.3.dist-info/RECORD,,
+dcclog-0.9.4.dist-info/LICENSE,sha256=td_TlLS2jUN5g6N7TjnV8ubpI0K3ibe7-C0q2J-Bb-4,1072
+dcclog-0.9.4.dist-info/METADATA,sha256=JQjIeNI7thPW6fTAZLv-iHGejCnbLNah48b2cPbmhCI,2388
+dcclog-0.9.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+dcclog-0.9.4.dist-info/entry_points.txt,sha256=AX1zZuvobNNYzZvFz5y3EUjA5YW67LoMgRZT4ndLI0w,59
+dcclog-0.9.4.dist-info/top_level.txt,sha256=QfeSnKmDAjqvNGhKBYUfxJcwG03knJAffrYt6M8PJM4,7
+dcclog-0.9.4.dist-info/RECORD,,
```

