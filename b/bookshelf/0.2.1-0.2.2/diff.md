# Comparing `tmp/bookshelf-0.2.1.tar.gz` & `tmp/bookshelf-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookshelf-0.2.1.tar", last modified: Wed Feb 15 22:10:24 2023, max compression
+gzip compressed data, was "bookshelf-0.2.2.tar", last modified: Thu Apr 13 11:40:35 2023, max compression
```

## Comparing `bookshelf-0.2.1.tar` & `bookshelf-0.2.2.tar`

### file list

```diff
@@ -1,108 +1,132 @@
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/
--rw-r--r--   0 jared     (1000) jared     (1000)     5451 2022-07-18 00:43:20.000000 bookshelf-0.2.1/.gitignore
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.646979 bookshelf-0.2.1/.gitlab/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/.gitlab/issue_templates/
--rw-r--r--   0 jared     (1000) jared     (1000)      610 2022-07-20 04:44:32.000000 bookshelf-0.2.1/.gitlab/issue_templates/Bug.md
--rw-r--r--   0 jared     (1000) jared     (1000)      526 2022-07-20 04:44:32.000000 bookshelf-0.2.1/.gitlab/issue_templates/Feature_Request.md
--rw-r--r--   0 jared     (1000) jared     (1000)      559 2022-07-20 04:46:35.000000 bookshelf-0.2.1/.gitlab/issue_templates/New_Book.md
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/.gitlab/merge_request_templates/
--rw-r--r--   0 jared     (1000) jared     (1000)      353 2023-02-14 10:25:52.000000 bookshelf-0.2.1/.gitlab/merge_request_templates/Default.md
--rw-r--r--   0 jared     (1000) jared     (1000)      333 2022-07-20 04:44:32.000000 bookshelf-0.2.1/.gitlab/merge_request_templates/New Book.md
--rw-r--r--   0 jared     (1000) jared     (1000)     1451 2022-11-23 05:38:44.000000 bookshelf-0.2.1/.gitlab-ci.yml
--rw-r--r--   0 jared     (1000) jared     (1000)      429 2022-07-18 00:43:20.000000 bookshelf-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 jared     (1000) jared     (1000)     4161 2023-02-14 23:15:10.000000 bookshelf-0.2.1/CHANGELOG.rst
--rw-r--r--   0 jared     (1000) jared     (1000)     1056 2022-11-23 05:38:44.000000 bookshelf-0.2.1/LICENSE
--rw-r--r--   0 jared     (1000) jared     (1000)     2897 2023-02-15 22:10:09.000000 bookshelf-0.2.1/Makefile
--rw-r--r--   0 jared     (1000) jared     (1000)     1932 2023-02-15 22:10:24.653646 bookshelf-0.2.1/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)     5753 2022-11-23 05:38:44.000000 bookshelf-0.2.1/README.rst
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/
--rw-r--r--   0 jared     (1000) jared     (1000)     1212 2022-07-19 01:42:28.000000 bookshelf-0.2.1/notebooks/README.md
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/ceds/
--rw-r--r--   0 jared     (1000) jared     (1000)     5580 2023-02-14 23:14:23.000000 bookshelf-0.2.1/notebooks/ceds/ceds.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1328 2023-02-14 23:14:23.000000 bookshelf-0.2.1/notebooks/ceds/ceds.yaml
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.646979 bookshelf-0.2.1/notebooks/examples/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/examples/multiple_versions/
--rw-r--r--   0 jared     (1000) jared     (1000)     2706 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/examples/multiple_versions/multiple_versions.py
--rw-r--r--   0 jared     (1000) jared     (1000)      713 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/examples/multiple_versions/multiple_versions.yaml
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/examples/simple/
--rw-r--r--   0 jared     (1000) jared     (1000)     2486 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/examples/simple/simple.py
--rw-r--r--   0 jared     (1000) jared     (1000)      415 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/examples/simple/simple.yaml
--rw-r--r--   0 jared     (1000) jared     (1000)       63 2022-07-18 00:43:20.000000 bookshelf-0.2.1/notebooks/jupytext.toml
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/primap-hist/
--rw-r--r--   0 jared     (1000) jared     (1000)     4652 2023-02-14 10:25:52.000000 bookshelf-0.2.1/notebooks/primap-hist/primap-hist.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2150 2023-02-14 23:14:23.000000 bookshelf-0.2.1/notebooks/primap-hist/primap-hist.yaml
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/rcmip-emissions/
--rw-r--r--   0 jared     (1000) jared     (1000)     1844 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/rcmip-emissions/rcmip-emissions.py
--rw-r--r--   0 jared     (1000) jared     (1000)      449 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/rcmip-emissions/rcmip-emissions.yaml
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/un-wpp/
--rw-r--r--   0 jared     (1000) jared     (1000)     7209 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/un-wpp/un-wpp.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1394 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/un-wpp/un-wpp.yaml
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/notebooks/wdi/
--rw-r--r--   0 jared     (1000) jared     (1000)     6476 2023-02-14 10:25:38.000000 bookshelf-0.2.1/notebooks/wdi/wdi.py
--rw-r--r--   0 jared     (1000) jared     (1000)      866 2022-11-23 05:38:44.000000 bookshelf-0.2.1/notebooks/wdi/wdi.yaml
--rw-r--r--   0 jared     (1000) jared     (1000)      747 2023-02-14 23:15:28.000000 bookshelf-0.2.1/pyproject.toml
--rw-r--r--   0 jared     (1000) jared     (1000)     3042 2023-02-15 22:10:24.653646 bookshelf-0.2.1/setup.cfg
--rw-r--r--   0 jared     (1000) jared     (1000)       58 2022-07-18 00:43:20.000000 bookshelf-0.2.1/setup.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.646979 bookshelf-0.2.1/src/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/src/bookshelf/
--rw-r--r--   0 jared     (1000) jared     (1000)      670 2022-11-23 05:38:44.000000 bookshelf-0.2.1/src/bookshelf/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     8575 2023-02-14 23:14:23.000000 bookshelf-0.2.1/src/bookshelf/book.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1284 2022-11-23 05:38:44.000000 bookshelf-0.2.1/src/bookshelf/cli.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/src/bookshelf/commands/
--rw-r--r--   0 jared     (1000) jared     (1000)       21 2022-07-18 23:00:10.000000 bookshelf-0.2.1/src/bookshelf/commands/__init__.py
--rw-r--r--   0 jared     (1000) jared     (1000)     2095 2023-02-14 23:14:23.000000 bookshelf-0.2.1/src/bookshelf/commands/cmd_publish.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1488 2023-02-14 23:14:23.000000 bookshelf-0.2.1/src/bookshelf/commands/cmd_run.py
--rw-r--r--   0 jared     (1000) jared     (1000)      518 2023-02-14 23:14:23.000000 bookshelf-0.2.1/src/bookshelf/constants.py
--rw-r--r--   0 jared     (1000) jared     (1000)      818 2022-11-23 05:38:44.000000 bookshelf-0.2.1/src/bookshelf/errors.py
--rw-r--r--   0 jared     (1000) jared     (1000)     8150 2023-02-14 23:14:23.000000 bookshelf-0.2.1/src/bookshelf/notebook.py
--rw-r--r--   0 jared     (1000) jared     (1000)     4588 2023-02-14 23:14:23.000000 bookshelf-0.2.1/src/bookshelf/schema.py
--rw-r--r--   0 jared     (1000) jared     (1000)    11736 2023-02-14 23:14:23.000000 bookshelf-0.2.1/src/bookshelf/shelf.py
--rw-r--r--   0 jared     (1000) jared     (1000)     6158 2022-11-23 05:38:44.000000 bookshelf-0.2.1/src/bookshelf/utils.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/src/bookshelf.egg-info/
--rw-r--r--   0 jared     (1000) jared     (1000)     1932 2023-02-15 22:10:24.000000 bookshelf-0.2.1/src/bookshelf.egg-info/PKG-INFO
--rw-r--r--   0 jared     (1000) jared     (1000)     2513 2023-02-15 22:10:24.000000 bookshelf-0.2.1/src/bookshelf.egg-info/SOURCES.txt
--rw-r--r--   0 jared     (1000) jared     (1000)        1 2023-02-15 22:10:24.000000 bookshelf-0.2.1/src/bookshelf.egg-info/dependency_links.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       49 2023-02-15 22:10:24.000000 bookshelf-0.2.1/src/bookshelf.egg-info/entry_points.txt
--rw-r--r--   0 jared     (1000) jared     (1000)      537 2023-02-15 22:10:24.000000 bookshelf-0.2.1/src/bookshelf.egg-info/requires.txt
--rw-r--r--   0 jared     (1000) jared     (1000)       10 2023-02-15 22:10:24.000000 bookshelf-0.2.1/src/bookshelf.egg-info/top_level.txt
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/tests/
--rw-r--r--   0 jared     (1000) jared     (1000)      732 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/conftest.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.650313 bookshelf-0.2.1/tests/integration/
--rw-r--r--   0 jared     (1000) jared     (1000)      681 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/integration/test_simple.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/notebooks/
--rw-r--r--   0 jared     (1000) jared     (1000)     3013 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/notebooks/test_notebooks.py
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.646979 bookshelf-0.2.1/tests/test-data/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.646979 bookshelf-0.2.1/tests/test-data/v0.1.0/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.1.0/example/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.0.0/
--rw-r--r--   0 jared     (1000) jared     (1000)      370 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.0.0/datapackage.json
--rw-r--r--   0 jared     (1000) jared     (1000)    13117 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.0.0/leakage_rates_low.csv
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.1.0/
--rw-r--r--   0 jared     (1000) jared     (1000)        5 2022-07-18 00:43:20.000000 bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.1.0/datapackage.json
--rw-r--r--   0 jared     (1000) jared     (1000)    13117 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.1.0/leakage_rates_low.csv
--rw-r--r--   0 jared     (1000) jared     (1000)      304 2022-07-18 00:43:20.000000 bookshelf-0.2.1/tests/test-data/v0.1.0/example/volume.json
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.646979 bookshelf-0.2.1/tests/test-data/v0.2.0/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.2.0/example/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.0.0_e001/
--rw-r--r--   0 jared     (1000) jared     (1000)      386 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.0.0_e001/datapackage.json
--rw-r--r--   0 jared     (1000) jared     (1000)    13117 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.0.0_e001/leakage_rates_low.csv
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.1.0_e001/
--rw-r--r--   0 jared     (1000) jared     (1000)        5 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.1.0_e001/datapackage.json
--rw-r--r--   0 jared     (1000) jared     (1000)    13117 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.1.0_e001/leakage_rates_low.csv
--rw-r--r--   0 jared     (1000) jared     (1000)      354 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/test-data/v0.2.0/example/volume.json
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.646979 bookshelf-0.2.1/tests/test-data/v0.2.1/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.2.1/example/
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.0.0_e001/
--rw-r--r--   0 jared     (1000) jared     (1000)      406 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.0.0_e001/datapackage.json
--rw-r--r--   0 jared     (1000) jared     (1000)    13117 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.0.0_e001/leakage_rates_low.csv
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.1.0_e001/
--rw-r--r--   0 jared     (1000) jared     (1000)        5 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.1.0_e001/datapackage.json
--rw-r--r--   0 jared     (1000) jared     (1000)    13117 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.1.0_e001/leakage_rates_low.csv
--rw-r--r--   0 jared     (1000) jared     (1000)      402 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/test-data/v0.2.1/example/volume.json
-drwxr-xr-x   0 jared     (1000) jared     (1000)        0 2023-02-15 22:10:24.653646 bookshelf-0.2.1/tests/unit/
--rw-r--r--   0 jared     (1000) jared     (1000)     1954 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/unit/conftest.py
--rw-r--r--   0 jared     (1000) jared     (1000)     3112 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/unit/test_book.py
--rw-r--r--   0 jared     (1000) jared     (1000)     4397 2022-11-23 05:38:44.000000 bookshelf-0.2.1/tests/unit/test_cli.py
--rw-r--r--   0 jared     (1000) jared     (1000)     3940 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/unit/test_notebook.py
--rw-r--r--   0 jared     (1000) jared     (1000)    10025 2023-02-14 23:14:23.000000 bookshelf-0.2.1/tests/unit/test_shelf.py
--rw-r--r--   0 jared     (1000) jared     (1000)     1529 2022-07-18 23:00:10.000000 bookshelf-0.2.1/tests/unit/test_utils.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.397691 bookshelf-0.2.2/
+-rw-r--r--   0 jared      (501) staff       (20)     5451 2022-07-17 06:52:23.000000 bookshelf-0.2.2/.gitignore
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.374893 bookshelf-0.2.2/.gitlab/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.381200 bookshelf-0.2.2/.gitlab/issue_templates/
+-rw-r--r--   0 jared      (501) staff       (20)      610 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/issue_templates/Bug.md
+-rw-r--r--   0 jared      (501) staff       (20)      526 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/issue_templates/Feature_Request.md
+-rw-r--r--   0 jared      (501) staff       (20)      559 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/issue_templates/New_Book.md
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.381607 bookshelf-0.2.2/.gitlab/merge_request_templates/
+-rw-r--r--   0 jared      (501) staff       (20)      353 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/merge_request_templates/Default.md
+-rw-r--r--   0 jared      (501) staff       (20)      333 2023-03-13 23:04:16.000000 bookshelf-0.2.2/.gitlab/merge_request_templates/New Book.md
+-rw-r--r--   0 jared      (501) staff       (20)     2159 2023-04-13 11:35:17.000000 bookshelf-0.2.2/.gitlab-ci.yml
+-rw-r--r--   0 jared      (501) staff       (20)      429 2022-07-17 06:52:23.000000 bookshelf-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 jared      (501) staff       (20)     4975 2023-04-13 11:35:17.000000 bookshelf-0.2.2/CHANGELOG.rst
+-rw-r--r--   0 jared      (501) staff       (20)     1056 2023-03-13 23:04:16.000000 bookshelf-0.2.2/LICENSE
+-rw-r--r--   0 jared      (501) staff       (20)     2656 2023-04-13 11:39:36.000000 bookshelf-0.2.2/Makefile
+-rw-r--r--   0 jared      (501) staff       (20)     1953 2023-04-13 11:40:35.397806 bookshelf-0.2.2/PKG-INFO
+-rw-r--r--   0 jared      (501) staff       (20)     5901 2023-04-13 11:35:17.000000 bookshelf-0.2.2/README.rst
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.382045 bookshelf-0.2.2/docs/
+-rw-r--r--   0 jared      (501) staff       (20)      638 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/Makefile
+-rw-r--r--   0 jared      (501) staff       (20)      769 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/make.bat
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.383550 bookshelf-0.2.2/docs/source/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.383742 bookshelf-0.2.2/docs/source/_static/
+-rw-r--r--   0 jared      (501) staff       (20)        0 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/_static/.gitkeep
+-rw-r--r--   0 jared      (501) staff       (20)     2557 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/conf.py
+-rw-r--r--   0 jared      (501) staff       (20)      986 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/configuration.rst
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.384219 bookshelf-0.2.2/docs/source/development/
+-rw-r--r--   0 jared      (501) staff       (20)     5595 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/development/contributing.rst
+-rw-r--r--   0 jared      (501) staff       (20)      176 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/development/index.rst
+-rw-r--r--   0 jared      (501) staff       (20)      856 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/development/releasing.rst
+-rw-r--r--   0 jared      (501) staff       (20)      363 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/index.rst
+-rw-r--r--   0 jared      (501) staff       (20)      105 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/installation.rst
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.385099 bookshelf-0.2.2/docs/source/reference/
+-rw-r--r--   0 jared      (501) staff       (20)       96 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.book.rst
+-rw-r--r--   0 jared      (501) staff       (20)      102 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.errors.rst
+-rw-r--r--   0 jared      (501) staff       (20)       99 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.shelf.rst
+-rw-r--r--   0 jared      (501) staff       (20)       99 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/bookshelf.utils.rst
+-rw-r--r--   0 jared      (501) staff       (20)      131 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/reference/index.rst
+-rw-r--r--   0 jared      (501) staff       (20)     2568 2023-04-13 11:35:17.000000 bookshelf-0.2.2/docs/source/usage.rst
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.385528 bookshelf-0.2.2/notebooks/
+-rw-r--r--   0 jared      (501) staff       (20)     1212 2022-07-19 03:22:48.000000 bookshelf-0.2.2/notebooks/README.md
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.385943 bookshelf-0.2.2/notebooks/ceds/
+-rw-r--r--   0 jared      (501) staff       (20)     5744 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ceds/ceds.py
+-rw-r--r--   0 jared      (501) staff       (20)     1328 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ceds/ceds.yaml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.375818 bookshelf-0.2.2/notebooks/examples/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.386269 bookshelf-0.2.2/notebooks/examples/multiple_versions/
+-rw-r--r--   0 jared      (501) staff       (20)     2706 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/multiple_versions/multiple_versions.py
+-rw-r--r--   0 jared      (501) staff       (20)      713 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/multiple_versions/multiple_versions.yaml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.386625 bookshelf-0.2.2/notebooks/examples/simple/
+-rw-r--r--   0 jared      (501) staff       (20)     2486 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/simple/simple.py
+-rw-r--r--   0 jared      (501) staff       (20)      415 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/examples/simple/simple.yaml
+-rw-r--r--   0 jared      (501) staff       (20)       63 2022-07-17 06:52:23.000000 bookshelf-0.2.2/notebooks/jupytext.toml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.387107 bookshelf-0.2.2/notebooks/primap-hist/
+-rw-r--r--   0 jared      (501) staff       (20)     4653 2023-04-13 05:34:27.000000 bookshelf-0.2.2/notebooks/primap-hist/primap-hist.py
+-rw-r--r--   0 jared      (501) staff       (20)     2280 2023-03-14 01:59:54.000000 bookshelf-0.2.2/notebooks/primap-hist/primap-hist.yaml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.387560 bookshelf-0.2.2/notebooks/rcmip-emissions/
+-rw-r--r--   0 jared      (501) staff       (20)     1844 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/rcmip-emissions/rcmip-emissions.py
+-rw-r--r--   0 jared      (501) staff       (20)      449 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/rcmip-emissions/rcmip-emissions.yaml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.387914 bookshelf-0.2.2/notebooks/ssp-basic-elements/
+-rw-r--r--   0 jared      (501) staff       (20)     2221 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ssp-basic-elements/ssp-basic-elements.py
+-rw-r--r--   0 jared      (501) staff       (20)     6775 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/ssp-basic-elements/ssp-basic-elements.yaml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.388280 bookshelf-0.2.2/notebooks/un-wpp/
+-rw-r--r--   0 jared      (501) staff       (20)     7209 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/un-wpp/un-wpp.py
+-rw-r--r--   0 jared      (501) staff       (20)     1394 2023-03-13 23:04:16.000000 bookshelf-0.2.2/notebooks/un-wpp/un-wpp.yaml
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.388876 bookshelf-0.2.2/notebooks/wdi/
+-rw-r--r--   0 jared      (501) staff       (20)     6476 2023-03-13 23:06:52.000000 bookshelf-0.2.2/notebooks/wdi/wdi.py
+-rw-r--r--   0 jared      (501) staff       (20)      866 2023-03-13 23:06:52.000000 bookshelf-0.2.2/notebooks/wdi/wdi.yaml
+-rw-r--r--   0 jared      (501) staff       (20)      747 2023-04-12 05:55:19.000000 bookshelf-0.2.2/pyproject.toml
+-rw-r--r--   0 jared      (501) staff       (20)     3137 2023-04-13 11:40:35.398352 bookshelf-0.2.2/setup.cfg
+-rw-r--r--   0 jared      (501) staff       (20)       58 2022-07-16 02:39:36.000000 bookshelf-0.2.2/setup.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.376457 bookshelf-0.2.2/src/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.390934 bookshelf-0.2.2/src/bookshelf/
+-rw-r--r--   0 jared      (501) staff       (20)      686 2023-04-13 05:34:27.000000 bookshelf-0.2.2/src/bookshelf/__init__.py
+-rw-r--r--   0 jared      (501) staff       (20)     9739 2023-04-13 11:35:17.000000 bookshelf-0.2.2/src/bookshelf/book.py
+-rw-r--r--   0 jared      (501) staff       (20)     1284 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/cli.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.392456 bookshelf-0.2.2/src/bookshelf/commands/
+-rw-r--r--   0 jared      (501) staff       (20)       21 2022-07-18 12:01:42.000000 bookshelf-0.2.2/src/bookshelf/commands/__init__.py
+-rw-r--r--   0 jared      (501) staff       (20)     2239 2023-04-12 05:57:25.000000 bookshelf-0.2.2/src/bookshelf/commands/cmd_publish.py
+-rw-r--r--   0 jared      (501) staff       (20)     1488 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/commands/cmd_run.py
+-rw-r--r--   0 jared      (501) staff       (20)      518 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/constants.py
+-rw-r--r--   0 jared      (501) staff       (20)      818 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/errors.py
+-rw-r--r--   0 jared      (501) staff       (20)     8391 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/notebook.py
+-rw-r--r--   0 jared      (501) staff       (20)     4581 2023-03-13 23:04:16.000000 bookshelf-0.2.2/src/bookshelf/schema.py
+-rw-r--r--   0 jared      (501) staff       (20)    11970 2023-04-13 11:35:17.000000 bookshelf-0.2.2/src/bookshelf/shelf.py
+-rw-r--r--   0 jared      (501) staff       (20)     6119 2023-04-13 05:34:27.000000 bookshelf-0.2.2/src/bookshelf/utils.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.391815 bookshelf-0.2.2/src/bookshelf.egg-info/
+-rw-r--r--   0 jared      (501) staff       (20)     1953 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/PKG-INFO
+-rw-r--r--   0 jared      (501) staff       (20)     3110 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/SOURCES.txt
+-rw-r--r--   0 jared      (501) staff       (20)        1 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/dependency_links.txt
+-rw-r--r--   0 jared      (501) staff       (20)       49 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/entry_points.txt
+-rw-r--r--   0 jared      (501) staff       (20)      644 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/requires.txt
+-rw-r--r--   0 jared      (501) staff       (20)       10 2023-04-13 11:40:35.000000 bookshelf-0.2.2/src/bookshelf.egg-info/top_level.txt
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.392642 bookshelf-0.2.2/tests/
+-rw-r--r--   0 jared      (501) staff       (20)      732 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/conftest.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.392814 bookshelf-0.2.2/tests/integration/
+-rw-r--r--   0 jared      (501) staff       (20)      681 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/integration/test_simple.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.393087 bookshelf-0.2.2/tests/notebooks/
+-rw-r--r--   0 jared      (501) staff       (20)     3243 2023-04-13 11:35:17.000000 bookshelf-0.2.2/tests/notebooks/test_notebooks.py
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377637 bookshelf-0.2.2/tests/test-data/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377093 bookshelf-0.2.2/tests/test-data/v0.1.0/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.393273 bookshelf-0.2.2/tests/test-data/v0.1.0/example/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.393698 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.0.0/
+-rw-r--r--   0 jared      (501) staff       (20)      370 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.0.0/datapackage.json
+-rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.0.0/leakage_rates_low.csv
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394119 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.1.0/
+-rw-r--r--   0 jared      (501) staff       (20)        5 2022-07-17 06:52:23.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.1.0/datapackage.json
+-rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.1.0/leakage_rates_low.csv
+-rw-r--r--   0 jared      (501) staff       (20)      304 2022-07-17 06:52:23.000000 bookshelf-0.2.2/tests/test-data/v0.1.0/example/volume.json
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377396 bookshelf-0.2.2/tests/test-data/v0.2.0/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394294 bookshelf-0.2.2/tests/test-data/v0.2.0/example/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394640 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.0.0_e001/
+-rw-r--r--   0 jared      (501) staff       (20)      386 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.0.0_e001/datapackage.json
+-rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.0.0_e001/leakage_rates_low.csv
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.394968 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.1.0_e001/
+-rw-r--r--   0 jared      (501) staff       (20)        5 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.1.0_e001/datapackage.json
+-rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.1.0_e001/leakage_rates_low.csv
+-rw-r--r--   0 jared      (501) staff       (20)      354 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.0/example/volume.json
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.377691 bookshelf-0.2.2/tests/test-data/v0.2.1/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.395139 bookshelf-0.2.2/tests/test-data/v0.2.1/example/
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.395525 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.0.0_e001/
+-rw-r--r--   0 jared      (501) staff       (20)      406 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.0.0_e001/datapackage.json
+-rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.0.0_e001/leakage_rates_low.csv
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.396045 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.1.0_e001/
+-rw-r--r--   0 jared      (501) staff       (20)        5 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.1.0_e001/datapackage.json
+-rw-r--r--   0 jared      (501) staff       (20)    13117 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.1.0_e001/leakage_rates_low.csv
+-rw-r--r--   0 jared      (501) staff       (20)      402 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/test-data/v0.2.1/example/volume.json
+drwxr-xr-x   0 jared      (501) staff       (20)        0 2023-04-13 11:40:35.397397 bookshelf-0.2.2/tests/unit/
+-rw-r--r--   0 jared      (501) staff       (20)     1953 2023-04-13 05:34:27.000000 bookshelf-0.2.2/tests/unit/conftest.py
+-rw-r--r--   0 jared      (501) staff       (20)     3112 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/unit/test_book.py
+-rw-r--r--   0 jared      (501) staff       (20)     4397 2023-03-13 23:04:16.000000 bookshelf-0.2.2/tests/unit/test_cli.py
+-rw-r--r--   0 jared      (501) staff       (20)     3951 2023-04-13 05:34:27.000000 bookshelf-0.2.2/tests/unit/test_notebook.py
+-rw-r--r--   0 jared      (501) staff       (20)    10278 2023-04-13 05:34:27.000000 bookshelf-0.2.2/tests/unit/test_shelf.py
+-rw-r--r--   0 jared      (501) staff       (20)     1529 2022-07-18 12:01:42.000000 bookshelf-0.2.2/tests/unit/test_utils.py
```

### Comparing `bookshelf-0.2.1/.gitignore` & `bookshelf-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/.gitlab/issue_templates/Bug.md` & `bookshelf-0.2.2/.gitlab/issue_templates/Bug.md`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/.gitlab/issue_templates/Feature_Request.md` & `bookshelf-0.2.2/.gitlab/issue_templates/Feature_Request.md`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/.gitlab/issue_templates/New_Book.md` & `bookshelf-0.2.2/.gitlab/issue_templates/New_Book.md`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/.gitlab-ci.yml` & `bookshelf-0.2.2/.gitlab-ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 image: python:3.9
 
 stages:
   - build
   - test
 
+# Use our linux CR runner by default
+default:
+  tags:
+    - docker
+    - linux
+    - cr
+
 variables:
     PIP_CACHE_DIR: "$CI_PROJECT_DIR/.cache/pip"
     BOOKSHELF_DOWNLOAD_CACHE_LOCATION: "$CI_PROJECT_DIR/.cache/pooch"
 
 cache: &global_cache
   key: ${CI_COMMIT_REF_SLUG}
   paths:
@@ -19,15 +26,14 @@
 
 build:
   stage: build
   script:
     - make -B virtual-environment
 
 
-# Test the rcmip package and CLI
 test: &test_config
   stage: test
   cache:
     <<: *global_cache
   before_script:
     - source venv/bin/activate
   script:
@@ -40,14 +46,33 @@
     when: always
     reports:
       coverage_report:
         coverage_format: cobertura
         path: coverage.xml
       junit: report.xml
 
+# Run a basic test-suite on Windows using python 3.11
+# This spawns a new VM for each job which can take a few minutes
+test-windows:
+  tags:
+    - shared-windows
+    - windows
+    - windows-1809
+  stage: test
+  cache: []  # Disable caching on Windows
+  script:
+    - choco install python --version=3.11.2 -y
+    - $env:Path = "C:\Python311;" + $env:Path
+    - python -m venv venv
+    - '& venv/Scripts/Activate.ps1'
+    - pip install -e .[tests]
+    # Ignore tests/notebooks on windows
+    - pytest -rfsxEX --ignore=tests/notebooks
+
+
 test:notebooks:
   <<: *test_config
   variables:
     BOOKSHELF_CACHE_LOCATION: out
   script:
     - pytest -n auto tests/notebooks --log-cli-level INFO
   artifacts:
@@ -60,7 +85,13 @@
   <<: *test_config
   script:
     - flake8 setup.py src tests notebooks
     - black --check src tests notebooks
     - mypy --install-types --non-interactive src --exclude src/bookshelf/__init__.py
     - pylint --fail-under=9.5 src
     - bandit -r src
+
+test:docs:
+  <<: *test_config
+  script:
+#    - pydocstyle src
+    - sphinx-build -M html docs/source docs/_build -qW
```

