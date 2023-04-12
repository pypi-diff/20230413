# Comparing `tmp/reminder-detector-1.0.5.tar.gz` & `tmp/reminder-detector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reminder-detector-1.0.5.tar", last modified: Sat Feb 25 21:57:59 2023, max compression
+gzip compressed data, was "reminder-detector-1.1.0.tar", last modified: Wed Apr 12 22:22:13 2023, max compression
```

## Comparing `reminder-detector-1.0.5.tar` & `reminder-detector-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:57:59.340338 reminder-detector-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:57:59.336338 reminder-detector-1.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:57:59.340338 reminder-detector-1.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    45129 2023-02-25 21:57:59.340338 reminder-detector-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:57:59.340338 reminder-detector-1.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    33871 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 21:57:59.340338 reminder-detector-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:57:59.336338 reminder-detector-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:57:59.340338 reminder-detector-1.0.5/src/reminder/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/src/reminder/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/src/reminder/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/src/reminder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-02-25 21:57:51.000000 reminder-detector-1.0.5/src/reminder/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 21:57:59.340338 reminder-detector-1.0.5/src/reminder_detector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45129 2023-02-25 21:57:59.000000 reminder-detector-1.0.5/src/reminder_detector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-25 21:57:59.000000 reminder-detector-1.0.5/src/reminder_detector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 21:57:59.000000 reminder-detector-1.0.5/src/reminder_detector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-25 21:57:59.000000 reminder-detector-1.0.5/src/reminder_detector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-25 21:57:59.000000 reminder-detector-1.0.5/src/reminder_detector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-25 21:57:59.000000 reminder-detector-1.0.5/src/reminder_detector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:22:13.028966 reminder-detector-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:22:13.024966 reminder-detector-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:22:13.024966 reminder-detector-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    45129 2023-04-12 22:22:13.028966 reminder-detector-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:22:13.028966 reminder-detector-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    33871 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 22:22:13.028966 reminder-detector-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:22:13.024966 reminder-detector-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:22:13.028966 reminder-detector-1.1.0/src/reminder/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/src/reminder/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/src/reminder/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/src/reminder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 22:22:02.000000 reminder-detector-1.1.0/src/reminder/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 22:22:13.028966 reminder-detector-1.1.0/src/reminder_detector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45129 2023-04-12 22:22:13.000000 reminder-detector-1.1.0/src/reminder_detector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-12 22:22:13.000000 reminder-detector-1.1.0/src/reminder_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 22:22:13.000000 reminder-detector-1.1.0/src/reminder_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 22:22:13.000000 reminder-detector-1.1.0/src/reminder_detector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 22:22:13.000000 reminder-detector-1.1.0/src/reminder_detector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 22:22:13.000000 reminder-detector-1.1.0/src/reminder_detector.egg-info/top_level.txt
```

### Comparing `reminder-detector-1.0.5/.github/workflows/python-package.yml` & `reminder-detector-1.1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `reminder-detector-1.0.5/.gitignore` & `reminder-detector-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `reminder-detector-1.0.5/LICENSE` & `reminder-detector-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reminder-detector-1.0.5/PKG-INFO` & `reminder-detector-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reminder-detector
-Version: 1.0.5
+Version: 1.1.0
 Summary: Implementation of the packing detection heuristic from the paper "Packed PE File Detection for Malware Forensics" of Han et al.
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `reminder-detector-1.0.5/README.md` & `reminder-detector-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `reminder-detector-1.0.5/docs/logo.png` & `reminder-detector-1.1.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `reminder-detector-1.0.5/pyproject.toml` & `reminder-detector-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reminder-detector-1.0.5/src/reminder/__info__.py` & `reminder-detector-1.1.0/src/reminder/__info__.py`

 * *Files identical despite different names*

