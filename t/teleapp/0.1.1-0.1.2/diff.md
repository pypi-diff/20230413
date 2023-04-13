# Comparing `tmp/teleapp-0.1.1-cp38-cp38-manylinux1_x86_64.whl.zip` & `tmp/teleapp-0.1.2-cp36-cp36m-manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 30048 bytes, number of entries: 11
+Zip file size: 104855 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-02 04:47 teleapp/__init__.py
--rw-rw-r--  2.0 unx      262 b- defN 23-Mar-02 06:08 teleapp/teleapp.py
+-rw-rw-r--  2.0 unx      354 b- defN 23-Apr-13 03:33 teleapp/teleapp.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-02 04:47 teleapp/cmd/__init__.py
--rwxrwxr-x  2.0 unx    55648 b- defN 23-Mar-02 09:41 teleapp/cmd/cmd.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x  2.0 unx   241040 b- defN 23-Apr-13 08:36 teleapp/cmd/cmd.cpython-36m-aarch64-linux-gnu.so
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-02 04:47 teleapp/const/__init__.py
--rwxrwxr-x  2.0 unx    28352 b- defN 23-Mar-02 09:41 teleapp/const/click_setting.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx      480 b- defN 23-Mar-02 09:41 teleapp-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      108 b- defN 23-Mar-02 09:41 teleapp-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       48 b- defN 23-Mar-02 09:41 teleapp-0.1.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Mar-02 09:41 teleapp-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      915 b- defN 23-Mar-02 09:41 teleapp-0.1.1.dist-info/RECORD
-11 files, 85821 bytes uncompressed, 28476 bytes compressed:  66.8%
+-rwxrwxr-x  2.0 unx    59240 b- defN 23-Apr-13 08:36 teleapp/const/click_setting.cpython-36m-aarch64-linux-gnu.so
+-rw-rw-r--  2.0 unx      535 b- defN 23-Apr-13 08:36 teleapp-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      113 b- defN 23-Apr-13 08:36 teleapp-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       49 b- defN 23-Apr-13 08:36 teleapp-0.1.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-13 08:36 teleapp-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      920 b- defN 23-Apr-13 08:36 teleapp-0.1.2.dist-info/RECORD
+11 files, 302259 bytes uncompressed, 103275 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -3,32 +3,32 @@
 
 Filename: teleapp/teleapp.py
 Comment: 
 
 Filename: teleapp/cmd/__init__.py
 Comment: 
 
-Filename: teleapp/cmd/cmd.cpython-38-x86_64-linux-gnu.so
+Filename: teleapp/cmd/cmd.cpython-36m-aarch64-linux-gnu.so
 Comment: 
 
 Filename: teleapp/const/__init__.py
 Comment: 
 
-Filename: teleapp/const/click_setting.cpython-38-x86_64-linux-gnu.so
+Filename: teleapp/const/click_setting.cpython-36m-aarch64-linux-gnu.so
 Comment: 
 
-Filename: teleapp-0.1.1.dist-info/METADATA
+Filename: teleapp-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: teleapp-0.1.1.dist-info/WHEEL
+Filename: teleapp-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: teleapp-0.1.1.dist-info/entry_points.txt
+Filename: teleapp-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: teleapp-0.1.1.dist-info/top_level.txt
+Filename: teleapp-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: teleapp-0.1.1.dist-info/RECORD
+Filename: teleapp-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teleapp/teleapp.py

```diff
@@ -6,9 +6,10 @@
 
 @click.group()
 def cli():
     pass
 
 
 @cli.command('start', short_help='teleapp start', context_settings=CONTEXT_SETTINGS)
-def start():
-    start_cmd()
+@click.option('--config', '-c', type=str, default='', help='model path config')
+def start(config):
+    start_cmd(config)
```

