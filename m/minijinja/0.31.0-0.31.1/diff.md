# Comparing `tmp/minijinja-0.31.0.tar.gz` & `tmp/minijinja-0.31.1.tar.gz`

## Comparing `minijinja-0.31.0.tar` & `minijinja-0.31.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 minijinja-0.31.0/local_dependencies/minijinja/Cargo.toml
--rw-r--r--   0     1001      123    10847 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/LICENSE
--rw-r--r--   0     1001      123     5444 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/README.md
--rw-r--r--   0     1001      123      598 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/doc-header.html
--rw-r--r--   0     1001      123    17588 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/ast.rs
--rw-r--r--   0     1001      123    30962 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/codegen.rs
--rw-r--r--   0     1001      123    11867 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/instructions.rs
--rw-r--r--   0     1001      123    18011 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/lexer.rs
--rw-r--r--   0     1001      123     7038 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/meta.rs
--rw-r--r--   0     1001      123      220 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/mod.rs
--rw-r--r--   0     1001      123    40316 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/parser.rs
--rw-r--r--   0     1001      123     4099 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/compiler/tokens.rs
--rw-r--r--   0     1001      123     2722 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/debug.rs
--rw-r--r--   0     1001      123     7292 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/defaults.rs
--rw-r--r--   0     1001      123    21455 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/environment.rs
--rw-r--r--   0     1001      123    10586 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/error.rs
--rw-r--r--   0     1001      123     2337 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/expression.rs
--rw-r--r--   0     1001      123    42561 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/filters.rs
--rw-r--r--   0     1001      123    10073 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/functions.rs
--rw-r--r--   0     1001      123     1822 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/key/deserialize.rs
--rw-r--r--   0     1001      123     9223 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/key/mod.rs
--rw-r--r--   0     1001      123     5980 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/key/serialize.rs
--rw-r--r--   0     1001      123    10220 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/lib.rs
--rw-r--r--   0     1001      123     5689 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/macros.rs
--rw-r--r--   0     1001      123     4186 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/output.rs
--rw-r--r--   0     1001      123     9329 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/source.rs
--rw-r--r--   0     1001      123    24382 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/syntax.rs
--rw-r--r--   0     1001      123     7333 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/template.rs
--rw-r--r--   0     1001      123    13302 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/tests.rs
--rw-r--r--   0     1001      123     3809 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/testutils.rs
--rw-r--r--   0     1001      123    11538 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/utils.rs
--rw-r--r--   0     1001      123    19916 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/value/argtypes.rs
--rw-r--r--   0     1001      123     2864 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/value/deserialize.rs
--rw-r--r--   0     1001      123    44469 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/value/mod.rs
--rw-r--r--   0     1001      123    18349 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/value/object.rs
--rw-r--r--   0     1001      123    10946 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/value/ops.rs
--rw-r--r--   0     1001      123    11516 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/value/serialize.rs
--rw-r--r--   0     1001      123     1685 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/vm/closure_object.rs
--rw-r--r--   0     1001      123     9844 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/vm/context.rs
--rw-r--r--   0     1001      123     1862 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/vm/fuel.rs
--rw-r--r--   0     1001      123     4433 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/vm/loop_object.rs
--rw-r--r--   0     1001      123     5550 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/vm/macro_object.rs
--rw-r--r--   0     1001      123    39138 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/vm/mod.rs
--rw-r--r--   0     1001      123     6127 2023-03-27 21:03:44.000000 minijinja-0.31.0/local_dependencies/minijinja/src/vm/state.rs
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 minijinja-0.31.0/Cargo.toml
--rw-r--r--   0     1001      123       47 2023-03-27 21:03:44.000000 minijinja-0.31.0/.gitignore
--rw-r--r--   0     1001      123       45 2023-03-27 21:03:44.000000 minijinja-0.31.0/.vscode/settings.json
--rw-r--r--   0     1001      123    10847 2023-03-27 21:03:44.000000 minijinja-0.31.0/LICENSE
--rw-r--r--   0     1001      123      415 2023-03-27 21:03:44.000000 minijinja-0.31.0/Makefile
--rw-r--r--   0     1001      123     6964 2023-03-27 21:03:44.000000 minijinja-0.31.0/README.md
--rw-r--r--   0     1001      123      571 2023-03-27 21:03:44.000000 minijinja-0.31.0/hello.py
--rw-r--r--   0     1001      123     1110 2023-03-27 21:03:44.000000 minijinja-0.31.0/pyproject.toml
--rw-r--r--   0     1001      123     3507 2023-03-27 21:03:44.000000 minijinja-0.31.0/python/minijinja/__init__.py
--rw-r--r--   0     1001      123      558 2023-03-27 21:03:44.000000 minijinja-0.31.0/python/minijinja/_internal.py
--rw-r--r--   0     1001      123    15658 2023-03-27 21:03:44.000000 minijinja-0.31.0/src/environment.rs
--rw-r--r--   0     1001      123     2406 2023-03-27 21:03:44.000000 minijinja-0.31.0/src/error_support.rs
--rw-r--r--   0     1001      123      303 2023-03-27 21:03:44.000000 minijinja-0.31.0/src/lib.rs
--rw-r--r--   0     1001      123     2935 2023-03-27 21:03:44.000000 minijinja-0.31.0/src/state.rs
--rw-r--r--   0     1001      123    11218 2023-03-27 21:03:44.000000 minijinja-0.31.0/src/typeconv.rs
--rw-r--r--   0     1001      123     5427 2023-03-27 21:03:44.000000 minijinja-0.31.0/tests/test_basic.py
--rw-r--r--   0     1001      123      541 2023-03-27 21:03:44.000000 minijinja-0.31.0/tests/test_security.py
--rw-r--r--   0     1001      123     2492 2023-03-27 21:03:44.000000 minijinja-0.31.0/tests/test_state.py
--rw-r--r--   0     1001      123    64252 2023-03-27 21:05:20.000000 minijinja-0.31.0/Cargo.lock
--rw-r--r--   0        0        0     7967 1970-01-01 00:00:00.000000 minijinja-0.31.0/PKG-INFO
+-rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 minijinja-0.31.1/local_dependencies/minijinja/Cargo.toml
+-rw-r--r--   0     1001      123    10847 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/LICENSE
+-rw-r--r--   0     1001      123     5444 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/README.md
+-rw-r--r--   0     1001      123      598 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/doc-header.html
+-rw-r--r--   0     1001      123    17588 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/ast.rs
+-rw-r--r--   0     1001      123    30962 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/codegen.rs
+-rw-r--r--   0     1001      123    11867 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/instructions.rs
+-rw-r--r--   0     1001      123    18011 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/lexer.rs
+-rw-r--r--   0     1001      123     7038 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/meta.rs
+-rw-r--r--   0     1001      123      220 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/mod.rs
+-rw-r--r--   0     1001      123    40316 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/parser.rs
+-rw-r--r--   0     1001      123     4099 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/compiler/tokens.rs
+-rw-r--r--   0     1001      123     2722 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/debug.rs
+-rw-r--r--   0     1001      123     7292 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/defaults.rs
+-rw-r--r--   0     1001      123    21455 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/environment.rs
+-rw-r--r--   0     1001      123    10576 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/error.rs
+-rw-r--r--   0     1001      123     2337 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/expression.rs
+-rw-r--r--   0     1001      123    42561 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/filters.rs
+-rw-r--r--   0     1001      123    10073 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/functions.rs
+-rw-r--r--   0     1001      123     1822 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/key/deserialize.rs
+-rw-r--r--   0     1001      123     9223 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/key/mod.rs
+-rw-r--r--   0     1001      123     5980 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/key/serialize.rs
+-rw-r--r--   0     1001      123    10220 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/lib.rs
+-rw-r--r--   0     1001      123     5689 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/macros.rs
+-rw-r--r--   0     1001      123     4186 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/output.rs
+-rw-r--r--   0     1001      123     9329 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/source.rs
+-rw-r--r--   0     1001      123    24382 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/syntax.rs
+-rw-r--r--   0     1001      123     7333 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/template.rs
+-rw-r--r--   0     1001      123    13302 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/tests.rs
+-rw-r--r--   0     1001      123     3809 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/testutils.rs
+-rw-r--r--   0     1001      123    11730 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/utils.rs
+-rw-r--r--   0     1001      123    19916 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/argtypes.rs
+-rw-r--r--   0     1001      123     2864 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/deserialize.rs
+-rw-r--r--   0     1001      123    44469 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/mod.rs
+-rw-r--r--   0     1001      123    18349 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/object.rs
+-rw-r--r--   0     1001      123    11170 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/ops.rs
+-rw-r--r--   0     1001      123    11516 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/value/serialize.rs
+-rw-r--r--   0     1001      123     1685 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/closure_object.rs
+-rw-r--r--   0     1001      123     9844 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/context.rs
+-rw-r--r--   0     1001      123     1862 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/fuel.rs
+-rw-r--r--   0     1001      123     4433 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/loop_object.rs
+-rw-r--r--   0     1001      123     5550 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/macro_object.rs
+-rw-r--r--   0     1001      123    39339 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/mod.rs
+-rw-r--r--   0     1001      123     6127 2023-04-13 19:56:21.000000 minijinja-0.31.1/local_dependencies/minijinja/src/vm/state.rs
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 minijinja-0.31.1/Cargo.toml
+-rw-r--r--   0     1001      123       47 2023-04-13 19:56:21.000000 minijinja-0.31.1/.gitignore
+-rw-r--r--   0     1001      123       45 2023-04-13 19:56:21.000000 minijinja-0.31.1/.vscode/settings.json
+-rw-r--r--   0     1001      123    10847 2023-04-13 19:56:21.000000 minijinja-0.31.1/LICENSE
+-rw-r--r--   0     1001      123      415 2023-04-13 19:56:21.000000 minijinja-0.31.1/Makefile
+-rw-r--r--   0     1001      123     7544 2023-04-13 19:56:21.000000 minijinja-0.31.1/README.md
+-rw-r--r--   0     1001      123      571 2023-04-13 19:56:21.000000 minijinja-0.31.1/hello.py
+-rw-r--r--   0     1001      123     1110 2023-04-13 19:56:21.000000 minijinja-0.31.1/pyproject.toml
+-rw-r--r--   0     1001      123     3604 2023-04-13 19:56:21.000000 minijinja-0.31.1/python/minijinja/__init__.py
+-rw-r--r--   0     1001      123      558 2023-04-13 19:56:21.000000 minijinja-0.31.1/python/minijinja/_internal.py
+-rw-r--r--   0     1001      123    17747 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/environment.rs
+-rw-r--r--   0     1001      123     2406 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/error_support.rs
+-rw-r--r--   0     1001      123      303 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/lib.rs
+-rw-r--r--   0     1001      123     2935 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/state.rs
+-rw-r--r--   0     1001      123    11218 2023-04-13 19:56:21.000000 minijinja-0.31.1/src/typeconv.rs
+-rw-r--r--   0     1001      123     6437 2023-04-13 19:56:21.000000 minijinja-0.31.1/tests/test_basic.py
+-rw-r--r--   0     1001      123      541 2023-04-13 19:56:21.000000 minijinja-0.31.1/tests/test_security.py
+-rw-r--r--   0     1001      123     2492 2023-04-13 19:56:21.000000 minijinja-0.31.1/tests/test_state.py
+-rw-r--r--   0     1001      123    66577 2023-04-13 19:57:01.000000 minijinja-0.31.1/Cargo.lock
+-rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 minijinja-0.31.1/PKG-INFO
```

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/Cargo.toml` & `minijinja-0.31.1/local_dependencies/minijinja/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "minijinja"
-version = "0.31.0"
+version = "0.31.1"
 edition = "2021"
 license = "Apache-2.0"
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 description = "a powerful template engine for Rust with minimal dependencies"
 homepage = "https://github.com/mitsuhiko/minijinja"
 repository = "https://github.com/mitsuhiko/minijinja"
 keywords = ["jinja", "jinja2", "templates"]
```

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/LICENSE` & `minijinja-0.31.1/local_dependencies/minijinja/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/README.md` & `minijinja-0.31.1/local_dependencies/minijinja/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dependencies for a small problem.  Additionally it tries not to re-invent
 something but stay in line with prior art to leverage an already existing
 ecosystem of editor integrations.
 
 ```
 $ cargo tree
 minimal v0.1.0 (examples/minimal)
-└── minijinja v0.31.0 (minijinja)
+└── minijinja v0.31.1 (minijinja)
     └── serde v1.0.144
 ```
 
 You can play with MiniJinja online [in the browser playground](https://mitsuhiko.github.io/minijinja-playground/)
 powered by a WASM build of MiniJinja.
 
 **Goals:**
```

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/doc-header.html` & `minijinja-0.31.1/local_dependencies/minijinja/doc-header.html`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/compiler/ast.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/ast.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/compiler/codegen.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/codegen.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/compiler/instructions.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/instructions.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/compiler/lexer.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/lexer.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/compiler/meta.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/meta.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/compiler/parser.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/parser.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/compiler/tokens.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/compiler/tokens.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/debug.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/debug.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/defaults.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/defaults.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/environment.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/environment.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/error.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/error.rs`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             ErrorKind::MissingArgument => "missing argument",
             ErrorKind::UnknownFilter => "unknown filter",
             ErrorKind::UnknownFunction => "unknown function",
             ErrorKind::UnknownTest => "unknown test",
             ErrorKind::UnknownMethod => "unknown method",
             ErrorKind::BadEscape => "bad string escape",
             ErrorKind::UndefinedError => "undefined value",
-            ErrorKind::BadSerialization => "could not serialize to internal format",
+            ErrorKind::BadSerialization => "could not serialize to value",
             ErrorKind::BadInclude => "could not render include",
             ErrorKind::EvalBlock => "could not render block",
             ErrorKind::CannotUnpack => "cannot unpack",
             ErrorKind::WriteFailure => "failed to write output",
             #[cfg(feature = "fuel")]
             ErrorKind::OutOfFuel => "engine ran out of fuel",
         }
```

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/expression.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/expression.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/filters.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/filters.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/functions.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/functions.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/key/deserialize.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/key/deserialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/key/mod.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/key/mod.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/key/serialize.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/key/serialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/lib.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/lib.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/macros.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/macros.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/output.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/output.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/source.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/source.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/syntax.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/syntax.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/template.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/template.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/tests.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/tests.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/testutils.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/testutils.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/utils.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -155,18 +155,24 @@
 
     /// Tries to iterate over a value while handling the undefined value.
     ///
     /// If the value is undefined, then iteration fails if the behavior is set to strict,
     /// otherwise it succeeds with an empty iteration.  This is also internally used in the
     /// engine to convert values to lists.
     pub(crate) fn try_iter(self, value: Value) -> Result<OwnedValueIterator, Error> {
+        self.assert_iterable(&value)
+            .and_then(|_| value.try_iter_owned())
+    }
+
+    /// Are we strict on iteration?
+    pub(crate) fn assert_iterable(self, value: &Value) -> Result<(), Error> {
         if matches!(self, UndefinedBehavior::Strict) && value.is_undefined() {
             Err(Error::from(ErrorKind::UndefinedError))
         } else {
-            value.try_iter_owned()
+            Ok(())
         }
     }
 }
 
 /// Helper to HTML escape a string.
 pub struct HtmlEscape<'a>(pub &'a str);
