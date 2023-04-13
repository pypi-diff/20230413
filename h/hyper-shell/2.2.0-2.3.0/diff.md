# Comparing `tmp/hyper-shell-2.2.0.tar.gz` & `tmp/hyper-shell-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper-shell-2.2.0.tar", last modified: Wed Mar 29 18:16:18 2023, max compression
+gzip compressed data, was "hyper-shell-2.3.0.tar", last modified: Thu Apr 13 15:55:39 2023, max compression
```

## Comparing `hyper-shell-2.2.0.tar` & `hyper-shell-2.3.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.204383 hyper-shell-2.2.0/
--rw-r--r--   0 geoffrey   (501) staff       (20)    11357 2020-12-21 02:22:57.000000 hyper-shell-2.2.0/LICENSE
--rw-r--r--   0 geoffrey   (501) staff       (20)     3740 2023-03-29 18:16:18.203852 hyper-shell-2.2.0/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)     2916 2022-08-05 01:42:32.000000 hyper-shell-2.2.0/README.rst
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.167604 hyper-shell-2.2.0/man/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.170828 hyper-shell-2.2.0/man/man1/
--rw-r--r--   0 geoffrey   (501) staff       (20)    50597 2023-03-29 18:13:34.000000 hyper-shell-2.2.0/man/man1/hyper-shell.1
--rw-r--r--   0 geoffrey   (501) staff       (20)      100 2022-01-10 02:23:40.000000 hyper-shell-2.2.0/pyproject.toml
--rw-r--r--   0 geoffrey   (501) staff       (20)       38 2023-03-29 18:16:18.204568 hyper-shell-2.2.0/setup.cfg
--rw-r--r--   0 geoffrey   (501) staff       (20)     2573 2023-03-21 20:31:18.000000 hyper-shell-2.2.0/setup.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.168090 hyper-shell-2.2.0/src/
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.172989 hyper-shell-2.2.0/src/hyper_shell.egg-info/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3740 2023-03-29 18:16:17.000000 hyper-shell-2.2.0/src/hyper_shell.egg-info/PKG-INFO
--rw-r--r--   0 geoffrey   (501) staff       (20)      975 2023-03-29 18:16:17.000000 hyper-shell-2.2.0/src/hyper_shell.egg-info/SOURCES.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)        1 2023-03-29 18:16:17.000000 hyper-shell-2.2.0/src/hyper_shell.egg-info/dependency_links.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       48 2023-03-29 18:16:17.000000 hyper-shell-2.2.0/src/hyper_shell.egg-info/entry_points.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)      132 2023-03-29 18:16:17.000000 hyper-shell-2.2.0/src/hyper_shell.egg-info/requires.txt
--rw-r--r--   0 geoffrey   (501) staff       (20)       11 2023-03-29 18:16:17.000000 hyper-shell-2.2.0/src/hyper_shell.egg-info/top_level.txt
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.176706 hyper-shell-2.2.0/src/hypershell/
--rw-r--r--   0 geoffrey   (501) staff       (20)     4541 2023-03-29 18:13:34.000000 hyper-shell-2.2.0/src/hypershell/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    33142 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/client.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    24675 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/cluster.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    11476 2022-11-15 22:14:14.000000 hyper-shell-2.2.0/src/hypershell/config.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.200729 hyper-shell-2.2.0/src/hypershell/core/
--rw-r--r--   0 geoffrey   (501) staff       (20)      132 2022-01-10 02:26:15.000000 hyper-shell-2.2.0/src/hypershell/core/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     5818 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/ansi.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     9053 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/config.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     3336 2022-06-27 20:48:08.000000 hyper-shell-2.2.0/src/hypershell/core/exceptions.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1833 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/fsm.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1892 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/heartbeat.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     4683 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/logging.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     2881 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/platform.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     4703 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/queue.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     6543 2022-11-15 22:14:14.000000 hyper-shell-2.2.0/src/hypershell/core/remote.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     7243 2022-01-10 02:26:15.000000 hyper-shell-2.2.0/src/hypershell/core/template.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     1537 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/core/thread.py
--rw-r--r--   0 geoffrey   (501) staff       (20)      793 2022-01-10 02:26:15.000000 hyper-shell-2.2.0/src/hypershell/core/types.py
-drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-03-29 18:16:18.203087 hyper-shell-2.2.0/src/hypershell/database/
--rw-r--r--   0 geoffrey   (501) staff       (20)     3850 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/database/__init__.py
--rw-r--r--   0 geoffrey   (501) staff       (20)     7679 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/database/core.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    13873 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/database/model.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    35160 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/server.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    21133 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/submit.py
--rw-r--r--   0 geoffrey   (501) staff       (20)    22966 2023-03-29 18:13:20.000000 hyper-shell-2.2.0/src/hypershell/task.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.763179 hyper-shell-2.3.0/
+-rw-r--r--   0 geoffrey   (501) staff       (20)    11357 2020-12-21 02:22:57.000000 hyper-shell-2.3.0/LICENSE
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-04-13 15:55:39.762696 hyper-shell-2.3.0/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2883 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/README.rst
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.740072 hyper-shell-2.3.0/man/
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.743531 hyper-shell-2.3.0/man/man1/
+-rw-r--r--   0 geoffrey   (501) staff       (20)    50674 2023-04-13 15:55:03.000000 hyper-shell-2.3.0/man/man1/hyper-shell.1
+-rw-r--r--   0 geoffrey   (501) staff       (20)      100 2022-01-10 02:23:40.000000 hyper-shell-2.3.0/pyproject.toml
+-rw-r--r--   0 geoffrey   (501) staff       (20)       38 2023-04-13 15:55:39.763324 hyper-shell-2.3.0/setup.cfg
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2652 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/setup.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.740878 hyper-shell-2.3.0/src/
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.746119 hyper-shell-2.3.0/src/hyper_shell.egg-info/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3771 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/PKG-INFO
+-rw-r--r--   0 geoffrey   (501) staff       (20)      975 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)        1 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       48 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/entry_points.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)      132 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/requires.txt
+-rw-r--r--   0 geoffrey   (501) staff       (20)       11 2023-04-13 15:55:39.000000 hyper-shell-2.3.0/src/hyper_shell.egg-info/top_level.txt
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.749046 hyper-shell-2.3.0/src/hypershell/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     3577 2023-04-13 15:55:03.000000 hyper-shell-2.3.0/src/hypershell/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    34622 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/client.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    25277 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/cluster.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    11691 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/config.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.759991 hyper-shell-2.3.0/src/hypershell/core/
+-rw-r--r--   0 geoffrey   (501) staff       (20)      132 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     5835 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/ansi.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     9053 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/config.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     4771 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/exceptions.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1833 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/fsm.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1892 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/heartbeat.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     6009 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/logging.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     2869 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/platform.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     5347 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/queue.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     6733 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/remote.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     7244 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/template.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     1597 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/core/thread.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)      793 2023-04-02 14:55:21.000000 hyper-shell-2.3.0/src/hypershell/core/types.py
+drwxr-xr-x   0 geoffrey   (501) staff       (20)        0 2023-04-13 15:55:39.761845 hyper-shell-2.3.0/src/hypershell/database/
+-rw-r--r--   0 geoffrey   (501) staff       (20)     4615 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/database/__init__.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)     7873 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/database/core.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    14166 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/database/model.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    36057 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/server.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    21890 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/submit.py
+-rw-r--r--   0 geoffrey   (501) staff       (20)    25736 2023-04-13 15:30:41.000000 hyper-shell-2.3.0/src/hypershell/task.py
```

### Comparing `hyper-shell-2.2.0/LICENSE` & `hyper-shell-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.2.0/PKG-INFO` & `hyper-shell-2.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hyper-shell
-Version: 2.2.0
+Version: 2.3.0
 Summary: Process shell commands over a distributed, asynchronous queue.
 Home-page: https://github.com/glentner/hyper-shell
 Author: Geoffrey Lentner
 Author-email: glentner@purdue.edu
 License: Apache Software License
 Keywords: distributed-computing command-line-tool shell-scripting high-performance-computing
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 Provides-Extra: postgres
 License-File: LICENSE
@@ -51,15 +52,15 @@
 Several tools offer similar functionality but not all together in a single tool with
 the ergonomics we provide. Novel design elements include but are not limited to
 (1) cross-platform, (2) client-server design, (3) staggered launch for large scales,
 (4) persistent hosting of the server, and optionally (5) a database in-the-loop for
 persisting task metadata and automated retries.
 
 *HyperShell* is pure Python and is tested on Linux, macOS, and Windows 10 in
-Python 3.9 and 3.10 environments. The server and client don't even need to use the same
+Python 3.9+ environments. The server and client don't even need to use the same
 platform simultaneously.
 
 
 Documentation
 -------------
 
 Documentation is available at `hyper-shell.readthedocs.io <https://hyper-shell.readthedocs.io>`_.
@@ -67,17 +68,17 @@
 comprehensive usage guide on the command line you can view the manual page with 
 ``man hyper-shell``.
 
 
 Contributions
 -------------
 
-Contributions are welcome. If you find bugs or have questions, open an *Issue* here. If and
-when the project grows, a code of conduct will be provided along side a more comprehensive set of
-guidelines for contributing; until then, just be kind.
+Contributions are welcome. If you find bugs or have questions, open an *Issue* here.
+We've added a Code of Conduct recently, adapted from the
+`Contributor Covenant <https://www.contributor-covenant.org/>`_, version 2.0.
 
 
 Citation
 --------
 
 If *HyperShell* has helped in your research please consider citing us.
```

### Comparing `hyper-shell-2.2.0/README.rst` & `hyper-shell-2.3.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Several tools offer similar functionality but not all together in a single tool with
 the ergonomics we provide. Novel design elements include but are not limited to
 (1) cross-platform, (2) client-server design, (3) staggered launch for large scales,
 (4) persistent hosting of the server, and optionally (5) a database in-the-loop for
 persisting task metadata and automated retries.
 
 *HyperShell* is pure Python and is tested on Linux, macOS, and Windows 10 in
-Python 3.9 and 3.10 environments. The server and client don't even need to use the same
+Python 3.9+ environments. The server and client don't even need to use the same
 platform simultaneously.
 
 
 Documentation
 -------------
 
 Documentation is available at `hyper-shell.readthedocs.io <https://hyper-shell.readthedocs.io>`_.
@@ -46,17 +46,17 @@
 comprehensive usage guide on the command line you can view the manual page with 
 ``man hyper-shell``.
 
 
 Contributions
 -------------
 
-Contributions are welcome. If you find bugs or have questions, open an *Issue* here. If and
-when the project grows, a code of conduct will be provided along side a more comprehensive set of
-guidelines for contributing; until then, just be kind.
+Contributions are welcome. If you find bugs or have questions, open an *Issue* here.
+We've added a Code of Conduct recently, adapted from the
+`Contributor Covenant <https://www.contributor-covenant.org/>`_, version 2.0.
 
 
 Citation
 --------
 
 If *HyperShell* has helped in your research please consider citing us.
```

### Comparing `hyper-shell-2.2.0/man/man1/hyper-shell.1` & `hyper-shell-2.3.0/man/man1/hyper-shell.1`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "HYPER-SHELL" "1" "Mar 29, 2023" "2.2.0" "hyper-shell"
+.TH "HYPER-SHELL" "1" "Apr 13, 2023" "2.3.0" "hyper-shell"
 .SH NAME
 hyper-shell \- Process shell commands over a distributed, asynchronous queue
 .SH SYNOPSIS
 .nf
 hyper\-shell [\-h] [\-v] ...
 .fi
 .sp
@@ -52,15 +52,15 @@
 .fi
 .sp
 .nf
 hyper\-shell config [\-h] {get | set | which | edit } [\-\-user | \-\-system] ...
 .fi
 .sp
 .nf
-hyper\-shell task [\-h] {submit | info | wait | run | search} ...
+hyper\-shell task [\-h] {submit | info | wait | run | search | update} ...
 .fi
 .sp
 .SH DESCRIPTION
 .sp
 \fBhyper\-shell\fP is an elegant, cross\-platform, high\-performance computing utility for processing
 shell commands over a distributed, asynchronous queue. It is a highly scalable workflow automation
 tool for many\-task scenarios.
@@ -723,15 +723,15 @@
 The full command\-line for some shell task.
 To use options, preface with leading \fB\-\-\fP\&.
 .UNINDENT
 .SH TASK INFO USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBtask\fP \fBinfo\fP \fB[\-h]\fP
-\fBID\fP \fB[\-\-json | \-\-stdout | \-\-stderr | \-\-x FIELD]\fP
+\fBID\fP \fB[\-\-yaml | \-\-json | \-\-stdout | \-\-stderr | \-\-x FIELD]\fP
 .UNINDENT
 .sp
 Get metadata and/or task outputs.
 .sp
 Query for the full metadata on task by ID.
 Extract a specific field using \fB\-x\fP/\fB\-\-extract\fP\&.
 .sp
@@ -743,14 +743,17 @@
 .TP
 .B ID
 Unique task UUID.
 .UNINDENT
 .SS Options
 .INDENT 0.0
 .TP
+.B \fB\-\-yaml\fP
+Format metadata output as YAML.
+.TP
 .B \fB\-\-json\fP
 Format metadata output as JSON.
 .TP
 .B \fB\-x\fP/\fB\-\-extract\fP \fIFIELD\fP
 Print this field only (e.g., \fB\-x submit_time\fP).
 .TP
 .B \fB\-\-stdout\fP
@@ -822,16 +825,16 @@
 Time in seconds to wait between polling (default: 5).
 .UNINDENT
 .SH TASK SEARCH USAGE
 .INDENT 0.0
 .TP
 .B \fBhyper\-shell\fP \fBtask\fP \fBsearch\fP \fB[\-h]\fP
 \fB[FIELD [FIELD ...]]\fP \fB[\-\-where COND [COND ...]]\fP
-\fB[\-\-order\-by FIELD [\-\-desc]]\fP \fB[\-x | \-\-json | \-\-csv]\fP
-\fB[\-\-count | \-\-limit NUM]\fP
+\fB[\-\-order\-by FIELD [\-\-desc]]\fP \fB[\-\-count | \-\-limit NUM]\fP
+\fB[\-\-format FORMAT | \-\-json | \-\-csv]\fP \fB[\-d CHAR]\fP
 .UNINDENT
 .sp
 Search for tasks in database.
 .sp
 A database must be configured.
 Fields will be columns in the output.
 Options relate to SQL concepts.
@@ -849,17 +852,14 @@
 .TP
 .B \fB\-w\fP, \fB\-\-where\fP \fICOND...\fP
 List of conditional statements to filter results (e.g., \fB\-w \(aqexit_status != 0\(aq\fP).
 .TP
 .B \fB\-s\fP, \fB\-\-order\-by\fP \fIFIELD\fP
 Order results by field.
 .TP
-.B \fB\-x\fP, \fB\-\-extract\fP
-Disable formatting for single column output.
-.TP
 .B \fB\-\-failed\fP
 Alias for \fB\-w \(aqexit_status != 0\(aq\fP\&.
 .TP
 .B \fB\-\-succeeded\fP
 Alias for \fB\-w \(aqexit_status == 0\(aq\fP\&.
 .TP
 .B \fB\-\-finished\fP
@@ -870,19 +870,22 @@
 .TP
 .B \fB\-\-json\fP
 Format output as JSON.
 .TP
 .B \fB\-\-csv\fP
 Format output as CSV.
 .TP
+.B \fB\-d\fP, \fB\-\-delimiter\fP \fICHAR\fP
+Field seperator for plain/csv formats.
+.TP
 .B \fB\-l\fP, \fB\-\-limit\fP \fINUM\fP
-Limit number of returned results.
+Limit the number of results.
 .TP
 .B \fB\-c\fP, \fB\-\-count\fP
-Only print number of results that would be returned.
+Show count of results.
 .UNINDENT
 .SH TASK UPDATE USAGE
 .sp
 \fBhyper\-shell\fP \fBtask\fP \fBupdate\fP \fB[\-h]\fP \fBID\fP \fBFIELD\fP \fBVALUE\fP
 .sp
 Update individual task metadata.
 .sp
```

### Comparing `hyper-shell-2.2.0/setup.py` & `hyper-shell-2.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Build and installation script for hyper-shell."""
 
 
 # standard libs
 import os
