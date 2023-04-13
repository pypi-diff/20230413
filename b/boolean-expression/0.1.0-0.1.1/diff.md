# Comparing `tmp/boolean_expression-0.1.0.tar.gz` & `tmp/boolean_expression-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boolean_expression-0.1.0.tar", max compression
+gzip compressed data, was "boolean_expression-0.1.1.tar", max compression
```

## Comparing `boolean_expression-0.1.0.tar` & `boolean_expression-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-04-11 05:21:55.851965 boolean_expression-0.1.0/LICENSE
--rw-r--r--   0        0        0     3174 2023-04-11 05:52:17.537556 boolean_expression-0.1.0/README.md
--rw-r--r--   0        0        0    15837 2023-04-11 05:22:33.905134 boolean_expression-0.1.0/boolean_expression.py
--rw-r--r--   0        0        0      610 2023-04-11 05:22:40.357036 boolean_expression-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 boolean_expression-0.1.0/setup.py
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 boolean_expression-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-13 04:46:32.387360 boolean_expression-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3175 2023-04-11 06:04:33.817547 boolean_expression-0.1.1/README.md
+-rw-r--r--   0        0        0    16943 2023-04-13 04:59:27.181807 boolean_expression-0.1.1/boolean_expression.py
+-rw-r--r--   0        0        0      610 2023-04-13 05:00:12.057307 boolean_expression-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3854 1970-01-01 00:00:00.000000 boolean_expression-0.1.1/setup.py
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 boolean_expression-0.1.1/PKG-INFO
```

### Comparing `boolean_expression-0.1.0/LICENSE` & `boolean_expression-0.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Alex L.
+Copyright (c) 2023 Alex Levy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `boolean_expression-0.1.0/README.md` & `boolean_expression-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 ```python
 GT("total", 0) & OR(alpha="A", bravo="B")
 ```
 
 ### Negation
 
-There are two ways of negating an expression. One is an atomic condition, equivalent to `X != Y`:
+There are two ways of negating an expression. One is an atomic comparison, equivalent to `X != Y`:
 
 ```python
 NE("some_name", "some_value")
 ```
 
 The other way to construct "not equal" is with a compound condition. The following Python expressions all produce the same data structure:
```

