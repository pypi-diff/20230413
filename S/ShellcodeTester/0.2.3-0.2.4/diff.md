# Comparing `tmp/ShellcodeTester-0.2.3.tar.gz` & `tmp/ShellcodeTester-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShellcodeTester-0.2.3.tar", last modified: Wed Apr 12 14:30:46 2023, max compression
+gzip compressed data, was "ShellcodeTester-0.2.4.tar", last modified: Wed Apr 12 23:52:10 2023, max compression
```

## Comparing `ShellcodeTester-0.2.3.tar` & `ShellcodeTester-0.2.4.tar`

### file list

```diff
@@ -1,49 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.082898 ShellcodeTester-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-12 14:30:46.082898 ShellcodeTester-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.070898 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 14:30:46.000000 ShellcodeTester-0.2.3/ShellcodeTester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.074899 ShellcodeTester-0.2.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.074899 ShellcodeTester-0.2.3/nasmshell/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.074899 ShellcodeTester-0.2.3/nasmshell/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/libs/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/nasmshell/nasmshell.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 14:30:46.082898 ShellcodeTester-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.078899 ShellcodeTester-0.2.3/shell_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/asmfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/assembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/disassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/inlineassembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shell_libs/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.078899 ShellcodeTester-0.2.3/shellcodetester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/shellcodetester/shellcodetester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:46.078899 ShellcodeTester-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 14:30:39.000000 ShellcodeTester-0.2.3/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 23:52:10.000000 ShellcodeTester-0.2.4/ShellcodeTester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/nasmshell/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/nasmshell/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/libs/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/nasmshell/nasmshell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/macosx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/macosx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.066291 ShellcodeTester-0.2.4/shell_bins/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:52:04.000000 ShellcodeTester-0.2.4/shell_bins/windows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/shell_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/asmfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/assembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/disassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/inlineassembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shell_libs/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/shellcodetester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8324 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/shellcodetester/shellcodetester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:10.070291 ShellcodeTester-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-12 23:52:02.000000 ShellcodeTester-0.2.4/tests/tests.py
```

### Comparing `ShellcodeTester-0.2.3/LICENSE` & `ShellcodeTester-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/PKG-INFO` & `ShellcodeTester-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.3
+Version: 0.2.4
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
@@ -206,9 +206,9 @@
   -q, --quiet                     Quiet mode, not show banners. (default: false)
 ```
 
 # Windows Users
 
 Check specific instructions by Windows Users
 
-[Windows Instructions](WINDOWS.md)
+[Windows Instructions](https://github.com/helviojunior/shellcodetester/blob/master/WINDOWS.md)
```

### Comparing `ShellcodeTester-0.2.3/README.md` & `ShellcodeTester-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -171,8 +171,8 @@
   -q, --quiet                     Quiet mode, not show banners. (default: false)
 ```
 
 # Windows Users
 
 Check specific instructions by Windows Users
 
-[Windows Instructions](WINDOWS.md)
+[Windows Instructions](https://github.com/helviojunior/shellcodetester/blob/master/WINDOWS.md)
```

### Comparing `ShellcodeTester-0.2.3/ShellcodeTester.egg-info/PKG-INFO` & `ShellcodeTester-0.2.4/ShellcodeTester.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShellcodeTester
-Version: 0.2.3
+Version: 0.2.4
 Summary: ShellcodeTester is a tool to assembly, compile and test ASM shellcode.
 Home-page: https://github.com/helviojunior/shellcodetester
 Author: Helvio Junior (M4v3r1ck)
 Author-email: helvio.junior@sec4us.com.br
 License: GPL-3.0
 Project-URL: Main Author, https://sec4us.com.br/instrutores/helvio-junior/
 Project-URL: Documentation, https://github.com/helviojunior/shellcodetester
@@ -206,9 +206,9 @@
   -q, --quiet                     Quiet mode, not show banners. (default: false)
 ```
 
 # Windows Users
 
 Check specific instructions by Windows Users
 
-[Windows Instructions](WINDOWS.md)
+[Windows Instructions](https://github.com/helviojunior/shellcodetester/blob/master/WINDOWS.md)
```

### Comparing `ShellcodeTester-0.2.3/ShellcodeTester.egg-info/SOURCES.txt` & `ShellcodeTester-0.2.4/ShellcodeTester.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 ShellcodeTester.egg-info/PKG-INFO
 ShellcodeTester.egg-info/SOURCES.txt
 ShellcodeTester.egg-info/dependency_links.txt
 ShellcodeTester.egg-info/entry_points.txt
 ShellcodeTester.egg-info/not-zip-safe
 ShellcodeTester.egg-info/requires.txt
 ShellcodeTester.egg-info/top_level.txt
-bin/__init__.py
 nasmshell/__init__.py
 nasmshell/args.py
 nasmshell/config.py
 nasmshell/nasmshell.py
 nasmshell/libs/__init__.py
 nasmshell/libs/cmd.py
+shell_bins/__init__.py
+shell_bins/linux/__init__.py
+shell_bins/macosx/__init__.py
+shell_bins/windows/__init__.py
 shell_libs/__init__.py
 shell_libs/__meta__.py
 shell_libs/asmfile.py
 shell_libs/assembler.py
 shell_libs/color.py
 shell_libs/compiler.py
 shell_libs/disassembler.py
