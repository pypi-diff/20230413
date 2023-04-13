# Comparing `tmp/test_pipinstall_whp-0.0.2.tar.gz` & `tmp/test_pipinstall_whp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/test_pipinstall_whp-0.0.2.tar", last modified: Thu Apr 13 08:27:34 2023, max compression
+gzip compressed data, was "dist/test_pipinstall_whp-0.0.3.tar", last modified: Thu Apr 13 08:39:18 2023, max compression
```

## Comparing `test_pipinstall_whp-0.0.2.tar` & `test_pipinstall_whp-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:27:34.000000 test_pipinstall_whp-0.0.2/
-drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:27:34.000000 test_pipinstall_whp-0.0.2/test_pipinstall_whp.egg-info/
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        1 2023-04-13 08:27:33.000000 test_pipinstall_whp-0.0.2/test_pipinstall_whp.egg-info/top_level.txt
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:27:33.000000 test_pipinstall_whp-0.0.2/test_pipinstall_whp.egg-info/PKG-INFO
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      190 2023-04-13 08:27:33.000000 test_pipinstall_whp-0.0.2/test_pipinstall_whp.egg-info/SOURCES.txt
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        1 2023-04-13 08:27:33.000000 test_pipinstall_whp-0.0.2/test_pipinstall_whp.egg-info/dependency_links.txt
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       38 2023-04-13 08:27:34.000000 test_pipinstall_whp-0.0.2/setup.cfg
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:27:34.000000 test_pipinstall_whp-0.0.2/PKG-INFO
--rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)      321 2023-04-13 08:26:51.000000 test_pipinstall_whp-0.0.2/setup.py
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       39 2023-04-13 08:22:24.000000 test_pipinstall_whp-0.0.2/README.md
+drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/PKG-INFO
+-rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)      409 2023-04-13 08:39:04.000000 test_pipinstall_whp-0.0.3/setup.py
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       39 2023-04-13 08:22:24.000000 test_pipinstall_whp-0.0.3/README.md
+drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp.egg-info/
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      282 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp.egg-info/PKG-INFO
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       20 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp.egg-info/top_level.txt
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        1 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp.egg-info/dependency_links.txt
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       38 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/setup.cfg
+drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:39:18.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp/
+-rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)       68 2023-04-13 03:24:36.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp/test_1.py
+-rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)       68 2023-04-13 03:24:56.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp/test_2.py
+-rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)       62 2023-04-13 03:20:48.000000 test_pipinstall_whp-0.0.3/test_pipinstall_whp/__init__.py
```