```

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/value/argtypes.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/value/argtypes.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/value/deserialize.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/value/deserialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/value/mod.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/value/mod.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/value/object.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/value/object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/value/ops.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/value/ops.rs`

 * *Files 6% similar despite different names*

```diff
@@ -259,14 +259,19 @@
         // otherwise we use format! to concat the two values
         _ => Value::from(format!("{left}{right}")),
     }
 }
 
 /// Implements a containment operation on values.
 pub fn contains(container: &Value, value: &Value) -> Result<Value, Error> {
+    // Special case where if the container is undefined, it cannot hold
+    // values.  For strict containment checks the vm has a special case.
+    if container.is_undefined() {
+        return Ok(Value::from(false));
+    }
     let rv = if let Some(s) = container.as_str() {
         if let Some(s2) = value.as_str() {
             s.contains(s2)
         } else {
             s.contains(&value.to_string())
         }
     } else if let Some(seq) = container.as_seq() {
```

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/value/serialize.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/value/serialize.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/vm/closure_object.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/vm/closure_object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/vm/context.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/vm/context.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/vm/fuel.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/vm/fuel.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/vm/loop_object.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/vm/loop_object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/vm/macro_object.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/vm/macro_object.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/vm/mod.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/vm/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -366,14 +366,17 @@
                     a = stack.pop();
                     b = stack.pop();
                     stack.push(ops::string_concat(b, &a));
                 }
                 Instruction::In => {
                     a = stack.pop();
                     b = stack.pop();
+                    // the in-operator can fail if the value is undefined and
+                    // we are in strict mode.
+                    ctx_ok!(state.undefined_behavior().assert_iterable(&a));
                     stack.push(ctx_ok!(ops::contains(&a, &b)));
                 }
                 Instruction::Neg => {
                     a = stack.pop();
                     stack.push(ctx_ok!(ops::neg(&a)));
                 }
                 Instruction::PushWith => {
```

### Comparing `minijinja-0.31.0/local_dependencies/minijinja/src/vm/state.rs` & `minijinja-0.31.1/local_dependencies/minijinja/src/vm/state.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/Cargo.toml` & `minijinja-0.31.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [package]
 name = "minijinja-py"
-version = "0.31.0"
+version = "0.31.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "minijinja_py"
 crate-type = ["cdylib"]
 
 [dependencies]
-minijinja = { version = "0.31.0", path = "local_dependencies/minijinja", features = ["source", "json", "urlencode", "fuel", "preserve_order", "speedups"] }
+minijinja = { version = "0.31.1", path = "local_dependencies/minijinja", features = ["source", "json", "urlencode", "fuel", "preserve_order", "speedups"] }
 once_cell = "1.17.0"
 pyo3 = { version = "0.18.0", features = ["extension-module", "serde", "abi3-py38"] }
 
 [package.metadata.maturin]
 name = "minijinja._lowlevel"
```

### Comparing `minijinja-0.31.0/LICENSE` & `minijinja-0.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/README.md` & `minijinja-0.31.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -104,14 +104,34 @@
 ```python
 env = Environment(auto_escape_callback=lambda x: x.endswith((".html", ".foo")))
 ```
 
 MiniJinja uses [markupsafe](https://github.com/pallets/markupsafe) if it's available
 on the Python side.  It will honor `__html__`.
 
+## Finalizers
+
+Instead of custom formatters like in MiniJinja, you can define a finalizer instead
+which is similar to how it works in Jinja2.  It's passed a value (or optional also
+the state as first argument whne `pass_state` is used) and can return a new value.
+If the special `NotImplemented` value is returned, the original value is rendered
+without any modification:
+
+```
+from minijinja import Environment
+
+def finalizer(value):
+    if value is None:
+	return ""
+    return NotImplemented
+
+env = Environment(finalizer=finalizer)
+assert env.render_str("{{ none }}") == ""
+```
+
 ## State Access
 
 Functions passed to the environment such as filters or global functions can
 optionally have the template state passed by using the `pass_state` parameter.
 This is similar to `pass_context` in Jinja2.  It can be used to look at the
 name of the template or to look up variables in the context.
```

### Comparing `minijinja-0.31.0/hello.py` & `minijinja-0.31.1/hello.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/pyproject.toml` & `minijinja-0.31.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "minijinja"
-version = "0.31.0"
+version = "0.31.1"
 description = "An experimental Python binding of the Rust MiniJinja template engine."
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "Armin Ronacher", email = "armin.ronacher@active-4.com" }
 ]
 maintainers = [
```

### Comparing `minijinja-0.31.0/python/minijinja/__init__.py` & `minijinja-0.31.1/python/minijinja/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         filters=None,
         tests=None,
         globals=None,
         debug=True,
         fuel=None,
         undefined_behavior=None,
         auto_escape_callback=None,
+        finalizer=None,
         reload_before_render=False,
     ):
         super().__init__()
         if loader is not None:
             if templates:
                 raise TypeError("Cannot set loader and templates at the same time")
             self.loader = loader
