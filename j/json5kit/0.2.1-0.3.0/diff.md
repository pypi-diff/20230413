# Comparing `tmp/json5kit-0.2.1.tar.gz` & `tmp/json5kit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json5kit-0.2.1.tar", last modified: Sun Sep 11 21:52:52 2022, max compression
+gzip compressed data, was "json5kit-0.3.0.tar", last modified: Thu Apr 13 21:51:33 2023, max compression
```

## Comparing `json5kit-0.2.1.tar` & `json5kit-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2022-09-11 21:52:52.722999 json5kit-0.2.1/
--rw-rw-r--   0 tushar    (1000) tushar    (1000)     1072 2022-04-14 08:01:42.000000 json5kit-0.2.1/LICENSE
--rw-rw-r--   0 tushar    (1000) tushar    (1000)     2133 2022-09-11 21:52:52.722999 json5kit-0.2.1/PKG-INFO
--rw-rw-r--   0 tushar    (1000) tushar    (1000)     1255 2022-09-11 21:52:04.000000 json5kit-0.2.1/README.md
--rw-rw-r--   0 tushar    (1000) tushar    (1000)     1170 2022-09-11 21:52:52.726999 json5kit-0.2.1/setup.cfg
--rw-rw-r--   0 tushar    (1000) tushar    (1000)       38 2022-04-14 08:01:42.000000 json5kit-0.2.1/setup.py
-drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2022-09-11 21:52:52.722999 json5kit-0.2.1/src/
-drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2022-09-11 21:52:52.722999 json5kit-0.2.1/src/json5kit/
--rw-rw-r--   0 tushar    (1000) tushar    (1000)    11317 2022-09-11 20:55:30.000000 json5kit-0.2.1/src/json5kit/__init__.py
--rw-rw-r--   0 tushar    (1000) tushar    (1000)     6520 2022-09-11 21:52:04.000000 json5kit-0.2.1/src/json5kit/nodes.py
-drwxrwxr-x   0 tushar    (1000) tushar    (1000)        0 2022-09-11 21:52:52.722999 json5kit-0.2.1/src/json5kit.egg-info/
--rw-rw-r--   0 tushar    (1000) tushar    (1000)     2133 2022-09-11 21:52:52.000000 json5kit-0.2.1/src/json5kit.egg-info/PKG-INFO
--rw-rw-r--   0 tushar    (1000) tushar    (1000)      262 2022-09-11 21:52:52.000000 json5kit-0.2.1/src/json5kit.egg-info/SOURCES.txt
--rw-rw-r--   0 tushar    (1000) tushar    (1000)        1 2022-09-11 21:52:52.000000 json5kit-0.2.1/src/json5kit.egg-info/dependency_links.txt
--rw-rw-r--   0 tushar    (1000) tushar    (1000)       29 2022-09-11 21:52:52.000000 json5kit-0.2.1/src/json5kit.egg-info/requires.txt
--rw-rw-r--   0 tushar    (1000) tushar    (1000)        9 2022-09-11 21:52:52.000000 json5kit-0.2.1/src/json5kit.egg-info/top_level.txt
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.727327 json5kit-0.3.0/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1072 2023-04-13 16:58:14.000000 json5kit-0.3.0/LICENSE
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-13 21:51:33.727432 json5kit-0.3.0/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1415 2023-04-13 21:46:23.000000 json5kit-0.3.0/README.md
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     1170 2023-04-13 21:51:33.727888 json5kit-0.3.0/setup.cfg
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       38 2023-04-13 16:58:14.000000 json5kit-0.3.0/setup.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.725056 json5kit-0.3.0/src/
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.726347 json5kit-0.3.0/src/json5kit/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)    11763 2023-04-13 21:33:38.000000 json5kit-0.3.0/src/json5kit/__init__.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     7225 2023-04-13 21:43:51.000000 json5kit-0.3.0/src/json5kit/nodes.py
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     3629 2023-04-13 21:44:53.000000 json5kit-0.3.0/src/json5kit/visitor.py
+drwxr-xr-x   0 tusharsadhwani   (501) staff       (20)        0 2023-04-13 21:51:33.727173 json5kit-0.3.0/src/json5kit.egg-info/
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)     2273 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/PKG-INFO
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)      286 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/SOURCES.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        1 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/dependency_links.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)       29 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/requires.txt
+-rw-r--r--   0 tusharsadhwani   (501) staff       (20)        9 2023-04-13 21:51:33.000000 json5kit-0.3.0/src/json5kit.egg-info/top_level.txt
```

### Comparing `json5kit-0.2.1/LICENSE` & `json5kit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json5kit-0.2.1/PKG-INFO` & `json5kit-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,37 +34,45 @@
 
 ```bash
 pip install json5kit
 ```
 
 ## Usage
 
