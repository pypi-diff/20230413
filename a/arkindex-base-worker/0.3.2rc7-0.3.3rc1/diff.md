# Comparing `tmp/arkindex-base-worker-0.3.2rc7.tar.gz` & `tmp/arkindex-base-worker-0.3.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.2rc7.tar", last modified: Wed Mar  1 12:57:50 2023, max compression
+gzip compressed data, was "arkindex-base-worker-0.3.3rc1.tar", last modified: Thu Apr 13 07:20:02 2023, max compression
```

## Comparing `arkindex-base-worker-0.3.2rc7.tar` & `arkindex-base-worker-0.3.3rc1.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 12:57:50.773471 arkindex-base-worker-0.3.2rc7/
--rw-r--r--   0 root         (0) root         (0)      248 2023-03-01 12:57:50.773471 arkindex-base-worker-0.3.2rc7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 12:57:50.769471 arkindex-base-worker-0.3.2rc7/arkindex_base_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      248 2023-03-01 12:57:50.000000 arkindex-base-worker-0.3.2rc7/arkindex_base_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1349 2023-03-01 12:57:50.000000 arkindex-base-worker-0.3.2rc7/arkindex_base_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 12:57:50.000000 arkindex-base-worker-0.3.2rc7/arkindex_base_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      320 2023-03-01 12:57:50.000000 arkindex-base-worker-0.3.2rc7/arkindex_base_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-01 12:57:50.000000 arkindex-base-worker-0.3.2rc7/arkindex_base_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 12:57:50.769471 arkindex-base-worker-0.3.2rc7/arkindex_worker/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10890 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15338 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/git.py
--rw-rw-rw-   0 root         (0) root         (0)    13490 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/image.py
--rw-rw-rw-   0 root         (0) root         (0)     9619 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/models.py
--rw-rw-rw-   0 root         (0) root         (0)     8012 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/reporting.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 12:57:50.769471 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/
--rw-rw-rw-   0 root         (0) root         (0)    11675 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15738 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10935 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/classification.py
--rw-rw-rw-   0 root         (0) root         (0)    15909 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/element.py
--rw-rw-rw-   0 root         (0) root         (0)    14657 2023-03-01 11:29:53.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6657 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    11709 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/training.py
--rw-rw-rw-   0 root         (0) root         (0)    18555 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/transcription.py
--rw-rw-rw-   0 root         (0) root         (0)     1460 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/version.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-03-01 12:57:50.773471 arkindex-base-worker-0.3.2rc7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 12:57:50.769471 arkindex-base-worker-0.3.2rc7/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17439 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    21292 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_base_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     8699 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    12961 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 12:57:50.769471 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32744 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    49974 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_elements.py
--rw-rw-rw-   0 root         (0) root         (0)    36695 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    18023 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     8245 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)    68419 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_transcriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10239 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    14944 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_git.py
--rw-rw-rw-   0 root         (0) root         (0)    14356 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     8224 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_reporting.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-03-01 11:19:06.000000 arkindex-base-worker-0.3.2rc7/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.566545 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1304 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-13 07:20:02.000000 arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.566545 arkindex-base-worker-0.3.3rc1/arkindex_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10890 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15338 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/git.py
+-rw-rw-rw-   0 root         (0) root         (0)    13490 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9619 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8012 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/reporting.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.566545 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15723 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10935 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)    19034 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/element.py
+-rw-rw-rw-   0 root         (0) root         (0)    14657 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6657 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    11714 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/training.py
+-rw-rw-rw-   0 root         (0) root         (0)    19105 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/transcription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1460 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      783 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17535 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    21312 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_base_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     8699 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    12961 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:20:02.570545 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32744 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    52801 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    36695 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18023 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     8330 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)    69404 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_transcriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10239 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    14944 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_git.py
+-rw-rw-rw-   0 root         (0) root         (0)    14356 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8224 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2023-04-13 07:17:22.000000 arkindex-base-worker-0.3.3rc1/tests/test_reporting.py
```

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_base_worker.egg-info/SOURCES.txt` & `arkindex-base-worker-0.3.3rc1/arkindex_base_worker.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 arkindex_base_worker.egg-info/top_level.txt
 arkindex_worker/__init__.py
 arkindex_worker/cache.py
 arkindex_worker/git.py
 arkindex_worker/image.py
 arkindex_worker/models.py
 arkindex_worker/reporting.py
-arkindex_worker/utils.py
 arkindex_worker/worker/__init__.py
 arkindex_worker/worker/base.py
 arkindex_worker/worker/classification.py
 arkindex_worker/worker/element.py
 arkindex_worker/worker/entity.py
 arkindex_worker/worker/metadata.py
 arkindex_worker/worker/training.py
@@ -27,15 +26,14 @@
 tests/test_base_worker.py
 tests/test_cache.py
 tests/test_element.py
 tests/test_git.py
 tests/test_image.py
 tests/test_merge.py
 tests/test_reporting.py
-tests/test_utils.py
 tests/test_elements_worker/__init__.py
 tests/test_elements_worker/test_classifications.py
 tests/test_elements_worker/test_cli.py
 tests/test_elements_worker/test_elements.py
 tests/test_elements_worker/test_entities.py
 tests/test_elements_worker/test_metadata.py
 tests/test_elements_worker/test_training.py
```

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/cache.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/git.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/image.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/models.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/models.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/reporting.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/reporting.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/__init__.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                     try:
                         self.update_activity(element.id, ActivityState.Error)
                     except Exception:
                         pass
                 self.report.error(element_id, e)
 
         # Save report as local artifact
