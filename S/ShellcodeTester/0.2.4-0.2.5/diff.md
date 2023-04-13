# Comparing `tmp/ShellcodeTester-0.2.4.tar.gz` & `tmp/ShellcodeTester-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellcodeTester-0.2.4.tar", last modified: Wed Apr 12 23:52:10 2023, max compression
+gzip compressed data, was "ShellcodeTester-0.2.5.tar", last modified: Thu Apr 13 03:21:24 2023, max compression
```

## Comparing `ShellcodeTester-0.2.4.tar` & `ShellcodeTester-0.2.5.tar`

### file list

```diff
@@ -1,55 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/nasmshell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/nasmshell/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/libs/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/nasmshell.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/linux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/macosx/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/macosx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/windows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/shell_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/asmfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/inlineassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/shellcodetester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/shellcodetester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.101195 ShellcodeTester-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-13 03:21:24.101195 ShellcodeTester-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.077195 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-13 03:21:24.000000 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-13 03:21:24.000000 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:21:24.000000 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-13 03:21:24.000000 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:21:24.000000 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-13 03:21:24.000000 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 03:21:24.000000 ShellcodeTester-0.2.5/ShellcodeTester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.077195 ShellcodeTester-0.2.5/nasmshell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/nasmshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/nasmshell/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/nasmshell/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.077195 ShellcodeTester-0.2.5/nasmshell/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/nasmshell/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/nasmshell/libs/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/nasmshell/nasmshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 03:21:24.101195 ShellcodeTester-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.077195 ShellcodeTester-0.2.5/shell_bins/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:21:19.000000 ShellcodeTester-0.2.5/shell_bins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.081195 ShellcodeTester-0.2.5/shell_bins/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:21:19.000000 ShellcodeTester-0.2.5/shell_bins/linux/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1951840 2023-04-13 03:20:17.000000 ShellcodeTester-0.2.5/shell_bins/linux/nasm
+-rw-r--r--   0 runner    (1001) docker     (123) 12329280 2023-04-13 03:20:07.000000 ShellcodeTester-0.2.5/shell_bins/linux/objdump
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.093195 ShellcodeTester-0.2.5/shell_bins/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:21:19.000000 ShellcodeTester-0.2.5/shell_bins/macosx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  3237896 2023-04-13 03:20:17.000000 ShellcodeTester-0.2.5/shell_bins/macosx/nasm
+-rw-r--r--   0 runner    (1001) docker     (123)   167120 2023-04-13 03:20:07.000000 ShellcodeTester-0.2.5/shell_bins/macosx/objdump
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.097195 ShellcodeTester-0.2.5/shell_bins/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:21:19.000000 ShellcodeTester-0.2.5/shell_bins/windows/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1638912 2023-04-13 03:20:17.000000 ShellcodeTester-0.2.5/shell_bins/windows/nasm.exe
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2410078 2023-04-13 03:20:17.000000 ShellcodeTester-0.2.5/shell_bins/windows/objdump.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.101195 ShellcodeTester-0.2.5/shell_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/asmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/inlineassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shell_libs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.101195 ShellcodeTester-0.2.5/shellcodetester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shellcodetester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shellcodetester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shellcodetester/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shellcodetester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shellcodetester/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/shellcodetester/shellcodetester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:24.101195 ShellcodeTester-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 03:21:17.000000 ShellcodeTester-0.2.5/tests/tests.py
```

### Comparing `ShellcodeTester-0.2.4/LICENSE` & `ShellcodeTester-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/PKG-INFO` & `ShellcodeTester-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.4
+Version: 0.2.5
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
```

### Comparing `ShellcodeTester-0.2.4/README.md` & `ShellcodeTester-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/ShellcodeTester.egg-info/PKG-INFO` & `ShellcodeTester-0.2.5/ShellcodeTester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.4
+Version: 0.2.5
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
```

### Comparing `ShellcodeTester-0.2.4/ShellcodeTester.egg-info/SOURCES.txt` & `ShellcodeTester-0.2.5/ShellcodeTester.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,22 @@
 nasmshell/args.py
 nasmshell/config.py
 nasmshell/nasmshell.py
 nasmshell/libs/__init__.py
 nasmshell/libs/cmd.py
 shell_bins/__init__.py
 shell_bins/linux/__init__.py
+shell_bins/linux/nasm
+shell_bins/linux/objdump
 shell_bins/macosx/__init__.py
+shell_bins/macosx/nasm
+shell_bins/macosx/objdump
 shell_bins/windows/__init__.py
+shell_bins/windows/nasm.exe
+shell_bins/windows/objdump.exe
 shell_libs/__init__.py
 shell_libs/__meta__.py
 shell_libs/asmfile.py
 shell_libs/assembler.py
 shell_libs/color.py
 shell_libs/compiler.py
 shell_libs/disassembler.py
```

### Comparing `ShellcodeTester-0.2.4/nasmshell/args.py` & `ShellcodeTester-0.2.5/nasmshell/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/nasmshell/config.py` & `ShellcodeTester-0.2.5/nasmshell/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/nasmshell/libs/cmd.py` & `ShellcodeTester-0.2.5/nasmshell/libs/cmd.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/nasmshell/nasmshell.py` & `ShellcodeTester-0.2.5/nasmshell/nasmshell.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/setup.py` & `ShellcodeTester-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/asmfile.py` & `ShellcodeTester-0.2.5/shell_libs/asmfile.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/assembler.py` & `ShellcodeTester-0.2.5/shell_libs/assembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/color.py` & `ShellcodeTester-0.2.5/shell_libs/color.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/compiler.py` & `ShellcodeTester-0.2.5/shell_libs/compiler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/disassembler.py` & `ShellcodeTester-0.2.5/shell_libs/disassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/inlineassembler.py` & `ShellcodeTester-0.2.5/shell_libs/inlineassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/logger.py` & `ShellcodeTester-0.2.5/shell_libs/logger.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/process.py` & `ShellcodeTester-0.2.5/shell_libs/process.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/runner.py` & `ShellcodeTester-0.2.5/shell_libs/runner.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/tools.py` & `ShellcodeTester-0.2.5/shell_libs/tools.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shell_libs/transform.py` & `ShellcodeTester-0.2.5/shell_libs/transform.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shellcodetester/args.py` & `ShellcodeTester-0.2.5/shellcodetester/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shellcodetester/config.py` & `ShellcodeTester-0.2.5/shellcodetester/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shellcodetester/password.py` & `ShellcodeTester-0.2.5/shellcodetester/password.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.4/shellcodetester/shellcodetester.py` & `ShellcodeTester-0.2.5/shellcodetester/shellcodetester.py`

 * *Files identical despite different names*

