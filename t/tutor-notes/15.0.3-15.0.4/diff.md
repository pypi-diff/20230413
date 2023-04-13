# Comparing `tmp/tutor-notes-15.0.3.tar.gz` & `tmp/tutor-notes-15.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-notes-15.0.3.tar", last modified: Mon Mar 20 18:12:27 2023, max compression
+gzip compressed data, was "dist/tutor-notes-15.0.4.tar", last modified: Thu Apr 13 15:48:20 2023, max compression
```

## Comparing `tutor-notes-15.0.3.tar` & `tutor-notes-15.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4302 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3304 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1641 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutor_notes.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     4302 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutor_notes.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1078 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutor_notes.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutor_notes.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutor_notes.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutor_notes.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutor_notes.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      903 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      217 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)       74 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      275 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      576 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)       47 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      143 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     2867 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/apps/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)     1073 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/templates/notes/apps/settings/tutor.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/build/notes/
--rw-r--r--   0 ci        (1000) ci        (1000)      868 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/templates/notes/build/notes/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)      574 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/templates/notes/tasks/lms/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      797 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/templates/notes/tasks/mysql/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-03-20 18:12:27.000000 tutor-notes-15.0.3/tutornotes/templates/notes/tasks/notes/
--rw-r--r--   0 ci        (1000) ci        (1000)       20 2023-03-20 18:12:17.000000 tutor-notes-15.0.3/tutornotes/templates/notes/tasks/notes/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4302 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3304 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1641 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4302 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1078 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutor_notes.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      903 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      217 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       74 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      275 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      576 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)       47 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      143 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/patches/openedx-lms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     2867 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/apps/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1073 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/apps/settings/tutor.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/build/notes/
+-rw-r--r--   0 ci        (1000) ci        (1000)      868 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/build/notes/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)      574 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      797 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-13 15:48:20.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/notes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       58 2023-04-13 15:48:10.000000 tutor-notes-15.0.4/tutornotes/templates/notes/tasks/notes/init
```

### Comparing `tutor-notes-15.0.3/LICENSE.txt` & `tutor-notes-15.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/PKG-INFO` & `tutor-notes-15.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-notes
-Version: 15.0.3
+Version: 15.0.4
 Summary: A Tutor plugin for student notes
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
```

### Comparing `tutor-notes-15.0.3/README.rst` & `tutor-notes-15.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/setup.py` & `tutor-notes-15.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutor_notes.egg-info/PKG-INFO` & `tutor-notes-15.0.4/tutor_notes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-notes
-Version: 15.0.3
+Version: 15.0.4
 Summary: A Tutor plugin for student notes
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
```

### Comparing `tutor-notes-15.0.3/tutor_notes.egg-info/SOURCES.txt` & `tutor-notes-15.0.4/tutor_notes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/patches/k8s-deployments` & `tutor-notes-15.0.4/tutornotes/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/patches/k8s-jobs` & `tutor-notes-15.0.4/tutornotes/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/patches/local-docker-compose-services` & `tutor-notes-15.0.4/tutornotes/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/plugin.py` & `tutor-notes-15.0.4/tutornotes/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/templates/notes/apps/settings/tutor.py` & `tutor-notes-15.0.4/tutornotes/templates/notes/apps/settings/tutor.py`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/templates/notes/build/notes/Dockerfile` & `tutor-notes-15.0.4/tutornotes/templates/notes/build/notes/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/templates/notes/tasks/lms/init` & `tutor-notes-15.0.4/tutornotes/templates/notes/tasks/lms/init`

 * *Files identical despite different names*

### Comparing `tutor-notes-15.0.3/tutornotes/templates/notes/tasks/mysql/init` & `tutor-notes-15.0.4/tutornotes/templates/notes/tasks/mysql/init`

 * *Files identical despite different names*

