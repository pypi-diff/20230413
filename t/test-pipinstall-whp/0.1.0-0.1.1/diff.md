# Comparing `tmp/test_pipinstall_whp-0.1.0.tar.gz` & `tmp/test_pipinstall_whp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/test_pipinstall_whp-0.1.0.tar", last modified: Thu Apr 13 08:48:08 2023, max compression
+gzip compressed data, was "dist/test_pipinstall_whp-0.1.1.tar", last modified: Thu Apr 13 08:56:12 2023, max compression
```

## Comparing `test_pipinstall_whp-0.1.0.tar` & `test_pipinstall_whp-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:48:08.000000 test_pipinstall_whp-0.1.0/
-drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:48:08.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp/
--rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:47:17.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp/__init__.py
--rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)       68 2023-04-13 03:24:56.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp/test_2.py
--rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)       68 2023-04-13 03:24:36.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp/test_1.py
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       39 2023-04-13 08:22:24.000000 test_pipinstall_whp-0.1.0/README.md
-drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:48:08.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp.egg-info/
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:48:07.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp.egg-info/PKG-INFO
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       20 2023-04-13 08:48:07.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp.egg-info/top_level.txt
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      282 2023-04-13 08:48:08.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp.egg-info/SOURCES.txt
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        1 2023-04-13 08:48:07.000000 test_pipinstall_whp-0.1.0/test_pipinstall_whp.egg-info/dependency_links.txt
--rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)      409 2023-04-13 08:48:03.000000 test_pipinstall_whp-0.1.0/setup.py
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       38 2023-04-13 08:48:08.000000 test_pipinstall_whp-0.1.0/setup.cfg
--rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:48:08.000000 test_pipinstall_whp-0.1.0/PKG-INFO
+drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       39 2023-04-13 08:22:24.000000 test_pipinstall_whp-0.1.1/README.md
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/PKG-INFO
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)       38 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/setup.cfg
+-rwxr-xr-x   0 hpwu       (872) sh_sdk     (611)      377 2023-04-13 08:55:48.000000 test_pipinstall_whp-0.1.1/setup.py
+drwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        0 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/test_pipinstall_whp.egg-info/
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      190 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/test_pipinstall_whp.egg-info/SOURCES.txt
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)      264 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/test_pipinstall_whp.egg-info/PKG-INFO
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        1 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/test_pipinstall_whp.egg-info/top_level.txt
+-rwxrwxrwx   0 hpwu       (872) sh_sdk     (611)        1 2023-04-13 08:56:12.000000 test_pipinstall_whp-0.1.1/test_pipinstall_whp.egg-info/dependency_links.txt
```

