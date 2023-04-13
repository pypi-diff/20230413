# Comparing `tmp/pyfakefs-5.2.1.tar.gz` & `tmp/pyfakefs-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfakefs-5.2.1.tar", last modified: Tue Apr 11 14:25:34 2023, max compression
+gzip compressed data, was "pyfakefs-5.2.2.tar", last modified: Thu Apr 13 17:55:43 2023, max compression
```

## Comparing `pyfakefs-5.2.1.tar` & `pyfakefs-5.2.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    43041 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/COPYING
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.595978 pyfakefs-5.2.1/pyfakefs/
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_file.py
--rw-r--r--   0 runner    (1001) docker     (123)   114825 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_filesystem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2180 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_filesystem_shutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    42868 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_filesystem_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_open.py
--rw-r--r--   0 runner    (1001) docker     (123)    49959 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_os.py
--rw-r--r--   0 runner    (1001) docker     (123)    17959 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    34457 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/fake_scandir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/mox3_stubout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/patched_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.599978 pyfakefs-5.2.1/pyfakefs/pytest_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_doctest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_plugin_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/pyfakefs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/all_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/all_tests_without_extra_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/dynamic_patch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/example_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_glob_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22146 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_shutil_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   105643 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    33469 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_unittest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    29625 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_vs_real_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    83871 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_open_test.py
--rw-r--r--   0 runner    (1001) docker     (123)   230257 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_os_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_pathlib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_stat_time_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fake_tempfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/pyfakefs/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/config_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/deprecated_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/fixtures/module_with_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/import_as_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/logsio.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/patched_packages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/performance_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyfakefs/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:25:34.595978 pyfakefs-5.2.1/pyfakefs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 14:25:34.000000 pyfakefs-5.2.1/pyfakefs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-11 14:25:34.603978 pyfakefs-5.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 14:25:21.000000 pyfakefs-5.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    43745 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/COPYING
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.844593 pyfakefs-5.2.2/pyfakefs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45851 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115325 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_filesystem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2180 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_filesystem_shutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42878 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_filesystem_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13113 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50722 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17959 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34457 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/fake_scandir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/mox3_stubout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/patched_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.852594 pyfakefs-5.2.2/pyfakefs/pytest_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_doctest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_param_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_module_fixture_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_plugin_failing_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_plugin_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/pyfakefs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/all_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/all_tests_without_extra_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/dynamic_patch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6954 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/example_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_glob_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22148 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_shutil_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105643 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_unittest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29625 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_vs_real_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83871 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_open_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)   230962 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_os_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_pathlib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22291 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_stat_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fake_tempfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/pyfakefs/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/config_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/deprecated_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/fixtures/module_with_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/import_as_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/logsio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/patched_packages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/performance_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyfakefs/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:55:43.848593 pyfakefs-5.2.2/pyfakefs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 17:55:43.000000 pyfakefs-5.2.2/pyfakefs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-13 17:55:43.860594 pyfakefs-5.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-13 17:55:29.000000 pyfakefs-5.2.2/setup.py
```

### Comparing `pyfakefs-5.2.1/CHANGES.md` & `pyfakefs-5.2.2/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 # pyfakefs Release Notes
 The released versions correspond to PyPI releases.
 