```

### Comparing `ShellcodeTester-0.2.3/nasmshell/args.py` & `ShellcodeTester-0.2.4/nasmshell/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/nasmshell/config.py` & `ShellcodeTester-0.2.4/nasmshell/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/nasmshell/libs/cmd.py` & `ShellcodeTester-0.2.4/nasmshell/libs/cmd.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/nasmshell/nasmshell.py` & `ShellcodeTester-0.2.4/nasmshell/nasmshell.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/setup.py` & `ShellcodeTester-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,33 +34,39 @@
         print("Unable to read requirements from the requirements.txt file"
               "That indicates this copy of the source code is incomplete.")
         sys.exit(2)
 
 with open(f"{here}/README.md", "r", encoding="utf-8") as f:
     readme = f.read()
 
-bin_files = []
-if os.path.isdir(f"{here}/bin"):
-    bin_files = [
-        os.path.join(dp, f).replace(here.strip('/') + '/', '').lstrip('/. ')
-        for dp, dn, filenames in os.walk(f"{here}/bin") for f in filenames
-    ]
+# Find package Data
+# each directory must contain __init__.py
+package_data = {"": ["LICENSE"]}
+package_data.update(
+    {
+        dp.replace(here.strip('/') + '/', '').lstrip('/. ').replace('\\', '/').replace('/', '.'): [
+            f for f in filenames if '.py' not in f.lower() and '.ds_store' not in f.lower()
+        ]
+        for dp, dn, filenames in os.walk(f"{here}/shell_bins") for f in filenames
+        if '.py' not in f.lower() and '.ds_store' not in f.lower()
+    }
+)
 
 setup(
     name=meta["__title__"],
     version=meta["__version__"],
     description=meta["__description__"],
     long_description=readme,
     long_description_content_type="text/markdown",
     author=meta["__author__"],
     author_email=meta["__author_email__"],
     url=meta["__url__"],
     packages=find_packages(),
-    package_data={"": ["LICENSE"]},
-    data_files=[('', ['requirements.txt'] + bin_files)],
+    package_data=package_data,
+    data_files=[('', ['requirements.txt'])],
     include_package_data=False,
     python_requires=">=3.7, <4",
     install_requires=requires,
     license=meta["__license__"],
     readme="README.md",
     zip_safe=False,
     classifiers=[
```

### Comparing `ShellcodeTester-0.2.3/shell_libs/asmfile.py` & `ShellcodeTester-0.2.4/shell_libs/asmfile.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shell_libs/assembler.py` & `ShellcodeTester-0.2.4/shell_libs/assembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shell_libs/color.py` & `ShellcodeTester-0.2.4/shell_libs/color.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shell_libs/compiler.py` & `ShellcodeTester-0.2.4/shell_libs/compiler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shell_libs/disassembler.py` & `ShellcodeTester-0.2.4/shell_libs/disassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shell_libs/inlineassembler.py` & `ShellcodeTester-0.2.4/shell_libs/inlineassembler.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shell_libs/logger.py` & `ShellcodeTester-0.2.4/shell_libs/logger.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shell_libs/process.py` & `ShellcodeTester-0.2.4/shell_libs/process.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,18 +68,21 @@
 
     @staticmethod
     def get_path():
         p = platform.system().lower()
         if p == 'darwin':
             p = 'macosx'
 
-        bin_path = Path(os.path.dirname(__file__) + f'../bin/{p}')
+        bin_path = os.path.join(Path(os.path.dirname(__file__)).resolve().parent, 'shell_bins', p)
         my_env = os.environ.copy()
-        return f"{bin_path}:" + my_env["PATH"]
-
+        if p == 'windows':
+            mingw64_path = os.path.join(Path(os.path.dirname(__file__)).resolve().parent, 'shell_bins', p, 'mingw64', 'bin')
+            return f"{bin_path};{mingw64_path};" + my_env["PATH"]
+        else:
+            return my_env["PATH"] + f":{bin_path}"
 
     @staticmethod
     def exists(program):
         ''' Checks if program is installed on this system '''
         #p = Process(['which', program])
         #stdout = p.stdout().strip()
         #stderr = p.stderr().strip()
```

### Comparing `ShellcodeTester-0.2.3/shell_libs/tools.py` & `ShellcodeTester-0.2.4/shell_libs/tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -133,7 +133,20 @@
                 j = 0
             i += 1
 
         if j == m:
             return i - m
         else:
             return -1
+
+    @staticmethod
+    def print_error(error: Exception):
+        Color.pl('\n{!} {R}Error:{O} %s{W}' % str(error))
+
+        Color.pl('\n{!} {O}Full stack trace below')
+        from traceback import format_exc
+        Color.p('\n{!}    ')
+        err = format_exc().strip()
+        err = err.replace('\n', '\n{W}{!} {W}   ')
+        err = err.replace('  File', '{W}{D}File')
+        err = err.replace('  Exception: ', '{R}Exception: {O}')
+        Color.pl(err + '{W}')
```

### Comparing `ShellcodeTester-0.2.3/shell_libs/transform.py` & `ShellcodeTester-0.2.4/shell_libs/transform.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shellcodetester/args.py` & `ShellcodeTester-0.2.4/shellcodetester/args.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shellcodetester/config.py` & `ShellcodeTester-0.2.4/shellcodetester/config.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shellcodetester/password.py` & `ShellcodeTester-0.2.4/shellcodetester/password.py`

 * *Files identical despite different names*

### Comparing `ShellcodeTester-0.2.3/shellcodetester/shellcodetester.py` & `ShellcodeTester-0.2.4/shellcodetester/shellcodetester.py`

 * *Files identical despite different names*