-> This is not the intended way to use the library. The correct way to modify a
-> tree would be to use visitors, which will be added soon.
-
 ```python
 >>> source = """
 ... {
 ...   "items": [1, 2, 4],  // change this to 3
 ... }
 ... """
 >>> import json5kit
 >>> tree = json5kit.parse(source)
 >>> print(tree.to_source())
 
 {
   "items": [1, 2, 4],  // change this to 3
 }
 
->>> tree.value.data[0][1].members[2] = json5kit.Json5Number('3', 3, [])
+>>> print(tree.to_json())
+{"items":[1,2,4]}
+>>> # Let's replace the `4` with `3` now:
+>>> class ReplaceFourWithThree(json5kit.Json5Transformer):
+...     def visit_Number(self, node):
+...         if node.value == 4:
+...             return node.replace(value=3)
+...         return node
+...
+>>> ReplaceFourWithThree().visit(tree)
 >>> print(tree.to_source())
 
 {
   "items": [1, 2, 3],  // change this to 3
 }
+>>> print(tree.to_json())
+{"items":[1,2,3]}
 ```
 
 ## Development / Testing
 
 - Clone the project:
 
   ```bash
@@ -94,9 +101,7 @@
   ```
 
 - Run type checking:
 
   ```bash
   mypy .
   ```
-
-
```

### Comparing `json5kit-0.2.1/README.md` & `json5kit-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -11,37 +11,45 @@
 
 ```bash
 pip install json5kit
 ```
 
 ## Usage
 
-> This is not the intended way to use the library. The correct way to modify a
-> tree would be to use visitors, which will be added soon.
-
 ```python
 >>> source = """
 ... {
 ...   "items": [1, 2, 4],  // change this to 3
 ... }
 ... """
 >>> import json5kit
 >>> tree = json5kit.parse(source)
 >>> print(tree.to_source())
 
 {
   "items": [1, 2, 4],  // change this to 3
 }
 
->>> tree.value.data[0][1].members[2] = json5kit.Json5Number('3', 3, [])
+>>> print(tree.to_json())
+{"items":[1,2,4]}
+>>> # Let's replace the `4` with `3` now:
+>>> class ReplaceFourWithThree(json5kit.Json5Transformer):
+...     def visit_Number(self, node):
+...         if node.value == 4:
+...             return node.replace(value=3)
+...         return node
+...
+>>> ReplaceFourWithThree().visit(tree)
 >>> print(tree.to_source())
 
 {
   "items": [1, 2, 3],  // change this to 3
 }
+>>> print(tree.to_json())
+{"items":[1,2,3]}
 ```
 
 ## Development / Testing
 
 - Clone the project:
 
   ```bash
```

### Comparing `json5kit-0.2.1/setup.cfg` & `json5kit-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = json5kit
-version = 0.2.1
+version = 0.3.0
 description = A Roundtrip parser and CST for JSON, JSONC and JSON5.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tusharsadhwani/json5kit
 author = Tushar Sadhwani
 author_email = tushar.sadhwani000@gmail.com
 license = MIT
```

### Comparing `json5kit-0.2.1/src/json5kit/__init__.py` & `json5kit-0.3.0/src/json5kit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Json5Number,
     Json5Object,
     Json5Primitive,
     Json5String,
     Json5Trivia,
     Json5Whitespace,
 )
+from json5kit.visitor import Json5Visitor, Json5Transformer
 
 
 class Json5ParseError(Exception):
     """Raised when the JSON5 string has bad syntax."""
 
     def __init__(self, message: str, index: int) -> None:
         super().__init__(message)
@@ -347,7 +348,30 @@
                 break
 
         return trivia_nodes
 
 
 def parse(source: str) -> Json5Node:
     return Json5Parser(source).parse()
+
+
+__all__ = [
+    "Json5ParseError",
+    "Json5Array",
+    "Json5Boolean",
+    "Json5Comma",
+    "Json5Comment",
+    "Json5File",
+    "Json5Key",
+    "Json5Newline",
+    "Json5Node",
+    "Json5Null",
+    "Json5Number",
+    "Json5Object",
+    "Json5Primitive",
+    "Json5String",
+    "Json5Trivia",
+    "Json5Whitespace",
+    "Json5Parser",
+    "Json5Visitor",
+    "Json5Transformer",
+]
```

### Comparing `json5kit-0.2.1/src/json5kit/nodes.py` & `json5kit-0.3.0/src/json5kit/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
-from multiprocessing.sharedctypes import Value
 
-from typing import Protocol
+from typing import Protocol, Self, runtime_checkable
 
 
+@runtime_checkable
 class Json5Node(Protocol):
     """Sets the expectation from a JSON5 node: be able to convert back to source."""
 
     trailing_trivia_nodes: list[Json5Trivia]
 
     def to_source(self) -> str:
         ...
@@ -33,45 +33,60 @@
         return self.source + "".join(
             trivia.source for trivia in self.trailing_trivia_nodes
         )
 
     def to_json(self) -> str:
         return self.source
 
+    def replace(self, value: object) -> Self:
+        # TODO: pass specific source?
+        source = str(value)
+
+        primitive_class = type(self)
+        return primitive_class(source, value, self.trailing_trivia_nodes.copy())
+
 
 class Json5Null(Json5Primitive):