### Comparing `bookshelf-0.2.1/CHANGELOG.rst` & `bookshelf-0.2.2/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,42 @@
     - Removed: now removed features
     - Fixed: any bug fixes
     - Security: in case of vulnerabilities.
 
 Unreleased
 ----------
 
-v0.2.1
+
+v0.2.2
 ------
 
+Added
+=====
+
+- (`!27 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/27>`_) Add sphinx-based documentation
+- (`!26 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/26>`_) Add ``force`` option to the publish CLI command to upload data even if a matching edition already exists
+- (`!25 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/25>`_) Add primap-hist v2.4.1 and v2.4.2
+
+Changed
+=======
+
+- (`!29 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/29>`_) Move ``python-dotenv`` from a development dependency to a core dependency
+- (`!23 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/23>`_) Fix CEDs unit names for all resources. Bumps ``ceds`` to ed.3
+
+Fixed
+=====
+
+- (`!28 <https://gitlab.com/climate-resource/bookshelf/bookshelf/-/merge_requests/28>`_) Fix file retrieval and publishing on windows
+
+v0.2.1
+------
 
 Changed
 =======
 
-- (`!21 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/21>`_) Replace NO2 with NOx in CEDs units
 - (`!20 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/20>`_) Updated ``DATA_FORMAT_VERSION`` to ``v0.2.1`` in order to handle extra field
 - (`!19 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/19>`_) Added gwp_context field to primap-hist for easier post processing
 - (`!19 <https://gitlab.com/climate-resource/bookshelf/bookshelf/merge_requests/19>`_) Fixed the uploading of new editions
 
 
 Added
 =====
