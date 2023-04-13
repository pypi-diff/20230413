# Comparing `tmp/uplc-0.6.2.tar.gz` & `tmp/uplc-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplc-0.6.2.tar", last modified: Thu Apr  6 19:25:25 2023, max compression
+gzip compressed data, was "uplc-0.6.3.tar", last modified: Thu Apr 13 21:05:39 2023, max compression
```

## Comparing `uplc-0.6.2.tar` & `uplc-0.6.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-06 19:25:25.615665 uplc-0.6.2/
--rw-r--r--   0 travis    (1000) travis    (1000)     1077 2023-04-06 19:17:37.000000 uplc-0.6.2/LICENSE.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-06 19:25:25.615665 uplc-0.6.2/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     2034 2023-04-06 19:17:37.000000 uplc-0.6.2/README.md
--rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-06 19:25:25.615665 uplc-0.6.2/setup.cfg
--rw-r--r--   0 travis    (1000) travis    (1000)     2056 2023-04-06 19:17:37.000000 uplc-0.6.2/setup.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-06 19:25:25.607665 uplc-0.6.2/uplc/
--rw-r--r--   0 travis    (1000) travis    (1000)      555 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4935 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/__main__.py
--rw-r--r--   0 travis    (1000) travis    (1000)    26560 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)     9066 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/flat_decoder.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10052 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/flat_encoder.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1202 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/lexer.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3357 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/machine.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-06 19:25:25.611665 uplc-0.6.2/uplc/optimizer/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/optimizer/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      630 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/optimizer/pre_evaluation.py
--rw-r--r--   0 travis    (1000) travis    (1000)    10960 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/parser.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-06 19:25:25.615665 uplc-0.6.2/uplc/tests/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/tests/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3391 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/tests/test_acceptance.py
--rw-r--r--   0 travis    (1000) travis    (1000)    13912 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/tests/test_hypothesis.py
--rw-r--r--   0 travis    (1000) travis    (1000)   211128 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/tests/test_misc.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1998 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/tools.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-06 19:25:25.615665 uplc-0.6.2/uplc/transformer/
--rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/transformer/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      784 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/transformer/debrujin_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)      938 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/transformer/undebrujin_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1815 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/transformer/unique_variables.py
--rw-r--r--   0 travis    (1000) travis    (1000)     3009 2023-04-06 19:17:37.000000 uplc-0.6.2/uplc/util.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-06 19:25:25.611665 uplc-0.6.2/uplc.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-06 19:25:25.000000 uplc-0.6.2/uplc.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)      673 2023-04-06 19:25:25.000000 uplc-0.6.2/uplc.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-06 19:25:25.000000 uplc-0.6.2/uplc.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       44 2023-04-06 19:25:25.000000 uplc-0.6.2/uplc.egg-info/entry_points.txt
--rw-r--r--   0 travis    (1000) travis    (1000)      110 2023-04-06 19:25:25.000000 uplc-0.6.2/uplc.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        5 2023-04-06 19:25:25.000000 uplc-0.6.2/uplc.egg-info/top_level.txt
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.850954 uplc-0.6.3/
+-rw-r--r--   0 travis    (1000) travis    (1000)     1077 2023-04-13 20:58:12.000000 uplc-0.6.3/LICENSE.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-13 21:05:39.850954 uplc-0.6.3/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)     2034 2023-04-13 20:58:12.000000 uplc-0.6.3/README.md
+-rw-r--r--   0 travis    (1000) travis    (1000)       38 2023-04-13 21:05:39.850954 uplc-0.6.3/setup.cfg
+-rw-r--r--   0 travis    (1000) travis    (1000)     2056 2023-04-13 20:58:12.000000 uplc-0.6.3/setup.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.842954 uplc-0.6.3/uplc/
+-rw-r--r--   0 travis    (1000) travis    (1000)      555 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     4935 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/__main__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    26686 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/ast.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     9066 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/flat_decoder.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    10052 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/flat_encoder.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1202 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/lexer.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3357 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/machine.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.846954 uplc-0.6.3/uplc/optimizer/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/optimizer/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      630 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/optimizer/pre_evaluation.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    10960 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/parser.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.846954 uplc-0.6.3/uplc/tests/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3391 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/test_acceptance.py
+-rw-r--r--   0 travis    (1000) travis    (1000)    14104 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/test_hypothesis.py
+-rw-r--r--   0 travis    (1000) travis    (1000)   211128 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tests/test_misc.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1998 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/tools.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.850954 uplc-0.6.3/uplc/transformer/
+-rw-r--r--   0 travis    (1000) travis    (1000)        0 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/__init__.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      784 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/debrujin_variables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)      938 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/undebrujin_variables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     1947 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/transformer/unique_variables.py
+-rw-r--r--   0 travis    (1000) travis    (1000)     3009 2023-04-13 20:58:12.000000 uplc-0.6.3/uplc/util.py
+drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2023-04-13 21:05:39.846954 uplc-0.6.3/uplc.egg-info/
+-rw-r--r--   0 travis    (1000) travis    (1000)     2807 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (1000) travis    (1000)      673 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        1 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)       44 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/entry_points.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)      110 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/requires.txt
+-rw-r--r--   0 travis    (1000) travis    (1000)        5 2023-04-13 21:05:39.000000 uplc-0.6.3/uplc.egg-info/top_level.txt
```

### Comparing `uplc-0.6.2/LICENSE.txt` & `uplc-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/PKG-INFO` & `uplc-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uplc
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python implementation of untyped plutus language core
 Home-page: https://github.com/opshin/uplc
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `uplc-0.6.2/README.md` & `uplc-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/setup.py` & `uplc-0.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     py_modules=["uplc"],
     packages=find_packages(),
     install_requires=[
         "frozendict==2.3.4",
         "cbor2==5.4.6",
         "frozenlist==1.3.3",
         "rply==0.7.8",
-        "pycardano==0.8.0",
+        "pycardano==0.8.1",
         "python-secp256k1-cardano==0.2.3",
     ],
     tests_require=[
         "pyaiken==0.4.0",
         "hypothesis==6.62.0",
         "parameterized==0.8.1",
     ],
```