@@ -48,14 +49,16 @@
                 self.add_test(name, callback)
         if globals is not None:
             for name, value in globals.items():
                 self.add_global(name, value)
         self.debug = debug
         if auto_escape_callback is not None:
             self.auto_escape_callback = auto_escape_callback
+        if finalizer is not None:
+            self.finalizer = finalizer
         if undefined_behavior is not None:
             self.undefined_behavior = undefined_behavior
         self.reload_before_render = reload_before_render
 
 
 DEFAULT_ENVIRONMENT = Environment()
```

### Comparing `minijinja-0.31.0/python/minijinja/_internal.py` & `minijinja-0.31.1/python/minijinja/_internal.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/src/environment.rs` & `minijinja-0.31.1/src/environment.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::ffi::c_void;
 use std::sync::atomic::{AtomicBool, AtomicPtr, Ordering};
 use std::sync::Mutex;
 
 use minijinja::value::{Rest, Value};
-use minijinja::{context, AutoEscape, Error, Source, State, UndefinedBehavior};
+use minijinja::{context, escape_formatter, AutoEscape, Error, Source, State, UndefinedBehavior};
 use pyo3::conversion::AsPyPointer;
 use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::{PyDict, PyTuple};
 
 use crate::error_support::{report_unraisable, to_minijinja_error, to_py_error};
 use crate::state::bind_state;