```

### Comparing `bookshelf-0.2.1/LICENSE` & `bookshelf-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/PKG-INFO` & `bookshelf-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookshelf
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of curated climate data sets
 Home-page: https://gitlab.com/climate-resource/bookshelf/bookshelf
 Author: Jared Lewis
 Author-email: jared.lewis@climate-rescource.com
 License: MIT
 Keywords: data management,climate
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: notebooks
 Provides-Extra: tests
+Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 
 bookshelf
 =========
```

### Comparing `bookshelf-0.2.1/README.rst` & `bookshelf-0.2.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 .. sec-end-index
 
 License
 -------
 
 .. sec-begin-license
 
-Licensed under MIT. See the LICENSE file for more information
+Bookshelf is licensed under MIT. See the LICENSE file for more information. The hosted
+books may be licensed under different conditions. The license for a specific book can
+be found in a Book's metadata.
 
 .. sec-end-license
 .. sec-end-long-description
 
 .. sec-begin-installation
 
 Installation
@@ -115,19 +117,19 @@
 contains metadata about the dataset. These notebooks are stored as plain text Python files
 using the `jupytext <https://jupytext.readthedocs.io/en/latest/>`_ plugin for Jupyter.
 See `notebooks/example.py <https://gitlab.com/climate-resource/bookshelf/-/blob/master/notebooks/example.py>`_
 for an example dataset. As part of the CI, these notebooks are run on each commit to ensure
 that the ``Books`` remain reproducible.
 
 Once the dataset has been developed, it can be deployed to the remote ``BookShelf`` so that
