# Comparing `tmp/cijoe-pkg-linux-0.9.6.tar.gz` & `tmp/cijoe-pkg-linux-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cijoe-pkg-linux-0.9.6.tar", last modified: Tue Mar 21 15:50:37 2023, max compression
+gzip compressed data, was "cijoe-pkg-linux-0.9.7.tar", last modified: Wed Apr 12 23:38:15 2023, max compression
```

## Comparing `cijoe-pkg-linux-0.9.6.tar` & `cijoe-pkg-linux-0.9.7.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.791339 cijoe-pkg-linux-0.9.6/src/cijoe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/src/cijoe/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/src/cijoe/linux/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/kmemleak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/null_blk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/src/cijoe/linux/selftest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/selftest/test_kmemleak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/selftest/test_null_blk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/src/cijoe/linux/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/build_kdebs.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/null_blk.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-21 15:50:29.000000 cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/transfer_and_install_kdebs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:50:37.795338 cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-21 15:50:37.000000 cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-21 15:50:37.000000 cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:50:37.000000 cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:50:37.000000 cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-21 15:50:37.000000 cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-21 15:50:37.000000 cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.919793 cijoe-pkg-linux-0.9.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.919793 cijoe-pkg-linux-0.9.7/src/cijoe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/configs/default-config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/kmemleak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/null_blk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/build_kdebs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/null_blk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/transfer_and_install_kdebs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_kmemleak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_null_blk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/example-worklets.workflow
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 23:38:07.000000 cijoe-pkg-linux-0.9.7/src/cijoe/linux/workflows/example.workflow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:38:15.923793 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 23:38:15.000000 cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/top_level.txt
```

### Comparing `cijoe-pkg-linux-0.9.6/LICENSE` & `cijoe-pkg-linux-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.6/PKG-INFO` & `cijoe-pkg-linux-0.9.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-linux
-Version: 0.9.6
-Summary: UNKNOWN
-Home-page: https://github.com/refenv/cijoe-pkg-linux/
+Version: 0.9.7
+Summary: A loosely coupled approach to systems development and testing
+Home-page: UNKNOWN
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
-License: BSD
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
+License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `cijoe-pkg-linux-0.9.6/README.rst` & `cijoe-pkg-linux-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/kmemleak.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/kmemleak.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/null_blk.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/null_blk.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/selftest/test_kmemleak.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_kmemleak.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/selftest/test_null_blk.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/selftest/test_null_blk.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/build_kdebs.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/build_kdebs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 -----------------
 
 with.localversion
 """
 from pathlib import Path
 
 
-def worklet_entry(args, cijoe, step):
+def main(args, cijoe, step):
     """Configure, build and collect the build-artifacts"""
 
     repos = Path(cijoe.config.options["linux"]["repository"]["path"]).resolve()
     err, _ = cijoe.run(f"[ -d {repos} ]")
     if err:
         return err
```

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/null_blk.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/null_blk.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ------------------
 """
 import errno
 
 import cijoe.linux.null_blk as null_blk
 
 
-def worklet_entry(args, cijoe, step):
+def main(args, cijoe, step):
     """Insert or remove the null_blk"""
 
     do = step.get("with", {"do": "insert"}).get("do", "insert")
     if do == "insert":
         err, _ = null_blk.insert(cijoe)
     elif do == "remove":
         err, _ = null_blk.remove(cijoe)
```

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/sysinfo.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/sysinfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Collects a bunch of information about the system kernel and hardware.
 
 Retargetable: True
 ------------------
 """
 
 
-def worklet_entry(args, cijoe, step):
+def main(args, cijoe, step):
     """Collect Linux system information"""
 
     commands = [
         "hostname",
         "lsb_release --all || cat /etc/os-release",
         "uname -a",
         "cat /boot/config-$(uname -r)",
```

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe/linux/worklets/transfer_and_install_kdebs.py` & `cijoe-pkg-linux-0.9.7/src/cijoe/linux/scripts/transfer_and_install_kdebs.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Transfer from local to remote, the config.transport.ssh determines the remote.
 """
 import errno
 import logging as log
 from pathlib import Path
 
 
-def worklet_entry(args, cijoe, step):
+def main(args, cijoe, step):
 
     deb_root = step.get("with", {}).get("local_kdebs_dir", None)
     if not deb_root:
         return errno.EINVAL
 
     deb_root = Path(deb_root)
     deb_root = (
```

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/PKG-INFO` & `cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-linux
-Version: 0.9.6
-Summary: UNKNOWN
-Home-page: https://github.com/refenv/cijoe-pkg-linux/
+Version: 0.9.7
+Summary: A loosely coupled approach to systems development and testing
+Home-page: UNKNOWN
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
-License: BSD
+Maintainer: Simon A. F. Lund
+Maintainer-email: os@safl.dk
+License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `cijoe-pkg-linux-0.9.6/src/cijoe_pkg_linux.egg-info/SOURCES.txt` & `cijoe-pkg-linux-0.9.7/src/cijoe_pkg_linux.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 LICENSE
 README.rst
 pyproject.toml
+setup.cfg
 setup.py
 src/cijoe/linux/__init__.py
 src/cijoe/linux/kmemleak.py
 src/cijoe/linux/null_blk.py
 src/cijoe/linux/configs/__init__.py
+src/cijoe/linux/configs/default-config.toml
+src/cijoe/linux/scripts/__init__.py
+src/cijoe/linux/scripts/build_kdebs.py
+src/cijoe/linux/scripts/null_blk.py
+src/cijoe/linux/scripts/sysinfo.py
+src/cijoe/linux/scripts/transfer_and_install_kdebs.py
 src/cijoe/linux/selftest/__init__.py
 src/cijoe/linux/selftest/test_kmemleak.py
 src/cijoe/linux/selftest/test_null_blk.py
 src/cijoe/linux/workflows/__init__.py
-src/cijoe/linux/worklets/__init__.py
-src/cijoe/linux/worklets/build_kdebs.py
-src/cijoe/linux/worklets/null_blk.py
-src/cijoe/linux/worklets/sysinfo.py
-src/cijoe/linux/worklets/transfer_and_install_kdebs.py
+src/cijoe/linux/workflows/example-worklets.workflow
+src/cijoe/linux/workflows/example.workflow
 src/cijoe_pkg_linux.egg-info/PKG-INFO
 src/cijoe_pkg_linux.egg-info/SOURCES.txt
 src/cijoe_pkg_linux.egg-info/dependency_links.txt
 src/cijoe_pkg_linux.egg-info/not-zip-safe
 src/cijoe_pkg_linux.egg-info/requires.txt
 src/cijoe_pkg_linux.egg-info/top_level.txt
```

