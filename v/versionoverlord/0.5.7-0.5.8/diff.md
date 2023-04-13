# Comparing `tmp/versionoverlord-0.5.7.tar.gz` & `tmp/versionoverlord-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versionoverlord-0.5.7.tar", last modified: Wed Mar 29 21:40:52 2023, max compression
+gzip compressed data, was "versionoverlord-0.5.8.tar", last modified: Thu Apr 13 18:22:41 2023, max compression
```

## Comparing `versionoverlord-0.5.7.tar` & `versionoverlord-0.5.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.135404 versionoverlord-0.5.7/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 versionoverlord-0.5.7/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45830 2023-03-29 21:40:52.135269 versionoverlord-0.5.7/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5651 2023-03-29 20:46:02.000000 versionoverlord-0.5.7/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-03-29 21:40:52.135441 versionoverlord-0.5.7/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1524 2023-03-29 19:49:19.000000 versionoverlord-0.5.7/setup.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.131697 versionoverlord-0.5.7/versionoverlord/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2402 2023-03-05 20:39:51.000000 versionoverlord-0.5.7/versionoverlord/BaseHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2188 2023-03-29 19:49:28.000000 versionoverlord-0.5.7/versionoverlord/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2032 2023-02-23 17:30:59.000000 versionoverlord-0.5.7/versionoverlord/DisplayVersions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1080 2023-03-05 20:25:19.000000 versionoverlord-0.5.7/versionoverlord/EnvironmentBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      629 2023-03-29 21:30:54.000000 versionoverlord-0.5.7/versionoverlord/FileNameToSlugs.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2245 2023-03-29 21:38:10.000000 versionoverlord-0.5.7/versionoverlord/GitHubAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1642 2023-03-27 15:42:18.000000 versionoverlord-0.5.7/versionoverlord/SlugHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2745 2023-03-27 15:41:21.000000 versionoverlord-0.5.7/versionoverlord/TemplateHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:09:59.000000 versionoverlord-0.5.7/versionoverlord/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.132718 versionoverlord-0.5.7/versionoverlord/circleci/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3292 2023-03-03 01:44:06.000000 versionoverlord-0.5.7/versionoverlord/circleci/HandleCircleCI.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-01 21:02:11.000000 versionoverlord-0.5.7/versionoverlord/circleci/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.133215 versionoverlord-0.5.7/versionoverlord/commands/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1334 2023-03-15 19:55:22.000000 versionoverlord-0.5.7/versionoverlord/commands/CreateSpecification.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1973 2023-03-29 21:23:22.000000 versionoverlord-0.5.7/versionoverlord/commands/QuerySlugs.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3656 2023-03-27 15:42:09.000000 versionoverlord-0.5.7/versionoverlord/commands/UpdateDependencies.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-15 02:24:41.000000 versionoverlord-0.5.7/versionoverlord/commands/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.134369 versionoverlord-0.5.7/versionoverlord/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      164 2023-02-27 00:53:40.000000 versionoverlord-0.5.7/versionoverlord/exceptions/NoFileException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-02-24 16:20:38.000000 versionoverlord-0.5.7/versionoverlord/exceptions/NoGitHubAccessTokenException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      342 2023-02-27 00:59:06.000000 versionoverlord-0.5.7/versionoverlord/exceptions/NoRequirementsTxtsException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-02-27 00:58:06.000000 versionoverlord-0.5.7/versionoverlord/exceptions/NoSetupPyFileException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-03-01 21:16:59.000000 versionoverlord-0.5.7/versionoverlord/exceptions/NotACircleCIProjectException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 versionoverlord-0.5.7/versionoverlord/exceptions/ProjectNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 versionoverlord-0.5.7/versionoverlord/exceptions/ProjectsBaseNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-02-24 16:20:52.000000 versionoverlord-0.5.7/versionoverlord/exceptions/UnknownGitHubRepositoryException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:25:38.000000 versionoverlord-0.5.7/versionoverlord/exceptions/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.134585 versionoverlord-0.5.7/versionoverlord/requirements/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3045 2023-03-02 22:02:08.000000 versionoverlord-0.5.7/versionoverlord/requirements/HandleRequirementsTxt.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-26 22:29:17.000000 versionoverlord-0.5.7/versionoverlord/requirements/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.134779 versionoverlord-0.5.7/versionoverlord/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:25:28.000000 versionoverlord-0.5.7/versionoverlord/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      857 2023-03-12 20:23:35.000000 versionoverlord-0.5.7/versionoverlord/resources/loggingConfiguration.json
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.135047 versionoverlord-0.5.7/versionoverlord/setup/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2648 2023-03-01 21:08:09.000000 versionoverlord-0.5.7/versionoverlord/setup/HandleSetupPy.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:21:11.000000 versionoverlord-0.5.7/versionoverlord/setup/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-29 21:40:52.132470 versionoverlord-0.5.7/versionoverlord.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45830 2023-03-29 21:40:52.000000 versionoverlord-0.5.7/versionoverlord.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1548 2023-03-29 21:40:52.000000 versionoverlord-0.5.7/versionoverlord.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-03-29 21:40:52.000000 versionoverlord-0.5.7/versionoverlord.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      227 2023-03-29 21:40:52.000000 versionoverlord-0.5.7/versionoverlord.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-03-29 21:40:52.000000 versionoverlord-0.5.7/versionoverlord.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       16 2023-03-29 21:40:52.000000 versionoverlord-0.5.7/versionoverlord.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.248697 versionoverlord-0.5.8/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 versionoverlord-0.5.8/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45827 2023-04-13 18:22:41.248554 versionoverlord-0.5.8/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5648 2023-04-07 13:27:31.000000 versionoverlord-0.5.8/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 18:22:41.248734 versionoverlord-0.5.8/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1524 2023-04-13 18:09:11.000000 versionoverlord-0.5.8/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.244903 versionoverlord-0.5.8/versionoverlord/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2402 2023-03-05 20:39:51.000000 versionoverlord-0.5.8/versionoverlord/BaseHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2188 2023-03-29 19:49:28.000000 versionoverlord-0.5.8/versionoverlord/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2032 2023-02-23 17:30:59.000000 versionoverlord-0.5.8/versionoverlord/DisplayVersions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1080 2023-03-05 20:25:19.000000 versionoverlord-0.5.8/versionoverlord/EnvironmentBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      629 2023-03-29 21:30:54.000000 versionoverlord-0.5.8/versionoverlord/FileNameToSlugs.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2245 2023-03-29 21:38:10.000000 versionoverlord-0.5.8/versionoverlord/GitHubAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1642 2023-03-27 15:42:18.000000 versionoverlord-0.5.8/versionoverlord/SlugHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2745 2023-03-27 15:41:21.000000 versionoverlord-0.5.8/versionoverlord/TemplateHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:09:59.000000 versionoverlord-0.5.8/versionoverlord/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.245880 versionoverlord-0.5.8/versionoverlord/circleci/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3292 2023-03-03 01:44:06.000000 versionoverlord-0.5.8/versionoverlord/circleci/HandleCircleCI.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-01 21:02:11.000000 versionoverlord-0.5.8/versionoverlord/circleci/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.246333 versionoverlord-0.5.8/versionoverlord/commands/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1351 2023-04-08 17:49:26.000000 versionoverlord-0.5.8/versionoverlord/commands/CreateSpecification.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1990 2023-04-08 17:50:44.000000 versionoverlord-0.5.8/versionoverlord/commands/QuerySlugs.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3673 2023-04-08 17:51:18.000000 versionoverlord-0.5.8/versionoverlord/commands/UpdateDependencies.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-15 02:24:41.000000 versionoverlord-0.5.8/versionoverlord/commands/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.247492 versionoverlord-0.5.8/versionoverlord/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      164 2023-02-27 00:53:40.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoFileException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-02-24 16:20:38.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoGitHubAccessTokenException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      342 2023-02-27 00:59:06.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoRequirementsTxtsException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-02-27 00:58:06.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoSetupPyFileException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-03-01 21:16:59.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NotACircleCIProjectException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 versionoverlord-0.5.8/versionoverlord/exceptions/ProjectNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 versionoverlord-0.5.8/versionoverlord/exceptions/ProjectsBaseNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-02-24 16:20:52.000000 versionoverlord-0.5.8/versionoverlord/exceptions/UnknownGitHubRepositoryException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:25:38.000000 versionoverlord-0.5.8/versionoverlord/exceptions/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.247713 versionoverlord-0.5.8/versionoverlord/requirements/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3045 2023-03-02 22:02:08.000000 versionoverlord-0.5.8/versionoverlord/requirements/HandleRequirementsTxt.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-26 22:29:17.000000 versionoverlord-0.5.8/versionoverlord/requirements/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.248017 versionoverlord-0.5.8/versionoverlord/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:25:28.000000 versionoverlord-0.5.8/versionoverlord/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      857 2023-03-12 20:23:35.000000 versionoverlord-0.5.8/versionoverlord/resources/loggingConfiguration.json
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.248326 versionoverlord-0.5.8/versionoverlord/setup/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2648 2023-03-01 21:08:09.000000 versionoverlord-0.5.8/versionoverlord/setup/HandleSetupPy.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:21:11.000000 versionoverlord-0.5.8/versionoverlord/setup/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.245650 versionoverlord-0.5.8/versionoverlord.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45827 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1548 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      227 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       16 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/top_level.txt
```

### Comparing `versionoverlord-0.5.7/LICENSE` & `versionoverlord-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/PKG-INFO` & `versionoverlord-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versionoverlord
-Version: 0.5.7
+Version: 0.5.8
 Summary: Dependency Manager
 Home-page: https://github.com/versionoverlord
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -678,15 +678,15 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 
 
 
 ## Rationale
 
