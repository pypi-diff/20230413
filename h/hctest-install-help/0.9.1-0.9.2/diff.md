# Comparing `tmp/hctest_install_help-0.9.1.tar.gz` & `tmp/hctest_install_help-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hctest_install_help-0.9.1.tar", last modified: Tue Apr 11 14:35:38 2023, max compression
+gzip compressed data, was "dist/hctest_install_help-0.9.2.tar", last modified: Thu Apr 13 07:44:47 2023, max compression
```

## Comparing `hctest_install_help-0.9.1.tar` & `hctest_install_help-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.650975 hctest_install_help-0.9.1/
--rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-11 14:35:38.650570 hctest_install_help-0.9.1/PKG-INFO
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.640054 hctest_install_help-0.9.1/hctest_install_help/
--rw-r--r--   0 mrding     (501) staff       (20)      109 2023-04-01 06:47:13.000000 hctest_install_help-0.9.1/hctest_install_help/__init__.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.644767 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/
--rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/__init__.py
--rwxr--r--   0 mrding     (501) staff       (20)     2098 2023-04-11 14:29:26.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/adb_env.py
--rw-r--r--   0 mrding     (501) staff       (20)      612 2023-04-01 07:06:08.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/check_env.py
--rwxr--r--   0 mrding     (501) staff       (20)      684 2023-04-01 05:46:48.000000 hctest_install_help-0.9.1/hctest_install_help/install_adb_env/run.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.646312 hctest_install_help-0.9.1/hctest_install_help/install_java_env/
--rw-r--r--   0 mrding     (501) staff       (20)       83 2023-04-03 11:03:37.000000 hctest_install_help-0.9.1/hctest_install_help/install_java_env/__init__.py
--rw-r--r--   0 mrding     (501) staff       (20)     1361 2023-04-11 14:33:30.000000 hctest_install_help-0.9.1/hctest_install_help/install_java_env/java_env.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.649686 hctest_install_help-0.9.1/hctest_install_help/package/
--rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.1/hctest_install_help/package/__init__.py
--rwxr--r--   0 mrding     (501) staff       (20)      399 2023-03-31 07:59:08.000000 hctest_install_help-0.9.1/hctest_install_help/package/mac_env.py
--rwxr--r--   0 mrding     (501) staff       (20)      610 2023-04-01 11:49:32.000000 hctest_install_help-0.9.1/hctest_install_help/package/unzip.py
--rwxr--r--   0 mrding     (501) staff       (20)     1826 2023-04-01 06:47:13.000000 hctest_install_help-0.9.1/hctest_install_help/package/windows_env.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-11 14:35:38.641933 hctest_install_help-0.9.1/hctest_install_help.egg-info/
--rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/PKG-INFO
--rw-r--r--   0 mrding     (501) staff       (20)      656 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/SOURCES.txt
--rw-r--r--   0 mrding     (501) staff       (20)        1 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/dependency_links.txt
--rw-r--r--   0 mrding     (501) staff       (20)       20 2023-04-11 14:35:38.000000 hctest_install_help-0.9.1/hctest_install_help.egg-info/top_level.txt
--rw-r--r--   0 mrding     (501) staff       (20)       38 2023-04-11 14:35:38.651114 hctest_install_help-0.9.1/setup.cfg
--rw-r--r--   0 mrding     (501) staff       (20)      625 2023-04-11 14:35:07.000000 hctest_install_help-0.9.1/setup.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.995027 hctest_install_help-0.9.2/
+-rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-13 07:44:47.994572 hctest_install_help-0.9.2/PKG-INFO
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.981506 hctest_install_help-0.9.2/hctest_install_help/
+-rw-r--r--   0 mrding     (501) staff       (20)      109 2023-04-01 06:47:13.000000 hctest_install_help-0.9.2/hctest_install_help/__init__.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.987051 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/
+-rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/__init__.py
+-rwxr--r--   0 mrding     (501) staff       (20)     2098 2023-04-13 06:40:51.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/adb_env.py
+-rw-r--r--   0 mrding     (501) staff       (20)      660 2023-04-13 07:37:18.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/check_env.py
+-rwxr--r--   0 mrding     (501) staff       (20)      755 2023-04-13 07:38:47.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/run.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.989869 hctest_install_help-0.9.2/hctest_install_help/install_java_env/
+-rw-r--r--   0 mrding     (501) staff       (20)       83 2023-04-03 11:03:37.000000 hctest_install_help-0.9.2/hctest_install_help/install_java_env/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     1420 2023-04-13 06:40:51.000000 hctest_install_help-0.9.2/hctest_install_help/install_java_env/java_env.py
+-rwxr--r--   0 mrding     (501) staff       (20)      505 2023-04-13 07:39:44.000000 hctest_install_help-0.9.2/hctest_install_help/install_java_env/run.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.993449 hctest_install_help-0.9.2/hctest_install_help/package/
+-rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.2/hctest_install_help/package/__init__.py
+-rwxr--r--   0 mrding     (501) staff       (20)      399 2023-03-31 07:59:08.000000 hctest_install_help-0.9.2/hctest_install_help/package/mac_env.py
+-rwxr--r--   0 mrding     (501) staff       (20)      786 2023-04-12 08:32:32.000000 hctest_install_help-0.9.2/hctest_install_help/package/unzip.py
+-rwxr--r--   0 mrding     (501) staff       (20)     2079 2023-04-13 07:37:18.000000 hctest_install_help-0.9.2/hctest_install_help/package/windows_env.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.983727 hctest_install_help-0.9.2/hctest_install_help.egg-info/
+-rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/PKG-INFO
+-rw-r--r--   0 mrding     (501) staff       (20)      700 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/SOURCES.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        1 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/dependency_links.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       20 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/top_level.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       38 2023-04-13 07:44:47.995179 hctest_install_help-0.9.2/setup.cfg
+-rw-r--r--   0 mrding     (501) staff       (20)      698 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/setup.py
```

### Comparing `hctest_install_help-0.9.1/hctest_install_help/install_adb_env/adb_env.py` & `hctest_install_help-0.9.2/hctest_install_help/install_adb_env/adb_env.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9.1/hctest_install_help/install_java_env/java_env.py` & `hctest_install_help-0.9.2/hctest_install_help/install_java_env/java_env.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,18 +18,25 @@
 
 java_execute_name = "java.exe" if sys.platform == "win32" else "java"
 for dir_path, dir_names, filenames in os.walk(target_path):
     for filename in filenames:
         if filename == java_execute_name:
             jdk_path = os.path.join(dir_path)
             break