-        self.report.save(os.path.join(self.work_dir, "ml_report.json"))
+        self.report.save(self.work_dir / "ml_report.json")
 
         if failed:
             logger.error(
                 "Ran on {} elements: {} completed, {} failed".format(
                     count, count - failed, failed
                 )
             )
```

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/base.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,23 +108,23 @@
         )
 
         # Call potential extra arguments
         self.add_arguments()
 
         # Setup workdir either in Ponos environment or on host's home
         if os.environ.get("PONOS_DATA"):
-            self.work_dir = os.path.join(os.environ["PONOS_DATA"], "current")
+            self.work_dir = Path(os.environ["PONOS_DATA"], "current")
         else:
             # We use the official XDG convention to store file for developers
             # https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html
             xdg_data_home = os.environ.get(
                 "XDG_DATA_HOME", os.path.expanduser("~/.local/share")
             )
-            self.work_dir = os.path.join(xdg_data_home, "arkindex")
-            os.makedirs(self.work_dir, exist_ok=True)
+            self.work_dir = Path(xdg_data_home, "arkindex")
+            self.work_dir.mkdir(parents=True, exist_ok=True)
 
         # Store task ID. This is only available when running in production
         # through a ponos agent
         self.task_id = os.environ.get("PONOS_TASK")
 
         self.worker_run_id = os.environ.get("ARKINDEX_WORKER_RUN_ID")
         if not self.worker_run_id:
@@ -373,15 +373,15 @@
            - the `--model-dir` CLI parameter
 
         :return: Path to the model on disk
         """
         if self.task_id:
             # When running in production with ponos, the agent
             # downloads the model and set it in the current task work dir
-            return Path(self.work_dir)
+            return self.work_dir
         else:
             model_dir = self.config.get("model_dir", self.args.model_dir)
             if model_dir is None:
                 raise ModelNotFoundError(
                     "No path to the model was provided. "
                     "Please provide model_dir either through configuration "
                     "or as CLI argument."
```

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/classification.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/classification.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/element.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/element.py`

 * *Files 16% similar despite different names*

```diff
@@ -277,44 +277,55 @@
 
     def list_element_children(
         self,
         element: Union[Element, CachedElement],
         folder: Optional[bool] = None,
         name: Optional[str] = None,
         recursive: Optional[bool] = None,
+        transcription_worker_version: Optional[Union[str, bool]] = None,
+        transcription_worker_run: Optional[Union[str, bool]] = None,
         type: Optional[str] = None,
         with_classes: Optional[bool] = None,
         with_corpus: Optional[bool] = None,
+        with_metadata: Optional[bool] = None,
         with_has_children: Optional[bool] = None,
         with_zone: Optional[bool] = None,
         worker_version: Optional[Union[str, bool]] = None,
+        worker_run: Optional[Union[str, bool]] = None,
     ) -> Union[Iterable[dict], Iterable[CachedElement]]:
         """
         List children of an element.
 
         :param element: Parent element to find children of.
         :param folder: Restrict to or exclude elements with folder types.
            This parameter is not supported when caching is enabled.
         :param name: Restrict to elements whose name contain a substring (case-insensitive).
            This parameter is not supported when caching is enabled.
         :param recursive: Look for elements recursively (grand-children, etc.)
            This parameter is not supported when caching is enabled.
+        :param transcription_worker_version: Restrict to elements that have a transcription created by a worker version with this UUID.
+           This parameter is not supported when caching is enabled.
+        :param transcription_worker_run: Restrict to elements that have a transcription created by a worker run with this UUID.
+           This parameter is not supported when caching is enabled.
         :param type: Restrict to elements with a specific type slug
            This parameter is not supported when caching is enabled.
         :param with_classes: Include each element's classifications in the response.
            This parameter is not supported when caching is enabled.
         :param with_corpus: Include each element's corpus in the response.
            This parameter is not supported when caching is enabled.
         :param with_has_children: Include the ``has_children`` attribute in the response,
            indicating if this element has child elements of its own.
            This parameter is not supported when caching is enabled.
+        :param with_metadata: Include each element's metadata in the response.
+           This parameter is not supported when caching is enabled.
         :param with_zone: Include the ``zone`` attribute in the response,
            holding the element's image and polygon.
            This parameter is not supported when caching is enabled.
         :param worker_version: Restrict to elements created by a worker version with this UUID.
+        :param worker_run: Restrict to elements created by a worker run with this UUID.
         :return: An iterable of dicts from the ``ListElementChildren`` API endpoint,
            or an iterable of [CachedElement][arkindex_worker.cache.CachedElement] when caching is enabled.
         """
         assert element and isinstance(
             element, (Element, CachedElement)
         ), "element shouldn't be null and should be an Element or CachedElement"
         query_params = {}
