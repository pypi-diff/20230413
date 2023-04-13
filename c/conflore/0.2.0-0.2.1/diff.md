# Comparing `tmp/conflore-0.2.0-py3-none-any.whl.zip` & `tmp/conflore-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 2601 bytes, number of entries: 6
+Zip file size: 3459 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       31 b- defN 80-Jan-01 00:00 conflore/__init__.py
--rw-r--r--  2.0 unx     2444 b- defN 80-Jan-01 00:00 conflore/conflore.py
+-rw-r--r--  2.0 unx     1504 b- defN 80-Jan-01 00:00 conflore/cache.py
+-rw-r--r--  2.0 unx     3119 b- defN 80-Jan-01 00:00 conflore/conflore.py
 -rw-r--r--  2.0 unx     1208 b- defN 80-Jan-01 00:00 conflore/load_and_dump.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 conflore-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 conflore-0.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      442 b- defN 16-Jan-01 00:00 conflore-0.2.0.dist-info/RECORD
-6 files, 4773 bytes uncompressed, 1805 bytes compressed:  62.2%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 conflore-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 conflore-0.2.1.dist-info/METADATA
+?rw-r--r--  2.0 unx      516 b- defN 16-Jan-01 00:00 conflore-0.2.1.dist-info/RECORD
+7 files, 7026 bytes uncompressed, 2553 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: conflore/__init__.py
 Comment: 
 
+Filename: conflore/cache.py
+Comment: 
+
 Filename: conflore/conflore.py
 Comment: 
 
 Filename: conflore/load_and_dump.py
 Comment: 
 
-Filename: conflore-0.2.0.dist-info/WHEEL
+Filename: conflore-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: conflore-0.2.0.dist-info/METADATA
+Filename: conflore-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: conflore-0.2.0.dist-info/RECORD
+Filename: conflore-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## conflore/conflore.py

```diff
@@ -8,26 +8,45 @@
 
 class Conflore:
     _data: dict
     _file: str
     _on_save_callbacks: t.Dict[str, t.Callable[[], t.Any]]
     _anonymous_callbacks: t.List[t.Callable[[], t.Any]]
     
-    def __init__(self, file: str, default: dict = None, auto_save=False):
+    def __init__(
+            self,
+            file: str,
+            default: dict = None,
+            auto_save=False,
+            **kwargs
+    ):
         """
         args:
             file: json, yaml, or pickle file.
+        kwargs:
+            version_number (int): if number is newer than the one in the file,
+                the file will be dropped.
         """
         self._anonymous_callbacks = []
         self._data = loads(file) if exists(file) else {}
         self._file = file
         self._on_save_callbacks = {}
         
-        if default and not exists(file):  # init
-            self._data.update(default)
+        if exists(file):
+            if v1 := kwargs.get('version_number'):
+                v0 = self._data.get('__conflore_version__', 0)
+                if v1 > v0:
+                    print(':p', f'auto drop config file "{file}" ({v1} > {v0})')
+                    self._data = {'__conflore_version__': v1, **(default or {})}
+                # else: do nothing
+            # else: do nothing
+        else:
+            self._data['__conflore_version__'] = kwargs.get('version_number', 0)
+            if default: self._data.update(default)
+        
         if auto_save:
             atexit.register(self.save)
     
     def __getitem__(self, item):
         return self._data[item]
     
     def __iter__(self):
```

## Comparing `conflore-0.2.0.dist-info/METADATA` & `conflore-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conflore
-Version: 0.2.0
+Version: 0.2.1
 Summary: Load and save configurations in a simple way.
 License: MIT
 Author: likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

