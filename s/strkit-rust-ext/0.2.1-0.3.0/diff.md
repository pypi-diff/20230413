# Comparing `tmp/strkit_rust_ext-0.2.1.tar.gz` & `tmp/strkit_rust_ext-0.3.0.tar.gz`

## Comparing `strkit_rust_ext-0.2.1.tar` & `strkit_rust_ext-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 strkit_rust_ext-0.2.1/Cargo.toml
--rw-r--r--   0     1001      123     3187 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/.github/workflows/build-release.yml
--rw-r--r--   0     1001      123      685 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/.gitignore
--rw-r--r--   0     1001      123    35149 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/LICENSE
--rw-r--r--   0     1001      123      328 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/README.md
--rw-r--r--   0     1001      123      377 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/pyproject.toml
--rw-r--r--   0     1001      123     1172 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/src/lib.rs
--rw-r--r--   0     1001      123      300 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/strkit_rust_ext.pyi
--rw-r--r--   0     1001      123      636 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/tests/test_snvs.py
--rw-r--r--   0     1001      123     7659 2023-04-09 14:29:04.000000 strkit_rust_ext-0.2.1/Cargo.lock
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 strkit_rust_ext-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      255 1970-01-01 00:00:00.000000 strkit_rust_ext-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      123     3187 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/.github/workflows/build-release.yml
+-rw-r--r--   0     1001      123      685 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/.gitignore
+-rw-r--r--   0     1001      123    35149 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/LICENSE
+-rw-r--r--   0     1001      123      328 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/README.md
+-rw-r--r--   0     1001      123      377 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/pyproject.toml
+-rw-r--r--   0     1001      123     4540 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      123      569 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/strkit_rust_ext.pyi
+-rw-r--r--   0     1001      123      669 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/tests/test_snvs.py
+-rw-r--r--   0     1001      123     7659 2023-04-13 12:10:29.000000 strkit_rust_ext-0.3.0/Cargo.lock
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 strkit_rust_ext-0.3.0/PKG-INFO
```

### Comparing `strkit_rust_ext-0.2.1/.github/workflows/build-release.yml` & `strkit_rust_ext-0.3.0/.github/workflows/build-release.yml`

 * *Files identical despite different names*

### Comparing `strkit_rust_ext-0.2.1/.gitignore` & `strkit_rust_ext-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `strkit_rust_ext-0.2.1/LICENSE` & `strkit_rust_ext-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strkit_rust_ext-0.2.1/Cargo.lock` & `strkit_rust_ext-0.3.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "strkit_rust_ext"
-version = "0.2.1"
+version = "0.3.0"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
```

### Comparing `strkit_rust_ext-0.2.1/PKG-INFO` & `strkit_rust_ext-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strkit_rust_ext
-Version: 0.2.1
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