@@ -323,57 +334,101 @@
             query_params["folder"] = folder
         if name:
             assert isinstance(name, str), "name should be of type str"
             query_params["name"] = name
         if recursive is not None:
             assert isinstance(recursive, bool), "recursive should be of type bool"
             query_params["recursive"] = recursive
+        if transcription_worker_version is not None:
+            assert isinstance(
+                transcription_worker_version, (str, bool)
+            ), "transcription_worker_version should be of type str or bool"
+            if isinstance(transcription_worker_version, bool):
+                assert (
+                    transcription_worker_version is False
+                ), "if of type bool, transcription_worker_version can only be set to False"
+            query_params["transcription_worker_version"] = transcription_worker_version
+        if transcription_worker_run is not None:
+            assert isinstance(
+                transcription_worker_run, (str, bool)
+            ), "transcription_worker_run should be of type str or bool"
+            if isinstance(transcription_worker_run, bool):
+                assert (
+                    transcription_worker_run is False
+                ), "if of type bool, transcription_worker_run can only be set to False"
+            query_params["transcription_worker_run"] = transcription_worker_run
         if type:
             assert isinstance(type, str), "type should be of type str"
             query_params["type"] = type
         if with_classes is not None:
             assert isinstance(with_classes, bool), "with_classes should be of type bool"
             query_params["with_classes"] = with_classes
         if with_corpus is not None:
             assert isinstance(with_corpus, bool), "with_corpus should be of type bool"
             query_params["with_corpus"] = with_corpus
         if with_has_children is not None:
             assert isinstance(
                 with_has_children, bool
             ), "with_has_children should be of type bool"
             query_params["with_has_children"] = with_has_children