-other users can consume it. The dataset can deployed using the ``save`` CLI as shown below:
+other users can consume it. The dataset can deployed using the ``publish`` CLI as shown below:
 
 .. code:: bash
 
-  bookshelf save my-dataset
+  bookshelf publish my-dataset
 
 This command first builds the ``Book`` in an isolated environment to ensure a reproducible
 build. Once the build is successful, the resulting ``Book``, including ``Resources`` is
 uploaded to an AWS S3 bucket. Deploying datasets requires valid AWS credentials, as well as ``BOOKSHELF_BUCKET`` and
 ``BOOKSHELF_BUCKET_PREFIX`` environment variables. These can be managed using a local
 ``.env`` file.
```

### Comparing `bookshelf-0.2.1/notebooks/README.md` & `bookshelf-0.2.2/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/ceds/ceds.py` & `bookshelf-0.2.2/notebooks/ceds/ceds.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # jupyter:
 #   jupytext:
 #     cell_metadata_filter: -pycharm
 #     text_representation:
 #       extension: .py
 #       format_name: percent
 #       format_version: '1.3'
-#       jupytext_version: 1.14.1
+#       jupytext_version: 1.14.0
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # %% [markdown]
@@ -71,14 +71,28 @@
     ceds_species = ["BC", "CH4", "CO2", "CO", "N2O", "NH3", "NMVOC", "NOx", "OC", "SO2"]
 
 
 # %% [markdown]
 # # Process
 
 # %%