### Comparing `uplc-0.6.2/uplc/__init__.py` & `uplc-0.6.3/uplc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
 import logging
 
 
-VERSION = (0, 6, 2)
+VERSION = (0, 6, 3)
 
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "nielstron"
 __author_email__ = "n.muendler@web.de"
 __copyright__ = "Copyright (C) 2023 nielstron"
 __license__ = "MIT"
 __url__ = "https://github.com/opshin/uplc"
```

### Comparing `uplc-0.6.2/uplc/__main__.py` & `uplc-0.6.3/uplc/__main__.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/ast.py` & `uplc-0.6.3/uplc/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,15 +791,18 @@
     state: frozendict.frozendict
     _fields = ["term"]
 
     def eval(self, context, state):
         return Return(context, BoundStateDelay(self.term, self.state | state))
 
     def dumps(self, dialect=UPLCDialect.Aiken) -> str:
-        return f"(delay {self.term.dumps(dialect=dialect)})"
+        s = f"(delay {self.term.dumps(dialect=dialect)})"
+        for k, v in reversed(self.state.items()):
+            s = f"[(lam {k} {s}) {v.dumps(dialect=dialect)}]"
+        return s
 
 
 @dataclass
 class Delay(BoundStateDelay):
     term: AST
     state: frozendict.frozendict = dataclasses.field(
         default_factory=frozendict.frozendict
```

### Comparing `uplc-0.6.2/uplc/flat_decoder.py` & `uplc-0.6.3/uplc/flat_decoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/flat_encoder.py` & `uplc-0.6.3/uplc/flat_encoder.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/lexer.py` & `uplc-0.6.3/uplc/lexer.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/machine.py` & `uplc-0.6.3/uplc/machine.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/optimizer/pre_evaluation.py` & `uplc-0.6.3/uplc/optimizer/pre_evaluation.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/parser.py` & `uplc-0.6.3/uplc/parser.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/tests/test_acceptance.py` & `uplc-0.6.3/uplc/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/tests/test_hypothesis.py` & `uplc-0.6.3/uplc/tests/test_hypothesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,20 @@
 uplc_builtin_fun = hst.builds(BuiltIn, hst.sampled_from(BuiltInFun))
 uplc_variable = hst.builds(Variable, uplc_name)
 
 
 class UnboundVariableVisitor(NodeVisitor):
     def __init__(self):
         self.scope = []
-        self.unbound = []
+        self.unbound = set()
 
     def check_bound(self, name: str):
         if name in self.scope:
             return
-        self.unbound.append(name)
+        self.unbound.add(name)
 
     def visit_Lambda(self, node: Lambda):
         self.scope.append(node.var_name)
         self.visit(node.term)
         self.scope.pop()
 
     def visit_Variable(self, node: Variable):
@@ -117,15 +117,15 @@
 
 
 @hst.composite
 def uplc_expr_all_bound(draw, uplc_expr):
     x = draw(uplc_expr)
     unbound_var_visitor = UnboundVariableVisitor()
     unbound_var_visitor.visit(x)
-    unbound_vars = unbound_var_visitor.unbound
+    unbound_vars = list(unbound_var_visitor.unbound)
     vars = draw(hst.permutations(unbound_vars))
     for v in vars:
         x = Lambda(v, x)
     return x
 
 
 def rec_expr_strategies(uplc_expr):
@@ -199,14 +199,18 @@
         UPLCDialect.Aiken,
     )
     def test_dumps_parse_roundtrip(self, p, dialect):
         self.assertEqual(parse(dumps(p, dialect)), p)
 
     @hypothesis.given(uplc_program)
     @hypothesis.settings(max_examples=1000, deadline=datetime.timedelta(seconds=10))