+        if with_metadata is not None:
+            assert isinstance(
+                with_metadata, bool
+            ), "with_metadata should be of type bool"
+            query_params["with_metadata"] = with_metadata
         if with_zone is not None:
             assert isinstance(with_zone, bool), "with_zone should be of type bool"
             query_params["with_zone"] = with_zone
         if worker_version is not None:
             assert isinstance(
                 worker_version, (str, bool)
             ), "worker_version should be of type str or bool"
             if isinstance(worker_version, bool):
                 assert (
                     worker_version is False
                 ), "if of type bool, worker_version can only be set to False"
             query_params["worker_version"] = worker_version
+        if worker_run is not None:
+            assert isinstance(
+                worker_run, (str, bool)
+            ), "worker_run should be of type str or bool"
+            if isinstance(worker_run, bool):
+                assert (
+                    worker_run is False
+                ), "if of type bool, worker_run can only be set to False"
+            query_params["worker_run"] = worker_run
 
         if self.use_cache:
             # Checking that we only received query_params handled by the cache
             assert set(query_params.keys()) <= {
                 "type",
                 "worker_version",
-            }, "When using the local cache, you can only filter by 'type' and/or 'worker_version'"
+                "worker_run",
+            }, "When using the local cache, you can only filter by 'type' and/or 'worker_version' and/or 'worker_run'"
 
             query = CachedElement.select().where(CachedElement.parent_id == element.id)
             if type:
                 query = query.where(CachedElement.type == type)
             if worker_version is not None:
                 # If worker_version=False, filter by manual worker_version e.g. None
-                worker_version_id = worker_version if worker_version else None
-                query = query.where(
-                    CachedElement.worker_version_id == worker_version_id
-                )
+                worker_version_id = worker_version or None
+                if worker_version_id:
+                    query = query.where(
+                        CachedElement.worker_version_id == worker_version_id
+                    )
+                else:
+                    query = query.where(CachedElement.worker_version_id.is_null())
+
+            if worker_run is not None:
+                # If worker_run=False, filter by manual worker_run e.g. None
+                worker_run_id = worker_run or None
+                if worker_run_id:
+                    query = query.where(CachedElement.worker_run_id == worker_run_id)
+                else:
+                    query = query.where(CachedElement.worker_run_id.is_null())
 
             return query
         else:
             children = self.api_client.paginate(
                 "ListElementChildren", id=element.id, **query_params
             )
```

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/entity.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/entity.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/metadata.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/training.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     Remove null attributes from an API body payload
     """
     return {key: value for key, value in kwargs.items() if value is not None}
 
 
 def skip_if_read_only(func):
     """
-    Return shortly in case the read_only attribute is evaluated to True
+    Return shortly in case the is_read_only property is evaluated to True
     """
 
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs):
-        if getattr(self, "read_only", False):
+        if getattr(self, "is_read_only", False):
             logger.warning(
                 "Cannot perform this operation as the worker is in read-only mode"
             )
             return
         return func(self, *args, **kwargs)
 
     return wrapper
```

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/transcription.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/transcription.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,16 @@
                 Required. Polygon of the element.
             text (str)
                 Required. Text of the transcription.
             confidence (float)
                 Required. Confidence score between 0 and 1.
             orientation ([TextOrientation][arkindex_worker.worker.transcription.TextOrientation])
                 Optional. Orientation of the transcription's text.