+
+
+def _fix_units(data: scmdata.ScmRun) -> scmdata.ScmRun:
+    data["variable"] = data["variable"].str.replace("SO2", "Sulfur")
+    data["variable"] = data["variable"].str.replace("NMVOC", "VOC")
+    data["unit"] = data["unit"].str.replace("NMVOC", "VOC")
+
+    return (
+        data.set_meta("unit", "kt NOx/yr", variable="Emissions|NOx", log_if_empty=False)
+        .set_meta("unit", "kt OC/yr", variable="Emissions|OC", log_if_empty=False)
+        .set_meta("unit", "kt BC/yr", variable="Emissions|BC", log_if_empty=False)
+    )
+
+
 def read_CEDS_format(fname: str) -> scmdata.ScmRun:
     fname_match = fnmatch.filter(ceds_archive_fnames, "*/" + fname)
 
     if len(fname_match) != 1:
         raise ValueError(f"Could not figure out match: {fname} -> {fname_match}")
     fname = fname_match[0].lstrip("./")
 
@@ -96,72 +110,57 @@
     for c in df.columns:
         if c.startswith("X"):
             columns.append(int(c[1:]))
         else:
             columns.append(c)
     df.columns = columns
 
-    return scmdata.ScmRun(df)
+    data = scmdata.ScmRun(df)
+    data["region"] = data["region"].str.replace("GLOBAL", "World")
+    return _fix_units(data)
 
 
 # %%
-res = []
+ceds_by_country = []
 
 for species in ceds_species:
-    res.append(read_CEDS_format(f"{species}_CEDS_emissions_by_country_*.csv"))
-res = scmdata.run_append(res)
-
-# %%
-res["variable"] = res["variable"].str.replace("SO2", "Sulfur")
-res["variable"] = res["variable"].str.replace("NMVOC", "VOC")
-res["unit"] = res["unit"].str.replace("NMVOC", "VOC")
-res["unit"] = res["unit"].str.replace("NO2", "NOx")
-
-# %%
-oc_emms = res.filter(variable="Emissions|OC")
-oc_emms["unit"] = "kt OC/yr"
-bc_emms = res.filter(variable="Emissions|BC")
-bc_emms["unit"] = "kt BC/yr"
-remainder_emms = res.filter(variable=["Emissions|BC", "Emissions|OC"], keep=False)
-
-res = scmdata.run_append([oc_emms, bc_emms, remainder_emms])
-
-# %%
-res.meta[["variable", "unit"]].drop_duplicates()
+    ceds_by_country.append(
+        read_CEDS_format(f"{species}_CEDS_emissions_by_country_*.csv")
+    )
+ceds_by_country = scmdata.run_append(ceds_by_country)
 
 # %%
-res.timeseries()
+# Check units
+ceds_by_country.meta[["variable", "unit"]].drop_duplicates()
 
 # %%
 # Check country codes
-for c in res.get_unique_meta("region"):
+for c in ceds_by_country.get_unique_meta("region"):
     if pycountry.countries.get(alpha_3=c) is None:
         print(c)
 
 # %%
-res["region"] = res["region"].str.replace("GLOBAL", "World")
-
-# %%
-res
+ceds_by_country
 
 # %%
-book.add_timeseries("by_country", res)
+book.add_timeseries("by_country", ceds_by_country)
 
 
 # %% [markdown]
 # # By country by sector
 
 # %%
 ceds_by_sector = []
 
 for species in ceds_species:
     ceds_by_sector.append(
         read_CEDS_format(f"{species}_CEDS_emissions_by_sector_country_*.csv")
     )
 ceds_by_sector = scmdata.run_append(ceds_by_sector)
+ceds_by_sector.get_unique_meta("region")
 
 # %%
 ceds_by_sector.get_unique_meta("sector")
 
 # %%
 ceds_by_sector
```

### Comparing `bookshelf-0.2.1/notebooks/ceds/ceds.yaml` & `bookshelf-0.2.2/notebooks/ceds/ceds.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: ceds
-edition: 2
+edition: 3
 license: CC-BY
 metadata:
   author: Jared Lewis
   author_email: jared.lewis@climate-resource.com
 
 versions:
   - version: v2021_04_21
