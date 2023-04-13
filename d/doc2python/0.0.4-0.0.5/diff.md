# Comparing `tmp/doc2python-0.0.4.tar.gz` & `tmp/doc2python-0.0.5.tar.gz`

## Comparing `doc2python-0.0.4.tar` & `doc2python-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 doc2python-0.0.4/config.pypirc
--rw-r--r--   0        0        0   333312 2020-02-02 00:00:00.000000 doc2python-0.0.4/test.doc
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 doc2python-0.0.4/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doc2python-0.0.4/src/doc2python/__init__.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 doc2python-0.0.4/src/doc2python/reader.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 doc2python-0.0.4/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 doc2python-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doc2python-0.0.4/README.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 doc2python-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 doc2python-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 doc2python-0.0.5/config.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doc2python-0.0.5/src/doc2python/__init__.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 doc2python-0.0.5/src/doc2python/reader.py
+-rw-r--r--   0        0        0   333312 2020-02-02 00:00:00.000000 doc2python-0.0.5/tests/test.doc
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 doc2python-0.0.5/tests/test.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 doc2python-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 doc2python-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 doc2python-0.0.5/README.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 doc2python-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 doc2python-0.0.5/PKG-INFO
```

### Comparing `doc2python-0.0.4/test.doc` & `doc2python-0.0.5/tests/test.doc`

 * *Files identical despite different names*

### Comparing `doc2python-0.0.4/src/doc2python/reader.py` & `doc2python-0.0.5/src/doc2python/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Union
 from pathlib import Path
 
-class reader:
-    def toString(path:Union[Path,str])->str:
-        
-        special_chars = {
+def toString(path:Union[Path,str])->str:    
+    special_chars = {
                 "b'\\t'": '\t',
                 "b'\\r'": '\n',
                 "b'\\x07'": '|',
                 "b'\\xc4'": 'Ä',
                 "b'\\xe4'": 'ä',
                 "b'\\xdc'": 'Ü',
                 "b'\\xfc'": 'ü',
@@ -27,16 +25,17 @@
                 "b' '": " ",
                 "b'.'": ".",
                 "b':'": ":",
                 "b'/'": "/",
                 "b'('": "(",
                 "b')'": ")",
             }
+    return _get_string(special_chars,path)
 
-        def _get_string(special_chars:dict,path:Union[Path,str])->str:
+def _get_string(special_chars:dict,path:Union[Path,str])->str:
             string = ''
             with open(path, 'rb') as stream:
                 stream.seek(2560) # Offset - text starts after byte 2560
                 current_stream = stream.read(1)
                 while not (str(current_stream) == "b'\\xfa'"):
                     if str(current_stream) in special_chars.keys():
                         string += special_chars[str(current_stream)]
@@ -45,9 +44,8 @@
                             char = current_stream.decode('UTF-8')
                             if char.isalnum():
                                 string += char
                         except UnicodeDecodeError:
                             string += ''
                             print(str(current_stream))
                     current_stream = stream.read(1)
-                return string
-        return _get_string(special_chars,path)
+                return string
```

### Comparing `doc2python-0.0.4/.gitignore` & `doc2python-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `doc2python-0.0.4/LICENSE` & `doc2python-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `doc2python-0.0.4/pyproject.toml` & `doc2python-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "doc2python"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Julian Mecking", email="jmeck2013@gmail.com" },
 ]
 description = "A simple .doc to string converter for python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

