# Comparing `tmp/ket-lang-0.5.2.tar.gz` & `tmp/ket-lang-0.5.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ket-lang-0.5.2.tar", last modified: Wed Mar 15 16:30:55 2023, max compression
+gzip compressed data, was "ket-lang-0.5.3b1.tar", last modified: Thu Apr 13 18:04:47 2023, max compression
```

## Comparing `ket-lang-0.5.2.tar` & `ket-lang-0.5.3b1.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.295706 ket-lang-0.5.2/
--rw-rw-rw-   0 root         (0) root         (0)    11455 2023-03-15 16:30:42.000000 ket-lang-0.5.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-03-15 16:30:42.000000 ket-lang-0.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7169 2023-03-15 16:30:55.295706 ket-lang-0.5.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6416 2023-03-15 16:30:42.000000 ket-lang-0.5.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-03-15 16:30:42.000000 ket-lang-0.5.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1131 2023-03-15 16:30:55.296706 ket-lang-0.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-03-15 16:30:42.000000 ket-lang-0.5.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.270704 ket-lang-0.5.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.275704 ket-lang-0.5.2/src/ket/
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    28956 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.277704 ket-lang-0.5.2/src/ket/clib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/clib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3937 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/clib/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     8828 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/clib/libket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.277704 ket-lang-0.5.2/src/ket/clib/libs/
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/clib/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.279704 ket-lang-0.5.2/src/ket/clib/libs/kbw/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      224 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/README.md
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/kbw.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.282705 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/bitwise.rs
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/c_wrapper.rs
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/convert.rs
--rw-rw-rw-   0 root         (0) root         (0)    20349 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/dense.rs
--rw-rw-rw-   0 root         (0) root         (0)     2213 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     9825 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/quantum_execution.rs
--rw-rw-rw-   0 root         (0) root         (0)    20230 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/kbw/src/sparse.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.285705 ket-lang-0.5.2/src/ket/clib/libs/libket/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8385 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/libket.h
--rw-rw-rw-   0 root         (0) root         (0)    10365 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/libket.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.288705 ket-lang-0.5.2/src/ket/clib/libs/libket/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.289705 ket-lang-0.5.2/src/ket/clib/libs/libket/src/c_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/c_wrapper/error.rs
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/c_wrapper/mod.rs
--rw-rw-rw-   0 root         (0) root         (0)     6838 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/c_wrapper/objects.rs
--rw-rw-rw-   0 root         (0) root         (0)    10980 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/c_wrapper/process.rs
--rw-rw-rw-   0 root         (0) root         (0)     5734 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/code_block.rs
--rw-rw-rw-   0 root         (0) root         (0)     4523 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     6098 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/gates.rs
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/instruction.rs
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/ir.rs
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/object.rs
--rw-rw-rw-   0 root         (0) root         (0)    19231 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/process.rs
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-15 16:30:43.000000 ket-lang-0.5.2/src/ket/clib/libs/libket/src/serialize.rs
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/clib/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.290706 ket-lang-0.5.2/src/ket/gates/
--rw-rw-rw-   0 root         (0) root         (0)     8530 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/gates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/gates/base_gates.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/gates/quantum_gate.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/import_ket.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.291705 ket-lang-0.5.2/src/ket/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/preprocessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/preprocessor/statements.py
--rw-rw-rw-   0 root         (0) root         (0)     8995 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/preprocessor/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     3751 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.292706 ket-lang-0.5.2/src/ket/standard/
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4593 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/standard/adj.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-03-15 16:30:42.000000 ket-lang-0.5.2/src/ket/standard/ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.294706 ket-lang-0.5.2/src/ket_lang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7169 2023-03-15 16:30:55.000000 ket-lang-0.5.2/src/ket_lang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2141 2023-03-15 16:30:55.000000 ket-lang-0.5.2/src/ket_lang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 16:30:55.000000 ket-lang-0.5.2/src/ket_lang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-03-15 16:30:55.000000 ket-lang-0.5.2/src/ket_lang.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 16:30:55.000000 ket-lang-0.5.2/src/ket_lang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-15 16:30:55.000000 ket-lang-0.5.2/src/ket_lang.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 16:30:55.295706 ket-lang-0.5.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-03-15 16:30:42.000000 ket-lang-0.5.2/tests/test_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/
+-rw-rw-rw-   0 root         (0) root         (0)    11455 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7166 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6412 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-04-13 18:04:47.266780 ket-lang-0.5.3b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.236778 ket-lang-0.5.3b1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.242778 ket-lang-0.5.3b1/src/ket/
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28956 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.244778 ket-lang-0.5.3b1/src/ket/clib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3937 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     8828 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/libket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.244778 ket-lang-0.5.3b1/src/ket/clib/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.247779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-13 18:04:35.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/kbw.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.250779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/bitwise.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/c_wrapper.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1942 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/convert.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20501 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/dense.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     9825 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/quantum_execution.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20230 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/sparse.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.250779 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/kbw/tests/shor.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.253779 ket-lang-0.5.3b1/src/ket/clib/libs/libket/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      351 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8385 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.h
+-rw-rw-rw-   0 root         (0) root         (0)    10365 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.257779 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.258780 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6838 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs
+-rw-rw-rw-   0 root         (0) root         (0)    10966 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)     5725 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/code_block.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6275 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/gates.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/instruction.rs
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/ir.rs
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/object.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20114 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-04-13 18:04:36.000000 ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/serialize.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/clib/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.259780 ket-lang-0.5.3b1/src/ket/gates/
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/base_gates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/gates/quantum_gate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/import_ket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     5795 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.261780 ket-lang-0.5.3b1/src/ket/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/statements.py
+-rw-rw-rw-   0 root         (0) root         (0)     8995 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/preprocessor/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3751 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.262780 ket-lang-0.5.3b1/src/ket/standard/
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/adj.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/src/ket/standard/ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.264780 ket-lang-0.5.3b1/src/ket_lang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7166 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-13 18:04:47.000000 ket-lang-0.5.3b1/src/ket_lang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 18:04:47.265780 ket-lang-0.5.3b1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3056 2023-04-13 18:04:34.000000 ket-lang-0.5.3b1/tests/test_gates.py
```

### Comparing `ket-lang-0.5.2/LICENSE` & `ket-lang-0.5.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/PKG-INFO` & `ket-lang-0.5.3b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.5.2
+Version: 0.5.3b1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: ev.crr97@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
@@ -27,32 +27,31 @@
 
 [[_TOC_]]
 
 Ket is an embedded programming language that introduces the ease of Python to quantum programming, letting anyone quickly prototype and test a quantum application.
 
 Python is the most widely used programming language for machine learning and data science and has been the language of choice for quantum programming. Ket is a Python-embedded language, but many can use it as a Python library in most cases. So you can use Ket together with NumPy, ScyPy, Pandas, and other popular Python libraries.
 
+Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See <https://quantumket.org> to learn more about Ket.
 
-Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See https://quantumket.org to learn more about Ket.
-
-## Installation :arrow_down:
+## Installation :arrow_down
 
 Ket requires Python 3.7 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
 
 You can install Ket using [`pip`](https://pip.pypa.io/en/stable/user_guide/). To do so, copy and paste the following command into your terminal:
 
 ```shell
 pip install ket-lang
 ```
 
-## Documentation :scroll:
+## Documentation :scroll
 
-Documentation available at https://quantumket.org.
+Documentation available at <https://quantumket.org>.
 
-## Examples :bulb:
+## Examples :bulb
 
 ### Grover's Algorithm
 
 ```py
 from ket import *
 from math import sqrt, pi
 
@@ -69,15 +68,15 @@
 
 n = 8
 looking_for = 13
 print(grover(n, phase_on(looking_for)))
 # 13
 ```
 
-### Shor's Algorithm 
+### Shor's Algorithm
 
 ```py
 from ket import *
 from ket.lib import qft
 from ket.plugins import pown
 from random import randint
 from functools import reduce
@@ -199,37 +198,37 @@
 # Bob Qubit:
 # |0⟩     (50.00%)
 #  0.707107               ≅      1/√2
 # |1⟩     (50.00%)
 #  0.500000+0.500000i     ≅  (1+i)/√4
 ```
 
-## Ket Development :hammer:
+## Ket Development :hammer
 
 Setup for Ket development:
 
 ```shell
 git clone https://gitlab.com/quantum-ket/ket.git
 cd ket
 pip install -e . --user
 ```
 
 If you are using [VS Code](https://code.visualstudio.com/), Ket has a [Dev Container](https://code.visualstudio.com/docs/remote/containers) :whale:.
 
-## Roadmap :notebook_with_decorative_cover:
+## Roadmap :notebook_with_decorative_cover
 
 * [ ] Quantum gate decomposition.
 * [ ] Quantum code optimization.
 * [ ] Quantum circuit visualization.
   
 * :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks like the [`qft`](https://quantumket.org/ket#ket.lib.qft).  
 * :package: Full quantum algorithm implementations must be packaged with  Ket as a dependency.
 * :x: Low-level quantum control, like pulse programming, is out of Ket's scope.
 
-## Cite Ket :book:
+## Cite Ket :book
 
 When using Ket for research projects, please cite:
 
 > Evandro Chagas Ribeiro da Rosa and Rafael de Santiago. 2021. Ket Quantum Programming. J. Emerg. Technol. Comput. Syst. 18, 1, Article 12 (January 2022), 25 pages. DOI: [10.1145/3474224](https://doi.org/10.1145/3474224)
 
 ```bibtex
 @article{ket,
@@ -248,10 +247,10 @@
    month = oct,
    articleno = {12},
    numpages = {25},
    keywords = {Quantum programming, cloud quantum computation, qubit simulation}
 }
 ```
 
-## Community :family:
+## Community :family
 
 Join the conversation on our [Discord](https://discord.gg/XkXvwRQ9aa).
```

### Comparing `ket-lang-0.5.2/README.md` & `ket-lang-0.5.3b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 
 [[_TOC_]]
 
 Ket is an embedded programming language that introduces the ease of Python to quantum programming, letting anyone quickly prototype and test a quantum application.
 
 Python is the most widely used programming language for machine learning and data science and has been the language of choice for quantum programming. Ket is a Python-embedded language, but many can use it as a Python library in most cases. So you can use Ket together with NumPy, ScyPy, Pandas, and other popular Python libraries.
 
+Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See <https://quantumket.org> to learn more about Ket.
 
-Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See https://quantumket.org to learn more about Ket.
-
-## Installation :arrow_down:
+## Installation :arrow_down
 
 Ket requires Python 3.7 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
 
 You can install Ket using [`pip`](https://pip.pypa.io/en/stable/user_guide/). To do so, copy and paste the following command into your terminal:
 
 ```shell
 pip install ket-lang
 ```
 
-## Documentation :scroll:
+## Documentation :scroll
 
-Documentation available at https://quantumket.org.
+Documentation available at <https://quantumket.org>.
 
-## Examples :bulb:
+## Examples :bulb
 
 ### Grover's Algorithm
 
 ```py
 from ket import *
 from math import sqrt, pi
 
@@ -47,15 +46,15 @@
 
 n = 8
 looking_for = 13
 print(grover(n, phase_on(looking_for)))
 # 13
 ```
 
-### Shor's Algorithm 
+### Shor's Algorithm
 
 ```py
 from ket import *
 from ket.lib import qft
 from ket.plugins import pown
 from random import randint
 from functools import reduce
@@ -177,37 +176,37 @@
 # Bob Qubit:
 # |0⟩     (50.00%)
 #  0.707107               ≅      1/√2
 # |1⟩     (50.00%)
 #  0.500000+0.500000i     ≅  (1+i)/√4
 ```
 
-## Ket Development :hammer:
+## Ket Development :hammer
 
 Setup for Ket development:
 
 ```shell
 git clone https://gitlab.com/quantum-ket/ket.git
 cd ket
 pip install -e . --user
 ```
 
 If you are using [VS Code](https://code.visualstudio.com/), Ket has a [Dev Container](https://code.visualstudio.com/docs/remote/containers) :whale:.
 
-## Roadmap :notebook_with_decorative_cover:
+## Roadmap :notebook_with_decorative_cover
 
 * [ ] Quantum gate decomposition.
 * [ ] Quantum code optimization.
 * [ ] Quantum circuit visualization.
   
 * :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks like the [`qft`](https://quantumket.org/ket#ket.lib.qft).  
 * :package: Full quantum algorithm implementations must be packaged with  Ket as a dependency.
 * :x: Low-level quantum control, like pulse programming, is out of Ket's scope.
 
-## Cite Ket :book:
+## Cite Ket :book
 
 When using Ket for research projects, please cite:
 
 > Evandro Chagas Ribeiro da Rosa and Rafael de Santiago. 2021. Ket Quantum Programming. J. Emerg. Technol. Comput. Syst. 18, 1, Article 12 (January 2022), 25 pages. DOI: [10.1145/3474224](https://doi.org/10.1145/3474224)
 
 ```bibtex
 @article{ket,
@@ -226,10 +225,10 @@
    month = oct,
    articleno = {12},
    numpages = {25},
    keywords = {Quantum programming, cloud quantum computation, qubit simulation}
 }
 ```
 
-## Community :family:
+## Community :family
 
-Join the conversation on our [Discord](https://discord.gg/XkXvwRQ9aa).
+Join the conversation on our [Discord](https://discord.gg/XkXvwRQ9aa).
```

### Comparing `ket-lang-0.5.2/setup.cfg` & `ket-lang-0.5.3b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/__init__.py` & `ket-lang-0.5.3b1/src/ket/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .process import *
 from .gates import __all__ as all_gate
 from .import_ket import __all__ as all_import
 from .base import __all__ as all_base
 from .standard import __all__ as all_standard
 from .process import __all__ as all_process
 
-__version__ = '0.5.2'
+__version__ = '0.5.3b1'
 __all__ = all_gate + all_import + all_base + all_standard + all_process
 
 from .import_ket import code_ket
 
 from .base import QUANTUM_EXECUTION_TARGET
 if QUANTUM_EXECUTION_TARGET is None:
     from .kbw import use_sparse
```

### Comparing `ket-lang-0.5.2/src/ket/__main__.py` & `ket-lang-0.5.3b1/src/ket/__main__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/base.py` & `ket-lang-0.5.3b1/src/ket/base.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/kbw.py` & `ket-lang-0.5.3b1/src/ket/clib/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libket.py` & `ket-lang-0.5.3b1/src/ket/clib/libket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/__init__.py` & `ket-lang-0.5.3b1/src/ket/clib/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/Cargo.toml` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "kbw"
-version = "0.1.4"
-authors = ["Evandro Chagas Ribeiro da Rosa <ev.crr97@gmail.com>"]
+version = "0.1.5"
+authors = ["Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>"]
 description = "Ket Bitwise Simulator"
 repository = "https://gitlab.com/quantum-ket/kbw"
 documentation = "https://quantumket.org"
 license = "Apache-2.0"
 readme = "README.md"
 edition = "2021"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-libket = "0.2.2"
+libket = "0.2.3"
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 bincode = "1.3"
 num = "0.4"
 rand = "0.8.5"
 rayon = "1.5.3"
 twox-hash = "1.6.3"
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/LICENSE` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/kbw.h` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/kbw.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/src/bitwise.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/bitwise.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/src/c_wrapper.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/c_wrapper.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/src/convert.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/convert.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/src/dense.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/dense.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use crate::error::{KBWError, Result};
 use crate::quantum_execution::QuantumExecution;
 use crate::{bitwise::*, convert};
 use itertools::Itertools;
 use ket::ir::Metrics;
+use num::complex::ComplexFloat;
 use num::{complex::Complex64, Zero};
 use rand::distributions::WeightedIndex;
 use rand::prelude::*;
 use rayon::prelude::*;
 use std::f64::consts::FRAC_1_SQRT_2;
 
 pub struct Dense {
@@ -63,23 +64,28 @@
         let args: Vec<&str> = args.split(' ').collect();
         let x: u64 = args[0].parse().unwrap();
         let n: u64 = args[1].parse().unwrap();
         let l = bit_len(n);
 
         next_state
             .par_iter_mut()
-            .enumerate()
-            .for_each(|(state, amp)| {
+            .for_each(|x| *x = Complex64::new(0.0, 0.0));
+
+        current_state.iter().enumerate().for_each(|(state, amp)| {
+            if amp.abs() > 1e-10 {
                 let a_b = (state & ((1 << qubits_size) - 1)) as u64;
                 let a = a_b >> l;
-                let mut b = a_b & ((1 << l) - 1);
-                b *= crate::bitwise::pown(x, a, n);
-                let a_b = (a << l) | b;
-                *amp = current_state[a_b as usize];
-            });
+                let b = a_b & ((1u64 << l) - 1);
+
+                let new_b = b * crate::bitwise::pown(x, a, n);
+                let a_b = (a << l) | new_b;
+
+                next_state[a_b as usize] = *amp;
+            }
+        });
     }
 
     fn dump_vec(&self, qubits: &[usize]) -> ket::DumpData {
         let state = self.get_current_state();
         let (basis_states, amplitudes_real, amplitudes_imag): (Vec<_>, Vec<_>, Vec<_>) = state
             .iter()
             .enumerate()
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/src/error.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/error.rs`

 * *Files 15% similar despite different names*

```diff
@@ -17,27 +17,23 @@
 }
 
 pub type Result<T> = result::Result<T, KBWError>;
 
 impl KBWError {
     pub fn to_str(&self) -> &'static str {
         match self {
-            KBWError::Success => "the call returned successfully",
-            KBWError::UndefinedError => "undefined error",
-            KBWError::Timeout => "quantum execution timeout",
-            KBWError::OutOfQubits => {
-                "cannot allocate more qubits (maybe you are deallocating too many qubits as dirty)"
-            }
-            KBWError::UnsupportedNumberOfQubits => {
-                "dense simulator do not allow more then 32 qubits"
-            }
-            KBWError::UnsupportedPlugin => "unsupported plugin gate",
-            KBWError::NotReadyForExecution => "not ready for execution",
-            KBWError::UndefinedSimMode => "undefined simulation mode",
-            KBWError::UndefinedDataType => "undefined data type",
+            KBWError::Success => "The function call completed successfully.",
+            KBWError::UndefinedError => "An undefined error occurred.",
+            KBWError::Timeout => "The quantum execution has timed out.",
+            KBWError::OutOfQubits => "Cannot allocate more qubits. Ensure you are not deallocating too many qubits as dirty.",
+            KBWError::UnsupportedNumberOfQubits => "The number of requested qubits is not supported.",
+            KBWError::UnsupportedPlugin => "The specified plugin gate is not supported.",
+            KBWError::NotReadyForExecution => "The process is not yet ready for execution.",
+            KBWError::UndefinedSimMode => "The simulation mode is undefined.",
+            KBWError::UndefinedDataType => "The data type is undefined.",
         }
     }
 
     pub fn error_code(&self) -> i32 {
         self.to_i32().unwrap()
     }
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/src/quantum_execution.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/quantum_execution.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/kbw/src/sparse.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/kbw/src/sparse.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/Cargo.toml` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "libket"
-version = "0.2.2"
-authors = ["Evandro Chagas Ribeiro da Rosa <ev.crr97@gmail.com>"]
+version = "0.2.3"
+authors = ["Evandro Chagas Ribeiro da Rosa <evandro@quantuloop.com>"]
 description = "Runtime library for the Ket programming language"
 repository = "https://gitlab.com/quantum-ket/libket"
 documentation = "https://quantumket.org"
 license = "Apache-2.0"
 readme = "README.md"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 bincode = "1.3"
-num = "0.4.0"
+num = "0.4"
 num-traits = "0.2"
 num-derive = "0.3.3"
 rand = "0.8.5"
 
 [lib]
 name = "ket"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/LICENSE` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/libket.h` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/libket.hpp` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/libket.hpp`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/c_wrapper/objects.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/c_wrapper/process.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/c_wrapper/process.rs`

 * *Files 0% similar despite different names*

```diff
@@ -392,10 +392,10 @@
 
 #[no_mangle]
 pub unsafe extern "C" fn ket_features_register_plugin(
     features: &mut Features,
     name: *const c_char,
 ) -> i32 {
     let name = unsafe { CStr::from_ptr(name) }.to_str().unwrap();
-    features.register_plugin(String::from(name));
+    features.register_plugin(name);
     KetError::Success.error_code()
 }
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/code_block.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/code_block.rs`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,16 @@
             Instruction::End(_) => {
                 if !self.adj_instructions.is_empty() {
                     return Err(KetError::NonGateInstruction);
                 }
                 self.ended = true;
                 self.block.depth = self
                     .gate_per_qubit
-                    .iter()
-                    .map(|(_, num)| *num)
+                    .values()
+                    .copied()
                     .max()
                     .unwrap_or_default();
                 Some(instruction)
             }
             _ => {
                 if !self.adj_instructions.is_empty() {
                     return Err(KetError::NonGateInstruction);
@@ -82,15 +82,15 @@
         } else {
             self.adj_instructions.push(Vec::new());
             Ok(())
         }
     }
 
     pub fn adj_end(&mut self) -> Result<()> {
-        if self.adj_instructions.is_empty(){
+        if self.adj_instructions.is_empty() {
             return Err(KetError::NoAdj);
         }
 
         if self.adj_instructions.len() == 1 {
             while let Some(instruction) = self.adj_instructions.last_mut().unwrap().pop() {
                 self.block.instructions.push(instruction);
             }
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/error.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/gates.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/gates.rs`

 * *Files 6% similar despite different names*

```diff
@@ -210,14 +210,21 @@
     Ok(result)
 }
 
 pub fn measure(qubits: &mut Quant) -> Result<Future> {
     qubits.process.borrow_mut().measure_ref(&mut qubits.qubits)
 }
 
+pub fn plugin(name: &str, args: &str, qubits: &Quant) -> Result<()> {
+    qubits
+        .process
+        .borrow_mut()
+        .apply_plugin_ref(name, &qubits.qubits, args)
+}
+
 pub fn dump(qubits: &Quant) -> Result<Dump> {
     qubits.process.borrow_mut().dump_ref(&qubits.qubits)
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/instruction.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/instruction.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/ir.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/ir.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/object.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/object.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/process.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/process.rs`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,16 @@
             classical_control_flow: false,
             allow_dump: false,
             allow_measure: true,
             continue_after_dump: false,
         }
     }
 
-    pub fn register_plugin(&mut self, plugin: String) {
-        self.plugins.insert(plugin);
+    pub fn register_plugin(&mut self, plugin: &str) {
+        self.plugins.insert(plugin.to_string());
     }
 }
 
 #[derive(Debug)]
 
 pub struct Process {
     pid: usize,
@@ -246,14 +246,46 @@
                 target: target.iter().map(|q| q.index()).collect(),
                 args: String::from(args),
             })?;
 
         Ok(())
     }
 
+    pub fn apply_plugin_ref(
+        &mut self,
+        name: &str,
+        target: &[Rc<RefCell<Qubit>>],
+        args: &str,
+    ) -> Result<()> {
+        if !self.features.plugins.contains(name) {
+            return Err(KetError::PluginNotRegistered);
+        }
+
+        if !self.ctrl_stack.is_empty() {
+            return Err(KetError::PluginOnCtrl);
+        }
+
+        for target in target {
+            self.match_pid(target.as_ref().borrow().deref())?;
+        }
+
+        self.metrics.plugins.insert(String::from(name));
+
+        self.blocks
+            .get_mut(self.current_block)
+            .unwrap()
+            .add_instruction(Instruction::Plugin {
+                name: String::from(name),
+                target: target.iter().map(|q| q.as_ref().borrow().index()).collect(),
+                args: String::from(args),
+            })?;
+
+        Ok(())
+    }
+
     pub fn measure(&mut self, qubits: &mut [&mut Qubit]) -> Result<Future> {
         if !self.features.allow_measure {
             return Err(KetError::MeasureNotAllowed);
         }
 
         for qubit in qubits.iter_mut() {
             self.match_pid(*qubit)?;
```

### Comparing `ket-lang-0.5.2/src/ket/clib/libs/libket/src/serialize.rs` & `ket-lang-0.5.3b1/src/ket/clib/libs/libket/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/clib/wrapper.py` & `ket-lang-0.5.3b1/src/ket/clib/wrapper.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/gates/__init__.py` & `ket-lang-0.5.3b1/src/ket/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/gates/base_gates.py` & `ket-lang-0.5.3b1/src/ket/gates/base_gates.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/gates/quantum_gate.py` & `ket-lang-0.5.3b1/src/ket/gates/quantum_gate.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/import_ket.py` & `ket-lang-0.5.3b1/src/ket/import_ket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/kbw.py` & `ket-lang-0.5.3b1/src/ket/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/lib.py` & `ket-lang-0.5.3b1/src/ket/lib.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/plugins.py` & `ket-lang-0.5.3b1/src/ket/plugins.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/preprocessor/statements.py` & `ket-lang-0.5.3b1/src/ket/preprocessor/statements.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/preprocessor/transformer.py` & `ket-lang-0.5.3b1/src/ket/preprocessor/transformer.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/process.py` & `ket-lang-0.5.3b1/src/ket/process.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/standard/__init__.py` & `ket-lang-0.5.3b1/src/ket/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/standard/adj.py` & `ket-lang-0.5.3b1/src/ket/standard/adj.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket/standard/ctrl.py` & `ket-lang-0.5.3b1/src/ket/standard/ctrl.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.5.2/src/ket_lang.egg-info/PKG-INFO` & `ket-lang-0.5.3b1/src/ket_lang.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.5.2
+Version: 0.5.3b1
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: ev.crr97@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
@@ -27,32 +27,31 @@
 
 [[_TOC_]]
 
 Ket is an embedded programming language that introduces the ease of Python to quantum programming, letting anyone quickly prototype and test a quantum application.
 
 Python is the most widely used programming language for machine learning and data science and has been the language of choice for quantum programming. Ket is a Python-embedded language, but many can use it as a Python library in most cases. So you can use Ket together with NumPy, ScyPy, Pandas, and other popular Python libraries.
 
+Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See <https://quantumket.org> to learn more about Ket.
 
-Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See https://quantumket.org to learn more about Ket.
-
-## Installation :arrow_down:
+## Installation :arrow_down
 
 Ket requires Python 3.7 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
 
 You can install Ket using [`pip`](https://pip.pypa.io/en/stable/user_guide/). To do so, copy and paste the following command into your terminal:
 
 ```shell
 pip install ket-lang
 ```
 
-## Documentation :scroll:
+## Documentation :scroll
 
-Documentation available at https://quantumket.org.
+Documentation available at <https://quantumket.org>.
 
-## Examples :bulb:
+## Examples :bulb
 
 ### Grover's Algorithm
 
 ```py
 from ket import *
 from math import sqrt, pi
 
@@ -69,15 +68,15 @@
 
 n = 8
 looking_for = 13
 print(grover(n, phase_on(looking_for)))
 # 13
 ```
 
-### Shor's Algorithm 
+### Shor's Algorithm
 
 ```py
 from ket import *
 from ket.lib import qft
 from ket.plugins import pown
 from random import randint
 from functools import reduce
@@ -199,37 +198,37 @@
 # Bob Qubit:
 # |0⟩     (50.00%)
 #  0.707107               ≅      1/√2
 # |1⟩     (50.00%)
 #  0.500000+0.500000i     ≅  (1+i)/√4
 ```
 
-## Ket Development :hammer:
+## Ket Development :hammer
 
 Setup for Ket development:
 
 ```shell
 git clone https://gitlab.com/quantum-ket/ket.git
 cd ket
 pip install -e . --user
 ```
 
 If you are using [VS Code](https://code.visualstudio.com/), Ket has a [Dev Container](https://code.visualstudio.com/docs/remote/containers) :whale:.
 
-## Roadmap :notebook_with_decorative_cover:
+## Roadmap :notebook_with_decorative_cover
 
 * [ ] Quantum gate decomposition.
 * [ ] Quantum code optimization.
 * [ ] Quantum circuit visualization.
   
 * :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks like the [`qft`](https://quantumket.org/ket#ket.lib.qft).  
 * :package: Full quantum algorithm implementations must be packaged with  Ket as a dependency.
 * :x: Low-level quantum control, like pulse programming, is out of Ket's scope.
 
-## Cite Ket :book:
+## Cite Ket :book
 
 When using Ket for research projects, please cite:
 
 > Evandro Chagas Ribeiro da Rosa and Rafael de Santiago. 2021. Ket Quantum Programming. J. Emerg. Technol. Comput. Syst. 18, 1, Article 12 (January 2022), 25 pages. DOI: [10.1145/3474224](https://doi.org/10.1145/3474224)
 
 ```bibtex
 @article{ket,
@@ -248,10 +247,10 @@
    month = oct,
    articleno = {12},
    numpages = {25},
    keywords = {Quantum programming, cloud quantum computation, qubit simulation}
 }
 ```
 
-## Community :family:
+## Community :family
 
 Join the conversation on our [Discord](https://discord.gg/XkXvwRQ9aa).
```

### Comparing `ket-lang-0.5.2/src/ket_lang.egg-info/SOURCES.txt` & `ket-lang-0.5.3b1/src/ket_lang.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 src/ket/clib/libs/kbw/src/c_wrapper.rs
 src/ket/clib/libs/kbw/src/convert.rs
 src/ket/clib/libs/kbw/src/dense.rs
 src/ket/clib/libs/kbw/src/error.rs
 src/ket/clib/libs/kbw/src/lib.rs
 src/ket/clib/libs/kbw/src/quantum_execution.rs
 src/ket/clib/libs/kbw/src/sparse.rs
+src/ket/clib/libs/kbw/tests/shor.rs
 src/ket/clib/libs/libket/.git
 src/ket/clib/libs/libket/.gitignore
+src/ket/clib/libs/libket/CHANGELOG.md
 src/ket/clib/libs/libket/Cargo.toml
 src/ket/clib/libs/libket/LICENSE
 src/ket/clib/libs/libket/README.md
 src/ket/clib/libs/libket/libket.h
 src/ket/clib/libs/libket/libket.hpp
 src/ket/clib/libs/libket/src/code_block.rs
 src/ket/clib/libs/libket/src/error.rs
```

### Comparing `ket-lang-0.5.2/tests/test_gates.py` & `ket-lang-0.5.3b1/tests/test_gates.py`

 * *Files identical despite different names*