@@ -18,14 +18,16 @@
 thread_local! {
     static CURRENT_ENV: AtomicPtr<c_void> = AtomicPtr::new(std::ptr::null_mut());
 }
 
 struct Inner {
     env: minijinja::Environment<'static>,
     loader: Option<Py<PyAny>>,
+    auto_escape_callback: Option<Py<PyAny>>,
+    finalizer_callback: Option<Py<PyAny>>,
 }
 
 /// Represents a MiniJinja environment.
 #[pyclass(subclass, module = "minijinja._lowlevel")]
 pub struct Environment {
     inner: Mutex<Inner>,
     reload_before_render: AtomicBool,
@@ -35,14 +37,16 @@
 impl Environment {
     #[new]
     fn py_new() -> PyResult<Self> {
         Ok(Environment {
             inner: Mutex::new(Inner {
                 env: minijinja::Environment::new(),
                 loader: None,
+                auto_escape_callback: None,
+                finalizer_callback: None,
             }),
             reload_before_render: AtomicBool::new(false),
         })
     }
 
     /// Enables or disables debug mode.
     #[setter]
@@ -219,17 +223,17 @@
     /// not able to raise an error.
     #[setter]
     pub fn set_auto_escape_callback(&self, callback: &PyAny) -> PyResult<()> {
         if !callback.is_callable() {
             return Err(PyRuntimeError::new_err("expected callback"));
         }
         let callback: Py<PyAny> = callback.into();
-        self.inner
-            .lock()
-            .unwrap()
+        let mut inner = self.inner.lock().unwrap();
+        inner.auto_escape_callback = Some(callback.clone());
+        inner
             .env
             .set_auto_escape_callback(move |name: &str| -> AutoEscape {
                 Python::with_gil(|py| {
                     let py_args = PyTuple::new(py, [name]);
                     let rv = match callback.call(py, py_args, None) {
                         Ok(value) => value,
                         Err(err) => {
@@ -256,14 +260,60 @@
                         AutoEscape::None
                     }
                 })
             });
         Ok(())
     }
 
+    #[getter]
+    pub fn get_auto_escape_callback(&self) -> PyResult<Option<Py<PyAny>>> {
+        Ok(self.inner.lock().unwrap().auto_escape_callback.clone())
+    }
+
+    /// Sets a finalizer.
+    ///
+    /// A finalizer is called before a value is rendered to customize it.
+    #[setter]
+    pub fn set_finalizer(&self, callback: &PyAny) -> PyResult<()> {
+        if !callback.is_callable() {
+            return Err(PyRuntimeError::new_err("expected callback"));
+        }
+        let callback: Py<PyAny> = callback.into();
+        let mut inner = self.inner.lock().unwrap();
+        inner.finalizer_callback = Some(callback.clone());
+        inner.env.set_formatter(move |output, state, value| {
+            Python::with_gil(|py| -> Result<(), Error> {
+                let maybe_new_value = bind_state(state, || -> Result<_, Error> {
+                    let args = std::slice::from_ref(value);
+                    let (py_args, py_kwargs) = to_python_args(py, callback.as_ref(py), args)
+                        .map_err(to_minijinja_error)?;
+                    let rv = callback
+                        .call(py, py_args, py_kwargs)
+                        .map_err(to_minijinja_error)?;
+                    if rv.is(&py.NotImplemented()) {
+                        Ok(None)
+                    } else {
+                        Ok(Some(to_minijinja_value(rv.as_ref(py))))
+                    }
+                })?;
+                let value = match maybe_new_value {
+                    Some(ref new_value) => new_value,
+                    None => value,
+                };
+                escape_formatter(output, state, value)
+            })
+        });
+        Ok(())
+    }
+
+    #[getter]
+    pub fn get_finalizer(&self) -> PyResult<Option<Py<PyAny>>> {
+        Ok(self.inner.lock().unwrap().finalizer_callback.clone())
+    }
+
     /// Sets a loader function for the environment.
     ///
     /// The loader function is invoked with the name of the template to load.  If the
     /// template exists the source code of the template should be returned a string,
     /// otherwise `None` can be used to indicate that the template does not exist.
     #[setter]
     pub fn set_loader(&self, callback: Option<&PyAny>) -> PyResult<()> {
```

### Comparing `minijinja-0.31.0/src/error_support.rs` & `minijinja-0.31.1/src/error_support.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/src/state.rs` & `minijinja-0.31.1/src/state.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/src/typeconv.rs` & `minijinja-0.31.1/src/typeconv.rs`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/tests/test_basic.py` & `minijinja-0.31.1/tests/test_basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import binascii
+import pytest
+
 from _pytest.unraisableexception import catch_unraisable_exception
-from minijinja import Environment, TemplateError, safe
+from minijinja import Environment, TemplateError, safe, pass_state
 
 
 def test_expression():
     env = Environment()
     rv = env.eval_expr("1 + b", b=42)
     assert rv == 43
     rv = env.eval_expr("range(n)", n=10)
@@ -126,32 +129,67 @@
     assert env.render_template("index.html") == "Hello from index.html"
     assert env.render_template("index.html") == "Hello from index.html"
     assert env.render_template("other.html") == "Hello from other.html"
     assert called == ["index.html", "index.html", "other.html"]
 
 
 def test_autoescape():
+    assert Environment().auto_escape_callback is None
+
     def auto_escape(name):
         assert name == "foo.html"
         return "html"
 
     env = Environment(
         auto_escape_callback=auto_escape,
         loader=lambda x: "Hello {{ foo }}",
     )
+    assert env.auto_escape_callback is auto_escape
 
     rv = env.render_template("foo.html", foo="<x>")
     assert rv == "Hello &lt;x&gt;"
 
     with catch_unraisable_exception() as cm:
         rv = env.render_template("invalid.html", foo="<x>")
         assert rv == "Hello <x>"
         assert cm.unraisable[0] is AssertionError
 
 
+def test_finalizer():
+    assert Environment().finalizer is None
+
+    @pass_state
+    def my_finalizer(state, value):
+        assert state.name == "<string>"
+        if value is None:
+            return ""
+        elif isinstance(value, bytes):
+            return binascii.b2a_hex(value).decode("utf-8")
+        return NotImplemented
+
+    env = Environment(finalizer=my_finalizer)
+
+    rv = env.render_str("[{{ foo }}]")
+    assert rv == "[]"
+    rv = env.render_str("[{{ foo }}]", foo=None)
+    assert rv == "[]"
+    rv = env.render_str("[{{ foo }}]", foo="test")
+    assert rv == "[test]"
+    rv = env.render_str("[{{ foo }}]", foo=b"test")
+    assert rv == "[74657374]"
+
+    def raising_finalizer(value):
+        1 / 0
+
+    env = Environment(finalizer=raising_finalizer)
+
+    with pytest.raises(ZeroDivisionError):
+        env.render_str("{{ whatever }}")
+
+
 def test_globals():
     env = Environment(globals={"x": 23, "y": lambda: 42})
     rv = env.eval_expr("[x, y(), z]", z=11)
     assert rv == [23, 42, 11]
 
 
 def test_honor_safe():
```

### Comparing `minijinja-0.31.0/tests/test_security.py` & `minijinja-0.31.1/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/tests/test_state.py` & `minijinja-0.31.1/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `minijinja-0.31.0/Cargo.lock` & `minijinja-0.31.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -341,17 +341,17 @@
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
 dependencies = [
@@ -392,17 +392,17 @@
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -467,15 +467,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.10",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
@@ -484,15 +484,15 @@
 name = "cxxbridge-macro"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.10",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "debug"
 version = "0.1.0"
 dependencies = [
  "minijinja",
@@ -517,22 +517,22 @@
 [[package]]
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
-name = "dynamic"
+name = "dynamic-context"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
-name = "dynamic-context"
+name = "dynamic-objects"
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "either"
@@ -559,22 +559,22 @@
 dependencies = [
  "minijinja",
  "serde_json",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.20"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "filters"
 version = "0.1.0"
 dependencies = [
  "minijinja",
@@ -602,76 +602,76 @@
 checksum = "76ee7a02da4d231650c7cea31349b889be2f45ddb3ef3032d2ec8185f6313fd2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "531ac96c6ff5fd7c62263c5e3c67a603af4fcaee2e1a0ae5565ba3a11e69e549"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "164713a5a0dcc3e7b4b1ed7d3b433cabc18025386f9339346e8daf15963cf7ac"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-io"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d422fa3cbe3b40dca574ab087abb5bc98258ea57eea3fd6f1fa7162c778b91"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb14ed937631bd8b8b8977f2c198443447a8355b6e3ca599f38c975e5a963b6"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec93083a4aecafb2a80a885c9de1f0ccae9dbd32c2bb54b0c3a65690e0b8d2f2"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -686,27 +686,27 @@
 version = "0.1.0"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -962,17 +962,17 @@
 checksum = "6cb51c9a029ddc91b07a787f1d86b53ccfa49b0e86688c946ebe8d3555685dd7"
 dependencies = [
  "libm",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
@@ -1072,14 +1072,22 @@
  "serde",
  "similar",
  "walkdir",
  "yaml-rust",
 ]
 
 [[package]]
+name = "invalid-value"
+version = "0.1.0"
+dependencies = [
+ "minijinja",
+ "serde",
+]
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -1133,17 +1141,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -1303,15 +1311,15 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "indexmap",
  "insta",
  "memo-map",
  "percent-encoding",
  "self_cell",
  "serde",
@@ -1319,15 +1327,15 @@
  "similar-asserts",
  "unicode-ident",
  "v_htmlescape",
 ]
 
 [[package]]
 name = "minijinja-autoreload"
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "minijinja",
  "notify",
 ]
 
 [[package]]
 name = "minijinja-dis"
@@ -1335,24 +1343,24 @@
 dependencies = [
  "argh",
  "minijinja",
 ]
 
 [[package]]
 name = "minijinja-py"
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "minijinja",
  "once_cell",
  "pyo3",
 ]
 
 [[package]]
 name = "minijinja-stack-ref"
-version = "0.31.0"
+version = "0.31.1"
 dependencies = [
  "minijinja",
 ]
 
 [[package]]
 name = "minimal"
 version = "0.1.0"
@@ -1488,50 +1496,50 @@
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "pest"
-version = "2.5.6"
+version = "2.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cbd939b234e95d72bc393d51788aec68aeeb5d51e748ca08ff3aad58cb722f7"
+checksum = "7b1403e8401ad5dedea73c626b99758535b342502f8d1e361f4a2dd952749122"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.5.6"
+version = "2.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a81186863f3d0a27340815be8f2078dd8050b14cd71913db9fbda795e5f707d7"
+checksum = "be99c4c1d2fc2769b1d00239431d711d08f6efedcecb8b6e30707160aee99c15"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.5.6"
+version = "2.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75a1ef20bf3193c15ac345acb32e26b3dc3223aff4d77ae4fc5359567683796b"
+checksum = "e56094789873daa36164de2e822b3888c6ae4b4f9da555a1103587658c805b1e"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.5.6"
+version = "2.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e3b284b1f13a20dc5ebc90aff59a51b8d7137c221131b52a7260c08cbc1cc80"
+checksum = "6733073c7cff3d8459fda0e42f13a047870242aed8b509fe98000928975f359e"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
@@ -1688,17 +1696,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proc-quote"
 version = "0.4.0"
@@ -1962,17 +1970,17 @@
 name = "self_cell"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ef965a420fe14fdac7dd018862966a4c14094f900e1650bbc71ddd7d580c8af"
 
 [[package]]
 name = "serde"
-version = "1.0.158"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "771d4d9c4163ee138805e12c710dd365e4f44be8be0503cb1bb9eb989425d9c9"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.4.5"
@@ -1982,28 +1990,28 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.158"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.10",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2110,17 +2118,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.10"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aad1363ed6d37b84299588d62d3a7d95b5a5c2d9aad5c85609fda12afaa1f40"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2180,15 +2188,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.10",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5516c27b78311c50bf42c071425c560ac799b11c30b31f87e3081965fe5e0180"
@@ -2231,17 +2239,17 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
 dependencies = [
  "autocfg",
  "pin-project-lite",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
@@ -2543,103 +2551,169 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.46.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
 dependencies = [
  "linked-hash-map",
 ]
```

### Comparing `minijinja-0.31.0/PKG-INFO` & `minijinja-0.31.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: minijinja
-Version: 0.31.0
+Version: 0.31.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 License-File: LICENSE
 Summary: An experimental Python binding of the Rust MiniJinja template engine.
 Keywords: jinja,template-engine
 Author-email: Armin Ronacher <armin.ronacher@active-4.com>
 Maintainer-email: Armin Ronacher <armin.ronacher@active-4.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Repository, https://github.com/mitsuhiko/minijinja
-Project-URL: Issue Tracker, https://github.com/mitsuhiko/minijinja/issues
 Project-URL: Donate, https://github.com/sponsors/mitsuhiko
+Project-URL: Issue Tracker, https://github.com/mitsuhiko/minijinja/issues
+Project-URL: Repository, https://github.com/mitsuhiko/minijinja
 
 <div align="center">
   <img src="https://github.com/mitsuhiko/minijinja/raw/main/artwork/logo.png" alt="" width=320>
   <p><strong>MiniJinja for Python: a powerful template engine for Rust and Python</strong></p>
 
 [![Build Status](https://github.com/mitsuhiko/minijinja/workflows/Tests/badge.svg?branch=main)](https://github.com/mitsuhiko/minijinja/actions?query=workflow%3ATests)
 [![License](https://img.shields.io/github/license/mitsuhiko/minijinja)](https://github.com/mitsuhiko/minijinja/blob/main/LICENSE)
@@ -125,14 +125,34 @@
 ```python
 env = Environment(auto_escape_callback=lambda x: x.endswith((".html", ".foo")))
 ```
 
 MiniJinja uses [markupsafe](https://github.com/pallets/markupsafe) if it's available
 on the Python side.  It will honor `__html__`.
 
+## Finalizers
+
+Instead of custom formatters like in MiniJinja, you can define a finalizer instead
+which is similar to how it works in Jinja2.  It's passed a value (or optional also
+the state as first argument whne `pass_state` is used) and can return a new value.
+If the special `NotImplemented` value is returned, the original value is rendered
+without any modification:
+
+```
+from minijinja import Environment
+
+def finalizer(value):
+    if value is None:
+	return ""
+    return NotImplemented
+
+env = Environment(finalizer=finalizer)
+assert env.render_str("{{ none }}") == ""
+```
+
 ## State Access
 
 Functions passed to the environment such as filters or global functions can
 optionally have the template state passed by using the `pass_state` parameter.
 This is similar to `pass_context` in Jinja2.  It can be used to look at the
 name of the template or to look up variables in the context.
```