+            element_confidence (float)
+                Optional. Confidence score of the element between 0 and 1.
 
         :returns: A list of dicts as returned by the ``CreateElementTranscriptions`` API endpoint.
         """
         assert element and isinstance(
             element, (Element, CachedElement)
         ), "element shouldn't be null and should be an Element or CachedElement"
         assert sub_element_type and isinstance(
@@ -274,14 +276,20 @@
             ), f"Transcription at index {index} in transcriptions: polygon should have at least three points"
             assert all(
                 isinstance(point, list) and len(point) == 2 for point in polygon
             ), f"Transcription at index {index} in transcriptions: polygon points should be lists of two items"
             assert all(
                 isinstance(coord, (int, float)) for point in polygon for coord in point
             ), f"Transcription at index {index} in transcriptions: polygon points should be lists of two numbers"
+
+            element_confidence = transcription.get("element_confidence")
+            assert element_confidence is None or (
+                isinstance(element_confidence, float) and 0 <= element_confidence <= 1
+            ), f"Transcription at index {index} in transcriptions: element_confidence should be either null or a float in [0..1] range"
+
         if self.is_read_only:
             logger.warning(
                 "Cannot create transcriptions as this worker is in read-only mode"
             )
             return
 
         annotations = self.request(
@@ -323,14 +331,15 @@
                             {
                                 "id": annotation["element_id"],
                                 "parent_id": element.id,
                                 "type": sub_element_type,
                                 "image_id": element.image_id,
                                 "polygon": transcription["polygon"],
                                 "worker_run_id": self.worker_run_id,
+                                "confidence": transcription.get("element_confidence"),
                             }
                         )
 
                     created_ids.add(annotation["element_id"])
 
                 transcriptions_to_insert.append(
                     {
```

### Comparing `arkindex-base-worker-0.3.2rc7/arkindex_worker/worker/version.py` & `arkindex-base-worker-0.3.3rc1/arkindex_worker/worker/version.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/setup.py` & `arkindex-base-worker-0.3.3rc1/setup.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/conftest.py` & `arkindex-base-worker-0.3.3rc1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,21 +330,23 @@
     )
     CachedElement.create(
         id=UUID("22222222-2222-2222-2222-222222222222"),
         parent_id=UUID("12341234-1234-1234-1234-123412341234"),
         type="page",
         polygon="[[1, 1], [2, 2], [2, 1], [1, 2]]",
         worker_version_id=UUID("56785678-5678-5678-5678-567856785678"),
+        worker_run_id=UUID("56785678-5678-5678-5678-567856785678"),
     )
     CachedElement.create(
         id=UUID("33333333-3333-3333-3333-333333333333"),
         parent_id=UUID("12341234-1234-1234-1234-123412341234"),
         type="paragraph",
         polygon="[[1, 1], [2, 2], [2, 1], [1, 2]]",
         worker_version_id=None,
+        worker_run_id=None,
     )
     assert CachedElement.select().count() == 3
 
 
 @pytest.fixture
 def mock_cached_transcriptions():
     """Insert few transcriptions in local cache, on a shared element"""
```

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_base_worker.py` & `arkindex-base-worker-0.3.3rc1/tests/test_base_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,38 +13,38 @@
 from arkindex_worker.worker import BaseWorker
 from arkindex_worker.worker.base import ModelNotFoundError
 
 
 def test_init_default_local_share(monkeypatch):
     worker = BaseWorker()
 
-    assert worker.work_dir == os.path.expanduser("~/.local/share/arkindex")
+    assert str(worker.work_dir) == os.path.expanduser("~/.local/share/arkindex")
 
 
 def test_init_default_xdg_data_home(monkeypatch):
     path = str(Path(__file__).absolute().parent)
     monkeypatch.setenv("XDG_DATA_HOME", path)
     worker = BaseWorker()
 
-    assert worker.work_dir == f"{path}/arkindex"
+    assert str(worker.work_dir) == f"{path}/arkindex"
 
 
 def test_init_with_local_cache(monkeypatch):
     worker = BaseWorker(support_cache=True)
 
-    assert worker.work_dir == os.path.expanduser("~/.local/share/arkindex")
+    assert str(worker.work_dir) == os.path.expanduser("~/.local/share/arkindex")
     assert worker.support_cache is True
 
 
 def test_init_var_ponos_data_given(monkeypatch):
     path = str(Path(__file__).absolute().parent)
     monkeypatch.setenv("PONOS_DATA", path)
     worker = BaseWorker()
 
-    assert worker.work_dir == f"{path}/current"
+    assert str(worker.work_dir) == f"{path}/current"
 
 
 def test_init_var_worker_run_id_missing(monkeypatch):
     monkeypatch.setattr(sys, "argv", ["worker"])
     monkeypatch.delenv("ARKINDEX_WORKER_RUN_ID")
     worker = BaseWorker()
     worker.args = worker.parser.parse_args()
```

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_cache.py` & `arkindex-base-worker-0.3.3rc1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_element.py` & `arkindex-base-worker-0.3.3rc1/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_classifications.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_cli.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_elements.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1310,34 +1310,63 @@
         mock_elements_worker.list_element_children(
             element=elt,
             with_zone="not bool",
         )
     assert str(e.value) == "with_zone should be of type bool"
 
 
-def test_list_element_children_wrong_worker_version(mock_elements_worker):
+def test_list_element_children_wrong_with_metadata(mock_elements_worker):
     elt = Element({"id": "12341234-1234-1234-1234-123412341234"})
 
     with pytest.raises(AssertionError) as e:
         mock_elements_worker.list_element_children(
             element=elt,
-            worker_version=1234,
+            with_metadata="not bool",
         )
-    assert str(e.value) == "worker_version should be of type str or bool"
+    assert str(e.value) == "with_metadata should be of type bool"
 
 
-def test_list_element_children_wrong_bool_worker_version(mock_elements_worker):
+@pytest.mark.parametrize(
+    "param, value",
+    (
+        ("worker_version", 1234),
+        ("worker_run", 1234),
+        ("transcription_worker_version", 1234),
+        ("transcription_worker_run", 1234),
+    ),
+)
+def test_list_element_children_wrong_worker_version(mock_elements_worker, param, value):
+    elt = Element({"id": "12341234-1234-1234-1234-123412341234"})
+
+    with pytest.raises(AssertionError) as e:
+        mock_elements_worker.list_element_children(
+            element=elt,
+            **{param: value},
+        )
+    assert str(e.value) == f"{param} should be of type str or bool"
+
+
+@pytest.mark.parametrize(
+    "param",
+    (
+        ("worker_version"),
+        ("worker_run"),
+        ("transcription_worker_version"),
+        ("transcription_worker_run"),
+    ),
+)
+def test_list_element_children_wrong_bool_worker_version(mock_elements_worker, param):
     elt = Element({"id": "12341234-1234-1234-1234-123412341234"})
 
     with pytest.raises(AssertionError) as e:
         mock_elements_worker.list_element_children(
             element=elt,
-            worker_version=True,
+            **{param: True},
         )
-    assert str(e.value) == "if of type bool, worker_version can only be set to False"
+    assert str(e.value) == f"if of type bool, {param} can only be set to False"
 
 
 def test_list_element_children_api_error(responses, mock_elements_worker):
     elt = Element({"id": "12341234-1234-1234-1234-123412341234"})
     responses.add(
         responses.GET,
         "http://testserver/api/v1/elements/12341234-1234-1234-1234-123412341234/children/",
@@ -1483,26 +1512,69 @@
         (
             "GET",
             "http://testserver/api/v1/elements/12341234-1234-1234-1234-123412341234/children/?worker_version=False",
         ),
     ]
 
 
+def test_list_element_children_manual_worker_run(responses, mock_elements_worker):
+    elt = Element({"id": "12341234-1234-1234-1234-123412341234"})
+    expected_children = [
+        {
+            "id": "0000",
+            "type": "page",
+            "name": "Test",
+            "corpus": {},
+            "thumbnail_url": None,
+            "zone": {},
+            "best_classes": None,
+            "has_children": None,
+            "worker_version_id": None,
+            "worker_run_id": None,
+        }
+    ]
+    responses.add(
+        responses.GET,
+        "http://testserver/api/v1/elements/12341234-1234-1234-1234-123412341234/children/?worker_run=False",
+        status=200,
+        json={
+            "count": 1,
+            "next": None,
+            "results": expected_children,
+        },
+    )
+
+    for idx, child in enumerate(
+        mock_elements_worker.list_element_children(element=elt, worker_run=False)
+    ):
+        assert child == expected_children[idx]
+
+    assert len(responses.calls) == len(BASE_API_CALLS) + 1
+    assert [
+        (call.request.method, call.request.url) for call in responses.calls
+    ] == BASE_API_CALLS + [
+        (
+            "GET",
+            "http://testserver/api/v1/elements/12341234-1234-1234-1234-123412341234/children/?worker_run=False",
+        ),
+    ]
+
+
 def test_list_element_children_with_cache_unhandled_param(
     mock_elements_worker_with_cache,
 ):
     elt = Element({"id": "12341234-1234-1234-1234-123412341234"})
 
     with pytest.raises(AssertionError) as e:
         mock_elements_worker_with_cache.list_element_children(
             element=elt, with_corpus=True
         )
     assert (
         str(e.value)
-        == "When using the local cache, you can only filter by 'type' and/or 'worker_version'"
+        == "When using the local cache, you can only filter by 'type' and/or 'worker_version' and/or 'worker_run'"
     )
 
 
 @pytest.mark.parametrize(
     "filters, expected_ids",
     (
         # Filter on element should give all elements inserted
@@ -1548,14 +1620,33 @@
         (
             {
                 "element": CachedElement(id="12341234-1234-1234-1234-123412341234"),
                 "worker_version": False,
             },
             ("33333333-3333-3333-3333-333333333333",),
         ),
+        # Filter on element and worker run should give second
+        (
+            {
+                "element": CachedElement(id="12341234-1234-1234-1234-123412341234"),
+                "worker_run": "56785678-5678-5678-5678-567856785678",
+            },
+            ("22222222-2222-2222-2222-222222222222",),
+        ),
+        # Filter on element, manual worker run should give first and third
+        (
+            {
+                "element": CachedElement(id="12341234-1234-1234-1234-123412341234"),
+                "worker_run": False,
+            },
+            (
+                "11111111-1111-1111-1111-111111111111",
+                "33333333-3333-3333-3333-333333333333",
+            ),
+        ),
     ),
 )
 def test_list_element_children_with_cache(
     responses,
     mock_elements_worker_with_cache,
     mock_cached_elements,
     filters,
```

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_entities.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_metadata.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_training.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,18 @@
         ("update_model_version"),
         ("upload_to_s3"),
         ("validate_model_version"),
     ],
 )
 def test_training_mixin_read_only(mock_training_worker, method, caplog):
     """All operations related to models versions returns early if the worker is configured as read only"""
-    mock_training_worker.read_only = True
+    # Set worker in read_only mode
+    mock_training_worker.worker_run_id = None
+    assert mock_training_worker.is_read_only
+
     assert mock_training_worker.model_version is None
     getattr(mock_training_worker, method)()
     assert mock_training_worker.model_version is None
     assert [(level, message) for _, level, message in caplog.record_tuples] == [
         (
             logging.WARNING,
             "Cannot perform this operation as the worker is in read-only mode",
```

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_transcriptions.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_transcriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         "confidence": 0.5,
         "text": "The",
     },
     {
         "polygon": [[0, 0], [2000, 0], [2000, 3000], [0, 3000]],
         "confidence": 0.75,
         "text": "first",
+        "element_confidence": 0.75,
     },
     {
         "polygon": [[1000, 300], [1200, 300], [1200, 500], [1000, 500]],
         "confidence": 0.9,
         "text": "line",
     },
 ]
@@ -1240,14 +1241,37 @@
             ],
         )
         assert (
             str(e.value)
             == "Transcription at index 1 in transcriptions: orientation shouldn't be null and should be of type TextOrientation"
         )
 
+    with pytest.raises(AssertionError) as e:
+        mock_elements_worker.create_element_transcriptions(
+            element=elt,
+            sub_element_type="page",
+            transcriptions=[
+                {
+                    "polygon": [[0, 0], [2000, 0], [2000, 3000], [0, 3000]],
+                    "confidence": 0.75,
+                    "text": "The",
+                },
+                {
+                    "polygon": [[100, 150], [700, 150], [700, 200], [100, 200]],
+                    "confidence": 0.75,
+                    "text": "word",
+                    "element_confidence": "not a confidence",
+                },
+            ],
+        )
+    assert (
+        str(e.value)
+        == "Transcription at index 1 in transcriptions: element_confidence should be either null or a float in [0..1] range"
+    )
+
 
 def test_create_element_transcriptions_api_error(responses, mock_elements_worker):
     elt = Element({"id": "12341234-1234-1234-1234-123412341234"})
     responses.add(
         responses.POST,
         f"http://testserver/api/v1/element/{elt.id}/transcriptions/bulk/",
         status=500,
@@ -1322,14 +1346,15 @@
                 "orientation": TextOrientation.HorizontalLeftToRight.value,
             },
             {
                 "polygon": [[0, 0], [2000, 0], [2000, 3000], [0, 3000]],
                 "confidence": 0.75,
                 "text": "first",
                 "orientation": TextOrientation.HorizontalLeftToRight.value,
+                "element_confidence": 0.75,
             },
             {
                 "polygon": [[1000, 300], [1200, 300], [1200, 500], [1000, 500]],
                 "confidence": 0.9,
                 "text": "line",
                 "orientation": TextOrientation.HorizontalLeftToRight.value,
             },
@@ -1407,14 +1432,15 @@
                 "orientation": TextOrientation.HorizontalLeftToRight.value,
             },
             {
                 "polygon": [[0, 0], [2000, 0], [2000, 3000], [0, 3000]],
                 "confidence": 0.75,
                 "text": "first",
                 "orientation": TextOrientation.HorizontalLeftToRight.value,
+                "element_confidence": 0.75,
             },
             {
                 "polygon": [[1000, 300], [1200, 300], [1200, 500], [1000, 500]],
                 "confidence": 0.9,
                 "text": "line",
                 "orientation": TextOrientation.HorizontalLeftToRight.value,
             },
@@ -1450,14 +1476,15 @@
         ),
         CachedElement(
             id=UUID("22222222-2222-2222-2222-222222222222"),
             parent_id=UUID("12341234-1234-1234-1234-123412341234"),
             type="page",
             polygon="[[0, 0], [2000, 0], [2000, 3000], [0, 3000]]",
             worker_run_id=UUID("56785678-5678-5678-5678-567856785678"),
+            confidence=0.75,
         ),
     ]
     assert list(CachedTranscription.select()) == [
         CachedTranscription(
             id=UUID("56785678-5678-5678-5678-567856785678"),
             element_id=UUID("11111111-1111-1111-1111-111111111111"),
             text="The",
```

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_elements_worker/test_worker.py` & `arkindex-base-worker-0.3.3rc1/tests/test_elements_worker/test_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_git.py` & `arkindex-base-worker-0.3.3rc1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_image.py` & `arkindex-base-worker-0.3.3rc1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_merge.py` & `arkindex-base-worker-0.3.3rc1/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.2rc7/tests/test_reporting.py` & `arkindex-base-worker-0.3.3rc1/tests/test_reporting.py`

 * *Files identical despite different names*