### Comparing `boolean_expression-0.1.0/boolean_expression.py` & `boolean_expression-0.1.1/boolean_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 """
 A basic library for representing boolean expressions, flattening them,
 and converting them into strings for other puprposes.
 """
+
+# MIT License
+#
+# Copyright (c) 2023 Alex Levy
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
 from __future__ import annotations
 
 import datetime
 from dataclasses import dataclass
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Iterable, Iterator, Tuple
@@ -466,15 +489,15 @@
 
     >>> condition1 = (
     ...     EQ("foo", 1)
     ...     | EQ("bar", datetime.date(2023, 1, 23))
     ...     | EQ("missing", None)
     ... )
     >>> AirtableRenderer().to_str(condition1)
-    "OR({foo}=1, {bar}='2023-01-23', {missing}=EMPTY())"
+    "OR({foo}=1, {bar}='2023-01-23', {missing}=BLANK())"
 
     >>> condition2 = GTE("baz", Decimal('3.5')) & NE("quux", False)
     >>> AirtableRenderer().to_str(condition2)
     'AND({baz}>=3.5, {quux}!=0)'
 
     >>> condition3 = (
     ...     LT("{Date Field}", Expression("TODAY()"))
@@ -498,15 +521,15 @@
     def format_field(self, field: str) -> str:
         if not (field.startswith("{") and field.endswith("}")):
             return "{" + field + "}"
         return field
 
     def format_value(self, value: Any) -> str:
         if value is None:
-            return "EMPTY()"
+            return "BLANK()"
         elif isinstance(value, bool):
             return str(int(value))
         elif isinstance(value, (datetime.date, datetime.datetime)):
             return repr(value.isoformat())
         elif isinstance(value, (int, float, Decimal, Expression)):
             return str(value)
         else:
```

### Comparing `boolean_expression-0.1.0/pyproject.toml` & `boolean_expression-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boolean_expression"
-version = "0.1.0"
+version = "0.1.1"
 description = "A simple library for constructing nested boolean expressions and rendering them in various dialects."
 authors = ["Alex Levy <mesozoic@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "boolean_expression.py"}]
 
 [tool.poetry.dependencies]
```

### Comparing `boolean_expression-0.1.0/setup.py` & `boolean_expression-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 modules = \
 ['boolean_expression']
 setup_kwargs = {
     'name': 'boolean-expression',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A simple library for constructing nested boolean expressions and rendering them in various dialects.',
-    'long_description': '# boolean_expression\n\nThis is a simple library for creating nested boolean expressions and rendering them in a variety of dialects. It is provided as a single file so that it can be vendored into other projects where an external dependency is not possible or desirable. It is not assumed to be universally useful, but might be handy to someone out there.\n\n## Getting started\n\nYou can use this library out-of-the-box as a miniature DSL to construct boolean expressions in your library, which can later be converted to a search expression, query language, or the like. For example:\n\n```python\nfrom boolean_expression import AND, OR, EQ, NOT\n\ncondition = AND(\n    EQ("id", record_id),\n    OR(\n        NOT(EQ("status", "private")),\n        EQ("status", "private") & EQ("owner", searching_user),\n    )\n)\n```\n\nThere are a few built-in renderers, like one that creates LDAP expressions. Given the above, the following code...\n\n```python\nfrom boolean_expression import LdapRenderer\nprint(LdapRenderer().to_str(condition))\n```\n\n...produces the following output:\n\n```\n(&(id=theRecordId)(|(!(status=private))(&(status=private)(owner=theUser))))\n```\n\nIn most cases, however, it is likely that if you\'re using this library you have your own particular needs and will need to implement your own renderer.\n\n## Usage\n\nDevelopers considering this library are encouraged to read the docstring tests, because they demonstrate 100% of the functionality of the library. Basics are reproduced below.\n\n### Equality\n\nComparisons express an lval and an rval which are not interpreted at all during construction (but which you could choose to interpret during rendering, if appropriate to your use case).\n\nTo specify a comparison where some name or expression is expected to match a value:\n\n```python\nEQ("some_name", expected_value)\n```\n\n### Less Than / Greater Than\n\nThere are convenience methods for these common types of comparisons:\n\n```python\nLT("some_name", 0)\nGT("some_name", 0)\nLTE("some_name", 0)\nGTE("some_name", 0)\n```\n\n### And / Or\n\nThese can be constructed in one of a few ways. The most straightforward is the "Excel style":\n\n```python\nAND(\n    GT("total", 0),\n    OR(\n        EQ("alpha", "A"),\n        EQ("bravo", "B")\n    )\n)\n```\n\n...which can be made more tersely by using `&` and `|` operators:\n\n```python\nGT("total", 0) & (EQ("alpha", "A") | EQ("bravo", "B"))\n```\n\nThe `AND()` and `OR()` functions also accept keyword arguments (which are all interpreted as `EQ`):\n\n```python\nGT("total", 0) & OR(alpha="A", bravo="B")\n```\n\n### Negation\n\nThere are two ways of negating an expression. One is an atomic condition, equivalent to `X != Y`:\n\n```python\nNE("some_name", "some_value")\n```\n\nThe other way to construct "not equal" is with a compound condition. The following Python expressions all produce the same data structure:\n\n```python\n~EQ("some_name", "some_value")\nNOT(EQ("some_name", "some_value"))\nCompound("NOT", [EQ("some_name", "some_value")])\n```\n\n### Raw Expressions\n\nShould your use case require it, the library also allows for inserting raw expressions into the data structure:\n\n```python\nAND(\n    NOT(OR(Role="Admin", Role="Owner")),\n    Expression("AttemptedDelete")\n)\n```\n',
+    'long_description': '# boolean_expression\n\nThis is a simple library for creating nested boolean expressions and rendering them in a variety of dialects. It is provided as a single file so that it can be vendored into other projects where an external dependency is not possible or desirable. It is not assumed to be universally useful, but might be handy to someone out there.\n\n## Getting started\n\nYou can use this library out-of-the-box as a miniature DSL to construct boolean expressions in your library, which can later be converted to a search expression, query language, or the like. For example:\n\n```python\nfrom boolean_expression import AND, OR, EQ, NOT\n\ncondition = AND(\n    EQ("id", record_id),\n    OR(\n        NOT(EQ("status", "private")),\n        EQ("status", "private") & EQ("owner", searching_user),\n    )\n)\n```\n\nThere are a few built-in renderers, like one that creates LDAP expressions. Given the above, the following code...\n\n```python\nfrom boolean_expression import LdapRenderer\nprint(LdapRenderer().to_str(condition))\n```\n\n...produces the following output:\n\n```\n(&(id=theRecordId)(|(!(status=private))(&(status=private)(owner=theUser))))\n```\n\nIn most cases, however, it is likely that if you\'re using this library you have your own particular needs and will need to implement your own renderer.\n\n## Usage\n\nDevelopers considering this library are encouraged to read the docstring tests, because they demonstrate 100% of the functionality of the library. Basics are reproduced below.\n\n### Equality\n\nComparisons express an lval and an rval which are not interpreted at all during construction (but which you could choose to interpret during rendering, if appropriate to your use case).\n\nTo specify a comparison where some name or expression is expected to match a value:\n\n```python\nEQ("some_name", expected_value)\n```\n\n### Less Than / Greater Than\n\nThere are convenience methods for these common types of comparisons:\n\n```python\nLT("some_name", 0)\nGT("some_name", 0)\nLTE("some_name", 0)\nGTE("some_name", 0)\n```\n\n### And / Or\n\nThese can be constructed in one of a few ways. The most straightforward is the "Excel style":\n\n```python\nAND(\n    GT("total", 0),\n    OR(\n        EQ("alpha", "A"),\n        EQ("bravo", "B")\n    )\n)\n```\n\n...which can be made more tersely by using `&` and `|` operators:\n\n```python\nGT("total", 0) & (EQ("alpha", "A") | EQ("bravo", "B"))\n```\n\nThe `AND()` and `OR()` functions also accept keyword arguments (which are all interpreted as `EQ`):\n\n```python\nGT("total", 0) & OR(alpha="A", bravo="B")\n```\n\n### Negation\n\nThere are two ways of negating an expression. One is an atomic comparison, equivalent to `X != Y`:\n\n```python\nNE("some_name", "some_value")\n```\n\nThe other way to construct "not equal" is with a compound condition. The following Python expressions all produce the same data structure:\n\n```python\n~EQ("some_name", "some_value")\nNOT(EQ("some_name", "some_value"))\nCompound("NOT", [EQ("some_name", "some_value")])\n```\n\n### Raw Expressions\n\nShould your use case require it, the library also allows for inserting raw expressions into the data structure:\n\n```python\nAND(\n    NOT(OR(Role="Admin", Role="Owner")),\n    Expression("AttemptedDelete")\n)\n```\n',
     'author': 'Alex Levy',
     'author_email': 'mesozoic@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'py_modules': modules,
     'python_requires': '>=3.8,<4.0',
```

### Comparing `boolean_expression-0.1.0/PKG-INFO` & `boolean_expression-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boolean-expression
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple library for constructing nested boolean expressions and rendering them in various dialects.
 License: MIT
 Author: Alex Levy
 Author-email: mesozoic@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -98,15 +98,15 @@
 
 ```python
 GT("total", 0) & OR(alpha="A", bravo="B")
 ```
 
 ### Negation
 
-There are two ways of negating an expression. One is an atomic condition, equivalent to `X != Y`:
+There are two ways of negating an expression. One is an atomic comparison, equivalent to `X != Y`:
 
 ```python
 NE("some_name", "some_value")
 ```
 
 The other way to construct "not equal" is with a compound condition. The following Python expressions all produce the same data structure:
```