```

### Comparing `bookshelf-0.2.1/notebooks/examples/multiple_versions/multiple_versions.py` & `bookshelf-0.2.2/notebooks/examples/multiple_versions/multiple_versions.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/examples/multiple_versions/multiple_versions.yaml` & `bookshelf-0.2.2/notebooks/examples/multiple_versions/multiple_versions.yaml`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/examples/simple/simple.py` & `bookshelf-0.2.2/notebooks/examples/simple/simple.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/primap-hist/primap-hist.py` & `bookshelf-0.2.2/notebooks/primap-hist/primap-hist.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 
 
 # %% [markdown]
 # # Process
 #
 # Minor renames and enrichment
 
+
 # %%
 def rename_variable(v):
     return (
         v.replace("KYOTOGHG", "Kyoto GHG")
         .replace("HFCS", "HFCs")
         .replace("PFCS", "PFCs")
         .replace("FGASES", "F-Gases")
```

### Comparing `bookshelf-0.2.1/notebooks/primap-hist/primap-hist.yaml` & `bookshelf-0.2.2/notebooks/primap-hist/primap-hist.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -33,23 +33,25 @@
       doi: 10.5281/zenodo.7179775
       files:
         - url: doi:10.5281/zenodo.7179775/Guetschow-et-al-2022-PRIMAP-hist_v2.4_no_rounding_11-Oct-2022.csv
           hash: md5:3a40d9abb47fe688295af36301424679
       documentation: https://zenodo.org/record/5494497
       author: Guetshow, Johannes; Pflueger, Mika
       time_domain: [ 1750, 2021 ]
-  - version: v2.4_alt
-    private: true
+  - version: v2.4.1
     dataset:
+      url: https://doi.org/10.5281/zenodo.7585420
+      doi: 10.5281/zenodo.7585420
       files:
-        - url: file://data/Guetschow-et-al-2022-PRIMAP-hist_v2.4_UNFCCC_no_rounding_30-Sep-2022.csv
-          hash: md5:3a40d9abb47fe688295af36301424679
+        - url: doi:10.5281/zenodo.7585420/Guetschow-et-al-2023-PRIMAP-hist_v2.4.1_final_no_rounding_16-Feb-2023.csv
+          hash: md5:c42d12533887c7b419608bce52f635f8
+      documentation: https://zenodo.org/record/7585420
       author: Guetshow, Johannes; Pflueger, Mika
       time_domain: [ 1750, 2021 ]
-  - version: v2.4.1_beta2
+  - version: v2.4.2
     private: true
     dataset:
       files:
-        - url: file://data/Guetschow-et-al-2023-PRIMAP-hist_v2.4.1_beta2_no_rounding_31-Jan-2023.csv
-          hash: md5:3a40d9abb47fe688295af36301424679
+        - url: file://data/Guetschow-et-al-2023a-PRIMAP-hist_v2.4.2_final_no_rounding_09-Mar-2023.csv
+          hash: md5:5d1fe818e7d373920cfca899fe48f7e5
       author: Guetshow, Johannes; Pflueger, Mika
       time_domain: [ 1750, 2021 ]
```

### Comparing `bookshelf-0.2.1/notebooks/rcmip-emissions/rcmip-emissions.py` & `bookshelf-0.2.2/notebooks/rcmip-emissions/rcmip-emissions.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/un-wpp/un-wpp.py` & `bookshelf-0.2.2/notebooks/un-wpp/un-wpp.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/un-wpp/un-wpp.yaml` & `bookshelf-0.2.2/notebooks/un-wpp/un-wpp.yaml`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/wdi/wdi.py` & `bookshelf-0.2.2/notebooks/wdi/wdi.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/notebooks/wdi/wdi.yaml` & `bookshelf-0.2.2/notebooks/wdi/wdi.yaml`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/pyproject.toml` & `bookshelf-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/setup.cfg` & `bookshelf-0.2.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -54,60 +54,67 @@
 	scmdata>=0.14.2
 	pooch
 	boto3
 	importlib-metadata; python_version < '3.8'
 	pydantic
 	datapackage
 	pycountry
+	appdirs
+	python-dotenv
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 notebooks = 
 	notebook
 	matplotlib
 	seaborn
-	python-dotenv
 	papermill
 	jupytext
 tests = 
-	codecov
 	coverage
 	pytest-cov
 	requests_mock
 	pytest>=4.0
 	pytest-mock
 	pytest-xdist
 	moto[s3]
+	%(notebooks)s
+docs = 
+	sphinx
+	sphinx_rtd_theme
+	sphinx-click
 dev = 
 	bandit
 	black == 22.3.0
 	flake8 == 4.0.1
 	isort == 5.5.2
 	mypy
 	pydocstyle
 	pylint >= 2.4.4
 	pre-commit
 	%(notebooks)s
 	%(tests)s
+	%(docs)s
 
 [options.entry_points]
 console_scripts = 
 	bookshelf = bookshelf.cli:main
 
 [flake8]
 max-line-length = 88
 ignore = E203, E266, E501, W503
 
 [isort]
 default_section = THIRDPARTY
 include_trailing_comma = true
 known_first_party = bookshelf
 profile = black
+skip_gitignore = true
 
 [mypy]
 disallow_incomplete_defs = true
 disallow_subclassing_any = true
 ignore_missing_imports = true
 no_implicit_optional = true
 warn_redundant_casts = true
```

### Comparing `bookshelf-0.2.1/src/bookshelf/__init__.py` & `bookshelf-0.2.2/src/bookshelf/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 
 try:
     from importlib.metadata import version as _version
 except ImportError:  # pragma: no cover
     # no recourse if the fallback isn't there either...
-    from importlib_metadata import version as _version  # noqa
+    from importlib_metadata import version as _version  # type: ignore  # noqa
 
 try:
     __version__ = _version("bookshelf")
 except Exception:  # pragma: no cover pylint: disable=broad-except
     # Local copy, not installed with setuptools
     __version__ = "unknown"
```

### Comparing `bookshelf-0.2.1/src/bookshelf/book.py` & `bookshelf-0.2.2/src/bookshelf/book.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
-Book
-
 A Book represents a single versioned dataset. A dataset can contain multiple resources
 each of which are loaded independently.
 """
 import glob
 import json
 import os.path
 import pathlib
-from typing import Any, Dict, List, Optional, Union, cast
+from typing import Any, Dict, Iterable, List, Optional, Union, cast
 
 import datapackage
 import pooch
 import scmdata
 
 from bookshelf.schema import Edition, NotebookMetadata, Version
 from bookshelf.utils import (
@@ -48,25 +46,71 @@
         -------
         str
             Version identification string
         """
         return f"{self.version}_e{self.edition:03}"
 
     @staticmethod
-    def relative_path(
+    def path_parts(
         name: str,
         version: Version,
         edition: Edition,
         fname: Optional[str] = None,
-    ) -> str:
+    ) -> Iterable[str]:
+        """
+        Build the parts needed to unambiguously reference an edition.
+
+        Parameters
+        ----------
+        name
+            Book name
+        version
+            Book version
+        edition
+            Book edition
+        fname
+            If provided, reference a specific file within the data
+        Returns
+        -------
+            Iterable of the parts, which can be joined as needed to get
+            a path.
+        """
         parts = [name, f"{version}_e{edition:03}"]
-        if fname:
+        if fname is not None:
             parts.append(fname)
