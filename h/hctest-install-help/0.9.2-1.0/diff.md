# Comparing `tmp/hctest_install_help-0.9.2.tar.gz` & `tmp/hctest_install_help-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hctest_install_help-0.9.2.tar", last modified: Thu Apr 13 07:44:47 2023, max compression
+gzip compressed data, was "dist/hctest_install_help-1.0.tar", last modified: Thu Apr 13 09:13:42 2023, max compression
```

## Comparing `hctest_install_help-0.9.2.tar` & `hctest_install_help-1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.995027 hctest_install_help-0.9.2/
--rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-13 07:44:47.994572 hctest_install_help-0.9.2/PKG-INFO
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.981506 hctest_install_help-0.9.2/hctest_install_help/
--rw-r--r--   0 mrding     (501) staff       (20)      109 2023-04-01 06:47:13.000000 hctest_install_help-0.9.2/hctest_install_help/__init__.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.987051 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/
--rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/__init__.py
--rwxr--r--   0 mrding     (501) staff       (20)     2098 2023-04-13 06:40:51.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/adb_env.py
--rw-r--r--   0 mrding     (501) staff       (20)      660 2023-04-13 07:37:18.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/check_env.py
--rwxr--r--   0 mrding     (501) staff       (20)      755 2023-04-13 07:38:47.000000 hctest_install_help-0.9.2/hctest_install_help/install_adb_env/run.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.989869 hctest_install_help-0.9.2/hctest_install_help/install_java_env/
--rw-r--r--   0 mrding     (501) staff       (20)       83 2023-04-03 11:03:37.000000 hctest_install_help-0.9.2/hctest_install_help/install_java_env/__init__.py
--rw-r--r--   0 mrding     (501) staff       (20)     1420 2023-04-13 06:40:51.000000 hctest_install_help-0.9.2/hctest_install_help/install_java_env/java_env.py
--rwxr--r--   0 mrding     (501) staff       (20)      505 2023-04-13 07:39:44.000000 hctest_install_help-0.9.2/hctest_install_help/install_java_env/run.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.993449 hctest_install_help-0.9.2/hctest_install_help/package/
--rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-0.9.2/hctest_install_help/package/__init__.py
--rwxr--r--   0 mrding     (501) staff       (20)      399 2023-03-31 07:59:08.000000 hctest_install_help-0.9.2/hctest_install_help/package/mac_env.py
--rwxr--r--   0 mrding     (501) staff       (20)      786 2023-04-12 08:32:32.000000 hctest_install_help-0.9.2/hctest_install_help/package/unzip.py
--rwxr--r--   0 mrding     (501) staff       (20)     2079 2023-04-13 07:37:18.000000 hctest_install_help-0.9.2/hctest_install_help/package/windows_env.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 07:44:47.983727 hctest_install_help-0.9.2/hctest_install_help.egg-info/
--rw-r--r--   0 mrding     (501) staff       (20)      413 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/PKG-INFO
--rw-r--r--   0 mrding     (501) staff       (20)      700 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/SOURCES.txt
--rw-r--r--   0 mrding     (501) staff       (20)        1 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/dependency_links.txt
--rw-r--r--   0 mrding     (501) staff       (20)       20 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/hctest_install_help.egg-info/top_level.txt
--rw-r--r--   0 mrding     (501) staff       (20)       38 2023-04-13 07:44:47.995179 hctest_install_help-0.9.2/setup.cfg
--rw-r--r--   0 mrding     (501) staff       (20)      698 2023-04-13 07:44:47.000000 hctest_install_help-0.9.2/setup.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 09:13:42.498826 hctest_install_help-1.0/
+-rw-r--r--   0 mrding     (501) staff       (20)      411 2023-04-13 09:13:42.498437 hctest_install_help-1.0/PKG-INFO
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 09:13:42.490420 hctest_install_help-1.0/hctest_install_help/
+-rw-r--r--   0 mrding     (501) staff       (20)      109 2023-04-01 06:47:13.000000 hctest_install_help-1.0/hctest_install_help/__init__.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 09:13:42.494024 hctest_install_help-1.0/hctest_install_help/install_adb_env/
+-rw-r--r--   0 mrding     (501) staff       (20)       83 2023-04-13 09:13:34.000000 hctest_install_help-1.0/hctest_install_help/install_adb_env/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     2098 2023-04-13 09:13:34.000000 hctest_install_help-1.0/hctest_install_help/install_adb_env/adb_env.py
+-rw-r--r--   0 mrding     (501) staff       (20)      660 2023-04-13 09:13:34.000000 hctest_install_help-1.0/hctest_install_help/install_adb_env/check_env.py
+-rw-r--r--   0 mrding     (501) staff       (20)      762 2023-04-13 09:13:34.000000 hctest_install_help-1.0/hctest_install_help/install_adb_env/run.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 09:13:42.495398 hctest_install_help-1.0/hctest_install_help/install_java_env/
+-rw-r--r--   0 mrding     (501) staff       (20)       83 2023-04-13 09:13:34.000000 hctest_install_help-1.0/hctest_install_help/install_java_env/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     1420 2023-04-13 09:13:34.000000 hctest_install_help-1.0/hctest_install_help/install_java_env/java_env.py
+-rw-r--r--   0 mrding     (501) staff       (20)      501 2023-04-13 09:13:34.000000 hctest_install_help-1.0/hctest_install_help/install_java_env/run.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 09:13:42.497672 hctest_install_help-1.0/hctest_install_help/package/
+-rwxr--r--   0 mrding     (501) staff       (20)       83 2023-03-31 07:59:08.000000 hctest_install_help-1.0/hctest_install_help/package/__init__.py
+-rwxr--r--   0 mrding     (501) staff       (20)      399 2023-03-31 07:59:08.000000 hctest_install_help-1.0/hctest_install_help/package/mac_env.py
+-rwxr--r--   0 mrding     (501) staff       (20)      786 2023-04-12 08:32:32.000000 hctest_install_help-1.0/hctest_install_help/package/unzip.py
+-rwxr--r--   0 mrding     (501) staff       (20)     2079 2023-04-13 07:37:18.000000 hctest_install_help-1.0/hctest_install_help/package/windows_env.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-04-13 09:13:42.492451 hctest_install_help-1.0/hctest_install_help.egg-info/
+-rw-r--r--   0 mrding     (501) staff       (20)      411 2023-04-13 09:13:42.000000 hctest_install_help-1.0/hctest_install_help.egg-info/PKG-INFO
+-rw-r--r--   0 mrding     (501) staff       (20)      700 2023-04-13 09:13:42.000000 hctest_install_help-1.0/hctest_install_help.egg-info/SOURCES.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        1 2023-04-13 09:13:42.000000 hctest_install_help-1.0/hctest_install_help.egg-info/dependency_links.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       20 2023-04-13 09:13:42.000000 hctest_install_help-1.0/hctest_install_help.egg-info/top_level.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       38 2023-04-13 09:13:42.498993 hctest_install_help-1.0/setup.cfg
+-rw-r--r--   0 mrding     (501) staff       (20)      696 2023-04-13 09:13:25.000000 hctest_install_help-1.0/setup.py
```

### Comparing `hctest_install_help-0.9.2/hctest_install_help/install_adb_env/adb_env.py` & `hctest_install_help-1.0/hctest_install_help/install_adb_env/adb_env.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9.2/hctest_install_help/install_adb_env/check_env.py` & `hctest_install_help-1.0/hctest_install_help/install_adb_env/check_env.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9.2/hctest_install_help/install_adb_env/run.py` & `hctest_install_help-1.0/hctest_install_help/install_adb_env/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 
 def start_install_help():
     if sys.platform == "win32":
         from hctest_install_help.package.windows_env import run_cmd_as_admin
         check_file = str(__file__).replace(f"run.py", "check_env.py")