### Comparing `reminder-detector-1.0.5/src/reminder/__main__.py` & `reminder-detector-1.1.0/src/reminder/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,77 @@
-# -*- coding: UTF-8 -*-
-import logging
-from argparse import ArgumentParser, RawTextHelpFormatter
-from ast import literal_eval
-from os.path import exists
-from time import perf_counter
-
-from .__info__ import __author__, __copyright__, __license__, __reference__, __source__, __version__
-from .__init__ import REMINDer
-
-
-def valid_file(path):
-    if not exists(path):
-        raise ValueError("input file does not exist")
-    return path
-
-
-class Positive:
-    def __init__(self, *types):
-        self._types = types
-    
-    def __call__(self, string):
-        try:
-            n = literal_eval(string)
-        except ValueError:
-            raise ValueError(string)
-        if not isinstance(n, self._types) or n < 0.:
-            raise ValueError(string)
-        return self._types[0](n)
-    
-    def __repr__(self):
-        return "positive %s" % "|".join(map(lambda x: x.__name__, self._types))
-
-
-def main():
-    """ Tool's main function """
-    descr = "REMINDer {}\n\nAuthor   : {}\nCopyright: {}\nLicense  : {}\nReference: {}\nSource   : {}\n" \
-            "\nThis tool applies a custom heuristic based on the entropy of the Entry Point section to determine if" \
-            " an executable is packed or not.\n\n"
-    descr = descr.format(__version__, __author__, __copyright__, __license__, __reference__, __source__)
-    examples = "usage examples:\n- " + "\n- ".join([
-        "reminder program.exe",
-        "reminder /bin/ls --entropy-threshold 6.9",
-    ])
-    parser = ArgumentParser(description=descr, epilog=examples, formatter_class=RawTextHelpFormatter, add_help=False)
-    parser.add_argument("path", type=valid_file, help="path to the executable file")
-    opt = parser.add_argument_group("optional arguments")
-    opt.add_argument("--entropy-threshold", type=Positive(float, int),
-                     help="threshold for the entropy of the Entry Point section")
-    extra = parser.add_argument_group("extra arguments")
-    extra.add_argument("-b", "--benchmark", action="store_true",
-                       help="enable benchmarking, output in seconds (default: False)")
-    extra.add_argument("-h", "--help", action="help", help="show this help message and exit")
-    extra.add_argument("-v", "--verbose", action="store_true", help="display debug information (default: False)")
-    args = parser.parse_args()
-    logging.basicConfig()
-    args.logger = logging.getLogger("reminder")
-    args.logger.setLevel([logging.INFO, logging.DEBUG][args.verbose])
-    code = 0
-    # execute the tool
-    if args.benchmark:
-        t1 = perf_counter()
-    try:
-        r = REMINDer(**vars(args)).detect(args.path)
-        dt = str(perf_counter() - t1) if args.benchmark else ""
-        print(str(r))
-        if dt != "":
-            print(dt)
-    except Exception as e:
-        if "magic not found." in str(e):
-            e.value = "Not a valid executable file"
-        if str(e) != "no result":
-            args.logger.exception(e)
-        code = 1
-    return code
-
+# -*- coding: UTF-8 -*-
+import logging
+from argparse import ArgumentParser, RawTextHelpFormatter
+from ast import literal_eval
+from os.path import exists
+from time import perf_counter
+
+from .__info__ import __author__, __copyright__, __license__, __reference__, __source__, __version__
+from .__init__ import REMINDer
+
+
+def valid_file(path):
+    if not exists(path):
+        raise ValueError("input file does not exist")
+    return path
+
+
+class Positive:
+    def __init__(self, *types):
+        self._types = types
+    
+    def __call__(self, string):
+        try:
+            n = literal_eval(string)
+        except ValueError:
+            raise ValueError(string)
+        if not isinstance(n, self._types) or n < 0.:
+            raise ValueError(string)
+        return self._types[0](n)
+    
+    def __repr__(self):
+        return "positive %s" % "|".join(map(lambda x: x.__name__, self._types))
+
+
+def main():
+    """ Tool's main function """
+    descr = "REMINDer {}\n\nAuthor   : {}\nCopyright: {}\nLicense  : {}\nReference: {}\nSource   : {}\n" \
+            "\nThis tool applies a custom heuristic based on the entropy of the Entry Point section to determine if" \
+            " an executable is packed or not.\n\n"
+    descr = descr.format(__version__, __author__, __copyright__, __license__, __reference__, __source__)
+    examples = "usage examples:\n- " + "\n- ".join([
+        "reminder program.exe",
+        "reminder /bin/ls --entropy-threshold 6.9",
+    ])
+    parser = ArgumentParser(description=descr, epilog=examples, formatter_class=RawTextHelpFormatter, add_help=False)
+    parser.add_argument("path", type=valid_file, help="path to the executable file")
+    opt = parser.add_argument_group("optional arguments")
+    opt.add_argument("--entropy-threshold", type=Positive(float, int),
+                     help="threshold for the entropy of the Entry Point section")
+    extra = parser.add_argument_group("extra arguments")
+    extra.add_argument("-b", "--benchmark", action="store_true",
+                       help="enable benchmarking, output in seconds (default: False)")
+    extra.add_argument("-h", "--help", action="help", help="show this help message and exit")
+    extra.add_argument("-v", "--verbose", action="store_true", help="display debug information (default: False)")
+    args = parser.parse_args()
+    logging.basicConfig()
+    args.logger = logging.getLogger("reminder")
+    args.logger.setLevel([logging.INFO, logging.DEBUG][args.verbose])
+    code = 0
+    # execute the tool
+    if args.benchmark:
+        t1 = perf_counter()
+    try:
+        r = REMINDer(**vars(args)).detect(args.path)
+        dt = str(perf_counter() - t1) if args.benchmark else ""
+        if r is not None:
+            print(str(r))
+        if dt != "":
+            print(dt)
+    except Exception as e:
+        if "magic not found." in str(e):
+            e.value = "Not a valid executable file"
+        if str(e) != "no result":
+            args.logger.exception(e)
+        code = 1
+    return code
+
```

### Comparing `reminder-detector-1.0.5/src/reminder_detector.egg-info/PKG-INFO` & `reminder-detector-1.1.0/src/reminder_detector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reminder-detector
-Version: 1.0.5
+Version: 1.1.0
 Summary: Implementation of the packing detection heuristic from the paper "Packed PE File Detection for Malware Forensics" of Han et al.
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