-These utilities are meant to solve a problem with related respositories and their dependency relationships
+These utilities are meant to solve a problem with related repositories and their dependency relationships
 
 Projects may have hierarchical dependencies.  See the following [Pyut](https://github.com/hasii2011/PyUt) dependency diagram. 
 
 
 
 ```mermaid
 ---
@@ -770,15 +770,15 @@
 
 
 
 ## Usage
 
 From the above dependency diagram assume the following:
 
-Both the `pyutmodel` and `hasiicommon` respositories have been updated.  We need to update the `ogl` dependencies to match the lastest of both.  Assume both `GITHUB_ACCESS_TOKEN` and `PROJECTS_BASE` are correctly set and `PROJECT` is set to `'ogl'`.  Use the following CLI invocation to create the specification file.
+Both the `pyutmodel` and `hasiicommon` repositories have been updated.  We need to update the `ogl` dependencies to match the latest of both.  Assume both `GITHUB_ACCESS_TOKEN` and `PROJECTS_BASE` are correctly set and `PROJECT` is set to `'ogl'`.  Use the following CLI invocation to create the specification file.
 
 ```
 createSpec -s hasii2011/pyutmodel -s hasii2011/hasiicommon
 ```
 
 The command creates the file `versionSpecification.csv` with the following contents.
```

### Comparing `versionoverlord-0.5.7/README.md` & `versionoverlord-0.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 
 
 
 ## Rationale
 
-These utilities are meant to solve a problem with related respositories and their dependency relationships
+These utilities are meant to solve a problem with related repositories and their dependency relationships
 
 Projects may have hierarchical dependencies.  See the following [Pyut](https://github.com/hasii2011/PyUt) dependency diagram. 
 
 
 
 ```mermaid
 ---
@@ -96,15 +96,15 @@
 
 
 
 ## Usage
 
 From the above dependency diagram assume the following:
 
-Both the `pyutmodel` and `hasiicommon` respositories have been updated.  We need to update the `ogl` dependencies to match the lastest of both.  Assume both `GITHUB_ACCESS_TOKEN` and `PROJECTS_BASE` are correctly set and `PROJECT` is set to `'ogl'`.  Use the following CLI invocation to create the specification file.
+Both the `pyutmodel` and `hasiicommon` repositories have been updated.  We need to update the `ogl` dependencies to match the latest of both.  Assume both `GITHUB_ACCESS_TOKEN` and `PROJECTS_BASE` are correctly set and `PROJECT` is set to `'ogl'`.  Use the following CLI invocation to create the specification file.
 
 ```
 createSpec -s hasii2011/pyutmodel -s hasii2011/hasiicommon
 ```
 
 The command creates the file `versionSpecification.csv` with the following contents.
```

### Comparing `versionoverlord-0.5.7/setup.py` & `versionoverlord-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 DATA_FILES = [
     ('versionoverlord/resources', ['versionoverlord/resources/loggingConfiguration.json']),
 ]
 
 setup(
     name="versionoverlord",
-    version="0.5.7",
+    version="0.5.8",
     author='Humberto A. Sanchez II',
     author_email='humberto.a.sanchez.ii@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Dependency Manager',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -32,17 +32,17 @@
         'versionoverlord.exceptions',
         'versionoverlord.requirements',
         'versionoverlord.resources',
         'versionoverlord.setup'
     ],
     include_package_data=True,
     install_requires=[
-        'PyGithub==1.58.0',
+        'PyGithub==1.58.1',
         'click~=8.1.3',
-        'hasiihelper~=0.1.0',
+        'hasiihelper~=0.2.0',
     ],
     entry_points={
         "console_scripts": [
             "querySlugs=versionoverlord.commands.QuerySlugs:commandHandler",
             "createSpec=versionoverlord.commands.CreateSpecification:commandHandler",
             "updateDeps=versionoverlord.commands.UpdateDependencies:commandHandler",
         ]
```

### Comparing `versionoverlord-0.5.7/versionoverlord/BaseHandler.py` & `versionoverlord-0.5.8/versionoverlord/BaseHandler.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/Common.py` & `versionoverlord-0.5.8/versionoverlord/Common.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/DisplayVersions.py` & `versionoverlord-0.5.8/versionoverlord/DisplayVersions.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/EnvironmentBase.py` & `versionoverlord-0.5.8/versionoverlord/EnvironmentBase.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/FileNameToSlugs.py` & `versionoverlord-0.5.8/versionoverlord/FileNameToSlugs.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/GitHubAdapter.py` & `versionoverlord-0.5.8/versionoverlord/GitHubAdapter.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/SlugHandler.py` & `versionoverlord-0.5.8/versionoverlord/SlugHandler.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/TemplateHandler.py` & `versionoverlord-0.5.8/versionoverlord/TemplateHandler.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/circleci/HandleCircleCI.py` & `versionoverlord-0.5.8/versionoverlord/circleci/HandleCircleCI.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/commands/CreateSpecification.py` & `versionoverlord-0.5.8/versionoverlord/commands/CreateSpecification.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class CreateSpecification:
     def __init__(self):
         self.logger: Logger = getLogger(__name__)
 
 
 @command()
-@version_option(version=f'{__version__}', message='%(version)s')
+@version_option(version=f'{__version__}', message='%(prog)s version %(version)s')
 @option('--slugs', '-s',  multiple=True, required=False, help='Create package update specification')
 def commandHandler(slugs: Tuple[str]):
     """
     \b
     This command creates .csv specification file
     It uses the following environment variables:
     \b
```

### Comparing `versionoverlord-0.5.7/versionoverlord/commands/QuerySlugs.py` & `versionoverlord-0.5.8/versionoverlord/commands/QuerySlugs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from versionoverlord.FileNameToSlugs import FileNameToSlugs
 
 from versionoverlord.SlugHandler import SlugHandler
 from versionoverlord.SlugHandler import Slugs
 
 
 @command()
-@version_option(version=f'{__version__}', message='%(version)s')
+@version_option(version=f'{__version__}', message='%(prog)s version %(version)s')
 @option('--slugs', '-s', required=False, multiple=True, help='GitHub slugs to query')
 @option('--input-file', '-i', required=False,           help='Use input file for slug list')
 def commandHandler(slugs: Tuple[str], input_file):
     """
         \b
         This command reads the repository for each input slug and displays
         their latest release version
```

### Comparing `versionoverlord-0.5.7/versionoverlord/commands/UpdateDependencies.py` & `versionoverlord-0.5.8/versionoverlord/commands/UpdateDependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 updatePackage.newVersion = SemanticVersion(row['NewVersion'])
                 packages.append(updatePackage)
 
         return packages
 
 
 @command()
-@version_option(version=f'{__version__}', message='%(version)s')
+@version_option(version=f'{__version__}', message='%(prog)s version %(version)s')
 @option('--specification', '-s', is_flag=False, flag_value='versionSpecification.csv', default='versionSpecification.csv',
         type=Path(exists=True, path_type=PyPath),
         required=False,
         help='Update the project using a specification file')
 @argument('projectsBase', envvar='PROJECTS_BASE')
 @argument('project', envvar='PROJECT')
 def commandHandler(projectsbase: str, project: str, specification: PyPath):
```

### Comparing `versionoverlord-0.5.7/versionoverlord/requirements/HandleRequirementsTxt.py` & `versionoverlord-0.5.8/versionoverlord/requirements/HandleRequirementsTxt.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/resources/loggingConfiguration.json` & `versionoverlord-0.5.8/versionoverlord/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord/setup/HandleSetupPy.py` & `versionoverlord-0.5.8/versionoverlord/setup/HandleSetupPy.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.7/versionoverlord.egg-info/PKG-INFO` & `versionoverlord-0.5.8/versionoverlord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versionoverlord
-Version: 0.5.7
+Version: 0.5.8
 Summary: Dependency Manager
 Home-page: https://github.com/versionoverlord
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -678,15 +678,15 @@
 
 [![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
 
 
 
 ## Rationale
 
-These utilities are meant to solve a problem with related respositories and their dependency relationships
+These utilities are meant to solve a problem with related repositories and their dependency relationships
 
 Projects may have hierarchical dependencies.  See the following [Pyut](https://github.com/hasii2011/PyUt) dependency diagram. 
 
 
 
 ```mermaid
 ---
@@ -770,15 +770,15 @@
 
 
 
 ## Usage
 
 From the above dependency diagram assume the following:
 
-Both the `pyutmodel` and `hasiicommon` respositories have been updated.  We need to update the `ogl` dependencies to match the lastest of both.  Assume both `GITHUB_ACCESS_TOKEN` and `PROJECTS_BASE` are correctly set and `PROJECT` is set to `'ogl'`.  Use the following CLI invocation to create the specification file.
+Both the `pyutmodel` and `hasiicommon` repositories have been updated.  We need to update the `ogl` dependencies to match the latest of both.  Assume both `GITHUB_ACCESS_TOKEN` and `PROJECTS_BASE` are correctly set and `PROJECT` is set to `'ogl'`.  Use the following CLI invocation to create the specification file.
 
 ```
 createSpec -s hasii2011/pyutmodel -s hasii2011/hasiicommon
 ```
 
 The command creates the file `versionSpecification.csv` with the following contents.
```

### Comparing `versionoverlord-0.5.7/versionoverlord.egg-info/SOURCES.txt` & `versionoverlord-0.5.8/versionoverlord.egg-info/SOURCES.txt`

 * *Files identical despite different names*