@@ -20,15 +20,15 @@
     content = source.read().strip()
     metadata = {key: re.search(key + r'\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
                 for key in ['__version__', '__authors__', '__contact__',
                             '__description__', '__license__', '__keywords__', '__website__']}
 
 
 # Core dependencies
-DEPS = ['cmdkit>=2.6.0', 'toml>=0.10.2', 'tomlkit>=0.11.0', 'pyyaml>=6.0',
+DEPS = ['cmdkit==2.6.1', 'toml>=0.10.2', 'tomlkit>=0.11.0', 'pyyaml>=6.0',
         'sqlalchemy>=1.4.22', 'rich>=10.16.2', 'paramiko>=2.9.1']
 
 # Dependencies for readthedocs.io
 if os.environ.get('READTHEDOCS') == 'True':
     DEPS.extend([
         'sphinx>=4.1.2',
         'sphinx-sitemap',
@@ -51,18 +51,19 @@
     keywords         = metadata['__keywords__'],
     url              = metadata['__website__'],
     packages         = find_packages('src'),
     package_dir      = {'': 'src', },
     include_package_data = True,
     long_description = long_description,
     long_description_content_type = 'text/x-rst',
-    classifiers      = ['Development Status :: 4 - Beta',
+    classifiers      = ['Development Status :: 5 - Production/Stable',
                         'Topic :: Utilities',
                         'Programming Language :: Python :: 3.9',
                         'Programming Language :: Python :: 3.10',
+                        'Programming Language :: Python :: 3.11',
                         'Operating System :: POSIX :: Linux',
                         'Operating System :: MacOS',
                         'Operating System :: Microsoft :: Windows',
                         'License :: OSI Approved :: Apache Software License', ],
     install_requires = DEPS,
     extras_require = {
         'postgres': ['psycopg2>=2.9.1', ],
```

### Comparing `hyper-shell-2.2.0/src/hyper_shell.egg-info/PKG-INFO` & `hyper-shell-2.3.0/src/hyper_shell.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hyper-shell
-Version: 2.2.0
+Version: 2.3.0
 Summary: Process shell commands over a distributed, asynchronous queue.
 Home-page: https://github.com/glentner/hyper-shell
 Author: Geoffrey Lentner
 Author-email: glentner@purdue.edu
 License: Apache Software License
 Keywords: distributed-computing command-line-tool shell-scripting high-performance-computing
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
 Provides-Extra: postgres
 License-File: LICENSE
@@ -51,15 +52,15 @@
 Several tools offer similar functionality but not all together in a single tool with
 the ergonomics we provide. Novel design elements include but are not limited to
 (1) cross-platform, (2) client-server design, (3) staggered launch for large scales,
 (4) persistent hosting of the server, and optionally (5) a database in-the-loop for
 persisting task metadata and automated retries.
 
 *HyperShell* is pure Python and is tested on Linux, macOS, and Windows 10 in
-Python 3.9 and 3.10 environments. The server and client don't even need to use the same
+Python 3.9+ environments. The server and client don't even need to use the same
 platform simultaneously.
 
 
 Documentation
 -------------
 
 Documentation is available at `hyper-shell.readthedocs.io <https://hyper-shell.readthedocs.io>`_.
@@ -67,17 +68,17 @@
 comprehensive usage guide on the command line you can view the manual page with 
 ``man hyper-shell``.
 
 
 Contributions
 -------------
 
-Contributions are welcome. If you find bugs or have questions, open an *Issue* here. If and
-when the project grows, a code of conduct will be provided along side a more comprehensive set of
-guidelines for contributing; until then, just be kind.
+Contributions are welcome. If you find bugs or have questions, open an *Issue* here.
+We've added a Code of Conduct recently, adapted from the
+`Contributor Covenant <https://www.contributor-covenant.org/>`_, version 2.0.
 
 
 Citation
 --------
 
 If *HyperShell* has helped in your research please consider citing us.
```

### Comparing `hyper-shell-2.2.0/src/hyper_shell.egg-info/SOURCES.txt` & `hyper-shell-2.3.0/src/hyper_shell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyper-shell-2.2.0/src/hypershell/__init__.py` & `hyper-shell-2.3.0/src/hypershell/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Initialization and entry-point for console application."""
 
 
 # standard libs
 import sys
-import functools
 
 # external libs
-from cmdkit.app import Application, ApplicationGroup, exit_status
+from cmdkit.app import Application, ApplicationGroup
 from cmdkit.cli import Interface
-from cmdkit.config import ConfigurationError
-from sqlalchemy.exc import OperationalError
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
-from hypershell.core.exceptions import write_traceback, handle_exception
 from hypershell.core.logging import Logger, initialize_logging
 from hypershell.submit import SubmitApp
 from hypershell.server import ServerApp
 from hypershell.client import ClientApp
 from hypershell.cluster import ClusterApp
 from hypershell.task import TaskGroupApp
 from hypershell.config import ConfigApp
-from hypershell.database import InitDBApp, DatabaseUninitialized
-from hypershell.database.model import Task
+from hypershell.database import InitDBApp
 
 # public interface
 __all__ = ['HyperShellApp', 'main', '__version__', '__license__']
 
 # project metadata
-__version__     = '2.2.0'
+__version__     = '2.3.0'
 __authors__     = 'Geoffrey Lentner'
 __contact__     = 'glentner@purdue.edu'
 __license__     = 'Apache Software License'
-__copyright__   = '2019-2022. All Rights Reserved.'
+__copyright__   = '2019-2023. All Rights Reserved.'
 __website__     = 'https://github.com/glentner/hyper-shell'
 __keywords__    = 'distributed-computing command-line-tool shell-scripting high-performance-computing'
 __description__ = 'Process shell commands over a distributed, asynchronous queue.'
 __citation__    = """\
 @inproceedings{lentner_2022,
     author = {Lentner, Geoffrey and Gorenstein, Lev},
     title = {HyperShell v2: Distributed Task Execution for HPC},
@@ -93,25 +88,14 @@
 {__website__}
 
 If this software has helped in your research please consider
 citing us (see --citation).\
 """
 
 
-# Globally defined exception cases for all applications
-Application.exceptions = {
-    RuntimeError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-    ConfigurationError: functools.partial(handle_exception, logger=log, status=exit_status.bad_config),
-    DatabaseUninitialized: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-    OperationalError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-    Task.NotFound: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-    Exception: functools.partial(write_traceback, logger=log, status=exit_status.runtime_error),
-}
-
-
 class HyperShellApp(ApplicationGroup):
     """Top-level application class for console application."""
 
     interface = Interface(APP_NAME,
                           colorize_usage(APP_USAGE),
                           colorize_usage(APP_HELP))
```

### Comparing `hyper-shell-2.2.0/src/hypershell/client.py` & `hyper-shell-2.3.0/src/hypershell/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Connect to server and run tasks.
 
 Example:
     >>> from hypershell.client import run_client
@@ -27,14 +27,15 @@
     the thread will be stopped regardless because it runs as a `daemon`.
 """
 
 
 # type annotations
 from __future__ import annotations
 from typing import List, Tuple, Optional, Callable, Dict, IO, Type
+from types import TracebackType
 
 # standard libs
 import os
 import sys
 import time
 import json
 import random
@@ -60,15 +61,15 @@
 from hypershell.core.config import default, config, load_task_env
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.thread import Thread
 from hypershell.core.queue import QueueClient, QueueConfig
 from hypershell.core.logging import HOSTNAME, INSTANCE, Logger
 from hypershell.core.template import Template, DEFAULT_TEMPLATE
 from hypershell.core.exceptions import (handle_exception, handle_disconnect,
-                                        handle_address_unknown, HostAddressInfo)
+                                        handle_address_unknown, HostAddressInfo, get_shared_exception_mapping)
 
 # public interface
 __all__ = ['run_client', 'ClientThread', 'ClientApp', 'ClientInfo', 'DEFAULT_NUM_TASKS', 'DEFAULT_DELAY', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
@@ -134,25 +135,25 @@
 
     task: Task
     tasks: List[Task]
 
     state = SchedulerState.START
     states = SchedulerState
 
-    def __init__(self, queue: QueueClient, local: Queue[Optional[Task]], no_confirm: bool = False) -> None:
+    def __init__(self: ClientScheduler, queue: QueueClient, local: Queue[Optional[Task]], no_confirm: bool = False) -> None:
         """Assign remote queue client and local task queue."""
         self.queue = queue
         self.local = local
         self.bundle = []
         self.tasks = []
         self.client_info = None
         self.no_confirm = no_confirm
 
     @functools.cached_property
-    def actions(self) -> Dict[SchedulerState, Callable[[], SchedulerState]]:
+    def actions(self: ClientScheduler) -> Dict[SchedulerState, Callable[[], SchedulerState]]:
         return {
             SchedulerState.START: self.start,
             SchedulerState.GET_REMOTE: self.get_remote,
             SchedulerState.UNPACK: self.unpack_bundle,
             SchedulerState.PUT_CONFIRM: self.put_confirm,
             SchedulerState.POP_TASK: self.pop_task,
             SchedulerState.PUT_LOCAL: self.put_local,
@@ -161,55 +162,55 @@
 
     @staticmethod
     def start() -> SchedulerState:
         """Jump to GET_REMOTE state."""
         log.debug('Started (scheduler)')
         return SchedulerState.GET_REMOTE
 
-    def get_remote(self) -> SchedulerState:
+    def get_remote(self: ClientScheduler) -> SchedulerState:
         """Get the next task bundle from the server."""
         try:
             self.bundle = self.queue.scheduled.get(timeout=2)
             self.queue.scheduled.task_done()
             if self.bundle is not None:
                 log.debug(f'Received {len(self.bundle)} tasks ({HOSTNAME}: {INSTANCE})')
                 return SchedulerState.UNPACK
             else:
                 log.debug('Disconnect received')
                 return SchedulerState.FINAL
         except QueueEmpty:
             return SchedulerState.GET_REMOTE
 
-    def unpack_bundle(self) -> SchedulerState:
+    def unpack_bundle(self: ClientScheduler) -> SchedulerState:
         """Unpack latest bundle of tasks."""
         self.tasks = [Task.unpack(data) for data in self.bundle]
         if not self.no_confirm:
             self.client_info = ClientInfo.from_tasks(self.tasks).pack()
             return SchedulerState.PUT_CONFIRM
         else:
             return SchedulerState.POP_TASK
 
-    def put_confirm(self) -> SchedulerState:
+    def put_confirm(self: ClientScheduler) -> SchedulerState:
         """Put confirmation details back on remote queue."""
         try:
             self.queue.confirmed.put(self.client_info, timeout=2)
             log.debug(f'Confirmed {len(self.tasks)} tasks ({HOSTNAME}: {INSTANCE})')
             return SchedulerState.POP_TASK
         except QueueFull:
             return SchedulerState.PUT_CONFIRM
 
-    def pop_task(self) -> SchedulerState:
+    def pop_task(self: ClientScheduler) -> SchedulerState:
         """Pop next task off current task list."""
         try:
             self.task = self.tasks.pop(0)
             return SchedulerState.PUT_LOCAL
         except IndexError:
             return SchedulerState.GET_REMOTE
 
-    def put_local(self) -> SchedulerState:
+    def put_local(self: ClientScheduler) -> SchedulerState:
         """Put latest task on the local task queue."""
         try:
             self.local.put(self.task, timeout=2)
             return SchedulerState.POP_TASK
         except QueueFull:
             return SchedulerState.PUT_LOCAL
 
@@ -219,24 +220,24 @@
         log.debug('Done (scheduler)')
         return SchedulerState.HALT
 
 
 class ClientSchedulerThread(Thread):
     """Run client scheduler in dedicated thread."""
 
-    def __init__(self, queue: QueueClient, local: Queue[Optional[bytes]], no_confirm: bool = False) -> None:
+    def __init__(self: ClientSchedulerThread, queue: QueueClient, local: Queue[Optional[bytes]], no_confirm: bool = False) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-client-scheduler')
         self.machine = ClientScheduler(queue=queue, local=local, no_confirm=no_confirm)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: ClientSchedulerThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: ClientSchedulerThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (scheduler)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 DEFAULT_BUNDLESIZE: int = default.client.bundlesize
@@ -266,105 +267,105 @@
     bundlesize: int
     bundlewait: int
     previous_send: datetime
 
     state = CollectorState.START
     states = CollectorState
 
-    def __init__(self, queue: QueueClient, local: Queue[Optional[Task]],
+    def __init__(self: ClientCollector, queue: QueueClient, local: Queue[Optional[Task]],
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
         """Collect tasks from local queue of finished tasks and push them to the server."""
         self.tasks = []
         self.bundle = []
         self.local = local
         self.queue = queue
         self.bundlesize = bundlesize
         self.bundlewait = bundlewait
 
     @functools.cached_property
-    def actions(self) -> Dict[CollectorState, Callable[[], CollectorState]]:
+    def actions(self: ClientCollector) -> Dict[CollectorState, Callable[[], CollectorState]]:
         return {
             CollectorState.START: self.start,
             CollectorState.GET_LOCAL: self.get_local,
             CollectorState.CHECK_BUNDLE: self.check_bundle,
             CollectorState.PACK_BUNDLE: self.pack_bundle,
             CollectorState.PUT_REMOTE: self.put_remote,
             CollectorState.FINAL: self.finalize,
         }
 
-    def start(self) -> CollectorState:
+    def start(self: ClientCollector) -> CollectorState:
         """Jump to GET_LOCAL state."""
         log.debug('Started (collector)')
         self.previous_send = datetime.now()
         return CollectorState.GET_LOCAL
 
-    def get_local(self) -> CollectorState:
+    def get_local(self: ClientCollector) -> CollectorState:
         """Get the next task from the local completed task queue."""
         try:
             task = self.local.get(timeout=1)
             self.local.task_done()
             if task:
                 self.tasks.append(task)
                 return CollectorState.CHECK_BUNDLE
             else:
                 return CollectorState.FINAL
         except QueueEmpty:
             return CollectorState.CHECK_BUNDLE
 
-    def check_bundle(self) -> CollectorState:
+    def check_bundle(self: ClientCollector) -> CollectorState:
         """Check state of task bundle and proceed with return if necessary."""
         wait_time = (datetime.now() - self.previous_send)
         since_last = wait_time.total_seconds()
         if len(self.tasks) >= self.bundlesize:
-            log.trace(f'Bundle size ({len(self.tasks)}) reached')
+            log.trace(f'Bundle size reached ({len(self.tasks)} tasks)')
             return CollectorState.PACK_BUNDLE
         elif since_last >= self.bundlewait:
             log.trace(f'Wait time exceeded ({wait_time})')
             return CollectorState.PACK_BUNDLE
         else:
             return CollectorState.GET_LOCAL
 
-    def pack_bundle(self) -> CollectorState:
+    def pack_bundle(self: ClientCollector) -> CollectorState:
         """Pack tasks into bundle before pushing back to server."""
         self.bundle = [task.pack() for task in self.tasks]
         return CollectorState.PUT_REMOTE
 
-    def put_remote(self) -> CollectorState:
+    def put_remote(self: ClientCollector) -> CollectorState:
         """Push out bundle of completed tasks."""
         if self.bundle:
             self.queue.completed.put(self.bundle)
-            log.trace(f'Returned bundle of {len(self.bundle)} tasks')
+            log.trace(f'Returned bundle ({len(self.bundle)} tasks)')
             self.tasks.clear()
             self.bundle.clear()
             self.previous_send = datetime.now()
         else:
             log.trace('No local tasks to return')
         return CollectorState.GET_LOCAL
 
-    def finalize(self) -> CollectorState:
+    def finalize(self: ClientCollector) -> CollectorState:
         """Push out any remaining tasks and halt."""
         self.put_remote()
         log.debug('Done (collector)')
         return CollectorState.HALT
 
 
 class ClientCollectorThread(Thread):
     """Run client collector within dedicated thread."""
 
-    def __init__(self, queue: QueueClient, local: Queue[Optional[bytes]],
+    def __init__(self: ClientCollectorThread, queue: QueueClient, local: Queue[Optional[bytes]],
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-client-collector')
         self.machine = ClientCollector(queue=queue, local=local, bundlesize=bundlesize, bundlewait=bundlewait)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: ClientCollectorThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: ClientCollectorThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (collector)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 def task_env(task: Task) -> Dict[str, str]:
@@ -404,131 +405,135 @@
 
     inbound: Queue[Optional[Task]]
     outbound: Queue[Optional[Task]]
 
     state = TaskState.START
     states = TaskState
 
-    def __init__(self, id: int, inbound: Queue[Optional[Task]], outbound: Queue[Optional[Task]],
+    def __init__(self: TaskExecutor, id: int, inbound: Queue[Optional[Task]], outbound: Queue[Optional[Task]],
                  template: str = DEFAULT_TEMPLATE, redirect_output: IO = None, redirect_errors: IO = None,
                  capture: bool = False) -> None:
         """Initialize task executor."""
         self.id = id
         self.template = Template(template)
         self.inbound = inbound
         self.outbound = outbound
         self.redirect_output = redirect_output or sys.stdout
         self.redirect_errors = redirect_errors or sys.stderr
         self.capture = capture
 
     @functools.cached_property
-    def actions(self) -> Dict[TaskState, Callable[[], TaskState]]:
+    def actions(self: TaskExecutor) -> Dict[TaskState, Callable[[], TaskState]]:
         return {
             TaskState.START: self.start,
             TaskState.GET_LOCAL: self.get_local,
             TaskState.CREATE_TASK: self.create_task,
             TaskState.START_TASK: self.start_task,
             TaskState.WAIT_TASK: self.wait_task,
             TaskState.PUT_LOCAL: self.put_local,
             TaskState.FINAL: self.finalize,
         }
 
-    def start(self) -> TaskState:
+    def start(self: TaskExecutor) -> TaskState:
         """Jump to GET_LOCAL state."""
         log.debug(f'Started (executor-{self.id})')
         return TaskState.GET_LOCAL
 
-    def get_local(self) -> TaskState:
+    def get_local(self: TaskExecutor) -> TaskState:
         """Get the next task from the local queue of new tasks."""
         try:
             self.task = self.inbound.get(timeout=1)
             self.inbound.task_done()
             return TaskState.CREATE_TASK if self.task else TaskState.FINAL
         except QueueEmpty:
             return TaskState.GET_LOCAL
 
-    def create_task(self) -> TaskState:
+    def create_task(self: TaskExecutor) -> TaskState:
         """Expand template and initialize task command-line."""
         try:
             self.task.client_id = INSTANCE
             self.task.client_host = HOSTNAME
             self.task.command = self.template.expand(self.task.args)
             return TaskState.START_TASK
         except Exception as error:
             log.error(f'{error.__class__.__name__}: {error}')
             self.task.start_time = datetime.now().astimezone()
             self.task.completion_time = datetime.now().astimezone()
             self.task.exit_status = -1
             return TaskState.PUT_LOCAL
 
-    def start_task(self) -> TaskState:
+    def start_task(self: TaskExecutor) -> TaskState:
         """Start current task locally."""
         env = task_env(self.task)
-        log.info(f'Running task ({self.task.id})')
-        log.debug(f'Running task ({self.task.id}: {self.task.command})')
         if self.capture:
             self.task.outpath = env['TASK_OUTPATH']
             self.task.errpath = env['TASK_ERRPATH']
             self.redirect_output = open(self.task.outpath, mode='w')
             self.redirect_errors = open(self.task.errpath, mode='w')
         self.task.start_time = datetime.now().astimezone()
         self.process = Popen(self.task.command, shell=True,
                              stdout=self.redirect_output, stderr=self.redirect_errors,
                              cwd=config.task.cwd, env=env)
+        log.info(f'Running task ({self.task.id})')
+        log.debug(f'Running task ({self.task.id}: {self.task.command})')
+        log.trace(f'Running task ({self.task.id}: pid={self.process.pid}, argv={self.task.command})')
         return TaskState.WAIT_TASK
 
-    def wait_task(self) -> TaskState:
+    def wait_task(self: TaskExecutor) -> TaskState:
         """Wait for current task to complete."""
         try:
             self.task.exit_status = self.process.wait(timeout=2)
             self.task.completion_time = datetime.now().astimezone()
             log.debug(f'Completed task ({self.task.id})')
             if self.capture:
                 self.redirect_output.close()
                 self.redirect_errors.close()
             return TaskState.PUT_LOCAL
         except TimeoutExpired:
+            # Only include time elapsed to the nearest second (we don't need fractions)
+            elapsed = timedelta(seconds=round((datetime.now().astimezone() - self.task.start_time).total_seconds()))
+            log.trace(f'Waiting on task ({self.task.id}: {elapsed})')
             return TaskState.WAIT_TASK
 
-    def put_local(self) -> TaskState:
+    def put_local(self: TaskExecutor) -> TaskState:
         """Put completed task on outbound queue."""
         try:
             self.outbound.put(self.task, timeout=1)
             return TaskState.GET_LOCAL
         except QueueFull:
             return TaskState.PUT_LOCAL
 
-    def finalize(self) -> TaskState:
+    def finalize(self: TaskExecutor) -> TaskState:
         """Push out any remaining tasks and halt."""
         log.debug(f'Done (executor-{self.id})')
         return TaskState.HALT
 
 
 class TaskThread(Thread):
     """Run task executor within dedicated thread."""
 
     id: int
 
-    def __init__(self,
+    def __init__(self: TaskThread,
                  id: int,
                  inbound: Queue[Optional[str]], outbound: Queue[Optional[str]],
                  template: str = DEFAULT_TEMPLATE, capture: bool = False,
                  redirect_output: IO = None, redirect_errors: IO = None) -> None:
         """Initialize task executor."""
         self.id = id
         super().__init__(name=f'hypershell-executor-{id}')
         self.machine = TaskExecutor(id=id, inbound=inbound, outbound=outbound, template=template,
                                     redirect_output=redirect_output, redirect_errors=redirect_errors,
                                     capture=capture)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: TaskThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: TaskThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning(f'Stopping (executor-{self.id})')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class HeartbeatState(State, Enum):
@@ -552,51 +557,51 @@
 
     no_wait: bool = False
     client_state: ClientState = ClientState.RUNNING
 
     state = HeartbeatState.START
     states = HeartbeatState
 
-    def __init__(self, queue: QueueClient, heartrate: int = DEFAULT_HEARTRATE) -> None:
+    def __init__(self: ClientHeartbeat, queue: QueueClient, heartrate: int = DEFAULT_HEARTRATE) -> None:
         """Initialize heartbeat machine."""
         self.queue = queue
         self.previous = datetime.now()
         self.heartrate = timedelta(seconds=heartrate)
 
     @functools.cached_property
-    def actions(self) -> Dict[HeartbeatState, Callable[[], HeartbeatState]]:
+    def actions(self: ClientHeartbeat) -> Dict[HeartbeatState, Callable[[], HeartbeatState]]:
         return {
             HeartbeatState.START: self.start,
             HeartbeatState.SUBMIT: self.submit,
             HeartbeatState.WAIT: self.wait,
             HeartbeatState.FINAL: self.finalize,
         }
 
     @staticmethod
     def start() -> HeartbeatState:
         """Jump to SUBMIT state."""
         log.debug(f'Started (heartbeat)')
         return HeartbeatState.SUBMIT
 
-    def submit(self) -> HeartbeatState:
+    def submit(self: ClientHeartbeat) -> HeartbeatState:
         """Publish new heartbeat to remote queue."""
         try:
             client_state = self.client_state  # atomic
             heartbeat = Heartbeat.new(state=client_state)
             self.queue.heartbeat.put(heartbeat.pack(), timeout=2)
             if client_state is ClientState.RUNNING:
                 log.trace(f'Heartbeat - running ({heartbeat.host}: {heartbeat.uuid})')
                 return HeartbeatState.WAIT
             else:
                 log.trace(f'Heartbeat - final ({heartbeat.host}: {heartbeat.uuid})')
                 return HeartbeatState.FINAL
         except QueueEmpty:
             return HeartbeatState.SUBMIT
 
-    def wait(self) -> HeartbeatState:
+    def wait(self: ClientHeartbeat) -> HeartbeatState:
         """Wait until next needed heartbeat."""
         if self.no_wait:
             return HeartbeatState.SUBMIT
         now = datetime.now()
         if (now - self.previous) < self.heartrate:
             time.sleep(1)
             return HeartbeatState.WAIT
@@ -610,29 +615,29 @@
         log.debug(f'Done (heartbeat)')
         return HeartbeatState.HALT
 
 
 class ClientHeartbeatThread(Thread):
     """Run heartbeat machine within dedicated thread."""
 
-    def __init__(self, queue: QueueClient, heartrate: int = DEFAULT_HEARTRATE) -> None:
+    def __init__(self: ClientHeartbeatThread, queue: QueueClient, heartrate: int = DEFAULT_HEARTRATE) -> None:
         """Initialize heartbeat machine."""
         super().__init__(name=f'hypershell-heartbeat')
         self.machine = ClientHeartbeat(queue=queue, heartrate=heartrate)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: ClientHeartbeatThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def signal_finished(self) -> None:
+    def signal_finished(self: ClientHeartbeatThread) -> None:
         """Set client state to communicate completion."""
         self.machine.client_state = ClientState.FINISHED
         self.machine.no_wait = True
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: ClientHeartbeatThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (heartbeat)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 # Only create one task executor by default
@@ -652,15 +657,15 @@
 
     inbound: Queue[Optional[Task]]
     outbound: Queue[Optional[Task]]
     scheduler: ClientSchedulerThread
     collector: ClientCollectorThread
     executors: List[TaskThread]
 
-    def __init__(self,
+    def __init__(self: ClientThread,
                  num_tasks: int = DEFAULT_NUM_TASKS,
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
                  address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port),
                  auth: str = QueueConfig.auth, template: str = DEFAULT_TEMPLATE,
                  redirect_output: IO = None, redirect_errors: IO = None,
                  heartrate: int = DEFAULT_HEARTRATE, capture: bool = False,
                  delay_start: float = DEFAULT_DELAY, no_confirm: bool = False) -> None:
@@ -679,72 +684,72 @@
                                                bundlesize=bundlesize, bundlewait=bundlewait)
         self.executors = [TaskThread(id=count+1,
                                      inbound=self.inbound, outbound=self.outbound,
                                      redirect_output=redirect_output, redirect_errors=redirect_errors,
                                      template=template, capture=capture)
                           for count in range(num_tasks)]
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: ClientThread) -> None:
         """Start child threads, wait."""
         log.debug(f'Started ({self.num_tasks} executors)')
         self.wait_start()
         with self.client:
             self.start_threads()
             self.wait_scheduler()
             self.wait_executors()
             self.wait_collector()
             self.wait_heartbeat()
         log.debug('Done')
 
-    def wait_start(self) -> None:
+    def wait_start(self: ClientThread) -> None:
         """Wait constant period or random interval."""
         if self.delay_start == 0:
             return
         if self.delay_start > 0:
             log.debug(f'Waiting ({self.delay_start} seconds)')
             time.sleep(self.delay_start)
         else:
             delay = random.uniform(0, -1 * self.delay_start)
             log.debug(f'Waiting random ({delay:.1f} seconds)')
             time.sleep(delay)
 
-    def start_threads(self) -> None:
+    def start_threads(self: ClientThread) -> None:
         """Start child threads."""
         self.scheduler.start()
         self.collector.start()
         self.heartbeat.start()
         for executor in self.executors:
             executor.start()
 
-    def wait_scheduler(self) -> None:
+    def wait_scheduler(self: ClientThread) -> None:
         """Wait for all tasks to be completed."""
         log.trace('Waiting (scheduler)')
         self.scheduler.join()
 
-    def wait_collector(self) -> None:
+    def wait_collector(self: ClientThread) -> None:
         """Signal collector to halt."""
         log.trace('Waiting (collector)')
         self.outbound.put(None)
         self.collector.join()
 
-    def wait_executors(self) -> None:
+    def wait_executors(self: ClientThread) -> None:
         """Send disconnect signal to each task executor thread."""
         for _ in self.executors:
             self.inbound.put(None)  # signal executors to shut down
         for thread in self.executors:
             log.trace(f'Waiting (executor-{thread.id})')
             thread.join()
 
-    def wait_heartbeat(self) -> None:
+    def wait_heartbeat(self: ClientThread) -> None:
         """Signal HALT on heartbeat."""
         log.trace('Waiting (heartbeat)')
         self.heartbeat.signal_finished()
         self.heartbeat.join()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: ClientThread, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         log.warning('Stopping')
         self.scheduler.stop(wait=wait, timeout=timeout)
         self.collector.stop(wait=wait, timeout=timeout)
         super().stop(wait=wait, timeout=timeout)
 
 
@@ -846,43 +851,46 @@
 
     exceptions = {
         EOFError: functools.partial(handle_disconnect, logger=log),
         ConnectionResetError: functools.partial(handle_disconnect, logger=log),
         ConnectionRefusedError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
         AuthenticationError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
         HostAddressInfo: functools.partial(handle_address_unknown, logger=log, status=exit_status.runtime_error),
-        **Application.exceptions,
+        **get_shared_exception_mapping(__name__),
     }
 
-    def run(self) -> None:
+    def run(self: ClientApp) -> None:
         """Run client."""
         try:
             self.check_args()
             run_client(num_tasks=self.num_tasks, bundlesize=self.bundlesize, bundlewait=self.bundlewait,
                        address=(self.host, self.port), auth=self.auth, template=self.template,
                        redirect_output=self.output_stream, redirect_errors=self.errors_stream,
                        capture=self.capture, delay_start=self.delay_start, no_confirm=self.no_confirm,
                        heartrate=config.client.heartrate)
         except gaierror:
             raise HostAddressInfo(f'Could not resolve host \'{self.host}\'')
 
-    def check_args(self) -> None:
+    def check_args(self: ClientApp) -> None:
         """Check for logical errors in command-line arguments."""
         if self.capture and (self.output_path or self.errors_path):
             raise ArgumentError('Cannot specify --capture with either --output or --errors')
 
     @functools.cached_property
-    def output_stream(self) -> IO:
+    def output_stream(self: ClientApp) -> IO:
         """IO stream for task outputs."""
         return sys.stdout if not self.output_path else open(self.output_path, mode='w')
 
     @functools.cached_property
-    def errors_stream(self) -> IO:
+    def errors_stream(self: ClientApp) -> IO:
         """IO stream for task errors."""
         return sys.stderr if not self.errors_path else open(self.errors_path, mode='w')
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self: ClientApp,
+                 exc_type: Optional[Type[Exception]],
+                 exc_val: Optional[Exception],
+                 exc_tb: Optional[TracebackType]) -> None:
         """Close IO streams if necessary."""
         if self.output_stream is not sys.stdout:
             self.output_stream.close()
         if self.errors_stream is not sys.stderr:
             self.errors_stream.close()
```

### Comparing `hyper-shell-2.2.0/src/hypershell/cluster.py` & `hyper-shell-2.3.0/src/hypershell/cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Run full cluster with server and clients.
 """
 
 
 # type annotations
 from __future__ import annotations
 from typing import IO, Optional, Iterable, List, Dict, Callable, Tuple, Type
+from types import TracebackType
 
 # standard libs
 import os
 import re
 import sys
 import time
 import secrets
@@ -27,14 +28,15 @@
 # internal libs
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.config import config, load_task_env, blame
 from hypershell.core.queue import QueueConfig
 from hypershell.core.thread import Thread
 from hypershell.core.logging import Logger, HOSTNAME
 from hypershell.core.template import DEFAULT_TEMPLATE
+from hypershell.core.exceptions import get_shared_exception_mapping
 from hypershell.database import initdb, checkdb
 from hypershell.client import ClientThread, DEFAULT_NUM_TASKS, DEFAULT_DELAY
 from hypershell.server import ServerThread, DEFAULT_BUNDLESIZE, DEFAULT_ATTEMPTS
 from hypershell.submit import DEFAULT_BUNDLEWAIT
 
 # public interface
 __all__ = ['run_local', 'run_cluster', 'run_ssh',
@@ -46,15 +48,15 @@
 
 class LocalCluster(Thread):
     """Run server with single local client."""
 
     server: ServerThread
     client: ClientThread
 
-    def __init__(self,
+    def __init__(self: LocalCluster,
                  source: Iterable[str] = None, num_tasks: int = 1, template: str = DEFAULT_TEMPLATE,
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
                  in_memory: bool = False, no_confirm: bool = False,
                  forever_mode: bool = False, restart_mode: bool = False,
                  max_retries: int = DEFAULT_ATTEMPTS, eager: bool = False,
                  redirect_failures: IO = None, redirect_output: IO = None, redirect_errors: IO = None,
                  delay_start: float = DEFAULT_DELAY, capture: bool = False) -> None:
@@ -66,37 +68,37 @@
                                    restart_mode=restart_mode, redirect_failures=redirect_failures)
         self.client = ClientThread(num_tasks=num_tasks, template=template, auth=auth, no_confirm=no_confirm,
                                    bundlesize=bundlesize, bundlewait=bundlewait, delay_start=delay_start,
                                    redirect_output=redirect_output, redirect_errors=redirect_errors,
                                    capture=capture)
         super().__init__(name='hypershell-cluster')
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: LocalCluster) -> None:
         """Start child threads, wait."""
         self.server.start()
         time.sleep(2)  # NOTE: give the server a chance to start
         self.client.start()
         self.client.join()
         self.server.join()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: LocalCluster, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         self.server.stop(wait=wait, timeout=timeout)
         self.client.stop(wait=wait, timeout=timeout)
         super().stop(wait=wait, timeout=timeout)
 
 
 class RemoteCluster(Thread):
     """Run server with remote clients via external launcher (e.g., MPI)."""
 
     server: ServerThread
     clients: Popen
     client_argv: str
 
-    def __init__(self,
+    def __init__(self: RemoteCluster,
                  source: Iterable[str] = None, num_tasks: int = 1, template: str = DEFAULT_TEMPLATE,
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
                  forever_mode: bool = False, restart_mode: bool = False,
                  bind: Tuple[str, int] = ('0.0.0.0', QueueConfig.port), delay_start: float = DEFAULT_DELAY,
                  launcher: str = 'mpirun', launcher_args: List[str] = None, remote_exe: str = 'hyper-shell',
                  max_retries: int = DEFAULT_ATTEMPTS, eager: bool = False, redirect_failures: IO = None,
                  in_memory: bool = False, no_confirm: bool = False, capture: bool = False) -> None:
@@ -113,25 +115,25 @@
         if no_confirm is True:
             client_args += ' --no-confirm'
         self.client_argv = (f'{launcher} {launcher_args} {remote_exe} client -H {HOSTNAME} -p {bind[1]} '
                             f'-N {num_tasks} -b {bundlesize} -w {bundlewait} -t "{template}" -k {auth} '
                             f'-d {delay_start} {client_args}')
         super().__init__(name='hypershell-cluster')
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: RemoteCluster) -> None:
         """Start child threads, wait."""
         self.server.start()
         time.sleep(2)  # NOTE: give the server a chance to start
         log.debug(f'Launching clients: {self.client_argv}')
         self.clients = Popen(self.client_argv, shell=True, stdout=sys.stdout, stderr=sys.stderr,
                              env={**os.environ, **load_task_env()})
         self.clients.wait()
         self.server.join()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: RemoteCluster, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         self.server.stop(wait=wait, timeout=timeout)
         self.clients.terminate()
         super().stop(wait=wait, timeout=timeout)
 
 
 class NodeList(list):
@@ -220,15 +222,15 @@
 class SSHCluster(Thread):
     """Run server with external ssh clients."""
 
     server: ServerThread
     clients: List[Popen]
     client_argv: List[str]
 
-    def __init__(self,
+    def __init__(self: SSHCluster,
                  source: Iterable[str] = None, num_tasks: int = 1, template: str = DEFAULT_TEMPLATE,
                  forever_mode: bool = False, restart_mode: bool = False,
                  bind: Tuple[str, int] = ('0.0.0.0', QueueConfig.port), remote_exe: str = 'hyper-shell',
                  launcher: str = 'ssh', launcher_args: List[str] = None, nodelist: List[str] = None,
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
                  max_retries: int = DEFAULT_ATTEMPTS, eager: bool = False, in_memory: bool = False,
                  no_confirm: bool = False, redirect_failures: IO = None, export_env: bool = False,
@@ -254,27 +256,27 @@
             client_args += ' --no-confirm'
         self.client_argv = [f'{launcher} {launcher_args} {host} {launcher_env} {remote_exe} '
                             f'client -H {HOSTNAME} -p {bind[1]} -N {num_tasks} -b {bundlesize} -w {bundlewait} '
                             f'-t \'"{template}"\' -k {auth} -d {delay_start} {client_args}'
                             for host in nodelist]
         super().__init__(name='hypershell-cluster')
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: SSHCluster) -> None:
         """Start child threads, wait."""
         self.server.start()
         time.sleep(2)  # NOTE: give the server a chance to start
         self.clients = []
         for argv in self.client_argv:
             log.debug(f'Launching client: {argv}')
             self.clients.append(Popen(argv, shell=True, stdout=sys.stdout, stderr=sys.stderr))
         for client in self.clients:
             client.wait()
         self.server.join()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: SSHCluster, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         self.server.stop(wait=wait, timeout=timeout)
         for client in self.clients:
             client.terminate()
         super().stop(wait=wait, timeout=timeout)
 
 
@@ -431,66 +433,70 @@
     interface.add_argument('-o', '--output', default=None, dest='output_path')
     interface.add_argument('-e', '--errors', default=None, dest='errors_path')
     interface.add_argument('-c', '--capture', action='store_true')
 
     failure_path: str = None
     interface.add_argument('-f', '--failures', default=None, dest='failure_path')
 
-    def run(self) -> None:
+    exceptions = {
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: ClusterApp) -> None:
         """Run cluster."""
         launcher = self.launchers.get(self.mode)
         launcher(source=self.source, num_tasks=self.num_tasks, template=self.template,
                  bundlesize=self.bundlesize, bundlewait=self.bundlewait, max_retries=self.max_retries,
                  in_memory=self.in_memory, no_confirm=self.no_confirm, forever_mode=self.forever_mode,
                  restart_mode=self.restart_mode, redirect_failures=self.failure_stream,
                  delay_start=self.delay_start, capture=self.capture)
 
-    def run_local(self, **options) -> None:
+    def run_local(self: ClusterApp, **options) -> None:
         """Run local cluster."""
         run_local(**options, redirect_output=self.output_stream, redirect_errors=self.errors_stream)
 
-    def run_launch(self, **options) -> None:
+    def run_launch(self: ClusterApp, **options) -> None:
         """Run remote cluster with custom launcher."""
         run_cluster(**options, launcher=self.launch_mode,
                     remote_exe=self.remote_exe, bind=('0.0.0.0', self.port))
 
-    def run_mpi(self, **options) -> None:
+    def run_mpi(self: ClusterApp, **options) -> None:
         """Run remote cluster with 'mpirun'."""
         run_cluster(**options, launcher='mpirun',
                     remote_exe=self.remote_exe, bind=('0.0.0.0', self.port))
 
-    def run_ssh(self, **options) -> None:
+    def run_ssh(self: ClusterApp, **options) -> None:
         """Run remote cluster with SSH."""
         if self.ssh_group:
             nodelist = NodeList.from_config(self.ssh_group)
         else:
             nodelist = NodeList.from_cmdline(self.ssh_mode if self.ssh_mode != '<default>' else None)
         run_ssh(**options, launcher='ssh', launcher_args=[self.ssh_args, ], nodelist=nodelist,
                 remote_exe=self.remote_exe, bind=('0.0.0.0', self.port), export_env=self.export_env)
 
     @cached_property
-    def launchers(self) -> Dict[str, Callable]:
+    def launchers(self: ClusterApp) -> Dict[str, Callable]:
         """Map of launchers."""
         return {
             'local': self.run_local,
             'launch': self.run_launch,
             'mpi': self.run_mpi,
             'ssh': self.run_ssh
         }
 
     @cached_property
-    def mode(self) -> str:
+    def mode(self: ClusterApp) -> str:
         """The launch mode to run the cluster."""
         for name in ['ssh', 'mpi', 'launch']:
             if getattr(self, f'{name}_mode'):
                 return name
         else:
             return 'local'
 
-    def check_arguments(self) -> None:
+    def check_arguments(self: ClusterApp) -> None:
         """Various checks on input arguments."""
         if self.restart_mode and self.in_memory:
             raise ArgumentError('Cannot restart without database (given --no-db)')
         if self.filepath is None and not self.restart_mode:
             self.filepath = '-'  # NOTE: assume STDIN
         if self.output_path and self.mode != 'local':
             raise ArgumentError('Cannot specify -o/--output PATH with remote clients')
@@ -508,51 +514,54 @@
             raise ArgumentError('Using --forever with --restart is invalid')
         if self.ssh_args and not self.ssh_mode:
             raise ArgumentError('Unexpected --ssh-args when not in --ssh mode')
         if self.ssh_group and self.ssh_mode != '<default>':
             raise ArgumentError('Cannot specify --ssh with target with --ssh-group')
 
     @cached_property
-    def output_stream(self) -> IO:
+    def output_stream(self: ClusterApp) -> IO:
         """IO stream to write task outputs."""
         return sys.stdout if not self.output_path else open(self.output_path, mode='w')
 
     @cached_property
-    def errors_stream(self) -> IO:
+    def errors_stream(self: ClusterApp) -> IO:
         """IO stream to write task errors."""
         return sys.stderr if not self.errors_path else open(self.errors_path, mode='w')
 
     @cached_property
-    def failure_stream(self) -> Optional[IO]:
+    def failure_stream(self: ClusterApp) -> Optional[IO]:
         """IO stream to write failed task args."""
         return None if not self.failure_path else open(self.failure_path, mode='w')
 
     @cached_property
-    def input_stream(self) -> Optional[IO]:
+    def input_stream(self: ClusterApp) -> Optional[IO]:
         """IO stream to read task command-line args."""
         if self.restart_mode:
             return None
         else:
             return sys.stdin if self.filepath == '-' else open(self.filepath, mode='r')
 
     @cached_property
-    def source(self) -> Iterable[str]:
+    def source(self: ClusterApp) -> Iterable[str]:
         """Input source for task command-line args."""
         return [] if self.restart_mode else self.input_stream
 
-    def __enter__(self) -> ClusterApp:
+    def __enter__(self: ClusterApp) -> ClusterApp:
         """Set up resources and attributes."""
         self.check_arguments()
         if config.database.provider == 'sqlite' or self.auto_initdb:
             initdb()  # Auto-initialize if local sqlite provider
         elif not self.in_memory:
             checkdb()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self: ClusterApp,
+                 exc_type: Optional[Type[Exception]],
+                 exc_val: Optional[Exception],
+                 exc_tb: Optional[TracebackType]) -> None:
         """Close IO streams if not standard streams."""
         if self.input_stream and self.input_stream is not sys.stdin:
             self.input_stream.close()
         if self.output_stream is not sys.stdout:
             self.output_stream.close()
         if self.errors_stream is not sys.stderr:
             self.errors_stream.close()
```

### Comparing `hyper-shell-2.2.0/src/hypershell/config.py` & `hyper-shell-2.3.0/src/hypershell/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Manage configuration."""
 
 
 # type annotations
 from __future__ import annotations
 from typing import Any
 
 # standard libs
 import os
 import sys
 import json
-import functools
 import subprocess
 
 # external libs
 import toml
-from cmdkit.app import Application, ApplicationGroup, exit_status
+from cmdkit.app import Application, ApplicationGroup
 from cmdkit.cli import Interface, ArgumentError
 from cmdkit.config import ConfigurationError
 from rich.console import Console
 from rich.syntax import Syntax
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.platform import path
 from hypershell.core.types import smart_coerce
 from hypershell.core.config import load_file, update, config as full_config
 from hypershell.core.logging import Logger
-from hypershell.core.exceptions import handle_exception
+from hypershell.core.exceptions import get_shared_exception_mapping
 
 # public interface
 __all__ = ['ConfigApp', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
@@ -65,15 +64,19 @@
                           colorize_usage(EDIT_HELP))
 
     site_name: str = 'user'
     site_interface = interface.add_mutually_exclusive_group()
     site_interface.add_argument('--user', action='store_const', const='user')
     site_interface.add_argument('--system', action='store_const', const='system')
 
-    def run(self) -> None:
+    exceptions = {
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: ConfigEditApp) -> None:
         """Business logic for `config edit`."""
 
         config_path = path[self.site_name].config
         editor = os.getenv('EDITOR', os.getenv('VISUAL', None))
         if not editor:
             raise RuntimeError('EDITOR or VISUAL environment variable not defined')
 
@@ -123,19 +126,18 @@
     site_interface.add_argument('--user', action='store_const', const='user', dest='site_name')
     site_interface.add_argument('--system', action='store_const', const='system', dest='site_name')
 
     expand: bool = False
     interface.add_argument('-x', '--expand', action='store_true')
 
     exceptions = {
-        ConfigurationError: functools.partial(handle_exception, logger=log, status=exit_status.bad_config),
-        **Application.exceptions,
+        **get_shared_exception_mapping(__name__)
     }
 
-    def run(self) -> None:
+    def run(self: ConfigGetApp) -> None:
         """Business logic for `config get`."""
 
         if self.site_name is None:
             config_path = 'configuration'  # Note: not meaningful for merged configuration
             config = full_config
         else:
             config_path = path[self.site_name].config
@@ -185,35 +187,35 @@
             self.print_output(value)
             return
         elif variable in config_section:
             self.print_output(config_section[variable])
         else:
             raise ConfigurationError(f'"{self.varpath}" not found in {config_path}')
 
-    def print_output(self, value: Any) -> None:
+    def print_output(self: ConfigGetApp, value: Any) -> None:
         """Format and print final `value`."""
         value = self.format_output(value)
         if sys.stdout.isatty():
             output = Syntax(value, 'toml', word_wrap=True,
                             theme = full_config.console.theme,
                             background_color = 'default')
             Console().print(output)
         else:
             # NOTE: JSON formatting puts quotations - we don't want these on raw output
             print(value.strip('"'), file=sys.stdout, flush=True)
 
-    def format_output(self, value: Any) -> str:
+    def format_output(self: ConfigGetApp, value: Any) -> str:
         """Format `value` as appropriate text."""
         if isinstance(value, dict):
             value = self.format_section(value)
         else:
             value = json.dumps(value)  # NOTE: close enough
         return value
 
-    def format_section(self, value: dict) -> str:
+    def format_section(self: ConfigGetApp, value: dict) -> str:
         """Format an entire section for output."""
         if self.varpath == '.':
             value = toml.dumps(value)
         else:
             value = toml.dumps({self.varpath: value})
         # NOTE: Fix weird formatting of section headings.
         #       The `toml.dumps` output has unnecessary quoting.
@@ -263,15 +265,19 @@
     interface.add_argument('value', type=smart_coerce)
 
     site_name: str = 'user'
     site_interface = interface.add_mutually_exclusive_group()
     site_interface.add_argument('--user', action='store_const', const='user', dest='site_name', default=site_name)
     site_interface.add_argument('--system', action='store_const', const='system', dest='site_name')
 
-    def run(self) -> None:
+    exceptions = {
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: ConfigSetApp) -> None:
         """Business logic for `config set`."""
 
         if '.' not in self.varpath:
             raise ArgumentError('Missing section in variable path')
 
         section, *subsections, variable = self.varpath.split('.')
 
@@ -311,15 +317,19 @@
     interface = Interface(WHICH_PROGRAM,
                           colorize_usage(WHICH_USAGE),
                           colorize_usage(WHICH_HELP))
 
     varpath: str = None
     interface.add_argument('varpath', metavar='VAR')
 
-    def run(self) -> None:
+    exceptions = {
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: ConfigWhichApp) -> None:
         """Business logic for `config which`."""
         try:
             site = full_config.which(*self.varpath.split('.'))
         except KeyError:
             log.critical(f'"{self.varpath}" not found')
             return
         if site in ('default', 'env', 'logging', ):
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/ansi.py` & `hyper-shell-2.3.0/src/hypershell/core/ansi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """ANSI color codes and methods."""
 
+
 # type annotations
 from __future__ import annotations
 from typing import Callable
 
 # standard libs
 import os
 import re
@@ -117,16 +118,16 @@
     """Add rich ANSI formatting to option syntax."""
     option_pattern = r'(?P<leader>[ /\[,])(?P<option>-[a-zA-Z]|--[a-z]+(-[a-z]+)?)\b'
     return re.sub(option_pattern + NOT_QUOTED, r'\g<leader>' + cyan(r'\g<option>'), text)
 
 
 def _format_special_args(text: str) -> str:
     """Add rich ANSI formatting to special argument syntax."""
-    metavars = ['FILE', 'PATH', 'ARGS', 'ID', 'NUM', 'CMD', 'SIZE', 'SEC', 'NAME', 'TEMPLATE',
-                'ADDR', 'HOST', 'PORT', 'KEY', 'SECTION', 'VAR', 'VALUE', 'FIELD', 'COND', ]
+    metavars = ['FILE', 'PATH', 'ARGS', 'ID', 'NUM', 'CMD', 'SIZE', 'SEC', 'NAME', 'TEMPLATE', 'CHAR',
+                'ADDR', 'HOST', 'PORT', 'KEY', 'SECTION', 'VAR', 'VALUE', 'FIELD', 'COND', 'FORMAT']
     metavars_pattern = r'\b(?P<arg>' + '|'.join(metavars) + r')\b'
     return re.sub(metavars_pattern + NOT_QUOTED, italic(r'\g<arg>'), text)
 
 
 def _format_special_marker(text: str) -> str:
     """Add rich ANSI formatting to special markers (e.g., '<stdout>')."""
     args = ['<stdout>', '<stderr>', '<stdin>', '<devnull>', '<none>', '<command>', '<args>', ]
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/config.py` & `hyper-shell-2.3.0/src/hypershell/core/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Runtime configuration for HyperShell."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/fsm.py` & `hyper-shell-2.3.0/src/hypershell/core/fsm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Instrumentation for building finite state machines."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/heartbeat.py` & `hyper-shell-2.3.0/src/hypershell/core/heartbeat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Heartbeat data passed between client and server."""
 
 
 # type annotations
 from __future__ import annotations
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/platform.py` & `hyper-shell-2.3.0/src/hypershell/core/platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Platform specific file paths and initialization."""
 
 
 # standard libs
 import os
 import sys
-import stat
 import ctypes
 
 # external libs
 from cmdkit.config import Namespace
 from cmdkit.app import exit_status
 
 # internal libs
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/queue.py` & `hyper-shell-2.3.0/src/hypershell/core/queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Queue server/client implementation."""
 
 
 # type annotations
 from __future__ import annotations
-from typing import Dict, List, Callable, Union, Optional, Any, Iterable
+from typing import Dict, List, Callable, Union, Optional, Any, Iterable, Type
+from types import TracebackType
 
 # standard libs
 from multiprocessing.managers import BaseManager
 from multiprocessing import JoinableQueue
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
@@ -32,15 +33,15 @@
 
     @classmethod
     def from_dict(cls, data: Dict[str, Union[str, int]]) -> QueueConfig:
         """Load config from existing dictionary values."""
         return cls(**data)
 
     @classmethod
-    def load(cls) -> QueueConfig:
+    def load(cls: Type[QueueConfig]) -> QueueConfig:
         """Initialize from global configuration."""
         return cls.from_dict({
             'host': _config.server.host,
             'port': _config.server.port,
             'auth': _config.server.auth,
             'size': _config.server.queuesize,
         })
@@ -51,66 +52,74 @@
 
     config: QueueConfig
     scheduled: JoinableQueue[Optional[List[bytes]]]
     completed: JoinableQueue[Optional[List[bytes]]]
     heartbeat: JoinableQueue[Optional[bytes]]
     confirmed: JoinableQueue[Optional[bytes]]
 
-    def __init__(self, config: QueueConfig) -> None:
+    def __init__(self: QueueInterface, config: QueueConfig) -> None:
         """Initialize queue interface."""
         self.config = config
         super().__init__(address=(self.config.host, self.config.port), authkey=self.config.auth.encode())
 
     @classmethod
-    def new(cls) -> QueueInterface:
+    def new(cls: Type[QueueInterface]) -> QueueInterface:
         """Create new interface from global configuration."""
         return cls(config=QueueConfig.load())
 
     @abstractmethod
-    def __enter__(self) -> QueueInterface:
+    def __enter__(self: QueueInterface) -> QueueInterface:
         """Start server or connect from client."""
 
     @abstractmethod
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self: QueueInterface,
+                 exc_type: Optional[Type[Exception]],
+                 exc_val: Optional[Exception],
+                 exc_tb: Optional[TracebackType]) -> None:
         """Stop or disconnect."""
 
 
 class QueueServer(QueueInterface):
     """Server for managing queue."""
 
-    def start(self, initializer: Optional[Callable[..., Any]] = ..., initargs: Iterable[Any] = ...) -> None:
+    def start(self: QueueServer,
+              initializer: Optional[Callable[..., Any]] = None,
+              initargs: Iterable[Any] = ()) -> None:
         """Initialize queues and start server."""
         self.scheduled = JoinableQueue(maxsize=self.config.size)
         self.completed = JoinableQueue(maxsize=self.config.size)
         self.heartbeat = JoinableQueue(maxsize=0)
         self.confirmed = JoinableQueue(maxsize=0)
         self.register('_get_scheduled', callable=self._get_scheduled)
         self.register('_get_completed', callable=self._get_completed)
         self.register('_get_heartbeat', callable=self._get_heartbeat)
         self.register('_get_confirmed', callable=self._get_confirmed)
         super().start()
 
-    def _get_scheduled(self) -> JoinableQueue[Optional[List[bytes]]]:
+    def _get_scheduled(self: QueueServer) -> JoinableQueue[Optional[List[bytes]]]:
         return self.scheduled
 
-    def _get_completed(self) -> JoinableQueue[Optional[List[bytes]]]:
+    def _get_completed(self: QueueServer) -> JoinableQueue[Optional[List[bytes]]]:
         return self.completed
 
-    def _get_heartbeat(self) -> JoinableQueue[Optional[bytes]]:
+    def _get_heartbeat(self: QueueServer) -> JoinableQueue[Optional[bytes]]:
         return self.heartbeat
 
-    def _get_confirmed(self) -> JoinableQueue[Optional[bytes]]:
+    def _get_confirmed(self: QueueServer) -> JoinableQueue[Optional[bytes]]:
         return self.confirmed
 
-    def __enter__(self) -> QueueServer:
+    def __enter__(self: QueueServer) -> QueueServer:
         """Start the server."""
         self.start()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self: QueueServer,
+                 exc_type: Optional[Type[Exception]],
+                 exc_val: Optional[Exception],
+                 exc_tb: Optional[TracebackType]) -> None:
         """Shutdown the server."""
         self.shutdown()
 
 
 class QueueClient(QueueInterface):
     """Client connection to queue manager."""
 
@@ -127,14 +136,17 @@
         self.register('_get_confirmed')
         super().connect()
         self.scheduled = self._get_scheduled()
         self.completed = self._get_completed()
         self.heartbeat = self._get_heartbeat()
         self.confirmed = self._get_confirmed()
 
-    def __enter__(self) -> QueueClient:
+    def __enter__(self: QueueClient) -> QueueClient:
         """Connect to server."""
         self.connect()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self: QueueClient,
+                 exc_type: Optional[Type[Exception]],
+                 exc_val: Optional[Exception],
+                 exc_tb: Optional[TracebackType]) -> None:
         """Disconnect from server."""
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/remote.py` & `hyper-shell-2.3.0/src/hypershell/core/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Manage remote connections and data."""
 
 
 # type annotations
 from __future__ import annotations
 from typing import Tuple, Optional, Type, Union, IO
 from types import TracebackType
 
 # standard libs
+import os
 import sys
 from dataclasses import dataclass
 
 # external libs
 from paramiko import SSHClient, SFTPClient, ProxyCommand, AutoAddPolicy, SSHConfig as SSHConfigParser
 from paramiko.channel import ChannelStdinFile, ChannelFile, ChannelStderrFile
 
@@ -43,52 +44,56 @@
     password: Optional[str] = None
     key_filename: Optional[str] = None
     sock: Optional[str] = None  # proxy-command
 
     @staticmethod
     def check_config(hostname: str, filepath: str = DEFAULT_SSH_CONFIG) -> Optional[dict]:
         """Check to see if `hostname` is defined in `filepath`, return `paramiko.SSHConfig`."""
+        if not os.path.exists(filepath):
+            return None
         with open(filepath, mode='r') as stream:
             ssh_config = SSHConfigParser()
             ssh_config.parse(stream)
             return ssh_config.lookup(hostname)
 
     @classmethod
     def from_config(cls: Type[SSHConfig], hostname: str, filepath: str = DEFAULT_SSH_CONFIG) -> SSHConfig:
         """Read configuration from file."""
-        profile = cls.check_config(hostname, filepath)
-        return cls(**{
-            'hostname': profile.get('hostname', hostname),
-            'username': profile.get('user', None),
-            'key_filename': profile.get('identityfile', None),
-            'sock': None if 'proxycommand' not in profile else ProxyCommand(profile['proxycommand']),
-        })
+        if profile := cls.check_config(hostname, filepath):
+            return cls(**{
+                'hostname': profile.get('hostname', hostname),
+                'username': profile.get('user', None),
+                'key_filename': profile.get('identityfile', None),
+                'sock': None if 'proxycommand' not in profile else ProxyCommand(profile['proxycommand']),
+            })
+        else:
+            return cls(hostname=hostname)
 
 
 class SSHConnection:
     """Connect to remote machine over SSH protocol."""
 
     config: SSHConfig
     client: SSHClient = None
 
     sftp: Optional[SFTPClient] = None
 
-    def __init__(self, hostname_or_config: Union[str, SSHConfig]) -> None:
+    def __init__(self: SSHConnection, hostname_or_config: Union[str, SSHConfig]) -> None:
         """Initialize with hostname or prepared SSHConfig."""
         if isinstance(hostname_or_config, SSHConfig):
             self.config = hostname_or_config
         else:
             self.config = SSHConfig.from_config(hostname_or_config)
 
     def __enter__(self: SSHConnection) -> SSHConnection:
         """Open connection."""
         self.open()
         return self
 
-    def __exit__(self,
+    def __exit__(self: SSHConnection,
                  exc_type: Optional[Type[Exception]],
                  exc_val: Optional[Exception],
                  exc_tb: Optional[TracebackType]) -> None:
         """Automatically close connection."""
         self.close()
 
     def open(self: SSHConnection) -> None:
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/template.py` & `hyper-shell-2.3.0/src/hypershell/core/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Template expansion facility for task execution."""
 
+
 # type annotations
 from __future__ import annotations
 from typing import Dict, Callable
 from types import ModuleType
 
 # standard libs
 import os
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/thread.py` & `hyper-shell-2.3.0/src/hypershell/core/thread.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Thread base class implementation."""
 
 
 # type annotations
 from __future__ import annotations
-from typing import Optional
+from typing import Optional, Type
 
 # standard libs
 import threading
 from abc import ABC, abstractmethod
 
 # public interface
 __all__ = ['Thread', ]
@@ -18,39 +18,39 @@
 
 class Thread(threading.Thread, ABC):
     """Extends threading.Thread to provide exception handling."""
 
     __exception: Exception = None
     __should_halt: bool = False
 
-    def __init__(self, name: str) -> None:
+    def __init__(self: Thread, name: str) -> None:
         super().__init__(name=name, daemon=True)
 
     @abstractmethod
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: Thread) -> None:
         """Implement `run` which may raise exceptions."""
 
-    def run(self) -> None:
+    def run(self: Thread) -> None:
         """Call `run_with_exceptions` within a try/except block."""
         try:
             self.run_with_exceptions()
         except Exception as exc:
             self.__exception = exc
 
     @classmethod
-    def new(cls, *args, **kwargs) -> Thread:
+    def new(cls: Type[Thread], *args, **kwargs) -> Thread:
         """Initialize and start the thread."""
         thread = cls(*args, **kwargs)
         thread.start()
         return thread
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: Thread, wait: bool = False, timeout: int = None) -> None:
         """Signal to terminate."""
         self.__should_halt = True
         if wait:
             self.join(timeout=timeout)
 
-    def join(self, timeout: Optional[float] = None) -> None:
+    def join(self: Thread, timeout: Optional[float] = None) -> None:
         """Calls Thread.join but re-raises exceptions."""
         super().join(timeout=timeout)
         if self.__exception:
             raise self.__exception
```

### Comparing `hyper-shell-2.2.0/src/hypershell/core/types.py` & `hyper-shell-2.3.0/src/hypershell/core/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Automatic type coercion of input data."""
 
 
 # type annotations
 from typing import TypeVar
```

### Comparing `hyper-shell-2.2.0/src/hypershell/database/__init__.py` & `hyper-shell-2.3.0/src/hypershell/database/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,54 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Database interface, models, and methods."""
 
 
+# type annotations
+from __future__ import annotations
+
 # standard libs
 import sys
+import functools
 
 # external libs
 from cmdkit.app import Application, exit_status
 from cmdkit.cli import Interface
 from cmdkit.config import ConfigurationError
 from sqlalchemy import inspect
 from sqlalchemy.orm import close_all_sessions
+from sqlalchemy.exc import OperationalError
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.logging import Logger
 from hypershell.core.config import config
-from hypershell.core.exceptions import write_traceback
+from hypershell.core.exceptions import (write_traceback, handle_exception, DatabaseUninitialized,
+                                        get_shared_exception_mapping)
 from hypershell.database.core import engine, in_memory, schema
 from hypershell.database.model import Model, Task
 
 # public interface
-__all__ = ['InitDBApp', 'initdb', 'truncatedb', 'checkdb', 'DatabaseUninitialized', 'DATABASE_ENABLED', ]
+__all__ = ['InitDBApp', 'initdb', 'truncatedb', 'checkdb', 'ensuredb', 'DATABASE_ENABLED', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
 
+try:
+    if not in_memory:
+        DATABASE_ENABLED = True
+    else:
+        DATABASE_ENABLED = False
+except Exception as error:
+    write_traceback(error, module=__name__)
+    sys.exit(exit_status.bad_config)
+
+
 def initdb() -> None:
     """Initialize database tables."""
     Model.metadata.create_all(engine)
 
 
 def truncatedb() -> None:
     """Truncate database tables."""
@@ -47,16 +63,23 @@
 
 def checkdb() -> None:
     """Ensure database connection and tables exist."""
     if not inspect(engine).has_table('task', schema=schema):
         raise DatabaseUninitialized('Use \'initdb\' to initialize the database')
 
 
-class DatabaseUninitialized(Exception):
-    """The database needs to be initialized before operations."""
+def ensuredb(auto_init: bool = False) -> None:
+    """Ensure database configuration before applying any operations."""
+    db = config.database.get('file', None) or config.database.get('database', None)
+    if config.database.provider == 'sqlite' and db in ('', ':memory:', None):
+        raise ConfigurationError('Missing database configuration')
+    if config.database.provider == 'sqlite' or auto_init is True:
+        initdb()
+    else:
+        checkdb()
 
 
 INITDB_PROGRAM = 'hyper-shell initdb'
 INITDB_USAGE = f"""\
 Usage:
 {INITDB_PROGRAM} [-h] [--truncate [--yes]]
 
@@ -85,15 +108,20 @@
 
     truncate: bool = False
     interface.add_argument('-t', '--truncate', action='store_true')
 
     auto_confirm: bool = False
     interface.add_argument('-y', '--yes', action='store_true', dest='auto_confirm')
 
-    def run(self) -> None:
+    exceptions = {
+        OperationalError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
+        **get_shared_exception_mapping(__name__),
+    }
+
+    def run(self: InitDBApp) -> None:
         """Business logic for `initdb`."""
         if not DATABASE_ENABLED:
             raise ConfigurationError('No database configured')
         elif not self.truncate:
             initdb()
         elif self.auto_confirm:
             truncatedb()
@@ -108,17 +136,7 @@
             response = input(f'Truncate database ({Task.count()} tasks)? [Y]es/no: ').strip()
             if response.lower() in ['', 'y', 'yes']:
                 truncatedb()
             elif response.lower() in ['n', 'no']:
                 print('Stopping')
             else:
                 raise RuntimeError(f'Stopping (invalid response: "{response}")')
-
-
-try:
-    if not in_memory:
-        DATABASE_ENABLED = True
-    else:
-        DATABASE_ENABLED = False
-except Exception as error:
-    write_traceback(error, module=__name__)
-    sys.exit(exit_status.bad_config)
```

### Comparing `hyper-shell-2.2.0/src/hypershell/database/core.py` & `hyper-shell-2.3.0/src/hypershell/database/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Core interface for database engine and session manager."""
 
 
 # type annotations
 from __future__ import annotations
-from typing import Any
+from typing import Any, Type
 
 # standard libs
 import sys
 import logging
 from urllib.parse import urlencode
 
 # external libs
@@ -37,130 +37,130 @@
 
     Example:
         >>> url = DatabaseURL(provider='postgresql', database='mine')
         >>> url.encode()
         'postgresql://localhost/mine'
     """
 
-    def __init__(self, **fields) -> None:
+    def __init__(self: DatabaseURL, **fields) -> None:
         """Initialize fields."""
         try:
             super().__init__(provider=fields.pop('provider'),
                              database=fields.pop('database', None),
                              file=fields.pop('file', None),
                              user=fields.pop('user', None),
                              password=fields.pop('password', None),
                              host=fields.pop('host', None),
                              port=fields.pop('port', None),
                              parameters=fields)
         except KeyError as _error:
             raise AttributeError('Missing \'provider\'') from _error
         self._validate()
 
-    def __getattr__(self, field: str) -> Any:
+    def __getattr__(self: DatabaseURL, field: str) -> Any:
         return self.get(field)
 
-    def __repr__(self) -> str:
+    def __repr__(self: DatabaseURL) -> str:
         """Interactive representation."""
         masked = self.__class__(**self)
         masked['password'] = None if self.password is None else '****'
         value = '<DatabaseURL('
         value += ', '.join([field + '=' + repr(masked.get(field))
                             for field in ('provider', 'database', 'file', 'user', 'password', 'host', 'port')
                             if masked.get(field) is not None])
         if self.parameters:
             value += ', ' + ', '.join([field + '=' + repr(value)
                                        for field, value in self.parameters.items()])
         return value + ')>'
 
-    def _validate(self) -> None:
+    def _validate(self: DatabaseURL) -> None:
         """Validate provided arguments."""
         if self.provider == 'sqlite':
             self._validate_for_sqlite()
         else:
             self._validate_database()
             self._validate_user_and_password()
 
-    def _validate_user_and_password(self) -> None:
+    def _validate_user_and_password(self: DatabaseURL) -> None:
         if self.user is not None and self.password is None:
             raise AttributeError('Must provide \'password\' if \'user\' provided')
         if self.user is None and self.password is not None:
             raise AttributeError('Must provide \'user\' if \'password\' provided')
 
-    def _validate_for_sqlite(self) -> None:
+    def _validate_for_sqlite(self: DatabaseURL) -> None:
         if self.file is not None and self.database is not None:
             raise AttributeError('Cannot provide both \'file\' and \'database\' for SQLite')
         for field in ('user', 'password', 'host', 'port'):
             if self.get(field) is not None:
                 raise AttributeError(f'Cannot provide \'{field}\' for SQLite')
 
-    def _validate_database(self) -> None:
+    def _validate_database(self: DatabaseURL) -> None:
         if self.file:
             raise AttributeError('Cannot provide \'file\' if not SQLite')
         if not self.database:
             raise AttributeError('Must provide \'database\' if not SQLite')
 
-    def encode(self) -> str:
+    def encode(self: DatabaseURL) -> str:
         """Construct URL string with encoded parameters."""
         return ''.join([
             f'{self.provider}://',
             self._format_user_and_password(),
             self._format_host_and_port(),
             self._format_database_or_file(),
             self._format_parameters(),
         ])
 
-    def _format_parameters(self) -> str:
+    def _format_parameters(self: DatabaseURL) -> str:
         if self.parameters:
             return '?' + urlencode(self.parameters)
         else:
             return ''
 
-    def _format_database_or_file(self) -> str:
+    def _format_database_or_file(self: DatabaseURL) -> str:
         if self.database:
             return f'/{self.database}'
         elif self.file:
             return f'/{self.file}'
         else:
             return ''
 
-    def _format_host_and_port(self) -> str:
+    def _format_host_and_port(self: DatabaseURL) -> str:
         if self.host and self.port:
             return f'{self.host}:{self.port}'
         elif self.host and not self.port:
             return f'{self.host}'
         elif self.port and not self.host:
             return f'localhost:{self.port}'
         else:
             if self.user or self.password:
                 return 'localhost'
             else:
                 return ''
 
-    def _format_user_and_password(self) -> str:
+    def _format_user_and_password(self: DatabaseURL) -> str:
         if self.user and self.password:
             return f'{self.user}:{self.password}@'
         else:
             return ''
 
-    def __str__(self) -> str:
+    def __str__(self: DatabaseURL) -> str:
         return self.encode()
 
     @staticmethod
     def _strip_endings(value: str, *endings: str):
         """Removing instances of each possible `endings` from `value`."""
         r = str(value)
         for ending in endings:
             pos = len(ending)
             if r[-pos:] == ending:
                 r = r[:-pos]
         return r
 
     @classmethod
-    def from_namespace(cls, ns: Namespace) -> DatabaseURL:
+    def from_namespace(cls: Type[DatabaseURL], ns: Namespace) -> DatabaseURL:
         fields = {}
         for key in ns.keys():
             key_ = cls._strip_endings(key, '_env', '_eval')
             fields[key_] = getattr(ns, key_)
         return cls(**fields)
```

### Comparing `hyper-shell-2.2.0/src/hypershell/database/model.py` & `hyper-shell-2.3.0/src/hypershell/database/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Database models."""
 
 
 # type annotations
 from __future__ import annotations
@@ -139,165 +139,165 @@
 
     class NotDistinct(NotDistinct):
         pass
 
     class AlreadyExists(AlreadyExists):
         pass
 
-    def __repr__(self) -> str:
+    def __repr__(self: Task) -> str:
         """String representation of record."""
         attrs = ', '.join([f'{name}={repr(getattr(self, name))}' for name in self.columns])
         return f'Task({attrs})'
 
-    def to_tuple(self) -> tuple:
+    def to_tuple(self: Task) -> tuple:
         """Convert fields into standard tuple."""
         return tuple([getattr(self, name) for name in self.columns])
 
-    def to_dict(self) -> Dict[str, Any]:
+    def to_dict(self: Task) -> Dict[str, Any]:
         """Convert record to dictionary."""
         return dict(zip(self.columns, self.to_tuple()))
 
-    def to_json(self) -> Dict[str, RT]:
+    def to_json(self: Task) -> Dict[str, RT]:
         """Convert record to JSON-serializable dictionary."""
         return {key: to_json_type(value) for key, value in self.to_dict().items()}
 
-    def pack(self) -> bytes:
+    def pack(self: Task) -> bytes:
         """Encode as raw JSON bytes."""
         return json.dumps(self.to_json()).encode()
 
     @classmethod
-    def from_dict(cls: Type[Model], data: Dict[str, VT]) -> Task:
+    def from_dict(cls: Type[Task], data: Dict[str, VT]) -> Task:
         """Build record from existing dictionary."""
         return cls(**data)
 
     @classmethod
-    def from_json(cls, data: Dict[str, RT]) -> Task:
+    def from_json(cls: Type[Task], data: Dict[str, RT]) -> Task:
         """Build record from JSON `text` string."""
         return cls.from_dict({key: from_json_type(value) for key, value in data.items()})
 
     @classmethod
-    def unpack(cls, data: bytes) -> Task:
+    def unpack(cls: Type[Task], data: bytes) -> Task:
         """Unpack raw JSON byte string."""
         return cls.from_json(json.loads(data.decode()))
 
     @classmethod
-    def from_id(cls, id: str, caching: bool = True) -> Task:
+    def from_id(cls: Type[Task], id: str, caching: bool = True) -> Task:
         """Look up task by unique `id`."""
         try:
             return cls.query(caching=caching).filter_by(id=id).one()
         except NoResultFound as error:
             raise cls.NotFound(f'No task with id={id}') from error
         except MultipleResultsFound as error:
             raise cls.NotDistinct(f'Multiple tasks with id={id}') from error
 
     @classmethod
-    def new(cls, args: str, attempt: int = 1, retried: bool = False, **other) -> Task:
+    def new(cls: Type[Task], args: str, attempt: int = 1, retried: bool = False, **other) -> Task:
         """Create a new Task."""
         return Task(id=str(gen_uuid()), args=str(args).strip(),
                     submit_id=INSTANCE, submit_host=HOSTNAME, submit_time=datetime.now().astimezone(),
                     attempt=attempt, retried=retried, **other)
 
     @classmethod
-    def query(cls, *fields: Column, caching: bool = True) -> Query:
+    def query(cls: Type[Task], *fields: Column, caching: bool = True) -> Query:
         """Get query interface for table with scoped session."""
         target = fields or [cls, ]
         if not caching:
             Session.expire_all()
         return Session.query(*target)
 
     @classmethod
-    def add_all(cls, tasks: List[Task]) -> List[Task]:
+    def add_all(cls: Type[Task], tasks: List[Task]) -> List[Task]:
         """Submit list of tasks to database."""
         task_ids = [task.id for task in tasks]  # NOTE: access after commit could trigger queries
         try:
             Session.add_all(tasks)
             Session.commit()
         except Exception:
             Session.rollback()
             raise
         else:
             for task_id in task_ids:
                 log.trace(f'Added task ({task_id})')
             return tasks
 
     @classmethod
-    def add(cls, task: Task) -> None:
+    def add(cls: Type[Task], task: Task) -> None:
         """Submit single task to database."""
         cls.add_all([task, ])
 
     @classmethod
-    def select_new(cls, limit: int) -> List[Task]:
+    def select_new(cls: Type[Task], limit: int) -> List[Task]:
         """Select unscheduled tasks up to some `limit` in order of submit_time."""
         return (cls.query()
                 .order_by(cls.submit_time)
                 .filter(cls.schedule_time.is_(None))
                 .limit(limit).all())
 
     @classmethod
-    def select_failed(cls, attempts: int, limit: int) -> List[Task]:
+    def select_failed(cls: Type[Task], attempts: int, limit: int) -> List[Task]:
         """Select failed tasks for retry up to some `limit` under given number of `attempts`."""
         return (cls.query()
                 .order_by(cls.completion_time)
                 .filter(cls.exit_status.isnot(None))
                 .filter(cls.exit_status != 0)
                 .filter(cls.attempt < attempts)
                 .filter(cls.retried.is_(False))
                 .limit(limit).all())
 
     @classmethod
-    def next(cls, limit: int, attempts: int = 1, eager: bool = False) -> List[Task]:
+    def next(cls: Type[Task], limit: int, attempts: int = 1, eager: bool = False) -> List[Task]:
         """Select tasks for scheduling including failed tasks for re-scheduling."""
         if eager:
             tasks = cls.__next_eager(attempts=attempts, limit=limit)
         else:
             tasks = cls.__next_not_eager(attempts, limit)
         for task in tasks:
             task.server_id = INSTANCE
             task.server_host = HOSTNAME
             task.schedule_time = datetime.now().astimezone()
         Session.commit()
         return tasks
 
     @classmethod
-    def __next_eager(cls, attempts: int, limit: int) -> List[Task]:
+    def __next_eager(cls: Type[Task], attempts: int, limit: int) -> List[Task]:
         """Select next batch of tasks from database preferring previously failed tasks."""
         tasks = cls.__schedule_next_failed_tasks(attempts, limit)
         if len(tasks) < limit:
             new_tasks = cls.select_new(limit=limit - len(tasks))
             tasks.extend(new_tasks)
             log.trace(f'Selected {len(new_tasks)} new tasks')
         return tasks
 
     @classmethod
-    def __next_not_eager(cls, attempts: int, limit: int) -> List[Task]:
+    def __next_not_eager(cls: Type[Task], attempts: int, limit: int) -> List[Task]:
         """Select next batch of tasks for database preferring novel tasks to old failed ones."""
         tasks = cls.select_new(limit=limit)
         log.trace(f'Selected {len(tasks)} new tasks')
         if len(tasks) < limit and attempts > 1:
             failed_tasks = cls.__schedule_next_failed_tasks(attempts=attempts, limit=limit - len(tasks))
             tasks.extend(failed_tasks)
         return tasks
 
     @classmethod
-    def __schedule_next_failed_tasks(cls, attempts: int, limit: int) -> List[Task]:
+    def __schedule_next_failed_tasks(cls: Type[Task], attempts: int, limit: int) -> List[Task]:
         """Select previously failed tasks for scheduling."""
         tasks = []
         failed_tasks = cls.select_failed(attempts=attempts, limit=limit)
         if failed_tasks:
             log.trace(f'Selected {len(failed_tasks)} previously failed tasks')
             new_tasks = [cls.new(args=task.args, attempt=task.attempt + 1, previous_id=task.id)
                          for task in failed_tasks]
             tasks.extend(new_tasks)
             cls.add_all(tasks)
             cls.update_all([{'id': old_task.id, 'retried': True, 'next_id': new_task.id}
                             for old_task, new_task in zip(failed_tasks, new_tasks)])
         return tasks
 
     @classmethod
-    def update_all(cls, changes: List[Dict[str, Any]]) -> None:
+    def update_all(cls: Type[Task], changes: List[Dict[str, Any]]) -> None:
         """
         Bulk update of tasks.
 
         Args:
             changes (list):
                 A list of dictionaries with fields representing
                 the changes to make to the Task records. The 'id' should
@@ -313,89 +313,89 @@
         """
         if changes:
             Session.bulk_update_mappings(cls, changes)
             Session.commit()  # NOTE: why is this necessary?
             log.trace(f'Updated {len(changes)} tasks')
 
     @classmethod
-    def update(cls, id: str, **changes) -> None:
+    def update(cls: Type[Task], id: str, **changes) -> None:
         """Update single task by `id` with `changes`."""
         cls.update_all([{'id': id, **changes}, ])
 
     @classmethod
-    def count(cls) -> int:
+    def count(cls: Type[Task]) -> int:
         """Count of tasks in database."""
         return cls.query().count()
 
     @classmethod
-    def count_remaining(cls) -> int:
+    def count_remaining(cls: Type[Task]) -> int:
         """Count of remaining unfinished tasks."""
         return cls.query().filter(cls.completion_time.is_(None)).count()
 
     @classmethod
-    def count_interrupted(cls) -> int:
+    def count_interrupted(cls: Type[Task]) -> int:
         """Count tasks that were scheduled but not completed."""
         return (
             cls.query()
             .filter(cls.schedule_time.isnot(None))
             .filter(cls.completion_time.is_(None))
             .count()
         )
 
     @classmethod
-    def select_interrupted(cls, limit: int) -> List[Task]:
+    def select_interrupted(cls: Type[Task], limit: int) -> List[Task]:
         """Select tasks that were scheduled but not completed."""
         return (
             cls.query()
             .order_by(cls.schedule_time)
             .filter(cls.schedule_time.isnot(None))
             .filter(cls.completion_time.is_(None))
             .limit(limit)
             .all()
         )
 
     @classmethod
-    def revert_interrupted(cls) -> None:
+    def revert_interrupted(cls: Type[Task]) -> None:
         """Revert scheduled but incomplete tasks to un-scheduled state."""
         while tasks := cls.select_interrupted(100):
             for task in tasks:
                 task.schedule_time = None
                 task.server_host = None
                 task.server_id = None
                 task.client_host = None
                 task.client_id = None
             Session.commit()
             for task in tasks:
                 log.trace(f'Reverted previous task ({task.id})')
 
     @classmethod
-    def select_orphaned(cls, client_id: str, limit: int) -> List[Task]:
+    def select_orphaned(cls: Type[Task], client_id: str, limit: int) -> List[Task]:
         """Select tasks that were orphaned from an evicted client."""
         return (
             cls.query()
             .order_by(cls.schedule_time)
             .filter(cls.schedule_time.isnot(None))
             .filter(cls.completion_time.is_(None))
             .filter(cls.client_id == client_id)
             .limit(limit)
             .all()
         )
 
     @classmethod
-    def revert_orphaned(cls, client_id: str) -> None:
+    def revert_orphaned(cls: Type[Task], client_id: str) -> None:
         """Revert orphaned tasks from an evicted client to un-scheduled state."""
         while tasks := cls.select_orphaned(client_id, 100):
             for task in tasks:
                 task.schedule_time = None
                 task.server_host = None
                 task.server_id = None
                 task.client_host = None
                 task.client_id = None
             Session.commit()
             for task in tasks:
                 log.trace(f'Reverted previous task ({task.id})')
 
 
 # Indices for efficient queries
-scheduled_index = Index('task_scheduled_index', Task.schedule_time)
-retries_index = Index('task_retries_index', Task.exit_status, Task.retried)
-client_completed_index = Index('task_client_completed_index', Task.client_id, Task.completion_time)
+index_scheduled = Index('task_scheduled_index', Task.schedule_time)
+index_retried = Index('task_retries_index', Task.exit_status, Task.retried)
+index_client_completed = Index('task_client_completed_index', Task.client_id, Task.completion_time)
```

### Comparing `hyper-shell-2.2.0/src/hypershell/server.py` & `hyper-shell-2.3.0/src/hypershell/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Schedule and update bundles of tasks from the database.
 
 The server can submit tasks for you so no need to directly submit before
 invoking the server (see `hypershell.submit`).
@@ -38,15 +38,16 @@
     your main program exits however, the thread will be stopped regardless because it
     runs as a `daemon`.
 """
 
 
 # type annotations
 from __future__ import annotations
-from typing import List, Dict, Tuple, Iterable, IO, Optional, Callable
+from typing import List, Dict, Tuple, Iterable, IO, Optional, Callable, Type
+from types import TracebackType
 
 # standard libs
 import sys
 import time
 from enum import Enum
 from datetime import datetime, timedelta
 from functools import cached_property
@@ -54,22 +55,23 @@
 
 # external libs
 from cmdkit.app import Application
 from cmdkit.cli import Interface, ArgumentError
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
+from hypershell.core.exceptions import get_shared_exception_mapping
 from hypershell.core.config import config, default
 from hypershell.core.logging import Logger
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.thread import Thread
 from hypershell.core.queue import QueueServer, QueueConfig
 from hypershell.core.heartbeat import Heartbeat, ClientState
 from hypershell.database.model import Task
-from hypershell.database import initdb, checkdb, DATABASE_ENABLED
+from hypershell.database import ensuredb, DATABASE_ENABLED
 from hypershell.submit import SubmitThread, LiveSubmitThread, DEFAULT_BUNDLEWAIT
 from hypershell.client import ClientInfo
 
 # public interface
 __all__ = ['serve_from', 'serve_file', 'serve_forever', 'ServerThread', 'ServerApp',
            'DEFAULT_BUNDLESIZE', 'DEFAULT_ATTEMPTS', ]
 
@@ -109,15 +111,15 @@
     restart_mode: bool
 
     state = SchedulerState.START
     states = SchedulerState
 
     startup_phase: bool = True
 
-    def __init__(self, queue: QueueServer, bundlesize: int = DEFAULT_BUNDLESIZE,
+    def __init__(self: Scheduler, queue: QueueServer, bundlesize: int = DEFAULT_BUNDLESIZE,
                  attempts: int = DEFAULT_ATTEMPTS, eager: bool = DEFAULT_EAGER_MODE,
                  forever_mode: bool = False, restart_mode: bool = False) -> None:
         """Initialize queue and parameters."""
         self.queue = queue
         self.bundle = []
         self.bundlesize = bundlesize
         self.attempts = attempts
@@ -125,24 +127,24 @@
         self.forever_mode = forever_mode
         self.restart_mode = restart_mode
         if self.restart_mode:
             # NOTE: Halt if everything in the database is already finished
             self.startup_phase = False
 
     @cached_property
-    def actions(self) -> Dict[SchedulerState, Callable[[], SchedulerState]]:
+    def actions(self: Scheduler) -> Dict[SchedulerState, Callable[[], SchedulerState]]:
         return {
             SchedulerState.START: self.start,
             SchedulerState.LOAD: self.load_bundle,
             SchedulerState.PACK: self.pack_bundle,
             SchedulerState.POST: self.post_bundle,
             SchedulerState.FINAL: self.finalize,
         }
 
-    def start(self) -> SchedulerState:
+    def start(self: Scheduler) -> SchedulerState:
         """Initial setup then jump to LOAD state."""
         log.debug('Started (scheduler)')
         if self.forever_mode:
             log.info('Scheduler will run forever')
         task_count = Task.count()
         tasks_remaining = Task.count_remaining()
         if task_count > 0:
@@ -152,33 +154,33 @@
             else:
                 tasks_interrupted = Task.count_interrupted()
                 log.info(f'Found {tasks_remaining} unfinished task(s)')
                 Task.revert_interrupted()
                 log.info(f'Reverted {tasks_interrupted} previously interrupted task(s)')
         return SchedulerState.LOAD
 
-    def load_bundle(self) -> SchedulerState:
+    def load_bundle(self: Scheduler) -> SchedulerState:
         """Load the next task bundle from the database."""
         self.tasks = Task.next(limit=self.bundlesize, attempts=self.attempts, eager=self.eager)
         if self.tasks:
             self.startup_phase = False
             return SchedulerState.PACK
         # An empty database must wait for at least one task
         elif not self.forever_mode and Task.count() > 0 and Task.count_remaining() == 0 and not self.startup_phase:
             return SchedulerState.FINAL
         else:
             time.sleep(DEFAULT_QUERY_PAUSE)
             return SchedulerState.LOAD
 
-    def pack_bundle(self) -> SchedulerState:
+    def pack_bundle(self: Scheduler) -> SchedulerState:
         """Pack tasks into bundle (list)."""
         self.bundle = [task.pack() for task in self.tasks]
         return SchedulerState.POST
 
-    def post_bundle(self) -> SchedulerState:
+    def post_bundle(self: Scheduler) -> SchedulerState:
         """Put bundle on outbound queue."""
         try:
             self.queue.scheduled.put(self.bundle, timeout=2)
             log.debug(f'Scheduled {len(self.tasks)} tasks')
             for task in self.tasks:
                 log.debug(f'Scheduled task ({task.id})')
             return SchedulerState.LOAD
@@ -191,35 +193,35 @@
         log.debug('Done (scheduler)')
         return SchedulerState.HALT
 
 
 class SchedulerThread(Thread):
     """Run scheduler within dedicated thread."""
 
-    def __init__(self, queue: QueueServer, bundlesize: int = DEFAULT_BUNDLESIZE,
+    def __init__(self: SchedulerThread, queue: QueueServer, bundlesize: int = DEFAULT_BUNDLESIZE,
                  attempts: int = DEFAULT_ATTEMPTS, eager: bool = DEFAULT_EAGER_MODE,
                  forever_mode: bool = False, restart_mode: bool = False) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-scheduler')
         self.machine = Scheduler(queue=queue, bundlesize=bundlesize, attempts=attempts, eager=eager,
                                  forever_mode=forever_mode, restart_mode=restart_mode)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: SchedulerThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: SchedulerThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (scheduler)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class ConfirmState(State, Enum):
-    """Finite states for Claim machine."""
+    """Finite states for task confirmation machine."""
     START = 0
     UNLOAD = 1
     UNPACK = 2
     UPDATE = 3
     FINAL = 4
     HALT = 5
 
@@ -231,54 +233,54 @@
     queue: QueueServer
     client_data: Optional[bytes]
     client_info: Optional[ClientInfo]
 
     state = ConfirmState.START
     states = ConfirmState
 
-    def __init__(self, queue: QueueServer, in_memory: bool = False) -> None:
+    def __init__(self: Confirm, queue: QueueServer, in_memory: bool = False) -> None:
         """Initialize machine."""
         self.in_memory = in_memory
         self.queue = queue
         self.client_data = None
         self.client_info = None
 
     @cached_property
-    def actions(self) -> Dict[ConfirmState, Callable[[], ConfirmState]]:
+    def actions(self: Confirm) -> Dict[ConfirmState, Callable[[], ConfirmState]]:
         return {
             ConfirmState.START: self.start,
             ConfirmState.UNLOAD: self.unload_info,
             ConfirmState.UNPACK: self.unpack_info,
             ConfirmState.UPDATE: self.update_info,
             ConfirmState.FINAL: self.finalize,
         }
 
     @staticmethod
     def start() -> ConfirmState:
         """Jump to UNLOAD state."""
         log.debug('Started (confirm)')
         return ConfirmState.UNLOAD
 
-    def unload_info(self) -> ConfirmState:
+    def unload_info(self: Confirm) -> ConfirmState:
         """Get the next task bundle confirmation from shared queue."""
         try:
             self.client_data = self.queue.confirmed.get(timeout=2)
             self.queue.confirmed.task_done()
             return ConfirmState.UNPACK if self.client_data else ConfirmState.FINAL
         except QueueEmpty:
             return ConfirmState.UNLOAD
 
-    def unpack_info(self) -> ConfirmState:
+    def unpack_info(self: Confirm) -> ConfirmState:
         """Unpack received client info."""
         self.client_info = ClientInfo.unpack(self.client_data)
         log.debug(f'Confirmed {len(self.client_info.task_ids)} tasks '
                   f'({self.client_info.client_host}: {self.client_info.client_id})')
         return ConfirmState.UPDATE
 
-    def update_info(self) -> ConfirmState:
+    def update_info(self: Confirm) -> ConfirmState:
         """Update client info in database for confirmed task bundle."""
         if not self.in_memory:
             Task.update_all(self.client_info.transpose())
         return ConfirmState.UNLOAD
 
     @staticmethod
     def finalize() -> ConfirmState:
@@ -286,24 +288,24 @@
         log.debug('Done (confirm)')
         return ConfirmState.HALT
 
 
 class ConfirmThread(Thread):
     """Run Confirm machine within dedicated thread."""
 
-    def __init__(self, queue: QueueServer, in_memory: bool = False) -> None:
+    def __init__(self: ConfirmThread, queue: QueueServer, in_memory: bool = False) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-confirm')
         self.machine = Confirm(queue=queue, in_memory=in_memory)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: ConfirmThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: ConfirmThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (confirm)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class ReceiverState(State, Enum):
@@ -325,53 +327,53 @@
 
     in_memory: bool
     redirect_failures: IO
 
     state = ReceiverState.START
     states = ReceiverState
 
-    def __init__(self, queue: QueueServer, in_memory: bool = False, redirect_failures: IO = None) -> None:
+    def __init__(self: Receiver, queue: QueueServer, in_memory: bool = False, redirect_failures: IO = None) -> None:
         """Initialize receiver."""
         self.queue = queue
         self.bundle = []
         self.in_memory = in_memory
         self.redirect_failures = redirect_failures
 
     @cached_property
-    def actions(self) -> Dict[ReceiverState, Callable[[], ReceiverState]]:
+    def actions(self: Receiver) -> Dict[ReceiverState, Callable[[], ReceiverState]]:
         return {
             ReceiverState.START: self.start,
             ReceiverState.UNLOAD: self.unload_bundle,
             ReceiverState.UNPACK: self.unpack_bundle,
             ReceiverState.UPDATE: self.update_tasks,
             ReceiverState.FINAL: self.finalize,
         }
 
     @staticmethod
     def start() -> ReceiverState:
         """Jump to UNLOAD state."""
         log.debug('Started (receiver)')
         return ReceiverState.UNLOAD
 
-    def unload_bundle(self) -> ReceiverState:
+    def unload_bundle(self: Receiver) -> ReceiverState:
         """Get the next bundle from the completed task queue."""
         try:
             self.bundle = self.queue.completed.get(timeout=2)
             self.queue.completed.task_done()
             return ReceiverState.UNPACK if self.bundle else ReceiverState.FINAL
         except QueueEmpty:
             log.trace('No completed tasks returned - waiting')
             return ReceiverState.UNLOAD
 
-    def unpack_bundle(self) -> ReceiverState:
+    def unpack_bundle(self: Receiver) -> ReceiverState:
         """Unpack previous bundle into list of tasks."""
         self.tasks = [Task.unpack(data) for data in self.bundle]
         return ReceiverState.UPDATE
 
-    def update_tasks(self) -> ReceiverState:
+    def update_tasks(self: Receiver) -> ReceiverState:
         """Update tasks in database with run details."""
         if not self.in_memory:
             Task.update_all([task.to_dict() for task in self.tasks])
         for task in self.tasks:
             log.debug(f'Completed task ({task.id})')
             if task.exit_status != 0:
                 log.warning(f'Non-zero exit status ({task.exit_status}) for task ({task.id})')
@@ -385,24 +387,27 @@
         log.debug('Done (receiver)')
         return ReceiverState.HALT
 
 
 class ReceiverThread(Thread):
     """Run receiver within dedicated thread."""
 
-    def __init__(self, queue: QueueServer, in_memory: bool = False, redirect_failures: IO = None) -> None:
+    def __init__(self: ReceiverThread,
+                 queue: QueueServer,
+                 in_memory: bool = False,
+                 redirect_failures: IO = None) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-receiver')
         self.machine = Receiver(queue=queue, in_memory=in_memory, redirect_failures=redirect_failures)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: ReceiverThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: ReceiverThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (receiver)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class HeartbeatState(State, Enum):
@@ -435,30 +440,30 @@
     scheduler_done: bool = False  # set by parent thread when scheduling is over
     should_signal: bool = False  # set by parent thread to signal clients
     latest_heartbeat: Heartbeat = None
 
     state = HeartbeatState.START
     states = HeartbeatState
 
-    def __init__(self, queue: QueueServer, evict_after: int = DEFAULT_EVICT,
+    def __init__(self: HeartMonitor, queue: QueueServer, evict_after: int = DEFAULT_EVICT,
                  in_memory: bool = False, no_confirm: bool = False) -> None:
         """Initialize with queue server."""
         self.queue = queue
         self.last_check = datetime.now()
         self.beats = {}
         self.in_memory = in_memory
         self.no_confirm = no_confirm
         if evict_after >= 10:
             self.wait_check = timedelta(seconds=int(evict_after / 10))
             self.evict_after = timedelta(seconds=evict_after)
         else:
             raise RuntimeError(f'Evict period must be greater than 10 seconds: given {evict_after}')
 
     @cached_property
-    def actions(self) -> Dict[HeartbeatState, Callable[[], HeartbeatState]]:
+    def actions(self: HeartMonitor) -> Dict[HeartbeatState, Callable[[], HeartbeatState]]:
         return {
             HeartbeatState.START: self.start,
             HeartbeatState.NEXT: self.get_next,
             HeartbeatState.UPDATE: self.update_client,
             HeartbeatState.SWITCH: self.switch_mode,
             HeartbeatState.CHECK: self.check_clients,
             HeartbeatState.SIGNAL: self.signal_clients,
@@ -467,29 +472,29 @@
 
     @staticmethod
     def start() -> HeartbeatState:
         """Jump to NEXT state."""
         log.debug('Started (heartbeat)')
         return HeartbeatState.NEXT
 
-    def get_next(self) -> HeartbeatState:
+    def get_next(self: HeartMonitor) -> HeartbeatState:
         """Get and stash heartbeat from clients."""
         try:
             hb_data = self.queue.heartbeat.get(timeout=2)
             self.queue.heartbeat.task_done()
             self.startup_phase = False
             if not hb_data:
                 return HeartbeatState.FINAL
             else:
                 self.latest_heartbeat = Heartbeat.unpack(hb_data)
                 return HeartbeatState.UPDATE
         except QueueEmpty:
             return HeartbeatState.SWITCH
 
-    def update_client(self) -> HeartbeatState:
+    def update_client(self: HeartMonitor) -> HeartbeatState:
         """Update client with heartbeat or disconnect."""
         hb = self.latest_heartbeat
         if hb.state is not ClientState.FINISHED:
             if hb.uuid not in self.beats:
                 log.debug(f'Registered client ({hb.host}: {hb.uuid})')
             else:
                 log.trace(f'Heartbeat - running ({hb.host}: {hb.uuid})')
@@ -497,44 +502,44 @@
             return HeartbeatState.SWITCH
         else:
             log.trace(f'Client disconnected ({hb.host}: {hb.uuid})')
             if hb.uuid in self.beats:
                 self.beats.pop(hb.uuid)
             return HeartbeatState.SWITCH
 
-    def switch_mode(self) -> HeartbeatState:
+    def switch_mode(self: HeartMonitor) -> HeartbeatState:
         """Decide to bail, signal, check, or get another heartbeat."""
         if self.startup_phase:
             return HeartbeatState.NEXT
         if self.should_signal:
             return HeartbeatState.SIGNAL
         if not self.beats and self.scheduler_done:
             return HeartbeatState.FINAL
         now = datetime.now()
         if (now - self.last_check) > self.wait_check:
             self.last_check = now
             return HeartbeatState.CHECK
         else:
             return HeartbeatState.NEXT
 
-    def check_clients(self) -> HeartbeatState:
+    def check_clients(self: HeartMonitor) -> HeartbeatState:
         """Check last heartbeat on all clients and evict if necessary."""
         log.debug(f'Checking clients ({len(self.beats)} connected)')
         for uuid in list(self.beats):
             hb = self.beats.get(uuid)
             age = self.last_check - hb.time
             if age > self.evict_after:
                 log.warning(f'Evicting client ({hb.host}: {uuid})')
                 self.beats.pop(uuid)
                 if not self.in_memory and not self.no_confirm:
                     log.warning(f'Reverting orphaned tasks ({hb.host}: {uuid})')
                     Task.revert_orphaned(uuid)
         return HeartbeatState.SWITCH
 
-    def signal_clients(self) -> HeartbeatState:
+    def signal_clients(self: HeartMonitor) -> HeartbeatState:
         """Send shutdown signal to all connected clients."""
         log.debug(f'Signaling clients ({len(self.beats)} connected)')
         for hb in self.beats.values():
             self.queue.scheduled.put(None)
             log.debug(f'Disconnect requested ({hb.host}: {hb.uuid})')
         self.should_signal = False
         return HeartbeatState.SWITCH
@@ -545,34 +550,34 @@
         log.debug('Done (heartbeat)')
         return HeartbeatState.HALT
 
 
 class HeartMonitorThread(Thread):
     """Run heart monitor within dedicated thread."""
 
-    def __init__(self, queue: QueueServer, evict_after: int = DEFAULT_EVICT,
+    def __init__(self: HeartMonitorThread, queue: QueueServer, evict_after: int = DEFAULT_EVICT,
                  in_memory: bool = False, no_confirm: bool = False) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-heartmonitor')
         self.machine = HeartMonitor(queue=queue, evict_after=evict_after,
                                     in_memory=in_memory, no_confirm=no_confirm)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: HeartMonitorThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def signal_clients(self) -> None:
+    def signal_clients(self: HeartMonitorThread) -> None:
         """Set signal flag to post sentinel for each connected clients."""
         self.machine.should_signal = True
 
-    def signal_scheduler_done(self) -> None:
+    def signal_scheduler_done(self: HeartMonitorThread) -> None:
         """Set flag to tell heart monitor that scheduler is done."""
         self.machine.scheduler_done = True
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: HeartMonitorThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (heartbeat)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class ServerThread(Thread):
@@ -583,15 +588,15 @@
     scheduler: Optional[SchedulerThread]
     confirm: Optional[ConfirmThread]
     receiver: ReceiverThread
     heartmonitor: HeartMonitorThread
     in_memory: bool
     no_confirm: bool
 
-    def __init__(self,
+    def __init__(self: ServerThread,
                  source: Iterable[str] = None,
                  in_memory: bool = False, no_confirm: bool = False,
                  forever_mode: bool = False, restart_mode: bool = False,
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
                  address: Tuple[str, int] = (QueueConfig.host, QueueConfig.port), auth: str = QueueConfig.auth,
                  max_retries: int = DEFAULT_ATTEMPTS - 1, eager: bool = False,
                  redirect_failures: IO = None, evict_after: int = DEFAULT_EVICT) -> None:
@@ -618,70 +623,70 @@
         else:
             self.confirm = ConfirmThread(queue=self.queue, in_memory=self.in_memory)
         self.receiver = ReceiverThread(queue=self.queue, in_memory=self.in_memory, redirect_failures=redirect_failures)
         self.heartmonitor = HeartMonitorThread(queue=self.queue, evict_after=evict_after,
                                                in_memory=in_memory, no_confirm=no_confirm)
         super().__init__(name='hypershell-server')
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: ServerThread) -> None:
         """Start child threads, wait."""
         log.debug('Started')
         with self.queue:
             self.start_threads()
             self.wait_submitter()
             self.wait_scheduler()
             self.wait_heartbeat()
             self.wait_receiver()
             self.wait_confirm()
         log.debug('Done')
 
-    def start_threads(self) -> None:
+    def start_threads(self: ServerThread) -> None:
         """Start child threads."""
         if self.submitter is not None:
             self.submitter.start()
         if self.scheduler is not None:
             self.scheduler.start()
         if not self.no_confirm:
             self.confirm.start()
         self.heartmonitor.start()
         self.receiver.start()
 
-    def wait_submitter(self) -> None:
+    def wait_submitter(self: ServerThread) -> None:
         """Wait on task submission to complete."""
         if self.submitter is not None:
             log.trace('Waiting (submitter)')
             self.submitter.join()
 
-    def wait_scheduler(self) -> None:
+    def wait_scheduler(self: ServerThread) -> None:
         """Wait scheduling until complete."""
         if self.scheduler is not None:
             log.trace('Waiting (scheduler)')
             self.scheduler.join()
 
-    def wait_heartbeat(self) -> None:
+    def wait_heartbeat(self: ServerThread) -> None:
         """Wait for heartmonitor to stop."""
         log.trace('Waiting (heartbeat)')
         self.heartmonitor.signal_scheduler_done()
         self.heartmonitor.signal_clients()
         self.heartmonitor.join()
 
-    def wait_receiver(self) -> None:
+    def wait_receiver(self: ServerThread) -> None:
         """Wait for receiver to stop."""
         log.trace('Waiting (receiver)')
         self.queue.completed.put(None)
         self.receiver.join()
 
-    def wait_confirm(self) -> None:
+    def wait_confirm(self: ServerThread) -> None:
         """Wait for confirm thread to stop."""
         if not self.no_confirm:
             log.trace('Waiting (confirm)')
             self.queue.confirmed.put(None)
             self.confirm.join()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: ServerThread, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         log.warning('Stopping')
         if self.submitter is not None:
             self.submitter.stop(wait=wait, timeout=timeout)
         if self.scheduler is not None:
             self.scheduler.stop(wait=wait, timeout=timeout)
         self.heartmonitor.stop(wait=wait, timeout=timeout)
@@ -831,62 +836,66 @@
 
     print_mode: bool = False
     failure_path: str = None
     output_interface = interface.add_mutually_exclusive_group()
     output_interface.add_argument('--print', action='store_true', dest='print_mode')
     output_interface.add_argument('-f', '--failures', default=None, dest='failure_path')
 
-    def run(self) -> None:
+    exceptions = {
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: ServerApp) -> None:
         """Run server."""
         if self.forever_mode:
             serve_forever(bundlesize=self.bundlesize, address=(self.host, self.port), auth=self.auth,
                           in_memory=self.in_memory, no_confirm=self.no_confirm,
                           max_retries=self.max_retries, eager=self.eager_mode,
                           redirect_failures=self.failure_stream, evict_after=config.server.evict)
         else:
             serve_from(source=self.input_stream, bundlesize=self.bundlesize, bundlewait=self.bundlewait,
                        address=(self.host, self.port), auth=self.auth, max_retries=self.max_retries,
                        in_memory=self.in_memory, no_confirm=self.no_confirm, evict_after=config.server.evict,
                        redirect_failures=self.failure_stream, restart_mode=self.restart_mode, eager=self.eager_mode)
 
-    def check_args(self):
+    def check_args(self: ServerApp):
         """Fail particular argument combinations."""
         if self.filepath and self.forever_mode:
             raise ArgumentError('Cannot specify both FILE and --forever')
         if self.filepath is None and not self.forever_mode:
             self.filepath = '-'  # NOTE: assume STDIN
         if self.restart_mode and self.forever_mode:
             raise ArgumentError('Using --forever with --restart is invalid')
 
     @cached_property
-    def input_stream(self) -> Optional[IO]:
+    def input_stream(self: ServerApp) -> Optional[IO]:
         """Input IO stream for task args."""
         if self.forever_mode or self.restart_mode:
             return None
         else:
             return sys.stdin if self.filepath == '-' else open(self.filepath, mode='r')
 
     @cached_property
-    def failure_stream(self) -> Optional[IO]:
+    def failure_stream(self: ServerApp) -> Optional[IO]:
         """IO stream for failed task args."""
         if self.print_mode:
             return sys.stdout
         elif self.failure_path:
             return sys.stdout if self.failure_path == '-' else open(self.failure_path, mode='w')
         else:
             return None
 
-    def __enter__(self) -> ServerApp:
-        """Open file if not stdin."""
+    def __enter__(self: ServerApp) -> ServerApp:
+        """Ensure context and database ready."""
         self.check_args()
-        if config.database.provider == 'sqlite' or self.auto_initdb:
-            initdb()  # Auto-initialize if local sqlite provider
-        elif not self.in_memory:
-            checkdb()
+        ensuredb()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self: ServerApp,
+                 exc_type: Optional[Type[Exception]],
+                 exc_val: Optional[Exception],
+                 exc_tb: Optional[TracebackType]) -> None:
         """Clean up IO if necessary."""
         if self.input_stream is not None and self.input_stream is not sys.stdin:
             self.input_stream.close()
         if self.failure_stream is not None and self.failure_path is not sys.stdout:
             self.failure_stream.close()
```

### Comparing `hyper-shell-2.2.0/src/hypershell/submit.py` & `hyper-shell-2.3.0/src/hypershell/submit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """
 Submit tasks to the database.
 
 Any iterable of command lines can be submitted directly.
 Example:
@@ -35,38 +35,39 @@
     your main program exits however, the thread will be stopped regardless because it
     runs as a `daemon`.
 """
 
 
 # type annotations
 from __future__ import annotations
-from typing import List, Iterable, Iterator, IO, Optional, Dict, Callable
+from typing import List, Iterable, Iterator, IO, Optional, Dict, Callable, Type
+from types import TracebackType
 
 # standard libs
 import io
 import sys
 import functools
 from enum import Enum
 from datetime import datetime
 from queue import Queue, Empty as QueueEmpty, Full as QueueFull
 
 # external libs
 from cmdkit.config import ConfigurationError
-from cmdkit.app import Application, exit_status
+from cmdkit.app import Application
 from cmdkit.cli import Interface
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.logging import Logger
 from hypershell.core.config import config, default
 from hypershell.core.fsm import State, StateMachine
 from hypershell.core.queue import QueueClient, QueueConfig
 from hypershell.core.thread import Thread
 from hypershell.core.template import Template, DEFAULT_TEMPLATE
-from hypershell.core.exceptions import handle_exception
+from hypershell.core.exceptions import get_shared_exception_mapping
 from hypershell.database.model import Task
 from hypershell.database import initdb, checkdb
 
 # public interface
 __all__ = ['submit_from', 'submit_file', 'SubmitThread', 'LiveSubmitThread',
            'SubmitApp', 'DEFAULT_BUNDLESIZE', 'DEFAULT_BUNDLEWAIT']
 
@@ -91,46 +92,46 @@
     queue: Queue[Optional[Task]]
     template: Template
     count: int
 
     state = LoaderState.START
     states = LoaderState
 
-    def __init__(self, source: Iterable[str], queue: Queue[Optional[Task]], template: str = DEFAULT_TEMPLATE) -> None:
+    def __init__(self: Loader, source: Iterable[str], queue: Queue[Optional[Task]], template: str = DEFAULT_TEMPLATE) -> None:
         """Initialize source to read tasks and submit to database."""
         self.template = Template(template)
         self.source = map(self.template.expand, map(str.strip, map(str, source)))
         self.queue = queue
         self.count = 0
 
     @functools.cached_property
-    def actions(self) -> Dict[LoaderState, Callable[[], LoaderState]]:
+    def actions(self: Loader) -> Dict[LoaderState, Callable[[], LoaderState]]:
         return {
             LoaderState.START: self.start,
             LoaderState.GET: self.get_task,
             LoaderState.PUT: self.put_task,
             LoaderState.FINAL: self.finalize,
         }
 
     @staticmethod
     def start() -> LoaderState:
         """Jump to GET state."""
         log.debug('Started (loader)')
         return LoaderState.GET
 
-    def get_task(self) -> LoaderState:
+    def get_task(self: Loader) -> LoaderState:
         """Get the next task from the source."""
         try:
             self.task = Task.new(args=next(self.source))
             log.trace(f'Loaded task ({self.task.args})')
             return LoaderState.PUT
         except StopIteration:
             return LoaderState.FINAL
 
-    def put_task(self) -> LoaderState:
+    def put_task(self: Loader) -> LoaderState:
         """Enqueue loaded task."""
         try:
             self.queue.put(self.task, timeout=1)
             self.count += 1
             return LoaderState.GET
         except QueueFull:
             return LoaderState.PUT
@@ -141,24 +142,27 @@
         log.debug('Done (loader)')
         return LoaderState.HALT
 
 
 class LoaderThread(Thread):
     """Run loader within dedicated thread."""
 
-    def __init__(self, source: Iterable[str], queue: Queue[Optional[Task]], template: str = DEFAULT_TEMPLATE) -> None:
+    def __init__(self: LoaderThread,
+                 source: Iterable[str],
+                 queue: Queue[Optional[Task]],
+                 template: str = DEFAULT_TEMPLATE) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-submit-loader')
         self.machine = Loader(source=source, queue=queue, template=template)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: LoaderThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: LoaderThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (loader)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class DatabaseCommitterState(State, Enum):
@@ -182,39 +186,40 @@
     bundlesize: int
     bundlewait: int
     previous_submit: datetime
 
     state = DatabaseCommitterState.START
     states = DatabaseCommitterState
 
-    def __init__(self,
+    def __init__(self: DatabaseCommitter,
                  queue: Queue[Optional[Task]],
-                 bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
+                 bundlesize: int = DEFAULT_BUNDLESIZE,
+                 bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
         """Initialize with task queue and buffering parameters."""
         self.queue = queue
         self.tasks = []
         self.bundlesize = bundlesize
         self.bundlewait = bundlewait
 
     @functools.cached_property
-    def actions(self) -> Dict[DatabaseCommitterState, Callable[[], DatabaseCommitterState]]:
+    def actions(self: DatabaseCommitter) -> Dict[DatabaseCommitterState, Callable[[], DatabaseCommitterState]]:
         return {
             DatabaseCommitterState.START: self.start,
             DatabaseCommitterState.GET: self.get_task,
             DatabaseCommitterState.COMMIT: self.commit,
             DatabaseCommitterState.FINAL: self.finalize,
         }
 
-    def start(self) -> DatabaseCommitterState:
+    def start(self: DatabaseCommitter) -> DatabaseCommitterState:
         """Jump to GET state."""
         log.debug('Started (committer: database)')
         self.previous_submit = datetime.now()
         return DatabaseCommitterState.GET
 
-    def get_task(self) -> DatabaseCommitterState:
+    def get_task(self: DatabaseCommitter) -> DatabaseCommitterState:
         """Get tasks from local queue and check buffer."""
         try:
             task = self.queue.get(timeout=1)
         except QueueEmpty:
             return DatabaseCommitterState.GET
         if task is not None:
             self.tasks.append(task)
@@ -222,97 +227,99 @@
             if len(self.tasks) >= self.bundlesize or since_last >= self.bundlewait:
                 return DatabaseCommitterState.COMMIT
             else:
                 return DatabaseCommitterState.GET
         else:
             return DatabaseCommitterState.FINAL
 
-    def commit(self) -> DatabaseCommitterState:
+    def commit(self: DatabaseCommitter) -> DatabaseCommitterState:
         """Commit tasks to database."""
         if self.tasks:
             Task.add_all(self.tasks)
             log.debug(f'Submitted {len(self.tasks)} tasks')
             self.tasks.clear()
             self.previous_submit = datetime.now()
         return DatabaseCommitterState.GET
 
-    def finalize(self) -> DatabaseCommitterState:
+    def finalize(self: DatabaseCommitter) -> DatabaseCommitterState:
         """Force final commit of tasks and halt."""
         self.commit()
         log.debug('Done (committer: database)')
         return DatabaseCommitterState.HALT
 
 
 class DatabaseCommitterThread(Thread):
     """Run committer within dedicated thread."""
 
-    def __init__(self, queue: Queue[Optional[Task]],
-                 bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
+    def __init__(self: DatabaseCommitterThread,
+                 queue: Queue[Optional[Task]],
+                 bundlesize: int = DEFAULT_BUNDLESIZE,
+                 bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-submit-committer')
         self.machine = DatabaseCommitter(queue=queue, bundlesize=bundlesize, bundlewait=bundlewait)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: DatabaseCommitterThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: DatabaseCommitterThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (committer: database)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class SubmitThread(Thread):
     """Manage asynchronous task queueing and submission workload."""
 
     source: Iterable[str]
     queue: Queue[Optional[Task]]
     loader: LoaderThread
     committer: DatabaseCommitterThread
 
-    def __init__(self, source: Iterable[str], bundlesize: int = DEFAULT_BUNDLESIZE,
+    def __init__(self: SubmitThread, source: Iterable[str], bundlesize: int = DEFAULT_BUNDLESIZE,
                  bundlewait: int = DEFAULT_BUNDLEWAIT, template: str = DEFAULT_TEMPLATE) -> None:
         """Initialize queue and child threads."""
         self.source = source
         self.queue = Queue(maxsize=bundlesize)
         self.loader = LoaderThread(source=source, queue=self.queue, template=template)
         self.committer = DatabaseCommitterThread(queue=self.queue, bundlesize=bundlesize, bundlewait=bundlewait)
         super().__init__(name='hypershell-submit')
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: SubmitThread) -> None:
         """Start child threads, wait."""
         log.debug(f'Started ({self.source_name})')
         self.loader.start()
         self.committer.start()
         self.loader.join()
         self.queue.put(None)
         self.committer.join()
         log.debug('Done')
 
     @functools.cached_property
-    def source_name(self) -> str:
+    def source_name(self: SubmitThread) -> str:
         """Log details of source."""
         if self.source is sys.stdin:
             return '<stdin>'
         elif isinstance(self.source, io.TextIOWrapper):
             return self.source.name
         else:
             return '<iterable>'
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: SubmitThread, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         log.warning('Stopping')
         self.loader.stop(wait=wait, timeout=timeout)
         self.queue.put(None)
         self.committer.stop(wait=wait, timeout=timeout)
         super().stop(wait=wait, timeout=timeout)
 
     @property
-    def task_count(self) -> int:
+    def task_count(self: SubmitThread) -> int:
         """Count of submitted tasks."""
         return self.loader.machine.count
 
 
 class QueueCommitterState(State, Enum):
     """Finite states for queue submitter."""
     START = 0
@@ -335,41 +342,41 @@
     bundlesize: int
     bundlewait: int
     previous_submit: datetime
 
     state = QueueCommitterState.START
     states = QueueCommitterState
 
-    def __init__(self, local: Queue[Optional[Task]], client: QueueClient,
+    def __init__(self: QueueCommitter, local: Queue[Optional[Task]], client: QueueClient,
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
         """Initialize with queue handles and buffering parameters."""
         self.local = local
         self.client = client
         self.tasks = []
         self.bundle = []
         self.bundlesize = bundlesize
         self.bundlewait = bundlewait
 
     @functools.cached_property
-    def actions(self) -> Dict[QueueCommitterState, Callable[[], QueueCommitterState]]:
+    def actions(self: QueueCommitter) -> Dict[QueueCommitterState, Callable[[], QueueCommitterState]]:
         return {
             QueueCommitterState.START: self.start,
             QueueCommitterState.GET: self.get_task,
             QueueCommitterState.PACK: self.pack_bundle,
             QueueCommitterState.COMMIT: self.commit,
             QueueCommitterState.FINAL: self.finalize,
         }
 
-    def start(self) -> QueueCommitterState:
+    def start(self: QueueCommitter) -> QueueCommitterState:
         """Jump to GET state."""
         log.debug('Started (committer: no database)')
         self.previous_submit = datetime.now()
         return QueueCommitterState.GET
 
-    def get_task(self) -> QueueCommitterState:
+    def get_task(self: QueueCommitter) -> QueueCommitterState:
         """Get tasks from local queue and check buffer."""
         try:
             task = self.local.get(timeout=1)
         except QueueEmpty:
             return QueueCommitterState.GET
         if task is not None:
             self.tasks.append(task)
@@ -377,23 +384,23 @@
             if len(self.tasks) >= self.bundlesize or since_last >= self.bundlewait:
                 return QueueCommitterState.PACK
             else:
                 return QueueCommitterState.GET
         else:
             return QueueCommitterState.FINAL
 
-    def pack_bundle(self) -> QueueCommitterState:
+    def pack_bundle(self: QueueCommitter) -> QueueCommitterState:
         """Pack tasks into bundle for remote queue."""
         if self.tasks:
             self.bundle = [task.pack() for task in self.tasks]
             return QueueCommitterState.COMMIT
         else:
             return QueueCommitterState.GET
 
-    def commit(self) -> QueueCommitterState:
+    def commit(self: QueueCommitter) -> QueueCommitterState:
         """Commit tasks to server scheduling queue."""
         try:
             if self.tasks:
                 self.client.scheduled.put(self.bundle, timeout=2)
                 for task in self.tasks:
                     log.trace(f'Scheduled task ({task.id})')
                 self.tasks = []
@@ -410,25 +417,25 @@
         log.debug('Done (committer: no database)')
         return QueueCommitterState.HALT
 
 
 class QueueCommitterThread(Thread):
     """Run queue committer within dedicated thread."""
 
-    def __init__(self, local: Queue[Optional[Task]], client: QueueClient,
+    def __init__(self: QueueCommitterThread, local: Queue[Optional[Task]], client: QueueClient,
                  bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
         """Initialize machine."""
         super().__init__(name='hypershell-submit-committer')
         self.machine = QueueCommitter(local=local, client=client, bundlesize=bundlesize, bundlewait=bundlewait)
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: QueueCommitterThread) -> None:
         """Run machine."""
         self.machine.run()
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: QueueCommitterThread, wait: bool = False, timeout: int = None) -> None:
         """Stop machine."""
         log.warning('Stopping (committer: no database)')
         self.machine.halt()
         super().stop(wait=wait, timeout=timeout)
 
 
 class LiveSubmitThread(Thread):
@@ -436,58 +443,62 @@
 
     source: Iterable[str]
     local: Queue[Optional[Task]]
     client: QueueClient
     loader: LoaderThread
     committer: QueueCommitterThread
 
-    def __init__(self, source: Iterable[str], queue_config: QueueConfig, template: str = DEFAULT_TEMPLATE,
-                 bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
+    def __init__(self: LiveSubmitThread,
+                 source: Iterable[str],
+                 queue_config: QueueConfig,
+                 template: str = DEFAULT_TEMPLATE,
+                 bundlesize: int = DEFAULT_BUNDLESIZE,
+                 bundlewait: int = DEFAULT_BUNDLEWAIT) -> None:
         """Initialize queue and child threads."""
         self.source = source
         self.local = Queue(maxsize=bundlesize)
         self.loader = LoaderThread(source=source, queue=self.local, template=template)
         self.client = QueueClient(config=queue_config)
         self.committer = QueueCommitterThread(local=self.local, client=self.client,
                                               bundlesize=bundlesize, bundlewait=bundlewait)
         super().__init__(name='hypershell-submit')
 
-    def run_with_exceptions(self) -> None:
+    def run_with_exceptions(self: LiveSubmitThread) -> None:
         """Start child threads, wait."""
         log.debug(f'Started ({self.source_name})')
         with self.client:
             self.loader.start()
             self.committer.start()
             log.trace('Waiting (loader)')
             self.loader.join()
             self.local.put(None)
             log.trace('Waiting (committer)')
             self.committer.join()
         log.debug('Done')
 
     @functools.cached_property
-    def source_name(self) -> str:
+    def source_name(self: LiveSubmitThread) -> str:
         """Log details of source."""
         if self.source is sys.stdin:
             return '<stdin>'
         elif isinstance(self.source, io.TextIOWrapper):
             return self.source.name
         else:
             return '<iterable>'
 
-    def stop(self, wait: bool = False, timeout: int = None) -> None:
+    def stop(self: LiveSubmitThread, wait: bool = False, timeout: int = None) -> None:
         """Stop child threads before main thread."""
         log.warning('Stopping')
         self.loader.stop(wait=wait, timeout=timeout)
         self.local.put(None)
         self.committer.stop(wait=wait, timeout=timeout)
         super().stop(wait=wait, timeout=timeout)
 
     @property
-    def task_count(self) -> int:
+    def task_count(self: LiveSubmitThread) -> int:
         """Count of submitted tasks."""
         return self.loader.machine.count
 
 
 def submit_from(source: Iterable[str], queue_config: QueueConfig = None,
                 bundlesize: int = DEFAULT_BUNDLESIZE, bundlewait: int = DEFAULT_BUNDLEWAIT,
                 template: str = DEFAULT_TEMPLATE) -> int:
@@ -562,43 +573,44 @@
 
     auto_initdb: bool = False
     interface.add_argument('--initdb', action='store_true', dest='auto_initdb')
 
     count: int = 0
 
     exceptions = {
-        FileNotFoundError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        ConfigurationError: functools.partial(handle_exception, logger=log, status=exit_status.bad_config),
-        **Application.exceptions,
+        **get_shared_exception_mapping(__name__)
     }
 
-    def run(self) -> None:
+    def run(self: SubmitApp) -> None:
         """Run submit thread."""
         self.submit_all()
         log.info(f'Submitted {self.count} tasks')
 
-    def submit_all(self) -> None:
+    def submit_all(self: SubmitApp) -> None:
         """Submit all tasks from source."""
         self.count = submit_from(self.source, template=self.template,
                                  bundlesize=self.bundlesize, bundlewait=self.bundlewait)
 
     @staticmethod
     def check_config():
         """Halt if we are not connected to database."""
         db = config.database.get('file', None) or config.database.get('database', None)
         if config.database.provider == 'sqlite' and db in ('', ':memory:', None):
             raise ConfigurationError('Submitting tasks to in-memory database has no effect')
 
-    def __enter__(self) -> SubmitApp:
+    def __enter__(self: SubmitApp) -> SubmitApp:
         """Open file if not stdin."""
         self.source = sys.stdin if self.filepath == '-' else open(self.filepath, mode='r')
         self.check_config()
         if config.database.provider == 'sqlite' or self.auto_initdb:
             initdb()  # Auto-initialize if local sqlite provider
         else:
             checkdb()
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self: SubmitApp,
+                 exc_type: Optional[Type[Exception]],
+                 exc_val: Optional[Exception],
+                 exc_tb: Optional[TracebackType]) -> None:
         """Close file if not stdin."""
         if self.source is not sys.stdin:
             self.source.close()
```

### Comparing `hyper-shell-2.2.0/src/hypershell/task.py` & `hyper-shell-2.3.0/src/hypershell/task.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# SPDX-FileCopyrightText: 2022 Geoffrey Lentner
+# SPDX-FileCopyrightText: 2023 Geoffrey Lentner
 # SPDX-License-Identifier: Apache-2.0
 
 """Task based operations."""
 
 
 # type annotations
 from __future__ import annotations
-from typing import List, Dict, Callable, IO, Tuple, Any
+from typing import List, Dict, Callable, IO, Tuple, Any, Optional, Type
 
 # standard libs
 import os
 import re
 import sys
 import csv
 import json
@@ -20,33 +20,33 @@
 from shutil import copyfileobj
 
 # external libs
 import yaml
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
-from cmdkit.config import ConfigurationError
 from cmdkit.app import Application, ApplicationGroup, exit_status
 from cmdkit.cli import Interface, ArgumentError
 from sqlalchemy import Column
-from sqlalchemy.exc import StatementError, OperationalError
+from sqlalchemy.exc import StatementError
 from sqlalchemy.orm import Query
 from sqlalchemy.orm.exc import StaleDataError
 from sqlalchemy.sql.elements import BinaryExpression
 
 # internal libs
 from hypershell.core.ansi import colorize_usage
 from hypershell.core.platform import default_path
 from hypershell.core.config import config
 from hypershell.core.exceptions import handle_exception
 from hypershell.core.logging import Logger, HOSTNAME
 from hypershell.core.remote import SSHConnection
 from hypershell.core.types import smart_coerce
+from hypershell.core.exceptions import get_shared_exception_mapping
 from hypershell.database.model import Task, to_json_type
-from hypershell.database import initdb, checkdb, DatabaseUninitialized
+from hypershell.database import ensuredb
 
 # public interface
 __all__ = ['TaskGroupApp', ]
 
 # initialize logger
 log = Logger.with_name(__name__)
 
@@ -76,16 +76,21 @@
     interface = Interface(SUBMIT_PROGRAM,
                           colorize_usage(SUBMIT_USAGE),
                           colorize_usage(SUBMIT_HELP))
 
     argv: List[str] = []
     interface.add_argument('argv', nargs='+')
 
-    def run(self) -> None:
+    exceptions = {
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: TaskSubmitApp) -> None:
         """Submit task to database."""
+        ensuredb()
         task = Task.new(args=' '.join(self.argv))
         Task.add(task)
         print(task.id)
 
 
 # Catch bad UUID before we touch the database
 UUID_PATTERN: re.Pattern = re.compile(
@@ -98,28 +103,29 @@
     if not UUID_PATTERN.match(value):
         raise ArgumentError(f'Bad UUID: \'{value}\'')
 
 
 INFO_PROGRAM = 'hyper-shell task info'
 INFO_USAGE = f"""\
 Usage: 
-{INFO_PROGRAM} [-h] ID [--json | --stdout | --stderr | -x FIELD]
+{INFO_PROGRAM} [-h] ID [--yaml | --json | --stdout | --stderr | -x FIELD]
 
 Get metadata and/or task outputs.\
 """
 
 INFO_HELP = f"""\
 {INFO_USAGE}
 
 Arguments:
   ID                    Unique task UUID.
 
 Options:
-      --json            Format as JSON.
-  -x, --extract  FIELD  Print this field only.
+      --yaml            Format task metadata as YAML.
+      --json            Format task metadata as JSON.
+  -x, --extract  FIELD  Print single field.
       --stdout          Fetch <stdout> from task.
       --stderr          Fetch <stderr> from task.
   -h, --help            Show this message and exit.\
 """
 
 
 class TaskInfoApp(Application):
@@ -128,87 +134,82 @@
     interface = Interface(INFO_PROGRAM,
                           colorize_usage(INFO_USAGE),
                           colorize_usage(INFO_HELP))
 
     uuid: str
     interface.add_argument('uuid')
 
-    format_json: bool = False
     print_stdout: bool = False
     print_stderr: bool = False
-    print_interface = interface.add_mutually_exclusive_group()
-    print_interface.add_argument('--json', action='store_true', dest='format_json')
-    print_interface.add_argument('--stdout', action='store_true', dest='print_stdout')
-    print_interface.add_argument('--stderr', action='store_true', dest='print_stderr')
-
     extract_field: str = None
-    interface.add_argument('-x', '--extract', default=None, choices=Task.columns, dest='extract_field')
+    output_format: str = 'normal'
+    output_formats: List[str] = ['normal', 'json', 'yaml']
+    output_interface = interface.add_mutually_exclusive_group()
+    output_interface.add_argument('--format', default=output_format, dest='output_format', choices=output_formats)
+    output_interface.add_argument('--json', action='store_const', const='json', dest='output_format')
+    output_interface.add_argument('--yaml', action='store_const', const='yaml', dest='output_format')
+    output_interface.add_argument('--stdout', action='store_true', dest='print_stdout')
+    output_interface.add_argument('--stderr', action='store_true', dest='print_stderr')
+    output_interface.add_argument('-x', '--extract', default=None, choices=Task.columns, dest='extract_field')
 
     exceptions = {
         Task.NotFound: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        StatementError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        FileNotFoundError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        RuntimeError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        **Application.exceptions,
+        **get_shared_exception_mapping(__name__)
     }
 
-    def run(self) -> None:
+    def run(self: TaskInfoApp) -> None:
         """Get metadata/status/outputs of task."""
+        ensuredb()
         check_uuid(self.uuid)
-        if self.extract_field and (self.print_stdout or self.print_stderr or self.format_json):
-            raise ArgumentError('Cannot use -x/--extract with other output formats')
         if self.extract_field:
-            print(json.dumps(getattr(self.task, self.extract_field)).strip('"'))
-        elif not (self.print_stdout or self.print_stderr):
-            self.write(self.task.to_json())
+            self.print_field()
         elif self.print_stdout:
-            if self.task.outpath:
-                self.write_file(self.outpath, sys.stdout)
-            else:
-                raise RuntimeError(f'No <stdout> for task ({self.uuid})')
+            self.print_file(self.outpath, self.task.outpath, sys.stdout)
         elif self.print_stderr:
-            if self.task.errpath:
-                self.write_file(self.errpath, sys.stderr)
-            else:
-                raise RuntimeError(f'No <stderr> file for task ({self.uuid})')
-
-    def write_file(self: TaskInfoApp, path: str, dest: IO) -> None:
-        """Write content from `path` to other `dest` stream."""
-        if not os.path.exists(path) and self.task.client_host != HOSTNAME:
-            log.debug(f'Fetching remote files ({self.task.client_host})')
-            self.copy_remote_files()
-        with open(path, mode='r') as stream:
-            copyfileobj(stream, dest)
+            self.print_file(self.errpath, self.task.errpath, sys.stderr)
+        elif self.output_format == 'normal':
+            print_normal(self.task)
+        else:
+            self.print_formatted()
 
-    def write(self, data: dict) -> None:
-        """Format and print `data` to console."""
-        formatter = self.format_method[self.format_name]
-        output = formatter(data)
+    def print_field(self: TaskInfoApp) -> None:
+        """Print single field."""
+        print(json.dumps(self.task.to_json().get(self.extract_field)).strip('"'))
+
+    def print_formatted(self: TaskInfoApp) -> None:
+        """Format and print task metadata to console."""
+        formatter = self.format_method[self.output_format]
+        output = formatter(self.task.to_json())  # NOTE: to_json() just means dict with converted value types
         if sys.stdout.isatty():
-            output = Syntax(output, self.format_name, word_wrap=True,
+            output = Syntax(output, self.output_format, word_wrap=True,
                             theme = config.console.theme, background_color = 'default')
             Console().print(output)
         else:
             print(output, file=sys.stdout, flush=True)
 
-    @functools.cached_property
-    def format_name(self) -> str:
-        """Either 'json' or 'yaml'."""
-        return 'yaml' if not self.format_json else 'json'
+    def print_file(self: TaskInfoApp, local_path: str, task_path: Optional[str], out_stream: IO) -> None:
+        """Print file contents, fetch from client if necessary."""
+        if task_path is None:
+            raise RuntimeError(f'No {out_stream.name} for task ({self.uuid})')
+        if not os.path.exists(local_path) and self.task.client_host != HOSTNAME:
+            self.copy_remote_files()
+        with open(local_path, mode='r') as in_stream:
+            copyfileobj(in_stream, out_stream)
 
     @functools.cached_property
-    def format_method(self) -> Dict[str, Callable[[dict], str]]:
+    def format_method(self: TaskInfoApp) -> Dict[str, Callable[[dict], str]]:
         """Format data method."""
         return {
             'yaml': functools.partial(yaml.dump, indent=4, sort_keys=False),
             'json': functools.partial(json.dumps, indent=4),
         }
 
     def copy_remote_files(self: TaskInfoApp) -> None:
-        """Copy output and error files and write to local streams."""
+        """Copy output and error files and to local host."""
+        log.debug(f'Fetching remote files ({self.task.client_host})')
         with SSHConnection(self.task.client_host) as remote:
             remote.get_file(self.task.outpath, self.outpath)
             remote.get_file(self.task.errpath, self.errpath)
 
     @functools.cached_property
     def task(self: TaskInfoApp) -> Task:
         """Look up the task from the database."""
@@ -271,28 +272,28 @@
     output_interface = interface.add_mutually_exclusive_group()
     output_interface.add_argument('--info', action='store_true', dest='print_info')
     output_interface.add_argument('--json', action='store_true', dest='format_json')
     output_interface.add_argument('--status', action='store_true', dest='print_status')
 
     exceptions = {
         Task.NotFound: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        StatementError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        **Application.exceptions,
+        **get_shared_exception_mapping(__name__)
     }
 
-    def run(self) -> None:
+    def run(self: TaskWaitApp) -> None:
         """Wait for task to complete."""
+        ensuredb()
         check_uuid(self.uuid)
         self.wait_task()
         if self.print_info or self.format_json:
             TaskInfoApp(uuid=self.uuid, format_json=self.format_json).run()
         elif self.print_status:
             TaskInfoApp(uuid=self.uuid, extract_field='exit_status').run()
 
-    def wait_task(self):
+    def wait_task(self: TaskWaitApp):
         """Wait for the task to complete."""
         log.info(f'Waiting on task ({self.uuid})')
         while True:
             task = Task.from_id(self.uuid, caching=False)
             if task.exit_status is None:
                 log.trace(f'Waiting ({self.uuid})')
                 time.sleep(self.interval)
@@ -332,63 +333,77 @@
 
     argv: List[str] = []
     interface.add_argument('argv', nargs='+')
 
     interval: int = DEFAULT_INTERVAL
     interface.add_argument('-n', '--interval', type=int, default=interval)
 
-    def run(self) -> None:
+    exceptions = {
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: TaskRunApp) -> None:
         """Submit task and wait for completion."""
+        ensuredb()
         task = Task.new(args=' '.join(self.argv))
         Task.add(task)
         TaskWaitApp(uuid=task.id, interval=self.interval).run()
         TaskInfoApp(uuid=task.id, print_stdout=True).run()
         TaskInfoApp(uuid=task.id, print_stderr=True).run()
 
 
 SEARCH_PROGRAM = 'hyper-shell task search'
 SEARCH_USAGE = f"""\
 Usage:
 hyper-shell task search [-h] [FIELD [FIELD ...]] [--where COND [COND ...]] 
-                        [--order-by FIELD [--desc]] [-x | --json | --csv] 
-                        [--count | --limit NUM]
-
+                        [--order-by FIELD [--desc]] [--count | --limit NUM]
+                        [--format FORMAT | --json | --csv]  [-d CHAR]
+                        
 Search for tasks in the database.\
 """
 
 SEARCH_HELP = f"""\
 {SEARCH_USAGE}
 
 Arguments:
-  FIELD                     Select specific named fields.
+  FIELD                      Select specific named fields.
 
 Options:
-  -w, --where     COND...   List of conditional statements.
-  -s, --order-by  FIELD     Order output by field.
-      --failed              Alias for "exit_status != 0"
-      --succeeded           Alias for "exit_status == 0"
-      --finished            Alias for "exit_status != null"
-      --remaining           Alias for "exit_status == null"
-  -x, --extract             Disable formatting for single column output.
-      --json                Format output as JSON.
-      --csv                 Format output as CSV.
-  -l, --limit     NUM       Limit the number of rows.
-  -c, --count               Show count of results.
-  -h, --help                Show this message and exit.\
+  -w, --where      COND...   List of conditional statements.
+  -s, --order-by   FIELD     Order output by field.
+      --failed               Alias for "exit_status != 0"
+      --succeeded            Alias for "exit_status == 0"
+      --finished             Alias for "exit_status != null"
+      --remaining            Alias for "exit_status == null"
+      --json                 Format output as JSON.
+      --csv                  Format output as CSV.
+      --format     FORMAT    Format output (normal, plain, table, csv, json).
+  -d, --delimiter  CHAR      Field seperator for plain/csv formats.
+  -l, --limit      NUM       Limit the number of results.
+  -c, --count                Show count of results.
+  -h, --help                 Show this message and exit.\
 """
 
 
+# Listing of all field names in order (default for search)
+ALL_FIELDS = list(Task.columns)
+
+
+# Reasonable limit on output delimiter (typically just single char).
+DELIMITER_MAX_SIZE = 100
+
+
 class TaskSearchApp(Application):
     """Search for tasks in database."""
 
     interface = Interface(SEARCH_PROGRAM,
                           colorize_usage(SEARCH_USAGE),
                           colorize_usage(SEARCH_HELP))
 
-    field_names: List[str] = list(Task.columns)
+    field_names: List[str] = ALL_FIELDS
     interface.add_argument('field_names', nargs='*', default=field_names)
 
     where_clauses: List[str] = None
     interface.add_argument('-w', '--where', nargs='*', default=[], dest='where_clauses')
 
     order_by: str = None
     order_desc: bool = False
@@ -407,45 +422,54 @@
     show_remaining: bool = False
     search_alias_interface = interface.add_mutually_exclusive_group()
     search_alias_interface.add_argument('--failed', action='store_true', dest='show_failed')
     search_alias_interface.add_argument('--finished', action='store_true', dest='show_finished')
     search_alias_interface.add_argument('--remaining', action='store_true', dest='show_remaining')
     search_alias_interface.add_argument('--succeeded', action='store_true', dest='show_succeeded')
 
-    output_format: str = 'table'
-    output_formats: List[str] = ['table', 'json', 'csv', ]
+    output_format: str = '<default>'  # 'plain' if field_names else 'normal'
+    output_formats: List[str] = ['normal', 'plain', 'table', 'json', 'csv']
     output_interface = interface.add_mutually_exclusive_group()
     output_interface.add_argument('--format', default=output_format, dest='output_format', choices=output_formats)
     output_interface.add_argument('--json', action='store_const', const='json', dest='output_format')
     output_interface.add_argument('--csv', action='store_const', const='csv', dest='output_format')
-    output_interface.add_argument('-x', '--extract', action='store_const', const='extract', dest='output_format')
 
-    def run(self) -> None:
+    output_delimiter: str = '<default>'  # <space> if plain, ',' if --csv, else not valid
+    interface.add_argument('-d', '--delimiter', default=output_delimiter, dest='output_delimiter')
+
+    exceptions = {
+        StatementError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: TaskSearchApp) -> None:
         """Search for tasks in database."""
+        ensuredb()
         self.check_field_names()
+        self.check_output_format()
         if self.show_count:
             print(self.build_query().count())
         else:
             self.print_output(self.build_query().all())
 
-    def build_query(self) -> Query:
+    def build_query(self: TaskSearchApp) -> Query:
         """Build original query interface."""
         query = Task.query(*self.fields)
         if self.order_by:
             field = getattr(Task, self.order_by)
             if self.order_desc:
                 field = field.desc()
             query = query.order_by(field)
         for where_clause in self.build_filters():
             query = query.filter(where_clause.compile())
         if self.limit:
             query = query.limit(self.limit)
         return query
 
-    def build_filters(self) -> List[WhereClause]:
+    def build_filters(self: TaskSearchApp) -> List[WhereClause]:
         """Create list of field selectors from command-line arguments."""
         if self.show_failed:
             self.where_clauses.append('exit_status != 0')
         if self.show_succeeded:
             self.where_clauses.append('exit_status == 0')
         if self.show_finished:
             self.where_clauses.append('exit_status != null')
@@ -453,66 +477,95 @@
             self.where_clauses.append('exit_status == null')
         if not self.where_clauses:
             return []
         else:
             return [WhereClause.from_cmdline(arg) for arg in self.where_clauses]
 
     @functools.cached_property
-    def fields(self) -> List[Column]:
+    def fields(self: TaskSearchApp) -> List[Column]:
         """Field instances to query against."""
         return [getattr(Task, name) for name in self.field_names]
 
     @functools.cached_property
-    def print_output(self) -> Callable[[List[Tuple]], None]:
+    def print_output(self: TaskSearchApp) -> Callable[[List[Tuple]], None]:
         """The requested output formatter."""
         return getattr(self, f'print_{self.output_format}')
 
-    def print_extract(self, results: List[Tuple]) -> None:
-        """Basic output from single column."""
-        if len(self.field_names) == 1:
-            for (value, ) in results:
-                print(json.dumps(to_json_type(value)).strip('"'), file=sys.stdout)
-        else:
-            raise ArgumentError(f'Cannot use -x/--extract for more than a single field')
-
-    def print_table(self, results: List[Tuple]) -> None:
-        """Print in table format from simple instances of ModelInterface."""
+    def print_table(self: TaskSearchApp, results: List[Tuple]) -> None:
+        """Print in table format."""
         table = Table(title=None)
         for name in self.field_names:
             table.add_column(name)
         for record in results:
             table.add_row(*[json.dumps(to_json_type(value)).strip('"') for value in record])
         Console().print(table)
 
-    def print_json(self, results: List[Tuple]) -> None:
-        """Print in JSON format from simple instances of ModelInterface."""
+    @staticmethod
+    def print_normal(results: List[Tuple]) -> None:
+        """Print semi-structured output with all field names."""
+        for record in results:
+            print('---')
+            print_normal(Task.from_dict(dict(zip(Task.columns, record))))
+
+    def print_plain(self: TaskSearchApp, results: List[Tuple]) -> None:
+        """Print plain text output with given field names, one task per line."""
+        for record in results:
+            data = [json.dumps(to_json_type(value)).strip('"') for value in record]
+            print(self.output_delimiter.join(map(str, data)))
+
+    def print_json(self: TaskSearchApp, results: List[Tuple]) -> None:
+        """Print in output in JSON format."""
         data = [{field: to_json_type(value) for field, value in zip(self.field_names, record)}
                 for record in results]
         if sys.stdout.isatty():
             Console().print(Syntax(json.dumps(data, indent=4, sort_keys=False), 'json',
                                    word_wrap=True, theme=config.console.theme,
                                    background_color='default'))
         else:
             print(json.dumps(data, indent=4, sort_keys=False), file=sys.stdout, flush=True)
 
-    def print_csv(self, results: List[Tuple]) -> None:
-        """Print in CVS format from simple instances of ModelInterface."""
-        writer = csv.writer(sys.stdout)
+    def print_csv(self: TaskSearchApp, results: List[Tuple]) -> None:
+        """Print output in CVS format."""
+        writer = csv.writer(sys.stdout, delimiter=self.output_delimiter)
         writer.writerow(self.field_names)
         for record in results:
             data = [to_json_type(value) for value in record]
             data = [value if isinstance(value, str) else json.dumps(value) for value in data]
             writer.writerow(data)
 
-    def check_field_names(self) -> None:
+    def check_field_names(self: TaskSearchApp) -> None:
         """Check field names are valid."""
         for name in self.field_names:
             if name not in Task.columns:
                 raise ArgumentError(f'Invalid field name \'{name}\'')
 
+    def check_output_format(self: TaskSearchApp) -> None:
+        """Check given output format is valid."""
+        if self.field_names == ALL_FIELDS:
+            if self.output_format == '<default>':
+                self.output_format = 'normal'
+        else:
+            if self.output_format == '<default>':
+                self.output_format = 'plain'
+            elif self.output_format == 'normal':
+                raise ArgumentError('Cannot use --format=normal with subset of field names')
+        if self.output_delimiter != '<default>' and self.output_format not in ['plain', 'csv']:
+            raise ArgumentError(f'Unused --delimiter for --format={self.output_format}')
+        if len(self.output_delimiter) > DELIMITER_MAX_SIZE:
+            raise ArgumentError(f'Output delimiter exceeds max size ({len(self.output_delimiter)} '
+                                f'> {DELIMITER_MAX_SIZE})')
+        if self.output_delimiter == '<default>':
+            if self.output_format == 'csv':
+                self.output_delimiter = ','
+            else:
+                self.output_delimiter = '\t'
+        elif self.output_format == 'csv' and len(self.output_delimiter) != 1:
+            # NOTE: csv module demands single-char delimiter
+            raise ArgumentError(f'Valid --csv output must use single-char delimiter')
+
 
 UPDATE_PROGRAM = 'hyper-shell task update'
 UPDATE_USAGE = f"""\
 Usage: 
 {UPDATE_PROGRAM} [-h] ID FIELD VALUE 
 
 Update individual task metadata.\
@@ -543,16 +596,22 @@
 
     field: str
     interface.add_argument('field', choices=list(Task.columns)[1:])  # NOTE: not ID!
 
     value: str
     interface.add_argument('value', type=smart_coerce)
 
-    def run(self) -> None:
+    exceptions = {
+        Task.NotFound: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
+        **get_shared_exception_mapping(__name__)
+    }
+
+    def run(self: TaskUpdateApp) -> None:
         """Update individual task attribute directly."""
+        ensuredb()
         check_uuid(self.uuid)
         try:
             Task.update(self.uuid, **{self.field: self.value, })
         except StaleDataError as err:
             raise Task.NotFound(str(err)) from err
 
 
@@ -595,34 +654,14 @@
         'info': TaskInfoApp,
         'wait': TaskWaitApp,
         'run': TaskRunApp,
         'search': TaskSearchApp,
         'update': TaskUpdateApp,
     }
 
-    # NOTE: ApplicationGroup only defines the CompletedCommand mechanism.
-    #       Extending this allows for a shared exception for all task commands
-    exceptions = {
-        ConfigurationError: functools.partial(handle_exception, logger=log, status=exit_status.bad_config),
-        DatabaseUninitialized: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        OperationalError: functools.partial(handle_exception, logger=log, status=exit_status.runtime_error),
-        **ApplicationGroup.exceptions
-    }
-
-    def __enter__(self: TaskGroupApp) -> TaskGroupApp:
-        """Resource initialization."""
-        db = config.database.get('file', None) or config.database.get('database', None)
-        if config.database.provider == 'sqlite' and db in ('', ':memory:', None):
-            raise ConfigurationError('Missing database configuration')
-        if config.database.provider == 'sqlite':
-            initdb()  # Auto-initialize if local sqlite provider
-        else:
-            checkdb()
-        return self
-
 
 @dataclass
 class WhereClause:
     """Parse and prepare query filters based on command-line argument."""
 
     field: str
     value: Any
@@ -635,27 +674,48 @@
         '>=': lambda lhs, rhs: lhs >= rhs,
         '<=': lambda lhs, rhs: lhs <= rhs,
         '>':  lambda lhs, rhs: lhs > rhs,
         '<':  lambda lhs, rhs: lhs < rhs,
         '~':  lambda lhs, rhs: lhs.regexp_match(rhs),
     }
 
-    def compile(self) -> BinaryExpression:
+    def compile(self: WhereClause) -> BinaryExpression:
         """Build binary expression object out of elements."""
         op_call = self.op_call.get(self.operand)
         return op_call(getattr(Task, self.field), self.value)
 
     @classmethod
-    def from_cmdline(cls, argument: str) -> WhereClause:
+    def from_cmdline(cls: Type[WhereClause], argument: str) -> WhereClause:
         """
         Construct from command-line `argument`.
 
         Example:
             >>> WhereClause.from_cmdline('exit_status != 0')
             WhereClause(field='exit_status', value=0, operand='!=')
         """
         match = cls.pattern.match(argument)
         if match:
             field, operand, value = match.groups()
             return WhereClause(field=field, value=smart_coerce(value), operand=operand)
         else:
             raise ArgumentError(f'Where clause not understood ({argument})')
+
+
+def print_normal(task: Task) -> None:
+    """Print semi-structured task metadata with all field names."""
+    task_data = {k: json.dumps(to_json_type(v)).strip('"') for k, v in task.to_dict().items()}
+    print(f'          id: {task_data["id"]}')
+    print(f'     command: {task_data["command"]} ({task_data["args"]})')
+    print(f' exit_status: {task_data["exit_status"]}')
+    print(f'   submitted: {task_data["submit_time"]}')
+    print(f'   scheduled: {task_data["schedule_time"]}')
+    print(f'     started: {task_data["start_time"]}')
+    print(f'   completed: {task_data["completion_time"]}')
+    print(f' submit_host: {task_data["submit_host"]} ({task_data["submit_id"]})')
+    print(f' server_host: {task_data["server_host"]} ({task_data["server_id"]})')
+    print(f' client_host: {task_data["client_host"]} ({task_data["client_id"]})')
+    print(f'     attempt: {task_data["attempt"]}')
+    print(f'     retried: {task_data["retried"]}')
+    print(f'     outpath: {task_data["outpath"]}')
+    print(f'     errpath: {task_data["errpath"]}')
+    print(f' previous_id: {task_data["previous_id"]}')
+    print(f'     next_id: {task_data["next_id"]}')
```