+        return parts
+
+    @classmethod
+    def relative_path(
+        cls,
+        name: str,
+        version: Version,
+        edition: Edition,
+        fname: Optional[str] = None,
+    ) -> str:
+        """
+        Build the relative path of the edition
 
-        return os.path.join(*parts)
+        Parameters
+        ----------
+        name
+            Book name
+        version
+            Book version
+        edition
+            Book edition
+        fname
+            If provided, reference a specific file within the data
+        Returns
+        -------
+            Relative path to the book or resource within the book
+        """
+        return os.path.join(
+            *cls.path_parts(name=name, version=version, edition=edition, fname=fname)
+        )
 
     def url(self, fname: Optional[str] = None) -> str:
         """
         Get the expected URL for the book
 
         This URL is generated locally using the provided remote bookshelf
 
@@ -78,15 +122,15 @@
         Returns
         -------
         str
             URL
         """
         return build_url(
             self.bookshelf,
-            self.relative_path(self.name, self.version, self.edition, fname),
+            *self.path_parts(self.name, self.version, self.edition, fname),
         )
 
 
 class LocalBook(_Book):
     """
     A local instance of a Book
 
@@ -146,15 +190,15 @@
         """
         return os.path.join(self.local_bookshelf, self.name, self.long_version(), fname)
 
     def as_datapackage(self) -> datapackage.Package:
         """
         Package representation of the book
 
-        :module:`datapackage` is used for handling the metadata. Modifying
+        :mod:`datapackage` is used for handling the metadata. Modifying
         the package also modifies the Book.
 
         Returns
         -------
         :class:`datapackage.Package`
             Metadata about the Book
         """
```

### Comparing `bookshelf-0.2.1/src/bookshelf/cli.py` & `bookshelf-0.2.2/src/bookshelf/cli.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/src/bookshelf/commands/cmd_publish.py` & `bookshelf-0.2.2/src/bookshelf/commands/cmd_publish.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,21 @@
     required=False,
 )
 @click.option(
     "--include-private/--no-include-private",
     help="Run private versions. These will likely fail if the data is not available locally",
     default=False,
 )
-def cli(name: str, version: list[str], include_private: bool) -> None:
+@click.option(
+    "--force",
+    is_flag=True,
+    help="Override the existing published data",
+    default=False,
+)
+def cli(name: str, version: list[str], include_private: bool, force: bool) -> None:
     """
     Build and upload a Book to the Bookshelf
 
     Uploading a Book requires the correct AWS credentials (until an authentication
     scheme is introduced). At Climate Resource we use aws-vault for managing multiple
     sets of AWS credentials. Documentation about the different sources of authentication
     can be found here: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html
@@ -51,11 +57,11 @@
                     output_directory=temp_dir,
                     force=False,
                     version=dataset_version,
                 )
                 logger.info(f"Finish building {name}@{book.long_version()}")
 
                 shelf = BookShelf()
-                shelf.publish(book)
+                shelf.publish(book, force=force)
             except Exception as exc:
                 logger.error(str(exc))
                 raise click.Abort() from exc
```

### Comparing `bookshelf-0.2.1/src/bookshelf/commands/cmd_run.py` & `bookshelf-0.2.2/src/bookshelf/commands/cmd_run.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/src/bookshelf/constants.py` & `bookshelf-0.2.2/src/bookshelf/constants.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/src/bookshelf/errors.py` & `bookshelf-0.2.2/src/bookshelf/errors.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/src/bookshelf/notebook.py` & `bookshelf-0.2.2/src/bookshelf/notebook.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,14 +248,28 @@
     book = shelf.load(short_name, metadata.version, edition=metadata.edition)
 
     logger.info(f"Notebook run successfully with hash: {book.hash()}")
     return book
 
 
 def get_available_versions(name: str, include_private: bool = False) -> list[str]:
+    """
+    Get a list of available versions of a book
+
+    Parameters
+    ----------
+    name
+        Package name
+    include_private
+        If True, also include private versions
+
+    Returns
+    -------
+        List of versions
+    """
     config, _ = _load_nb_config(name)
 
     versions = config.versions
     if not include_private:
         versions = [v for v in versions if not v.private]
 
     return [v.version for v in versions]
```

### Comparing `bookshelf-0.2.1/src/bookshelf/schema.py` & `bookshelf-0.2.2/src/bookshelf/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         Get the latest version for a volume
 
         Returns
         -------
         Version string
         """
         ordered_versions = sorted([v.version for v in self.versions if not v.private])
-        if not len(ordered_versions):
+        if not ordered_versions:
             raise ValueError("No published volumes")
 
         return ordered_versions[-1]
 
     def get_version(self, version: Version) -> List[BookVersion]:
         """
         Get a set of books for a given version
@@ -180,15 +180,15 @@
         return res
 
 
 class ConfigSchema(BaseModel):
     """
     Schema for a given Volume (A collection of Books with the same name)
 
