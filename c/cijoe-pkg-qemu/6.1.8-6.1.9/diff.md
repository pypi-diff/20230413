# Comparing `tmp/cijoe-pkg-qemu-6.1.8.tar.gz` & `tmp/cijoe-pkg-qemu-6.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cijoe-pkg-qemu-6.1.8.tar", last modified: Mon Oct  3 12:02:37 2022, max compression
+gzip compressed data, was "cijoe-pkg-qemu-6.1.9.tar", last modified: Tue Oct  4 08:52:45 2022, max compression
```

## Comparing `cijoe-pkg-qemu-6.1.8.tar` & `cijoe-pkg-qemu-6.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      857 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.703423 cijoe-pkg-qemu-6.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.703423 cijoe-pkg-qemu-6.1.8/src/cijoe/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/auxilary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/auxilary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/selftest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/selftest/test_nop.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/build_x86.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/guest_bootimg.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/guest_cloudinit.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/guest_kill.py
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/guest_start.py
--rw-r--r--   0 runner    (1001) docker     (121)     3984 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/guest_start_nvme.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/install.py
--rw-r--r--   0 runner    (1001) docker     (121)     8930 2022-10-03 12:02:28.000000 cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 12:02:37.707423 cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-10-03 12:02:37.000000 cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-03 12:02:37.000000 cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 12:02:37.000000 cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 12:02:37.000000 cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-03 12:02:37.000000 cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-03 12:02:37.000000 cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.690365 cijoe-pkg-qemu-6.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-10-04 08:52:45.690365 cijoe-pkg-qemu-6.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      857 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-04 08:52:45.690365 cijoe-pkg-qemu-6.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.682365 cijoe-pkg-qemu-6.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.682365 cijoe-pkg-qemu-6.1.9/src/cijoe/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.686365 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.686365 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/auxilary/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/auxilary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.686365 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/configs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.686365 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/selftest/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/selftest/test_nop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.686365 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.690365 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/build_x86.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/guest_bootimg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/guest_cloudinit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/guest_kill.py
+-rw-r--r--   0 runner    (1001) docker     (121)      531 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/guest_start.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4038 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/guest_start_nvme.py
+-rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/install.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8930 2022-10-04 08:52:33.000000 cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 08:52:45.690365 cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-10-04 08:52:45.000000 cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-04 08:52:45.000000 cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 08:52:45.000000 cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 08:52:45.000000 cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-10-04 08:52:45.000000 cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-04 08:52:45.000000 cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/top_level.txt
```

### Comparing `cijoe-pkg-qemu-6.1.8/LICENSE` & `cijoe-pkg-qemu-6.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-qemu-6.1.8/PKG-INFO` & `cijoe-pkg-qemu-6.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-qemu
-Version: 6.1.8
+Version: 6.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/refenv/cijoe-pkg-qemu/
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cijoe-pkg-qemu-6.1.8/README.rst` & `cijoe-pkg-qemu-6.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-qemu-6.1.8/setup.py` & `cijoe-pkg-qemu-6.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 a specific version of the kernel, then the version number tracks the main cijoe package
 instead.
 """
 from setuptools import find_namespace_packages, setup
 
 setup(
     name="cijoe-pkg-qemu",
-    version="6.1.8",
+    version="6.1.9",
     author="Simon A. F. Lund",
     author_email="os@safl.dk",
     url="https://github.com/refenv/cijoe-pkg-qemu/",
     license="BSD",
     install_requires=[
         "cijoe>=0.9.1",
         "psutil",
```

### Comparing `cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/build_x86.py` & `cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/build_x86.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/guest_start.py` & `cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/guest_start.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/worklets/guest_start_nvme.py` & `cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/worklets/guest_start_nvme.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,23 @@
     drive_size = "8G"
 
     controller1 = {
         "id": "nvme0",
         "serial": "deadbeef",
         "bus": "pcie_downstream_port1",
         "mdts": 7,
+        "ioeventfd": "on",
     }
 
     controller2 = {
         "id": "nvme1",
         "serial": "adcdbeef",
         "bus": "pcie_downstream_port2",
         "mdts": 7,
+        "ioeventfd": "on",
     }
 
     drive1 = {
         "id": "nvme0n1",
         "file": str(nvme_img_root / "nvme0n1.img"),
         "format": "raw",
         "if": "none",
```

### Comparing `cijoe-pkg-qemu-6.1.8/src/cijoe/qemu/wrapper.py` & `cijoe-pkg-qemu-6.1.9/src/cijoe/qemu/wrapper.py`

 * *Files identical despite different names*

### Comparing `cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/PKG-INFO` & `cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cijoe-pkg-qemu
-Version: 6.1.8
+Version: 6.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/refenv/cijoe-pkg-qemu/
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cijoe-pkg-qemu-6.1.8/src/cijoe_pkg_qemu.egg-info/SOURCES.txt` & `cijoe-pkg-qemu-6.1.9/src/cijoe_pkg_qemu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