+    value: None
+
     def __init__(self, trailing_trivia_nodes: list[Json5Trivia]) -> None:
         super().__init__(
             source="null",
             value=None,
             trailing_trivia_nodes=trailing_trivia_nodes,
         )
 
 
 class Json5Boolean(Json5Primitive):
+    value: bool
+
     def __init__(
         self,
         source: str,
         value: bool,
         trailing_trivia_nodes: list[Json5Trivia],
     ) -> None:
         super().__init__(source, value, trailing_trivia_nodes)
 
 
 class Json5Number(Json5Primitive):
+    value: float
+
     def __init__(
         self,
         source: str,
         value: float,
         trailing_trivia_nodes: list[Json5Trivia],
     ) -> None:
         super().__init__(source, value, trailing_trivia_nodes)
 
 
 class Json5String(Json5Primitive):
+    value: str
+
     def __init__(
         self,
         source: str,
         value: str,
         trailing_trivia_nodes: list[Json5Trivia],
     ) -> None:
         super().__init__(source, value, trailing_trivia_nodes)
@@ -175,43 +190,59 @@
     def __init__(
         self,
         data: list[tuple[Json5Key, Json5Node]],  # TODO: identifier support
         leading_trivia_nodes: list[Json5Trivia],
         trailing_trivia_nodes: list[Json5Trivia],
     ) -> None:
         super().__init__(leading_trivia_nodes, trailing_trivia_nodes)
-        self.data = data
+        self.keys: list[Json5Key] = []
+        self.values: list[Json5Node] = []
+        for key, value in data:
+            self.keys.append(key)
+            self.values.append(value)
 
     def to_source(self) -> str:
         """Converts the node back to its original source."""
         return (
             "{"
             + "".join(trivia.source for trivia in self.leading_trivia_nodes)
             + "".join(
-                f"{key.to_source()}{value.to_source()}" for key, value in self.data
+                f"{key.to_source()}{value.to_source()}"
+                for key, value in zip(self.keys, self.values)
             )
             + "}"
             + "".join(trivia.source for trivia in self.trailing_trivia_nodes)
         )
 
     def to_json(self) -> str:
         """Converts the node to JSON, without whitespace."""
         return (
             "{"
-            + ",".join(f"{key.to_json()}{value.to_json()}" for key, value in self.data)
+            + ",".join(
+                f"{key.to_json()}{value.to_json()}"
+                for key, value in zip(self.keys, self.values)
+            )
             + "}"
         )
 
 
 class Json5Trivia:
     """Base class for "trivial" information like whitespace, newlines and comments."""
 
+    trailing_trivia_nodes = ()
+
     def __init__(self, source: str) -> None:
         self.source = source
 
+    def to_source(self) -> str:
+        return self.source
+
+    def to_json(self) -> str:
+        return self.source
+
 
 class Json5Comment(Json5Trivia):
     """JSON5 single line comments, eg. `// foo`."""
 
 
 class Json5Whitespace(Json5Trivia):
     """Any run of continuous whitespace characters in a JSON5 file."""
```

### Comparing `json5kit-0.2.1/src/json5kit.egg-info/PKG-INFO` & `json5kit-0.3.0/src/json5kit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: json5kit
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Roundtrip parser and CST for JSON, JSONC and JSON5.
 Home-page: https://github.com/tusharsadhwani/json5kit
 Author: Tushar Sadhwani
 Author-email: tushar.sadhwani000@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,37 +34,45 @@
 
 ```bash
 pip install json5kit
 ```
 
 ## Usage
 
-> This is not the intended way to use the library. The correct way to modify a
-> tree would be to use visitors, which will be added soon.
-
 ```python
 >>> source = """
 ... {
 ...   "items": [1, 2, 4],  // change this to 3
 ... }
 ... """
 >>> import json5kit
 >>> tree = json5kit.parse(source)
 >>> print(tree.to_source())
 
 {
   "items": [1, 2, 4],  // change this to 3
 }
 
->>> tree.value.data[0][1].members[2] = json5kit.Json5Number('3', 3, [])
+>>> print(tree.to_json())
+{"items":[1,2,4]}
+>>> # Let's replace the `4` with `3` now:
+>>> class ReplaceFourWithThree(json5kit.Json5Transformer):
+...     def visit_Number(self, node):
+...         if node.value == 4:
+...             return node.replace(value=3)
+...         return node
+...
+>>> ReplaceFourWithThree().visit(tree)
 >>> print(tree.to_source())
 
 {
   "items": [1, 2, 3],  // change this to 3
 }
+>>> print(tree.to_json())
+{"items":[1,2,3]}
 ```
 
 ## Development / Testing
 
 - Clone the project:
 
   ```bash
@@ -94,9 +101,7 @@
   ```
 
 - Run type checking:
 
   ```bash
   mypy .
   ```
-
-
```