-    A volume can hold multiple versions of the same data (
+    A volume can hold multiple versions of the same data
     """
 
     name: str
     edition: Edition
     description: Optional[str]
     license: str
     source_file: str
```

### Comparing `bookshelf-0.2.1/src/bookshelf/shelf.py` & `bookshelf-0.2.2/src/bookshelf/shelf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
-BookShelf
-
-A BookShelf is a collection of Books
+A BookShelf is a collection of Books that can be queried and fetched as needed.
 """
 import json
 import logging
 import os
 import pathlib
 from typing import Iterable, List, Optional, Tuple, Union, cast
 
@@ -168,15 +166,18 @@
         metadata_fragment = LocalBook.relative_path(
             name, version, edition, "datapackage.json"
         )
         metadata_fname = self.path / metadata_fragment
 
         if not metadata_fname.exists():
             try:
-                url = build_url(self.remote_bookshelf, metadata_fragment)
+                url = build_url(
+                    self.remote_bookshelf,
+                    *LocalBook.path_parts(name, version, edition, "datapackage.json"),
+                )
                 fetch_file(
                     url,
                     local_fname=metadata_fname,
                     known_hash=None,
                     force=force,
                 )
             except requests.exceptions.HTTPError as http_error:
@@ -292,24 +293,29 @@
 
         s3 = boto3.client("s3")  # pylint: disable=invalid-name
         bucket = get_env_var("BUCKET", add_prefix=True)
         prefix = get_env_var("BUCKET_PREFIX", add_prefix=True)
 
         logger.info(f"Beginning to upload {book.name}@{book.version}")
         for resource_file in files:
-            key = os.path.join(
-                prefix, book.name, book.long_version(), os.path.basename(resource_file)
+            key = "/".join(
+                (
+                    prefix,
+                    book.name,
+                    book.long_version(),
+                    os.path.basename(resource_file),
+                )
             )
             _upload_file(s3, bucket, key, resource_file)
 
         # Update the metadata with the latest version information
         # Note that this doesn't have any guardrails and is susceptible to race conditions
         # Shouldn't be a problem for testing, but shouldn't be used in production
         meta_fname = _update_volume_meta(book, self.remote_bookshelf)
-        key = os.path.join(prefix, book.name, os.path.basename(meta_fname))
+        key = "/".join((prefix, book.name, os.path.basename(meta_fname)))
         _upload_file(s3, bucket, key, meta_fname)
 
         logger.info(
             f"Book {book.name}@{book.version} ed.{book.edition} uploaded successfully"
         )
 
     def _resolve_version(
```

### Comparing `bookshelf-0.2.1/src/bookshelf/utils.py` & `bookshelf-0.2.2/src/bookshelf/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,31 +96,31 @@
         fname=local_fname,
         known_hash=known_hash,
         downloader=downloader,
         retry_if_failed=retry_count,
     )
 
 
-def build_url(bookshelf: str, *paths: Union[str, pathlib.Path]) -> str:
+def build_url(bookshelf: str, *paths: str) -> str:
     """
     Build a URL
 
     Parameters
     ----------
     bookshelf: str
         The remote bookshelf
-    paths : list of str or pathlib.Path
+    paths : list of str
         A collection of paths that form the path of the URL
     Returns
     -------
     str
         The merged URL
 
     """
-    return os.path.join(bookshelf, *paths)
+    return "/".join([bookshelf, *paths])
 
 
 def fetch_file(
     url: str,
     local_fname: pathlib.Path,
     known_hash: Optional[str] = None,
     force: Optional[bool] = False,
```

### Comparing `bookshelf-0.2.1/src/bookshelf.egg-info/PKG-INFO` & `bookshelf-0.2.2/src/bookshelf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookshelf
-Version: 0.2.1
+Version: 0.2.2
 Summary: A collection of curated climate data sets
 Home-page: https://gitlab.com/climate-resource/bookshelf/bookshelf
 Author: Jared Lewis
 Author-email: jared.lewis@climate-rescource.com
 License: MIT
 Keywords: data management,climate
 Classifier: Development Status :: 4 - Beta
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: notebooks
 Provides-Extra: tests
+Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 
 bookshelf
 =========
```

### Comparing `bookshelf-0.2.1/src/bookshelf.egg-info/requires.txt` & `bookshelf-0.2.2/src/bookshelf.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 click-log
 scmdata>=0.14.2
 pooch
 boto3
 pydantic
 datapackage
 pycountry
+appdirs
+python-dotenv
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [dev]
 bandit
 black==22.3.0
@@ -18,36 +20,45 @@
 mypy
 pydocstyle
 pylint>=2.4.4
 pre-commit
 notebook
 matplotlib
 seaborn
-python-dotenv
 papermill
 jupytext
-codecov
 coverage
 pytest-cov
 requests_mock
 pytest>=4.0
 pytest-mock
 pytest-xdist
 moto[s3]
+sphinx
+sphinx_rtd_theme
+sphinx-click
+
+[docs]
+sphinx
+sphinx_rtd_theme
+sphinx-click
 
 [notebooks]
 notebook
 matplotlib
 seaborn
-python-dotenv
 papermill
 jupytext
 
 [tests]
-codecov
 coverage
 pytest-cov
 requests_mock
 pytest>=4.0
 pytest-mock
 pytest-xdist
 moto[s3]
+notebook
+matplotlib
+seaborn
+papermill
+jupytext
```

### Comparing `bookshelf-0.2.1/tests/conftest.py` & `bookshelf-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/integration/test_simple.py` & `bookshelf-0.2.2/tests/integration/test_simple.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/notebooks/test_notebooks.py` & `bookshelf-0.2.2/tests/notebooks/test_notebooks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import sys
 import tempfile
 from glob import glob
 
 import pytest
 
 from bookshelf import BookShelf
 from bookshelf.errors import UnknownBook
@@ -12,14 +13,21 @@
     get_notebook_directory,
     run_notebook,
 )
 
 logger = logging.getLogger("test-notebooks")
 
 
+if sys.platform.startswith("win"):
+    # https://gitlab.com/climate-resource/bookshelf/bookshelf/-/issues/23
+    pytest.skip(
+        "skipping notebook tests on windows, see issue !23", allow_module_level=True
+    )
+
+
 def find_notebooks():
     NOTEBOOK_DIRECTORY = get_notebook_directory()
 
     logger.info(f"Looking for notebooks in {NOTEBOOK_DIRECTORY}")
     notebooks = glob(os.path.join(NOTEBOOK_DIRECTORY, "**", "*.py"), recursive=True)
 
     notebook_info = []
```

### Comparing `bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.0.0/leakage_rates_low.csv` & `bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.0.0/leakage_rates_low.csv`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/test-data/v0.1.0/example/v1.1.0/leakage_rates_low.csv` & `bookshelf-0.2.2/tests/test-data/v0.1.0/example/v1.1.0/leakage_rates_low.csv`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.0.0_e001/leakage_rates_low.csv` & `bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.0.0_e001/leakage_rates_low.csv`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/test-data/v0.2.0/example/v1.1.0_e001/leakage_rates_low.csv` & `bookshelf-0.2.2/tests/test-data/v0.2.0/example/v1.1.0_e001/leakage_rates_low.csv`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.0.0_e001/leakage_rates_low.csv` & `bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.0.0_e001/leakage_rates_low.csv`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/test-data/v0.2.1/example/v1.1.0_e001/leakage_rates_low.csv` & `bookshelf-0.2.2/tests/test-data/v0.2.1/example/v1.1.0_e001/leakage_rates_low.csv`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/unit/conftest.py` & `bookshelf-0.2.2/tests/unit/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     fname = os.path.join(TEST_DATA_DIR, fname)
     with open(fname) as fh:
         return fh.read()
 
 
 @pytest.fixture(scope="function", autouse=True)
 def remote_bookshelf(requests_mock, monkeypatch):
-
     prefix = f"https://bookshelf.local/{DATA_FORMAT_VERSION}"
     monkeypatch.setenv("BOOKSHELF_REMOTE", prefix)
 
     class MockRemoteBookshelf:
         def __init__(self):
             self.mocker = requests_mock
             self.meta = {}
```

### Comparing `bookshelf-0.2.1/tests/unit/test_book.py` & `bookshelf-0.2.2/tests/unit/test_book.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/unit/test_cli.py` & `bookshelf-0.2.2/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `bookshelf-0.2.1/tests/unit/test_notebook.py` & `bookshelf-0.2.2/tests/unit/test_notebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         book = run_notebook(
             nb_name,
             output_directory=td,
             version=version,
         )
 
         with pytest.raises(
-            ValueError, match=f"{os.path.join(td, version)} is not empty"
+            ValueError, match=re.escape(f"{os.path.join(td, version)} is not empty")
         ):
             run_notebook(
                 nb_name,
                 output_directory=td,
                 version=version,
             )
         run_notebook(
```

### Comparing `bookshelf-0.2.1/tests/unit/test_shelf.py` & `bookshelf-0.2.2/tests/unit/test_shelf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 import json
 import logging
 import os
 import pathlib
+import platform
 import re
 
 import appdirs
 import boto3
 import boto3.exceptions
 import moto
 import pytest
@@ -50,15 +51,23 @@
 
 def test_local_cache(monkeypatch):
     # Override the local_bookshelf fixture
     monkeypatch.delenv("BOOKSHELF_CACHE_LOCATION")
 
     shelf = BookShelf()
 
-    exp = pathlib.Path(appdirs.user_cache_dir()) / "bookshelf" / DATA_FORMAT_VERSION
+    if platform.system() == "Windows":
+        exp = (
+            pathlib.Path(appdirs.user_cache_dir())
+            / "bookshelf"
+            / "Cache"
+            / DATA_FORMAT_VERSION
+        )
+    else:
+        exp = pathlib.Path(appdirs.user_cache_dir()) / "bookshelf" / DATA_FORMAT_VERSION
     assert shelf.path == exp
 
 
 def test_load_missing(shelf, remote_bookshelf):
     remote_bookshelf.mocker.get(
         f"/{DATA_FORMAT_VERSION}/missing/volume.json", status_code=404
     )
@@ -198,15 +207,17 @@
     # Modify bucket used (this bucket hasn't been created)
     bucket = "test-bucket-wrong"
     monkeypatch.setenv("BOOKSHELF_BUCKET", bucket)
 
     caplog.set_level(logging.ERROR)
 
     book = LocalBook.create_new("new-package", "v1.0.0")
-    with pytest.raises(UploadError, match=f"Failed to upload {book.files()[0]} to s3"):
+    with pytest.raises(
+        UploadError, match=re.escape(f"Failed to upload {book.files()[0]} to s3")
+    ):
         shelf.publish(book)
 
     assert "NoSuchBucket" in caplog.text
     assert bucket in caplog.text
 
 
 def test_publish_existing(shelf, remote_bookshelf):
```

### Comparing `bookshelf-0.2.1/tests/unit/test_utils.py` & `bookshelf-0.2.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