+    @hypothesis.example(parse("(program 0.0.0 [(lam a (delay a)) (lam c c)])"))
+    @hypothesis.example(
+        parse("(program 0.0.0 [(lam a (lam b (error))) (lam _ (error))])")
+    )
     @hypothesis.example(
         parse("(program 0.0.0 [(force (builtin mkCons)) (lam _ (error))])")
     )
     @hypothesis.example(
         parse("(program 0.0.0 (lam _ [(builtin mkPairData) (lam ' _)]))")
     )
     @hypothesis.example(parse("(program 0.0.0 (lam _ _))"))
```

### Comparing `uplc-0.6.2/uplc/tests/test_misc.py` & `uplc-0.6.3/uplc/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/tools.py` & `uplc-0.6.3/uplc/tools.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/transformer/debrujin_variables.py` & `uplc-0.6.3/uplc/transformer/debrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/transformer/undebrujin_variables.py` & `uplc-0.6.3/uplc/transformer/undebrujin_variables.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc/transformer/unique_variables.py` & `uplc-0.6.3/uplc/transformer/unique_variables.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,32 +28,35 @@
     def pop_map(self):
         self.scopes.pop(-1)
 
     def visit_BoundStateLambda(self, node: BoundStateLambda):
         new_map = {}
         for k, v in node.state.items():
             nk = self.push_map(k)
-            new_map[nk] = v
+            new_map[nk] = self.visit(v)
         n = self.push_map(node.var_name)
         nc = copy(node)
         nc.state = frozendict.frozendict(new_map)
         nc.var_name = n
         nc.term = self.visit(node.term)
         self.pop_map()
         for _ in node.state.keys():
             self.pop_map()
         return nc
 
     def visit_Lambda(self, node: Lambda):
         return self.visit_BoundStateLambda(node)
 
     def visit_BoundStateDelay(self, node: BoundStateDelay):
-        for k in node.state.keys():
-            self.push_map(k)
+        new_map = {}
+        for k, v in node.state.items():
+            nk = self.push_map(k)
+            new_map[nk] = self.visit(v)
         nc = copy(node)
+        nc.state = frozendict.frozendict(new_map)
         nc.term = self.visit(node.term)
         for _ in node.state.keys():
             self.pop_map()
         return nc
 
     def visit_ForcedBuiltIn(self, node: ForcedBuiltIn):
         nc = copy(node)
```

### Comparing `uplc-0.6.2/uplc/util.py` & `uplc-0.6.3/uplc/util.py`

 * *Files identical despite different names*

### Comparing `uplc-0.6.2/uplc.egg-info/PKG-INFO` & `uplc-0.6.3/uplc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uplc
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python implementation of untyped plutus language core
 Home-page: https://github.com/opshin/uplc
 Author: nielstron
 Author-email: n.muendler@web.de
 License: MIT
 Keywords: python cardano smart contract blockchain verification haskell
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `uplc-0.6.2/uplc.egg-info/SOURCES.txt` & `uplc-0.6.3/uplc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