+## [Version 5.2.2](https://pypi.python.org/pypi/pyfakefs/5.2.2) (2023-04-13)
+Fixes a regression in 5.2.0
+
+### Changes
+* Made the user and group IDs accessible via dedicated ``get_uid`` and ``get_gid``
+  functions (for symmetry to ``set_uid`` / ``set_gid``)
+
+### Fixes
+* The test fixture is now included in the source distribution and installed
+  with the package.
+* Some public constants in `fake_filesystem` that had been moved to `helpers` are
+  made accessible from there again (see [#809](../../issues/809)).
+* Add missing fake implementations for `os.getuid` and `os.getgid` (Posix only)
+* Make sure a `/tmp` path exists under linux (`TMPDIR` may point elsewhere)
+  (see [#810](../../issues/810))
+
+
 ## [Version 5.2.1](https://pypi.python.org/pypi/pyfakefs/5.2.1) (2023-04-11)
 Support for latest Python 3.12 version.
 
 ### Changes
 * Adapted fake pathlib to changes in Python 3.12a7 (last alpha version)
 
 ### Fixes
```

### Comparing `pyfakefs-5.2.1/COPYING` & `pyfakefs-5.2.2/COPYING`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/PKG-INFO` & `pyfakefs-5.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.2.1
+Version: 5.2.2
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.2.1/README.md` & `pyfakefs-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/extra_packages.py` & `pyfakefs-5.2.2/pyfakefs/extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_file.py` & `pyfakefs-5.2.2/pyfakefs/fake_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,18 @@
         # to be backwards compatible regarding argument order, we raise on None
         if filesystem is None:
             raise ValueError("filesystem shall not be None")
         self.filesystem: "FakeFilesystem" = filesystem
         self._side_effect: Optional[Callable] = side_effect
         self.name: AnyStr = name  # type: ignore[assignment]
         self.stat_result = FakeStatResult(
-            filesystem.is_windows_fs, helpers.USER_ID, helpers.GROUP_ID, helpers.now()
+            filesystem.is_windows_fs,
+            helpers.get_uid(),
+            helpers.get_gid(),
+            helpers.now(),
         )
         if st_mode >> 12 == 0:
             st_mode |= S_IFREG
         self.stat_result.st_mode = st_mode
         self.st_size: int = 0
         self.encoding: Optional[str] = real_encoding(encoding)
         self.errors: str = errors or "strict"
```

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_filesystem.py` & `pyfakefs-5.2.2/pyfakefs/fake_filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,18 +155,27 @@
 FakeFileOpen = fake_open.FakeFileOpen
 FakeIoModule = fake_io.FakeIoModule
 if sys.platform != "win32":
     FakeFcntlModule = fake_io.FakeFcntlModule
 PatchMode = fake_io.PatchMode
 
 is_root = helpers.is_root
+get_uid = helpers.get_uid
 set_uid = helpers.set_uid
+get_gid = helpers.get_gid
 set_gid = helpers.set_gid
 reset_ids = helpers.reset_ids
 
+PERM_READ = helpers.PERM_READ
+PERM_WRITE = helpers.PERM_WRITE
+PERM_EXE = helpers.PERM_EXE
+PERM_DEF = helpers.PERM_DEF
+PERM_DEF_FILE = helpers.PERM_DEF_FILE
+PERM_ALL = helpers.PERM_ALL
+
 
 class FakeFilesystem:
     """Provides the appearance of a real directory tree for unit testing.
 
     Attributes:
         path_separator: The path separator, corresponds to `os.path.sep`.
         alternative_path_separator: Corresponds to `os.path.altsep`.
@@ -731,15 +740,15 @@
 
     def utime(
         self,
         path: AnyStr,
         times: Optional[Tuple[Union[int, float], Union[int, float]]] = None,
         *,
         ns: Optional[Tuple[int, int]] = None,
-        follow_symlinks: bool = True
+        follow_symlinks: bool = True,
     ) -> None:
         """Change the access and modified times of a file.
 
         Args:
             path: (str) Path to the file.
             times: 2-tuple of int or float numbers, of the form (atime, mtime)
                 which is used to set the access and modified times in seconds.
@@ -1616,18 +1625,18 @@
                     self.raise_os_error(errno.EACCES, target.path)
         except KeyError:
             self.raise_os_error(errno.ENOENT, path)
         return target
 
     @staticmethod
     def _can_read(target, owner_can_read):
-        if target.st_uid == helpers.USER_ID:
+        if target.st_uid == helpers.get_uid():
             if owner_can_read or target.st_mode & 0o400:
                 return True
-        if target.st_gid == helpers.GROUP_ID:
+        if target.st_gid == get_gid():
             if target.st_mode & 0o040:
                 return True
         return target.st_mode & 0o004
 
     def get_object(self, file_path: AnyPath, check_read_perm: bool = True) -> FakeFile:
         """Search for the specified filesystem object within the fake
         filesystem.
@@ -2910,9 +2919,18 @@
 def _run_doctest() -> TestResults:
     import doctest
     import pyfakefs
 
     return doctest.testmod(pyfakefs.fake_filesystem)
 
 
+def __getattr__(name):
+    # backwards compatibility for read access to globals moved to helpers
+    if name == "USER_ID":
+        return helpers.USER_ID
+    if name == "GROUP_ID":
+        return helpers.GROUP_ID
+    raise AttributeError(f"No attribute {name!r}.")
+
+
 if __name__ == "__main__":
     _run_doctest()
```

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_filesystem_shutil.py` & `pyfakefs-5.2.2/pyfakefs/fake_filesystem_shutil.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_filesystem_unittest.py` & `pyfakefs-5.2.2/pyfakefs/fake_filesystem_unittest.py`

 * *Files 0% similar despite different names*

```diff
@@ -891,16 +891,16 @@
         linecache.open = self.original_open  # type: ignore[attr-defined]
         tokenize._builtin_open = self.original_open  # type: ignore
 
         # the temp directory is assumed to exist at least in `tempfile`,
         # so we create it here for convenience
         assert self.fs is not None
         self.fs.create_dir(temp_dir)
-        if sys.platform == "darwin" and not self.fs.exists("/tmp"):
-            # under macOS, we also create a link in /tmp for convenience
+        if sys.platform != "win32" and not self.fs.exists("/tmp"):
+            # under Posix, we also create a link in /tmp if the path does not exist
             self.fs.create_symlink("/tmp", temp_dir)
             # reset the used size to 0 to avoid having the link size counted
             # which would make disk size tests more complicated
             next(iter(self.fs.mount_points.values()))["used_size"] = 0
 
     def start_patching(self) -> None:
         if not self._patching:
```

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_io.py` & `pyfakefs-5.2.2/pyfakefs/fake_io.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_open.py` & `pyfakefs-5.2.2/pyfakefs/fake_open.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_os.py` & `pyfakefs-5.2.2/pyfakefs/fake_os.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     to_string,
     matching_string,
     AnyString,
     to_bytes,
     PERM_EXE,
     PERM_DEF,
     is_root,
+    get_uid,
+    get_gid,
 )
 
 if TYPE_CHECKING:
     from pyfakefs.fake_filesystem import FakeFilesystem
 
 NR_STD_STREAMS = 3
 
@@ -130,14 +132,19 @@
             _dir += [
                 "fdatasync",
                 "getxattr",
                 "listxattr",
                 "removexattr",
                 "setxattr",
             ]
+        if sys.platform != "win32":
+            _dir += [
+                "getgid",
+                "getuid",
+            ]
         if use_scandir:
             _dir += ["scandir"]
         return _dir
 
     def __init__(self, filesystem: "FakeFilesystem"):
         """Also exposes self.path (to fake os.path).
 
@@ -1268,14 +1275,30 @@
             source.seek(position)
         if contents:
             written = dest.write(contents)
             dest.flush()
             return written
         return 0
 
+    def getuid(self) -> int:
+        """Returns the user id set in the fake filesystem.
+        If not changed using ``set_uid``, this is the uid of the real system.
+        """
+        if self.filesystem.is_windows_fs:
+            raise NameError("name 'getuid' is not defined")
+        return get_uid()
+
+    def getgid(self) -> int:
+        """Returns the group id set in the fake filesystem.
+        If not changed using ``set_gid``, this is the gid of the real system.
+        """
+        if self.filesystem.is_windows_fs:
+            raise NameError("name 'getgid' is not defined")
+        return get_gid()
+
     def fake_functions(self, original_functions) -> Set:
         functions = set()
         for fn in original_functions:
             if hasattr(self, fn.__name__):
                 functions.add(getattr(self, fn.__name__))
             else:
                 functions.add(fn)
```

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_path.py` & `pyfakefs-5.2.2/pyfakefs/fake_path.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_pathlib.py` & `pyfakefs-5.2.2/pyfakefs/fake_pathlib.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/fake_scandir.py` & `pyfakefs-5.2.2/pyfakefs/fake_scandir.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/helpers.py` & `pyfakefs-5.2.2/pyfakefs/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,26 +40,36 @@
     USER_ID = 1
     GROUP_ID = 1
 else:
     USER_ID = os.getuid()
     GROUP_ID = os.getgid()
 
 
+def get_uid() -> int:
+    """Get the global user id. Same as ``os.getuid()``"""
+    return USER_ID
+
+
 def set_uid(uid: int) -> None:
     """Set the global user id. This is used as st_uid for new files
     and to differentiate between a normal user and the root user (uid 0).
     For the root user, some permission restrictions are ignored.
 
     Args:
         uid: (int) the user ID of the user calling the file system functions.
     """
     global USER_ID
     USER_ID = uid
 
 
+def get_gid() -> int:
+    """Get the global group id. Same as ``os.getgid()``"""
+    return GROUP_ID
+
+
 def set_gid(gid: int) -> None:
     """Set the global group id. This is only used to set st_gid for new files,
     no permission checks are performed.
 
     Args:
         gid: (int) the group ID of the user calling the file system functions.
     """
```

### Comparing `pyfakefs-5.2.1/pyfakefs/mox3_stubout.py` & `pyfakefs-5.2.2/pyfakefs/mox3_stubout.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/patched_packages.py` & `pyfakefs-5.2.2/pyfakefs/patched_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_plugin.py` & `pyfakefs-5.2.2/pyfakefs/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/conftest.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/example.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_check_failed_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_doctest_test.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_doctest_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_param_test.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_param_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_fixture_test.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_module_fixture_test.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_module_fixture_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/pytest_tests/pytest_plugin_test.py` & `pyfakefs-5.2.2/pyfakefs/pytest_tests/pytest_plugin_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/all_tests.py` & `pyfakefs-5.2.2/pyfakefs/tests/all_tests.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/all_tests_without_extra_packages.py` & `pyfakefs-5.2.2/pyfakefs/tests/all_tests_without_extra_packages.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/dynamic_patch_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/dynamic_patch_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/example.py` & `pyfakefs-5.2.2/pyfakefs/tests/example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/example_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/example_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_glob_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_glob_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_shutil_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_shutil_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import shutil
 import sys
 import tempfile
 import unittest
 from pathlib import Path
 
 from pyfakefs import fake_filesystem_unittest
-from pyfakefs.helpers import USER_ID, set_uid, is_root
+from pyfakefs.helpers import get_uid, set_uid, is_root
 from pyfakefs.tests.test_utils import RealFsTestMixin
 
 is_windows = sys.platform == "win32"
 
 
 class RealFsTestCase(fake_filesystem_unittest.TestCase, RealFsTestMixin):
     def __init__(self, methodName="runTest"):
         fake_filesystem_unittest.TestCase.__init__(self, methodName)
         RealFsTestMixin.__init__(self)
 
     def setUp(self):
         RealFsTestMixin.setUp(self)
         self.cwd = os.getcwd()
-        self.uid = USER_ID
+        self.uid = get_uid()
         set_uid(1000)
         if not self.use_real_fs():
             self.setUpPyfakefs()
             self.filesystem = self.fs
             self.os = os
             self.open = open
             self.create_basepath()
```

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_unittest_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_unittest_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,15 +658,15 @@
         self.setUpPyfakefs()
 
     def testTempDirExists(self):
         self.assertTrue(os.path.exists(tempfile.gettempdir()))
 
     @unittest.skipIf(sys.platform == "win32", "POSIX only test")
     def testTmpExists(self):
-        # directory under Linux, link under macOS
+        # directory or link under Linux, link under macOS
         self.assertTrue(os.path.exists("/tmp"))
 
 
 class TestTempFileReload(unittest.TestCase):
     """Regression test for #356 to make sure that reloading the tempfile
     does not affect other tests."""
```

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_filesystem_vs_real_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_filesystem_vs_real_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_open_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_open_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_os_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_os_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import errno
 import os
 import stat
 import sys
 import unittest
 
-from pyfakefs.helpers import IN_DOCKER, IS_PYPY, GROUP_ID, USER_ID
+from pyfakefs.helpers import IN_DOCKER, IS_PYPY, get_uid, get_gid
 
 from pyfakefs import fake_filesystem, fake_os, fake_open, fake_file
 from pyfakefs.fake_filesystem import (
     FakeFileOpen,
     is_root,
     set_uid,
     set_gid,
@@ -5399,68 +5399,88 @@
 
     def chmod(self, path, mode):
         if self.is_windows_fs:
             self.filesystem.chmod(path, mode, force_unix_mode=True)
         else:
             self.os.chmod(path, mode)
 
+    def test_getuid(self):
+        self.skip_real_fs()  # won't change user in real fs
+        self.check_posix_only()
+        uid = self.os.getuid()
+        set_uid(uid + 10)
+        self.assertEqual(uid + 10, self.os.getuid())
+        self.assertEqual(uid + 10, get_uid())
+        set_uid(uid)
+        self.assertEqual(uid, self.os.getuid())
+
+    def test_getgid(self):
+        self.skip_real_fs()  # won't change group in real fs
+        self.check_posix_only()
+        gid = self.os.getgid()
+        set_gid(gid + 10)
+        self.assertEqual(gid + 10, self.os.getgid())
+        self.assertEqual(gid + 10, get_gid())
+        set_gid(gid)
+        self.assertEqual(gid, self.os.getgid())
+
     def test_listdir_unreadable_dir(self):
         if not is_root():
             self.assert_raises_os_error(errno.EACCES, self.os.listdir, self.dir_path)
         else:
             self.assertEqual(["some_file"], self.os.listdir(self.dir_path))
 
     def test_listdir_user_readable_dir(self):
         self.chmod(self.dir_path, 0o600)
         self.assertEqual(["some_file"], self.os.listdir(self.dir_path))
         self.chmod(self.dir_path, 0o000)
 
     def test_listdir_user_readable_dir_from_other_user(self):
         self.skip_real_fs()  # won't change user in real fs
         self.check_posix_only()
-        user_id = USER_ID
+        user_id = get_uid()
         set_uid(user_id + 1)
         dir_path = self.make_path("dir1")
         self.create_dir(dir_path, perm=0o600)
         self.assertTrue(self.os.path.exists(dir_path))
         set_uid(user_id)
         if not is_root():
             with self.assertRaises(PermissionError):
                 self.os.listdir(dir_path)
         else:
             self.assertEqual(["some_file"], self.os.listdir(self.dir_path))
 
     def test_listdir_group_readable_dir_from_other_user(self):
         self.skip_real_fs()  # won't change user in real fs
-        user_id = USER_ID
+        user_id = get_uid()
         set_uid(user_id + 1)
         dir_path = self.make_path("dir1")
         self.create_dir(dir_path, perm=0o660)
         self.assertTrue(self.os.path.exists(dir_path))
         set_uid(user_id)
         self.assertEqual([], self.os.listdir(dir_path))
 
     def test_listdir_group_readable_dir_from_other_group(self):
         self.skip_real_fs()  # won't change user in real fs
         self.check_posix_only()
-        group_id = GROUP_ID
+        group_id = self.os.getgid()
         set_gid(group_id + 1)
         dir_path = self.make_path("dir1")
         self.create_dir(dir_path, perm=0o060)
         self.assertTrue(self.os.path.exists(dir_path))
         set_gid(group_id)
         if not is_root():
             with self.assertRaises(PermissionError):
                 self.os.listdir(dir_path)
         else:
             self.assertEqual([], self.os.listdir(dir_path))
 
     def test_listdir_other_readable_dir_from_other_group(self):
         self.skip_real_fs()  # won't change user in real fs
-        group_id = GROUP_ID
+        group_id = get_gid()
         set_gid(group_id + 1)
         dir_path = self.make_path("dir1")
         self.create_dir(dir_path, perm=0o004)
         self.assertTrue(self.os.path.exists(dir_path))
         set_gid(group_id)
         self.assertEqual([], self.os.listdir(dir_path))
 
@@ -5485,15 +5505,15 @@
         self.create_dir(dir_path, perm=0o000)
         self.assertTrue(self.os.path.exists(dir_path))
         self.os.rmdir(dir_path)
         self.assertFalse(self.os.path.exists(dir_path))
 
     def test_remove_unreadable_dir_from_other_user(self):
         self.skip_real_fs()  # won't change user in real fs
-        user_id = USER_ID
+        user_id = get_uid()
         set_uid(user_id + 1)
         dir_path = self.make_path("dir1")
         self.create_dir(dir_path, perm=0o000)
         self.assertTrue(self.os.path.exists(dir_path))
         set_uid(user_id)
         if not is_root():
             with self.assertRaises(PermissionError):
```

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_pathlib_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_pathlib_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_stat_time_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_stat_time_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fake_tempfile_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/fake_tempfile_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fixtures/deprecated_property.py` & `pyfakefs-5.2.2/pyfakefs/tests/fixtures/deprecated_property.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/fixtures/module_with_attributes.py` & `pyfakefs-5.2.2/pyfakefs/tests/fixtures/module_with_attributes.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/import_as_example.py` & `pyfakefs-5.2.2/pyfakefs/tests/import_as_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/logsio.py` & `pyfakefs-5.2.2/pyfakefs/tests/logsio.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_example.py` & `pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_example.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/mox3_stubout_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/mox3_stubout_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/patched_packages_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/patched_packages_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/performance_test.py` & `pyfakefs-5.2.2/pyfakefs/tests/performance_test.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs/tests/test_utils.py` & `pyfakefs-5.2.2/pyfakefs/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/pyfakefs.egg-info/PKG-INFO` & `pyfakefs-5.2.2/pyfakefs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfakefs
-Version: 5.2.1
+Version: 5.2.2
 Summary: pyfakefs implements a fake file system that mocks the Python file system modules.
 Home-page: https://github.com/pytest-dev/pyfakefs
 Author: Google
 Author-email: google-pyfakefs@google.com
 Maintainer: John McGehee
 Maintainer-email: pyfakefs@johnnado.com
 License: http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pyfakefs-5.2.1/pyfakefs.egg-info/SOURCES.txt` & `pyfakefs-5.2.2/pyfakefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfakefs-5.2.1/setup.cfg` & `pyfakefs-5.2.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 universal = 0
 
 [options]
 packages = find:
 install_requires = 
 python_requires = >=3.7
 test_suite = pyfakefs.tests
+include_package_data = True
 
 [options.packages.find]
 exclude = docs
 
 [options.entry_points]
 pytest11 = 
 	pytest_fakefs = pyfakefs.pytest_plugin
```