+
 if sys.platform == "win32":
     from hctest_install_help.package.windows_env import *
+
+    JAVA_HOME_PATH = jdk_path.replace(r"\bin", "")
+
     import subprocess
-    add_system_env_path(r"%JAVA_HOME%{}".format(jdk_path.replace(target_path, '')))
-    add_system_env(JAVA_HOME_NAME, target_path)
+
+    add_system_env(JAVA_HOME_NAME, JAVA_HOME_PATH)
+    add_system_env_path(r"%JAVA_HOME%{}".format(r"\bin"))
     subprocess.call(["attrib", "+h", target_path])
 
 else:
     from hctest_install_help.package.mac_env import *
-    add_system_env_path(r"$JAVA_HOME{}".format(jdk_path.replace(target_path, '')))
-    add_system_env(JAVA_HOME_NAME, target_path)
+
+    JAVA_HOME_PATH = jdk_path.replace("/bin", "")
+    add_system_env(JAVA_HOME_NAME, JAVA_HOME_PATH)
+    add_system_env_path(r"$JAVA_HOME{}".format("/bin"))
```

### Comparing `hctest_install_help-0.9.1/hctest_install_help/package/unzip.py` & `hctest_install_help-0.9.2/hctest_install_help/package/unzip.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # -*- coding: utf-8 -*-
 # author: 华测-长风老师
 # file name：unzip.py
 
 import zipfile
 import os
 import sys
+import tarfile
 
 
 def get_home_path():
     env_vars = os.environ
     home_path = "USERPROFILE" if sys.platform == "win32" else "HOME"
     return env_vars[home_path]
 
 
 def unzip(source_path, target_path):
-    with zipfile.ZipFile(source_path, 'r') as zip_ref:
-        zip_ref.extractall(target_path)
+    if source_path.endswith("zip"):
+        with zipfile.ZipFile(source_path, 'r') as zip_ref:
+            zip_ref.extractall(target_path)
+    else:
+        with tarfile.open(source_path, "r:gz") as tar:
+            tar.extractall(path=target_path)
+
     for root, dirs, files in os.walk(target_path):
         for file in files:
             os.chmod(os.path.join(root, file), 0o755)
 
 
 if __name__ == '__main__':
     print(get_home_path())
```

### Comparing `hctest_install_help-0.9.1/hctest_install_help/package/windows_env.py` & `hctest_install_help-0.9.2/hctest_install_help/package/windows_env.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # -*- coding: utf-8 -*-
 # author: 华测-长风老师
 # file name：windows_env.py
 
 
 import winreg
+import ctypes
+
+
+def run_cmd_as_admin(cmd):
+    if not ctypes.windll.shell32.IsUserAnAdmin():
+        ctypes.windll.shell32.ShellExecuteW(None, "runas", "cmd.exe", "/k {}".format(cmd), None, 1)
+    else:
+        import os
+        os.system(cmd)
 
 
 def add_system_env_path(path_):
     try:
 
         key = winreg.OpenKey(winreg.HKEY_LOCAL_MACHINE, r'SYSTEM\CurrentControlSet\Control\Session Manager\Environment',
                              0, winreg.KEY_ALL_ACCESS)
```

### Comparing `hctest_install_help-0.9.1/hctest_install_help.egg-info/SOURCES.txt` & `hctest_install_help-0.9.2/hctest_install_help.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 hctest_install_help.egg-info/top_level.txt
 hctest_install_help/install_adb_env/__init__.py
 hctest_install_help/install_adb_env/adb_env.py
 hctest_install_help/install_adb_env/check_env.py
 hctest_install_help/install_adb_env/run.py
 hctest_install_help/install_java_env/__init__.py
 hctest_install_help/install_java_env/java_env.py
+hctest_install_help/install_java_env/run.py
 hctest_install_help/package/__init__.py
 hctest_install_help/package/mac_env.py
 hctest_install_help/package/unzip.py
 hctest_install_help/package/windows_env.py
```

### Comparing `hctest_install_help-0.9.1/setup.py` & `hctest_install_help-0.9.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 # author: 华测-长风老师
 # file name：setup.py
 from setuptools import setup, find_packages
-
+"""
+python3 setup.py sdist bdist_wheel
+python3 -m twine upload dist/*
+"""
 setup(
     name="hctest_install_help",
-    version="0.9.1",
+    version="0.9.2",
     description="辅助帮你下载安装文件",
     author="cf",
     author_email="dingjun_baby@yeah.net",
     url="https://github.com/pypa/sampleproject",
     packages=find_packages(),
     # install_requires=[
     #     'requests',
```