-        os.system(f'{sys.executable} {check_file}')
+        run_cmd_as_admin(f'{sys.executable} {check_file}')
 
         env_file = str(__file__).replace(f"run.py", "adb_env.py")
         run_cmd_as_admin(f"{sys.executable} {env_file}")
 
     else:
         check_file = str(__file__).replace(f"run.py", "check_env.py")
         os.system(f'{sys.executable} {check_file}')
```

### Comparing `hctest_install_help-0.9.2/hctest_install_help/install_java_env/java_env.py` & `hctest_install_help-1.0/hctest_install_help/install_java_env/java_env.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9.2/hctest_install_help/package/unzip.py` & `hctest_install_help-1.0/hctest_install_help/package/unzip.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9.2/hctest_install_help/package/windows_env.py` & `hctest_install_help-1.0/hctest_install_help/package/windows_env.py`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9.2/hctest_install_help.egg-info/SOURCES.txt` & `hctest_install_help-1.0/hctest_install_help.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hctest_install_help-0.9.2/setup.py` & `hctest_install_help-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 """
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload dist/*
 """
 setup(
     name="hctest_install_help",
-    version="0.9.2",
+    version="1.0",
     description="辅助帮你下载安装文件",
     author="cf",
     author_email="dingjun_baby@yeah.net",
     url="https://github.com/pypa/sampleproject",
     packages=find_packages(),
     # install_requires=[
     #     'requests',
```

