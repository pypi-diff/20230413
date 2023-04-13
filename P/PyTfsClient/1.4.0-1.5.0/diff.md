# Comparing `tmp/PyTfsClient-1.4.0.tar.gz` & `tmp/PyTfsClient-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PyTfsClient-1.4.0.tar", last modified: Tue Apr  4 22:00:08 2023, max compression
+gzip compressed data, was "dist\PyTfsClient-1.5.0.tar", last modified: Thu Apr 13 20:16:44 2023, max compression
```

## Comparing `PyTfsClient-1.4.0.tar` & `PyTfsClient-1.5.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.669295 PyTfsClient-1.4.0/
--rw-rw-rw-   0        0        0      642 2023-04-04 22:00:08.669295 PyTfsClient-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1606 2023-04-02 15:45:08.000000 PyTfsClient-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-04 22:00:08.669295 PyTfsClient-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1437 2023-04-04 21:59:45.000000 PyTfsClient-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.360852 PyTfsClient-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.470985 PyTfsClient-1.4.0/src/PyTfsClient.egg-info/
--rw-rw-rw-   0        0        0      642 2023-04-04 22:00:07.000000 PyTfsClient-1.4.0/src/PyTfsClient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2049 2023-04-04 22:00:07.000000 PyTfsClient-1.4.0/src/PyTfsClient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 22:00:07.000000 PyTfsClient-1.4.0/src/PyTfsClient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-02 15:09:42.000000 PyTfsClient-1.4.0/src/PyTfsClient.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-04-04 22:00:07.000000 PyTfsClient-1.4.0/src/PyTfsClient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-04 22:00:07.000000 PyTfsClient-1.4.0/src/PyTfsClient.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.525728 PyTfsClient-1.4.0/src/pytfsclient/
--rw-rw-rw-   0        0        0        0 2022-03-04 20:05:30.000000 PyTfsClient-1.4.0/src/pytfsclient/__init__.py
--rw-rw-rw-   0        0        0     2646 2023-03-29 19:42:52.000000 PyTfsClient-1.4.0/src/pytfsclient/client_connection.py
--rw-rw-rw-   0        0        0     3134 2023-03-29 19:42:41.000000 PyTfsClient-1.4.0/src/pytfsclient/client_factory.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.542233 PyTfsClient-1.4.0/src/pytfsclient/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:13:58.000000 PyTfsClient-1.4.0/src/pytfsclient/models/__init__.py
--rw-rw-rw-   0        0        0      105 2023-03-22 09:45:37.000000 PyTfsClient-1.4.0/src/pytfsclient/models/client_error.py
--rw-rw-rw-   0        0        0      720 2023-04-02 16:30:27.000000 PyTfsClient-1.4.0/src/pytfsclient/models/deprecated.py
--rw-rw-rw-   0        0        0      700 2023-04-02 16:30:17.000000 PyTfsClient-1.4.0/src/pytfsclient/models/obsolete.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.562713 PyTfsClient-1.4.0/src/pytfsclient/models/project/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:43:11.000000 PyTfsClient-1.4.0/src/pytfsclient/models/project/__init__.py
--rw-rw-rw-   0        0        0     1554 2023-03-29 17:33:25.000000 PyTfsClient-1.4.0/src/pytfsclient/models/project/tfs_project.py
--rw-rw-rw-   0        0        0     1281 2023-03-22 16:38:20.000000 PyTfsClient-1.4.0/src/pytfsclient/models/project/tfs_team.py
--rw-rw-rw-   0        0        0     1658 2023-04-03 18:00:27.000000 PyTfsClient-1.4.0/src/pytfsclient/models/project/tfs_team_member.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.586284 PyTfsClient-1.4.0/src/pytfsclient/models/workitems/
--rw-rw-rw-   0        0        0        0 2023-03-22 19:36:56.000000 PyTfsClient-1.4.0/src/pytfsclient/models/workitems/__init__.py
--rw-rw-rw-   0        0        0      356 2023-03-22 19:51:06.000000 PyTfsClient-1.4.0/src/pytfsclient/models/workitems/tfs_update_relations_result.py
--rw-rw-rw-   0        0        0     1307 2023-03-28 19:56:14.000000 PyTfsClient-1.4.0/src/pytfsclient/models/workitems/tfs_wiql_result.py
--rw-rw-rw-   0        0        0     7526 2023-04-04 21:58:09.000000 PyTfsClient-1.4.0/src/pytfsclient/models/workitems/tfs_workitem.py
--rw-rw-rw-   0        0        0     4442 2023-04-04 18:19:59.000000 PyTfsClient-1.4.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py
--rw-rw-rw-   0        0        0     2486 2023-03-22 20:02:12.000000 PyTfsClient-1.4.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.595999 PyTfsClient-1.4.0/src/pytfsclient/services/
--rw-rw-rw-   0        0        0        0 2023-03-21 17:34:23.000000 PyTfsClient-1.4.0/src/pytfsclient/services/__init__.py
--rw-rw-rw-   0        0        0      816 2023-03-29 19:49:19.000000 PyTfsClient-1.4.0/src/pytfsclient/services/base_client.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.612455 PyTfsClient-1.4.0/src/pytfsclient/services/helpers/
--rw-rw-rw-   0        0        0        0 2023-03-26 17:08:24.000000 PyTfsClient-1.4.0/src/pytfsclient/services/helpers/__init__.py
--rw-rw-rw-   0        0        0      296 2023-03-22 07:33:30.000000 PyTfsClient-1.4.0/src/pytfsclient/services/helpers/batch_iterable.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.614572 PyTfsClient-1.4.0/src/pytfsclient/services/http/
--rw-rw-rw-   0        0        0        0 2023-03-21 17:05:15.000000 PyTfsClient-1.4.0/src/pytfsclient/services/http/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-03-29 16:55:45.000000 PyTfsClient-1.4.0/src/pytfsclient/services/http/http_client.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.622588 PyTfsClient-1.4.0/src/pytfsclient/services/mention_client/
--rw-rw-rw-   0        0        0        0 2023-03-26 17:11:25.000000 PyTfsClient-1.4.0/src/pytfsclient/services/mention_client/__init__.py
--rw-rw-rw-   0        0        0     1551 2023-03-28 16:41:22.000000 PyTfsClient-1.4.0/src/pytfsclient/services/mention_client/mention_client.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.630582 PyTfsClient-1.4.0/src/pytfsclient/services/project_client/
--rw-rw-rw-   0        0        0        0 2023-03-26 17:14:04.000000 PyTfsClient-1.4.0/src/pytfsclient/services/project_client/__init__.py
--rw-rw-rw-   0        0        0    11100 2023-03-29 19:50:06.000000 PyTfsClient-1.4.0/src/pytfsclient/services/project_client/project_client.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.640180 PyTfsClient-1.4.0/src/pytfsclient/services/workitem_client/
--rw-rw-rw-   0        0        0        0 2023-03-26 17:14:13.000000 PyTfsClient-1.4.0/src/pytfsclient/services/workitem_client/__init__.py
--rw-rw-rw-   0        0        0    21208 2023-04-04 21:50:06.000000 PyTfsClient-1.4.0/src/pytfsclient/services/workitem_client/workitem_client.py
--rw-rw-rw-   0        0        0     2674 2023-04-02 12:54:07.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_client.py
--rw-rw-rw-   0        0        0     2904 2023-04-02 16:36:55.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_client_factory.py
--rw-rw-rw-   0        0        0     4187 2023-04-02 12:57:01.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_project_client.py
--rw-rw-rw-   0        0        0     4527 2023-04-01 16:47:59.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_project_model.py
--rw-rw-rw-   0        0        0     1042 2023-04-02 12:57:49.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_wiql_model.py
--rw-rw-rw-   0        0        0    13483 2023-04-02 12:58:05.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_workitem_client.py
--rw-rw-rw-   0        0        0     6809 2023-04-02 15:03:03.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_workitem_model.py
--rw-rw-rw-   0        0        0     3074 2023-04-02 14:57:56.000000 PyTfsClient-1.4.0/src/pytfsclient/tfs_workitem_relation_model.py
-drwxrwxrwx   0        0        0        0 2023-04-04 22:00:08.665331 PyTfsClient-1.4.0/test/
--rw-rw-rw-   0        0        0     5924 2023-04-02 15:05:35.000000 PyTfsClient-1.4.0/test/test_backward_compatibility.py
--rw-rw-rw-   0        0        0     1052 2023-04-03 18:05:59.000000 PyTfsClient-1.4.0/test/test_client_connection.py
--rw-rw-rw-   0        0        0     1361 2023-04-01 11:28:49.000000 PyTfsClient-1.4.0/test/test_http_client_auth.py
--rw-rw-rw-   0        0        0     4568 2023-04-01 12:09:54.000000 PyTfsClient-1.4.0/test/test_http_client_basic.py
--rw-rw-rw-   0        0        0     9906 2023-04-04 21:57:30.000000 PyTfsClient-1.4.0/test/test_integration.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.924593 PyTfsClient-1.5.0/
+-rw-rw-rw-   0        0        0      642 2023-04-13 20:16:44.924593 PyTfsClient-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 20:16:44.932733 PyTfsClient-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1437 2023-04-13 20:16:37.000000 PyTfsClient-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.590897 PyTfsClient-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.691203 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/
+-rw-rw-rw-   0        0        0      642 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2049 2023-04-13 20:16:44.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-02 15:09:42.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-13 20:16:43.000000 PyTfsClient-1.5.0/src/PyTfsClient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.747708 PyTfsClient-1.5.0/src/pytfsclient/
+-rw-rw-rw-   0        0        0        0 2022-03-04 20:05:30.000000 PyTfsClient-1.5.0/src/pytfsclient/__init__.py
+-rw-rw-rw-   0        0        0     3536 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/client_connection.py
+-rw-rw-rw-   0        0        0     6046 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/client_factory.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.787366 PyTfsClient-1.5.0/src/pytfsclient/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:13:58.000000 PyTfsClient-1.5.0/src/pytfsclient/models/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/client_error.py
+-rw-rw-rw-   0        0        0      720 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/deprecated.py
+-rw-rw-rw-   0        0        0      700 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/obsolete.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.804530 PyTfsClient-1.5.0/src/pytfsclient/models/project/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:43:11.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/__init__.py
+-rw-rw-rw-   0        0        0     2628 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_project.py
+-rw-rw-rw-   0        0        0     1925 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_team.py
+-rw-rw-rw-   0        0        0     3082 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_team_member.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.836623 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/
+-rw-rw-rw-   0        0        0        0 2023-03-22 19:36:56.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/__init__.py
+-rw-rw-rw-   0        0        0      364 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_update_relations_result.py
+-rw-rw-rw-   0        0        0     1816 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_wiql_result.py
+-rw-rw-rw-   0        0        0     8989 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem.py
+-rw-rw-rw-   0        0        0     6842 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem_changes.py
+-rw-rw-rw-   0        0        0     3829 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.844616 PyTfsClient-1.5.0/src/pytfsclient/services/
+-rw-rw-rw-   0        0        0        0 2023-03-21 17:34:23.000000 PyTfsClient-1.5.0/src/pytfsclient/services/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/base_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.850873 PyTfsClient-1.5.0/src/pytfsclient/services/helpers/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/helpers/__init__.py
+-rw-rw-rw-   0        0        0      303 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/helpers/batch_iterable.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.863565 PyTfsClient-1.5.0/src/pytfsclient/services/http/
+-rw-rw-rw-   0        0        0        0 2023-03-21 17:05:15.000000 PyTfsClient-1.5.0/src/pytfsclient/services/http/__init__.py
+-rw-rw-rw-   0        0        0     5035 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/http/http_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.873850 PyTfsClient-1.5.0/src/pytfsclient/services/mention_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/mention_client/__init__.py
+-rw-rw-rw-   0        0        0     2302 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/mention_client/mention_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.887364 PyTfsClient-1.5.0/src/pytfsclient/services/project_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/project_client/__init__.py
+-rw-rw-rw-   0        0        0    13722 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/project_client/project_client.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.896489 PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/
+-rw-rw-rw-   0        0        0        0 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/__init__.py
+-rw-rw-rw-   0        0        0    26102 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/workitem_client.py
+-rw-rw-rw-   0        0        0     2674 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_client.py
+-rw-rw-rw-   0        0        0     2904 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_client_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_project_client.py
+-rw-rw-rw-   0        0        0     4527 2023-04-01 16:47:59.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_project_model.py
+-rw-rw-rw-   0        0        0     1042 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_wiql_model.py
+-rw-rw-rw-   0        0        0    13483 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_client.py
+-rw-rw-rw-   0        0        0     6809 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_model.py
+-rw-rw-rw-   0        0        0     3074 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_relation_model.py
+drwxrwxrwx   0        0        0        0 2023-04-13 20:16:44.922271 PyTfsClient-1.5.0/test/
+-rw-rw-rw-   0        0        0     5924 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_backward_compatibility.py
+-rw-rw-rw-   0        0        0     1052 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_client_connection.py
+-rw-rw-rw-   0        0        0     1361 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_http_client_auth.py
+-rw-rw-rw-   0        0        0     4568 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_http_client_basic.py
+-rw-rw-rw-   0        0        0     9903 2023-04-13 20:16:25.000000 PyTfsClient-1.5.0/test/test_integration.py
```

### Comparing `PyTfsClient-1.4.0/PKG-INFO` & `PyTfsClient-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTfsClient
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems
 Home-page: https://github.com/TopTuK/PyTfsClient
 Author: TopTuK
 Author-email: cydoor88@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: TFS,AZURE,TFS API,Team Foundation Server
```

### Comparing `PyTfsClient-1.4.0/README.md` & `PyTfsClient-1.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# TESTS
+[![Run tests](https://github.com/TopTuK/PyTfsClient/actions/workflows/tests.yaml/badge.svg?branch=master)](https://github.com/TopTuK/PyTfsClient/actions/workflows/tests.yaml)
+
 # PyTfsClient library (TFS API Python client)
 
 Microsoft Team Foundation Server Python Library is a Microsoft TFS API Python client that can work with Microsoft TFS.
 
 ## Installing
 Feel free to use command "pip install pytfsclient"
 
@@ -41,7 +44,10 @@
     wi.update_fields()
     print('Item custom field: {}'.format(wi['Custom.Field']))
 
     workitems = client.get_workitems([1, 2, 3])
     for wi in workitems:
         print('Item: id={}, Title={}'.format(wi.id, wi.title))
     ```
+
+# Coding style
+https://google.github.io/styleguide/pyguide.html
```

### Comparing `PyTfsClient-1.4.0/setup.py` & `PyTfsClient-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ### Execute
 # python setup.py sdist
 # twine upload dist/*
 
 # https://docs.python.org/3/distutils/setupscript.html
 setup(
     name='PyTfsClient',
-    version='1.4.0',
+    version='1.5.0',
     license='MIT',
     description='Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems',
     url='https://github.com/TopTuK/PyTfsClient',
     author='TopTuK',
     author_email='cydoor88@gmail.com',
     package_dir={'': 'src'},
     packages=find_packages(where='src', include=['pytfsclient*'], exclude=['.test', '*.test', 'test', 'test*', 'test.*']),
```

### Comparing `PyTfsClient-1.4.0/src/PyTfsClient.egg-info/PKG-INFO` & `PyTfsClient-1.5.0/src/PyTfsClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: PyTfsClient
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python Microsoft Team Foundation Server Library is a  client that can work with Microsoft TFS workitems
 Home-page: https://github.com/TopTuK/PyTfsClient
 Author: TopTuK
 Author-email: cydoor88@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: TFS,AZURE,TFS API,Team Foundation Server
```

### Comparing `PyTfsClient-1.4.0/src/PyTfsClient.egg-info/SOURCES.txt` & `PyTfsClient-1.5.0/src/PyTfsClient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/client_connection.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-from .services.http.http_client import HttpClient
+from .client_connection import ClientConnection
 
-class ClientConnection:
-    """
-    """
-    
-    # Constructor
-    def __init__(self, http_client: HttpClient, project_name: str='DefaultCollection') -> None:
-        server_url = http_client.base_url
-
-        if not server_url.endswith('/'):
-            server_url += '/'
-        
-        self.__server_url = server_url
-        self.__http_client = http_client
-
-        def get_collection_and_project():
-            splitted_project = project_name.split('/')
-            collection = splitted_project[0]
-            project = None
-
-            if len(splitted_project) > 1:
-                project = splitted_project[1]
-                # If not space
-                if project:
-                    project = project.split('/')[0]
+class TfsClientError(Exception):
+    '''
+    TfsClientError exception raised in API calls
+    '''
+    pass
 
-            return collection, project
-        
-        # Remove part after / in project_name, like DefaultCollection/MyProject => DefaultCollection
-        collection, project = get_collection_and_project()
+class TfsBaseClient:
+    def __init__(self, client_connection: ClientConnection) -> None:
+        assert client_connection, 'Client connection is None'
 
-        # Assign Collection and Project
-        self.__collection = collection
-        self.__project_name = project
+        self.__client_connection = client_connection
 
-    ### Properties section ###
+        self._url = client_connection.api_url
+        self._url_prj = client_connection.project_url
 
     @property
+    def client_connection(self) -> ClientConnection:
+        return self.__client_connection
+    
+    @property
     def server_url(self) -> str:
         """
         :return: TFS server URL (str)
         """
-        return self.__server_url
-    
+        return self.__client_connection.server_url
+
     @property
     def collection(self) -> str:
         """
         :return: current TFS collection
         """
-        return self.__collection
+        return self.__client_connection.collection
 
     @property
     def project_name(self) -> str:
         """
         :return: current TFS project name
         """
-        return self.__project_name
+        return self.__client_connection.project_name
+    
+    @property
+    def api_url(self) -> str:
+        """
+        :return: TFS server api URL
+        """
+        return self.__client_connection.api_url
+
+    @property
+    def project_url(self) -> str:
+        """
+        :return: TFS server project api URL
+        """
+        return self.__client_connection.project_url
     
     @project_name.setter
     def project_name(self, name: str) -> None:
         """
         :setter: sets TFS server project name and project api url
         """
-        self.__project_name = name
+
+        self.__client_connection.project_name = name
     
     @property
-    def http_client(self) -> HttpClient:
+    def http_client(self):
         """
         :return: configured HTTP client
         """
-        return self.__http_client
-    
-    # Remove part after / in project-name, like DefaultCollection/MyProject => DefaultCollection
-    # API responce only in Project, without subproject    
-    @property
-    def api_url(self) -> str:
+        return self.__client_connection.http_client
+
+    def authentificate_with_password(self, user_name: str, user_password: str) -> None:
         """
-        :return: TFS server api URL ending with '/'
+        Authorize with user name and password
+        
+        :param user_name (str): user name
+        :param user_password (str): user password
         """
-        return f'{self.__collection}/_apis/'
+        self.__client_connection.http_client.authentificate_with_password(user_name, user_password)
 
-    # API response only for Collection/Project
-    @property
-    def project_url(self) -> str:
+    def authentificate_with_pat(self, personal_access_token: str) -> None:
         """
-        :return: TFS server project api URL ending with '/'
+        Authorize with personal access token (PAT)
+
+        :param personal_access_token (str): user personal access token
         """
-        return f'{self.__collection}/{self.__project_name}/_apis/' if self.__project_name else self.api_url
+        assert personal_access_token, 'TfsBaseClient::authentificate_with_pat: personal access token can\'t be None'
+
+        self.__client_connection.http_client.authentificate_with_pat(personal_access_token)
+    
+
+
+
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/models/deprecated.py` & `PyTfsClient-1.5.0/src/pytfsclient/models/deprecated.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/models/obsolete.py` & `PyTfsClient-1.5.0/src/pytfsclient/models/obsolete.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/models/project/tfs_team.py` & `PyTfsClient-1.5.0/src/pytfsclient/models/project/tfs_team.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,84 @@
-class TfsTeam:
-    """
-    TFS Team model class
-    """
+from ..client_error import ClientError
+
+class Team:
+    '''
+    Team model class contains infromation about TFS/Azure team such as id, name and url
+    '''
 
     @property
     def id(self) -> str:
-        """
-        ID of TFS Team
-        """
+        '''
+        Returns:
+            ID of TFS/Azure Team
+        '''
         return self.__id
 
     @property
     def name(self) -> str:
-        """
-        Name of TFS Team
-        """
+        '''
+        Returns:
+            Name of TFS/Azure Team
+        '''
         return self.__name
 
     @property
     def url(self) -> str:
-        """
-        URL of TFS Team
-        """
+        '''
+        Returns:
+            URL of TFS/Azure Team
+        '''
         return self.__url
 
     @classmethod
     def create(cls, id: str, name: str, url: str = None):
-        """
-        Creates TFSTeam instance.
+        '''
+        Classmethod creates instance of Team class.
 
-        :param: id (str): ID of TFS team. Can\'t be None.
-        :param: name (str): name of TFS team. Can\'t be None.
-        :param: url (str): url for TFS team
-        :return: TFSTeam instance.
-        """
-        assert id, 'Id can\'t be None'
-        assert name, 'Name can\'t be None'
+        Args:
+            id (str): ID of TFS team. Can\'t be None.
+            name (str): name of TFS team. Can\'t be None.
+            url (str): url for TFS team
+
+        Returns:
+            Instance of Team class
+
+        Raises:
+            ClientError: if id or name is None
+        '''
+
+        if not id:
+            raise ClientError('Id can\'t be None')
+        
+        if not name:
+            raise ClientError('Name can\'t be None')
 
         team = cls()
 
         team.__id = id
         team.__name = name
         team.__url = url
 
         return team
 
     @classmethod
     def from_json(cls, json_item):
-        """
-        Creates TfsTeam object from given json object
-        """
+        '''
+        Classmethod creates instance of Team class from given json object
+
+        Args:
+            json_item (object): JSON object with 'id', 'name' and 'url' attributes.
+
+        Returns:
+            Instance of Team class
+        '''
+
         team = cls()
 
-        team.__id = json_item['id']
-        team.__name = json_item['name']
-        team.__url = json_item['url']
+        try:
+            team.__id = json_item['id']
+            team.__name = json_item['name']
+            team.__url = json_item['url']
+        except Exception as ex:
+            raise ClientError(ex)
 
         return team
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/models/workitems/tfs_workitem.py` & `PyTfsClient-1.5.0/src/pytfsclient/models/workitems/tfs_workitem.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,173 +1,210 @@
 from enum import Enum
 from typing import List, Dict
 from .tfs_update_relations_result import UpdateRelationsResult
 from .tfs_workitem_relation import WorkitemRelation
 from .tfs_workitem_changes import WorkitemChange
+from ..client_error import ClientError
 
 _IgnoreFields = [
     'System.Id',
     'System.WorkItemType'
 ]
 
 class UpdateFieldsResult(Enum):
-    """
-    Update workitem fields result.
+    '''
+    ENUM: update workitem fields result.
 
-    Enum values:
+    Values:
     - UPDATE_EXCEPTION: exception raised
     - UPDATE_FAIL: Fail to get result. Fields are not updated.
     - UPDATE_EMPTY: Nothing to update result
     - UPDATE_SUCCESS: Fields successfully updated
-    """
+    '''
+
     UPDATE_EXCEPTION = 1
     UPDATE_FAIL = 2
     UPDATE_EMPTY = 3
 
     UPDATE_SUCCESS = 0
 
 class Workitem:
-    """
-    Workitem model class. Contains properties of workitem
-    """
+    '''
+    Workitem model class. Contains information about properties of workitem.
+    '''
 
     ### Properties region ###
 
     @property
     def id(self) -> int:
-        """
-        Id of workitem
-        """
+        '''
+        Returns:
+            Id of workitem: int
+        '''
+
         return self.__id
     
     @property
     def url(self) -> str:
-        """
-        URL of workitem
-        """
+        '''
+        Returns:
+            URL of workitem.
+        '''
+
         return self.__url
     
     @property
     def revision(self) -> int:
-        """
-        Revision of workitem.
-        """
+        '''
+        Returns:
+            Current revision of workitem: int
+        '''
+
         return self.__fields['System.Rev'] if 'System.Rev' in self.__fields else None
     
     @property
     def type_name(self) -> str:
-        """
-        Returns type name of workitem.
-        """
+        '''
+        Returns:
+            Type name of workitem: str
+        '''
+
         return self.__type_name
     
     @property
     def title(self) -> str:
-        """
-        Current title of workitem. Can be edited.
-        Returns None if workitem doesn't contain title
-        """
+        '''
+        Returns:
+            Current title of workitem. Can be edited.
+            None if workitem doesn't contain title property.
+        '''
+
         if 'System.Title' in self.__updated_fields:
             return self.__updated_fields['System.Title']
         
         return self.__fields['System.Title'] if 'System.Title' in self.__fields else None
     
     @title.setter
     def title(self, value: str) -> None:
+        '''
+        Set title property
+        '''
+
         self.__updated_fields['System.Title'] = value
 
     @property
     def description(self) -> str:
-        """
-        Returns description property of workitem. Can be edited.
-        If workitem does not contain 'System.Description' property by default then retuns None
-        """
+        '''
+        Returns:
+            Description property of workitem. Can be edited.
+            If workitem does not contain 'System.Description' property returns None
+        '''
+
         if 'System.Description' in self.__updated_fields:
             return self.__updated_fields['System.Description']
 
         return self.__fields['System.Description'] if 'System.Description' in self.__fields else None
 
     @description.setter
     def description(self, value: str) -> None:
         self.__updated_fields['System.Description'] = value
 
     @property
     def assigned_to(self) -> str:
-        """
-        Return AssignedTo property of workitem. 
-        If workitem contains AssignedTo property then returns 'displayName'.
-        If workitem doesn't contain AssignedTo property then returns None.
-        """
+        '''
+        Returns:
+            AssignedTo property of workitem: str
+            If workitem contains AssignedTo property then returns 'displayName'.
+            If workitem doesn't contain AssignedTo property then returns None.
+        '''
+
         if 'System.AssignedTo' in self.__updated_fields:
             return self.__updated_fields['System.AssignedTo']
 
         if 'System.AssignedTo' in self.__fields:
             user = self.__fields['System.AssignedTo']
             if 'displayName' in user:
                 return user['displayName']
             else:
                 return str(user)
 
         return None
     
     @property
     def fields_keys(self) -> List[str]:
-        """
-        Returns current list of fields names of workitem (properties names)
-        """
+        '''
+        Returns:
+            List of fields names of workitem (properties names).
+        '''
+
         return self.__fields.keys()
     
     @property
     def fields(self) -> Dict[str, str]:
-        """
-        Returns Dictonary(str, str) of
-        """
+        '''
+        Returns:
+            Dictonary(str, str) of fields and values
+        '''
+
         # Merge two dictonaries
         # python 3.9 and higher (z = x | y)
         # Using z = { **x, **y }
         return { **self.__updated_fields, **self.__fields }
     
     def __getitem__(self, fld_name: str) -> str:
-        """
-        Returns value of field of workitem.
-        :param: fld_name (str) - field name
-        """
-        assert fld_name, 'Field name can\'t be None'
+        '''
+        Returns:
+            Value of field of workitem.
+            key (str): field name
+        '''
+
+        if not fld_name:
+            raise ClientError('Field name can\'t be None')
 
         if fld_name in self.__updated_fields:
             return self.__updated_fields[fld_name]
         
         return self.__fields[fld_name] if fld_name in self.__fields else None
     
     def __setitem__(self, fld_name: str, fld_value: str) -> None:
-        """
+        '''
         Sets workitem property value.
 
-        :param: fld_name (str): property name. Can't be None.
-        :param: fld_value (str): property value. Can't be None.
-        """
-        assert fld_name, 'Field name can\'t be None'
-        assert fld_value, 'Field value can\'t be None'
+        Args:
+            fld_name (str): property name. Can't be None.
+            fld_value (str): property value. Can't be None.
+        '''
+
+        if not fld_name:
+            raise ClientError('Field name can\'t be None')
+        
+        if not fld_value:
+            raise ClientError('Field value can\'t be None')
 
         self.__updated_fields[fld_name] = fld_value
 
     @property
     def relations(self) -> List[WorkitemRelation]:
-        """
-        Returns list of relations (TfsWorkitemRelation) of workitem
-        """
+        '''
+        Returns:
+            List of relations of workitem: List[WorkitemRelation]
+        '''
+
         return self.__relations
     
     ### END PROPERTY REGION ###
 
     # Update internal workitem fields
     def update_fields(self) -> UpdateFieldsResult:
-        """
-        Updates values of fields of workitem.
-        """
+        '''
+        Updates on server values of fields of workitem.
+        
+        Returns:
+            Result of operation: UpdateFieldsResult
+        '''
 
         if len(self.__updated_fields) == 0:
             return UpdateFieldsResult.UPDATE_EMPTY
         
         try:
             # update workitem fields
             item = self.__client.update_workitem_fields(self.id, self.__updated_fields, expand='fields')
@@ -180,26 +217,37 @@
 
             return UpdateFieldsResult.UPDATE_SUCCESS
         except:
             return UpdateFieldsResult.UPDATE_EXCEPTION
     
     def get_changes(self, skip: int = 0, top: int = -1) -> List[WorkitemChange]:
         '''
-        Get history changes of workitem
+        Get history changes of workitem.
+
+        Returns:
+            workitem changes history: List[WorkitemChange]
         '''
 
         return self.__client.get_workitem_changes(self.id, skip, top)
 
     ### RELATION REGION ###
 
     def add_relation(self, destination_workitem, relation_type_name: str, \
         relation_attributes = None) -> UpdateRelationsResult:
-        """
+        '''
         Adds relation to workitem.
-        """
+
+        Args:
+            destination_workitem (int, Workitem): destination workitem
+            relation_type_name (str): relation type name
+            relation_attributes: relation attributes
+        
+        Returns:
+            Update relations result: UpdateRelationsResult
+        '''
 
         try:
             item = self.__client.add_relation(self.id, destination_workitem, relation_type_name, \
                 relation_attributes)
             
             if not item:
                 return UpdateRelationsResult.UPDATE_FAIL
@@ -209,38 +257,55 @@
         except:
             return UpdateRelationsResult.UPDATE_EXCEPTION
 
     ### END RELATION REGION ###
 
     @classmethod
     def from_json(cls, client, json_item):
-        """
-        Creates TfsWorkitem instance from given json item instance.
-        """
+        '''
+        Classmethod creates Workitem instance from given json item.
+
+        Args:
+            client (WorkitemClient): WorkitemClient instance
+            json_item (object): JSON object with attributes
+
+        Returns:
+            Workitem class instance
+        
+        Raises:
+            ClientError with information about exception
+        '''
+
+        if not client:
+            raise ClientError('client is None')
         
         wi = cls()
 
-        wi.__client = client # WorkitemClient
-        wi.__raw = json_item
+        try:
+            wi.__client = client # WorkitemClient
+            wi.__raw = json_item
 
-        wi.__id = json_item['id']
-        wi.__url = json_item['url']
+            wi.__id = json_item['id']
+            wi.__url = json_item['url']
 
-        wi.__updated_fields = {}
+            wi.__updated_fields = {}
 
-        # Fields
-        if 'fields' in json_item:
-            wi.__fields = { fld : value for (fld, value) in json_item['fields'].items() if fld not in _IgnoreFields }
-            wi.__type_name = json_item['fields']['System.WorkItemType'] if 'System.WorkItemType' in json_item['fields'] else None
-        else:
-            wi.__fields = {}
-            wi.__type_name = None
-
-        # Relations
-        wi.__relations = None
-        if 'relations' in json_item:
-            wi.__relations = [WorkitemRelation.from_json(json_relation) for json_relation in json_item['relations']]
-        else:
-            wi.__relations = []
+            # Fields
+            if 'fields' in json_item:
+                wi.__fields = { fld : value for (fld, value) in json_item['fields'].items() if fld not in _IgnoreFields }
+                wi.__type_name = json_item['fields']['System.WorkItemType'] if 'System.WorkItemType' in json_item['fields'] else None
+            else:
+                wi.__fields = {}
+                wi.__type_name = None
+
+            # Relations
+            wi.__relations = None
+            if 'relations' in json_item:
+                wi.__relations = [WorkitemRelation.from_json(json_relation) for json_relation in json_item['relations']]
+            else:
+                wi.__relations = []
+                
+        except Exception as ex:
+            raise ClientError(ex)
 
         return wi
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/models/workitems/tfs_workitem_relation.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_relation_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from .models.workitems.tfs_workitem_relation import WorkitemRelation
 
 class RelationTypes(Enum):
     PARENT = 0
     CHILD = 1
     AFFECTS = 2
     AFFECTEDBY = 3
     RELATED = 4
@@ -11,23 +12,20 @@
     RelationTypes.PARENT : 'System.LinkTypes.Hierarchy-Reverse',
     RelationTypes.CHILD : 'System.LinkTypes.Hierarchy-Forward',
     RelationTypes.AFFECTS : 'Microsoft.VSTS.Common.Affects-Forward',
     RelationTypes.AFFECTEDBY : 'Microsoft.VSTS.Common.Affects-Reverse',
     RelationTypes.RELATED : 'System.LinkTypes.Related'
 }
 
-_WORKITEM_SUBSTR = 'workItems/'
-_WORKITEM_SUBSTR_LENGTH = len(_WORKITEM_SUBSTR)
-
-class WorkitemRelation:
+class TfsWorkitemRelation:
     """
     TFS relation model class.
     """
-
-    ### Properties region ###
+    __WORKITEM_SUBSTR = 'workItems/'
+    __WORKITEM_SUBSTR_LENGTH = len(__WORKITEM_SUBSTR)
 
     @property
     def destination_id(self) -> int:
         """
         Id of destination workitem.
         """
         return self.__destination_id
@@ -41,17 +39,16 @@
     
     @property
     def relation_name(self) -> str:
         """
         Relation type name.
         """
         return self.__relation_name
-    
-    ### END OF PROPERTIES REGION ###
 
+    #@staticmethod
     @classmethod
     def from_json(cls, json_item):
         """
         Creates TfsWorkitem instance from given json item instance.
         
         :return: TfsWorkitem instance.
         """
@@ -60,37 +57,51 @@
 
         url = json_item['url']
         relation.__url = url
 
         relation_name = json_item['rel']
         relation.__relation_name = relation_name
 
-        # Get workitem ID closure
         def get_id():
             wi_id = None
 
-            start_idx = url.find(_WORKITEM_SUBSTR)
+            start_idx = url.find(TfsWorkitemRelation.__WORKITEM_SUBSTR)
             if start_idx > 1:
-                start = int(start_idx + _WORKITEM_SUBSTR_LENGTH)
+                start = int(start_idx + TfsWorkitemRelation.__WORKITEM_SUBSTR_LENGTH)
                 wi_id = int(url[start:])
 
             return wi_id
 
         relation.__destination_id = get_id()
 
         return relation
     
+    #@staticmethod
     @classmethod
     def create(cls, relation_name: str, workitem):
         """
-        Creates relation for given relation type name and Tfs Workitem instance.
+        Creates relation for given relation type name and TfsWorkitem instance.
+        
+        :param: relation_name (str): relation type name. Can't be None.
+        :param: workitem (TfsWorkitem): TfsWorkitem instance, Can't be None.
+        :return: TfsWorkitem instance.
         """
-        assert relation_name, 'Relation name can\'t be None'
-        assert workitem, 'Workitem can\'t be None'
+        assert relation_name, 'TfsWorkitemRelation::create: relation name can\'t be None'
+        assert workitem, 'TfsWorkitemRelation::create: workitem can\'t be None'
 
-        relation = WorkitemRelation()
+        relation = TfsWorkitemRelation()
 
         relation.__relation_name = relation_name
         relation.__url = workitem.url
         relation.__destination_id = workitem.id
 
+        return relation
+    
+    @classmethod
+    def from_relation(cls, rel: WorkitemRelation):
+        relation = cls()
+
+        relation.__relation_name = rel.relation_name
+        relation.__url = rel.url
+        relation.__destination_id = rel.destination_id
+
         return relation
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/services/http/http_client.py` & `PyTfsClient-1.5.0/src/pytfsclient/services/http/http_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,28 +19,32 @@
     def __init__(self, base_url: str = None) -> None:
         if base_url:
             self.base_url = base_url
         
         super(_BaseUrlSession, self).__init__()
 
     def request(self, method, url, *args, **kwargs):
-        """Send the request after generating the complete URL"""
+        '''
+        Sends the request after generating the complete URL
+        '''
         
         request_url = self.create_url(url)
         return super(_BaseUrlSession, self).request(method, request_url, *args, **kwargs)
     
     def create_url(self, url: str):
-        """Create the URL based off this partial path"""
+        '''
+        Creates the URL based off this partial path
+        '''
 
         return urljoin(self.base_url, url)
     
 class HttpClient:
-    """
+    '''
     Http client public class
-    """
+    '''
 
     # Constructor
     def __init__(self, base_url: str, verify: bool=False) -> None:
         if not base_url.endswith('/'):
             base_url += '/'
         
         # store base url
@@ -64,26 +68,30 @@
         self.__httpClient.base_url = base_url
 
     @property
     def verify_ssl(self) -> bool:
         return self.__verify_ssl
     
     def authentificate_with_password(self, user_name: str, user_password: str) -> None:
-        """Set NTLM authication"""
+        '''
+        Set NTLM authication
+        '''
 
         if not user_name:
             raise HttpException('HttpClient::authentificate_with_password: \"user_name\" can\'t be None')
 
         if not user_password:
             raise HttpException('HttpClient::authentificate_with_password: \"user_password\" can\'t be None')
 
         self.__httpClient.auth = HttpNtlmAuth(user_name, user_password)
 
     def authentificate_with_pat(self, personal_access_token: str) -> None:
-        """Set personal access token authication (PAT)"""
+        '''
+        Set personal access token authication (PAT)
+        '''
 
         if not personal_access_token:
             raise HttpException('HttpClient::authentificate_with_pat: personal access token can\'t be None')
 
         pat = ':' + personal_access_token
         pat_base64 = b'Basic ' + base64.b64encode(pat.encode("utf8"))
 
@@ -98,51 +106,59 @@
             cookies=cookies,
             verify=self.__verify_ssl)
         response.raise_for_status()
 
         return response
     
     def post(self, resource: str, data, query_params=None, custom_headers=None):
-        """Make HTTP POST request"""
+        '''
+        Make HTTP POST request
+        '''
 
         response = self.__httpClient.post(resource, 
             data=data, 
             params=query_params, 
             headers=custom_headers,
             verify=self.__verify_ssl)
         response.raise_for_status()
 
         return response
     
     def post_json(self, resource: str, json_data, query_params=None, custom_headers=None):
-        """Make HTTP POST request with JSON data"""
+        '''
+        Make HTTP POST request with JSON data
+        '''
 
         response = self.__httpClient.post(resource, 
             json=json_data, 
             params=query_params, 
             headers=custom_headers,
             verify=self.__verify_ssl)
         response.raise_for_status()
 
         return response
     
     def patch(self, resource: str, data, query_params=None, custom_headers=None):
-        """Make HTTP PATCH request"""
+        '''
+        Make HTTP PATCH request
+        '''
 
         response = self.__httpClient.patch(resource,
             data=data,
             params=query_params,
             headers=custom_headers,
             verify=self.__verify_ssl)
         response.raise_for_status()
 
         return response
     
     def patch_json(self, resource: str, json_data, query_params=None, custom_headers=None):
-        """Make HTTP PATCH request with JSON body"""
+        '''
+        Make HTTP PATCH request with JSON body
+        '''
 
         response = self.__httpClient.patch(resource,
             json=json_data,
             params=query_params,
             headers=custom_headers,
             verify=self.__verify_ssl)
         response.raise_for_status()
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/services/project_client/project_client.py` & `PyTfsClient-1.5.0/src/pytfsclient/services/project_client/project_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 from ...models.client_error import ClientError
-from ...models.project.tfs_project import TfsProject
-from ...models.project.tfs_team import TfsTeam
-from ...models.project.tfs_team_member import TfsTeamMember
+from ...models.project.tfs_project import Project
+from ...models.project.tfs_team import Team
+from ...models.project.tfs_team_member import TeamMember
 from ...services.base_client import BaseClient
 from ...client_connection import ClientConnection
 from typing import List
 
 class ProjectClient(BaseClient):
-    """
-    Tfs ProjectClient facade for managing projects, teams and team members
-    """
+    '''
+    ProjectClient facade for managing projects, teams and team members
+    '''
 
     _URL_PROJECTS = 'projects'
     _URL_TEAMS = 'teams'
     _URL_TEAM_MEMBERS = 'members'
 
     # Constructor
     def __init__(self, client_connection: ClientConnection) -> None:
         super().__init__(client_connection)
     
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0
-    def get_projects(self, skip: int = 0) -> List[TfsProject]:
-        """
-        Returns current list of Tfs projects 
-        """
+    def get_projects(self, skip: int = 0) -> List[Project]:
+        '''
+        Returns current list of Tfs/Azure projects.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-6.0
+
+        Args:
+            skip (int): number top project to skip. Default: 0
+
+        Returns:
+            List of project: List[Project]
+        
+        Raises:
+            ClientError with information about exception
+        '''
         
         request_url = f'{self.client_connection.api_url}{self._URL_PROJECTS}'
         query_params = {
             'api-version': self.api_version,
             '$skip' : str(skip)
         }
 
@@ -44,28 +53,37 @@
                 json_items = response.json()
                 if ('count' in json_items) and (int(json_items['count']) == 0):
                     hasNext = False
                     continue
 
                 if 'value' in json_items:
                     json_items = json_items['value']
-                    projects += [TfsProject.from_json(json_item) for json_item in json_items]
+                    projects += [Project.from_json(json_item) for json_item in json_items]
                     query_params['$skip'] = str(len(projects))
                 else:
                     raise ClientError('ProjectClient::get_projects: response doesn\'t have \'value\' attribute')
             
             return projects
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_projects: exception raised. Msg: {ex}', ex)
 
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
-    def get_all_teams(self, current_user: bool = False) -> List[TfsTeam]:
-        """
-        Return list of TFS teams
-        """
+    def get_all_teams(self, current_user: bool = False) -> List[Team]:
+        '''
+        Return list of TFS/Azure teams.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
+
+        Args:
+            current_user (bool): If true return all the teams requesting user is member, otherwise return all the teams user has read access.
+        
+        Returns:
+            List of TFS/Azure teams: List[Team]
+        
+        Raises:
+            ClientError with information about exception
+        '''
 
         request_url = f'{self.client_connection.api_url}{self._URL_TEAMS}'
         query_params = {
             'api-version': self.api_version_preview,
             '$mine' : str(current_user)
         }
 
@@ -74,28 +92,41 @@
 
             if not response:
                 raise ClientError('ProjectClient::get_all_teams: can\'t get response from TFS server')
             
             json_items = response.json()
             if 'value' in json_items:
                 json_items = json_items['value']
-                return [TfsTeam.from_json(json_item) for json_item in json_items]
+                return [Team.from_json(json_item) for json_item in json_items]
             else:
                 raise ClientError('ProjectClient::get_all_teams: response doesn\'t have \'value\' attribute')
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_all_teams: exception raised. Msg: {ex}', ex)
 
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
-    def get_project_teams(self, project: TfsProject, expand: bool = False, \
-                          current_user: bool = False, skip: int = 0) -> List[TfsTeam]:
-        """
-        Get a list of teams of project.
-        """
+    def get_project_teams(self, project: Project, expand: bool = False, \
+                          current_user: bool = False, skip: int = 0) -> List[Team]:
+        '''
+        Get a list of teams of given project.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
+
+        Args:
+            project (Project): Project class instance
+            expand (bool): a value indicating whether or not to expand Identity information in the result WebApiTeam object. Default: False
+            current_user (bool): If true return all the teams requesting user is member, otherwise return all the teams user has read access. Default: False
+            skip (int): Number of teams to skip. Default: 0
+        
+        Returns:
+            List of teams: List[Team]
+        
+        Raises:
+            ClientError if project is None or bad request
+        '''
 
-        assert project, 'ProjectClient::get_project_teams: project can\'t be None'
+        if not project:
+            raise ClientError('ProjectClient::get_project_teams: project can\'t be None')
 
         request_url = f'{self.client_connection.api_url}{self._URL_PROJECTS}/{project.id}/{self._URL_TEAMS}'
         query_params = {
             'api-version' : self.api_version,
             '$expandIdentity' : str(expand),
             '$mine' : str(current_user),
             '$skip' : str(skip)
@@ -114,31 +145,45 @@
                 json_items = response.json()
                 if ('count' in json_items) and (int(json_items['count']) == 0):
                     hasNext = False
                     continue
 
                 if 'value' in json_items:
                     json_items = json_items['value']
-                    teams += [TfsTeam.from_json(json_item) for json_item in json_items]
+                    teams += [Team.from_json(json_item) for json_item in json_items]
                     query_params['$skip'] = str(len(teams))
                 else:
                     raise ClientError('ProjectClient::get_project_teams: response doesn\'t have \'value\' attribute')
                 
             return teams
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_project_teams: exception raised. Msg: {ex}', ex)
         
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-team-members-with-extended-properties?view=azure-devops-rest-6.0
-    def get_project_team_members(self, project: TfsProject, team: TfsTeam) -> List[TfsTeamMember]:
-        """
+    def get_project_team_members(self, project: Project, team: Team) -> List[TeamMember]:
+        '''
         Get a list of members for a specific team and a project.
-        """
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-team-members-with-extended-properties?view=azure-devops-rest-6.0
+
+        Args:
+            project (Project): project instance of the team project the team belongs to.
+            team (Team): team instance
+
+        Returns:
+            List of team members: List[TeamMember]
+        
+        Raises:
+            ClientError if project or team is None
+            ClientError if bad request
+        '''
         
-        assert project, 'ProjectClient::get_project_team_members: project can\'t be None'
-        assert team, 'ProjectClient::get_project_team_members: team can\'t be None'
+        if not project:
+            raise ClientError('ProjectClient::get_project_team_members: project can\'t be None')
+        
+        if not team:
+            raise ClientError('ProjectClient::get_project_team_members: team can\'t be None')
 
         request_url = f'{self.client_connection.api_url}{self._URL_PROJECTS}/{project.id}/{self._URL_TEAMS}/{team.id}/{self._URL_TEAM_MEMBERS}'
         query_params = {
             'api-version' : self.api_version,
             '$skip' : '0'
         }
 
@@ -155,31 +200,44 @@
                 json_items = response.json()
                 if ('count' in json_items) and (int(json_items['count']) == 0):
                         hasNext = False
                         continue
                 
                 if 'value' in json_items:
                     json_items = json_items['value']
-                    members += [TfsTeamMember.from_json(json_item['identity']) for json_item in json_items]
+                    members += [TeamMember.from_json(json_item['identity']) for json_item in json_items]
                     query_params['$skip'] = str(len(members))
                 else:
                     raise ClientError('ProjectClient::get_project_team_members: response doesn\'t have \'value\' attribute')
                 
             return members
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_project_team_members: exception raised. Msg: {ex}', ex)
 
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
-    def get_project_teams(self, project: TfsProject, expand: bool = False, \
-                          current_user: bool = False, skip: int = 0) -> List[TfsTeam]:
-        """
-        Get a list of members for a specific team and a project
-        """
+    def get_project_teams(self, project: Project, expand: bool = False, \
+                          current_user: bool = False, skip: int = 0) -> List[Team]:
+        '''
+        Get a list of members for a specific team and a project.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-teams?view=azure-devops-rest-6.0
+
+        Args:
+            project (Project): project instance. Can't be None
+            expand (bool): A value indicating whether or not to expand Identity information in the result WebApiTeam object. Default: False
+            current_user (bool): If true return all the teams requesting user is member, otherwise return all the teams user has read access. Default: False
+            skip (int): Number of teams to skip. Default: 0
+        
+        Returns:
+            List of teams: List[Team]
+        
+        Raises:
+            ClientError if project is None or bad request
+        '''
 
-        assert project, 'ProjectClient::get_project_teams: project can\'t be None'
+        if not project:
+            raise ClientError('ProjectClient::get_project_teams: project can\'t be None')
 
         request_url = f'{self.client_connection.api_url}{self._URL_PROJECTS}/{project.id}/{self._URL_TEAMS}'
         query_params = {
             'api-version' : self.api_version,
             '$expandIdentity' : str(expand),
             '$mine' : str(current_user),
             '$skip' : str(skip)
@@ -198,31 +256,46 @@
                 json_items = response.json()
                 if ('count' in json_items) and (int(json_items['count']) == 0):
                     hasNext = False
                     continue
 
                 if 'value' in json_items:
                     json_items = json_items['value']
-                    teams += [TfsTeam.from_json(json_item) for json_item in json_items]
+                    teams += [Team.from_json(json_item) for json_item in json_items]
                     query_params['$skip'] = str(len(teams))
                 else:
                     raise ClientError('ProjectClient::get_project_teams: response doesn\'t have \'value\' attribute')
             
             return teams
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_project_teams: exception raised. Msg: {ex}', ex)
 
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-team-members-with-extended-properties?view=azure-devops-rest-6.0
-    def get_project_team_members(self, project: TfsProject, team: TfsTeam) -> List[TfsTeamMember]:
-        """
+    def get_project_team_members(self, project: Project, team: Team) -> List[TeamMember]:
+        '''
         Get a list of members for a specific team and a project.
-        """
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get-team-members-with-extended-properties?view=azure-devops-rest-6.0
+
+        Args:
+            project (Project): project instance of the team project the team belongs to.
+            team (Team): team instance
+
+        Returns:
+            List of team members: List[TeamMember]
+        
+        Raises:
+            ClientError if project or team is None
+            ClientError if bad request
+
+        '''
+        
+        if not project:
+            raise ClientError('ProjectClient::get_project_team_members: project can\'t be None')
         
-        assert project, 'ProjectClient::get_project_team_members: project can\'t be None'
-        assert team, 'ProjectClient::get_project_team_members: team can\'t be None'
+        if not team:
+            raise ClientError('ProjectClient::get_project_team_members: team can\'t be None')
 
         request_url = f'{self.client_connection.api_url}{self._URL_PROJECTS}/{project.id}/{self._URL_TEAMS}/{team.id}/{self._URL_TEAM_MEMBERS}'
         query_params = {
             'api-version' : self.api_version,
             '$skip' : '0'
         }
 
@@ -239,15 +312,15 @@
                 json_items = response.json()
                 if ('count' in json_items) and (int(json_items['count']) == 0):
                     hasNext = False
                     continue
 
                 if 'value' in json_items:
                     json_items = json_items['value']
-                    members += [TfsTeamMember.from_json(json_item['identity']) for json_item in json_items]
+                    members += [TeamMember.from_json(json_item['identity']) for json_item in json_items]
                     query_params['$skip'] = str(len(members))
                 else:
                     raise ClientError('ProjectClient::get_project_team_members: response doesn\'t have \'value\' attribute')
 
             return members
         except Exception as ex:
             raise ClientError(f'ProjectClient::get_project_team_members: exception raised. Msg: {ex}', ex)
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/services/workitem_client/workitem_client.py` & `PyTfsClient-1.5.0/src/pytfsclient/services/workitem_client/workitem_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from ...models.workitems.tfs_workitem_relation import WorkitemRelation
 from ...models.workitems.tfs_workitem_changes import WorkitemChange
 from ..base_client import BaseClient
 from ...client_connection import ClientConnection
 from ..helpers.batch_iterable import batch
 
 class WorkitemClient(BaseClient):
-    """
-    TFS Workitem Client facade for managing workitems and relations
-    """
+    '''
+    Workitem Client facade for managing workitems and relations.
+    '''
 
     _WORKITEM_URL = 'wit/workitems'
     _WIQL_URL = 'wit/wiql'
     _QUERY_URL = 'wit/queries'
 
     # Constructor
     def __init__(self, client_connection: ClientConnection) -> None:
         super().__init__(client_connection)
 
     def _get_items(self, request_url: str, query_params, under_project: bool = False) -> List[Workitem]:
-        """
+        '''
         Return list of Workitem or raise an exception
-        """
+        '''
         
         url = f'{self.client_connection.project_url}{request_url}' if under_project else f'{self.client_connection.api_url}{request_url}'
         
         try:
             http_response = self.http_client.get(url, query_params=query_params)
 
             if not http_response:
@@ -44,21 +44,34 @@
         except ValueError as ex:
             raise ClientError(f'WorkitemClient::get_items: EXCEPTION raised, http response is not json. Msg: {ex}', ex)
         except HTTPError as ex:
             raise ClientError(f'WorkitemClient::get_items: EXCEPTION raised. Got http error', ex)
         except Exception as ex:
             raise ClientError(f'WorkitemClient::get_items: EXCEPTION raised. Msg: {ex}', ex)
 
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/list?view=azure-devops-rest-6.0
     def get_workitems(self, item_ids, item_fields: List[str] = None, expand: str = 'All', batch_size: int = 50) -> List[Workitem]:
-        """
-        Return list of Workitems for given list of item ids.
-        """
-        
-        assert item_ids, 'WorkitemClient::get_workitems: item ids can\'t be None'
+        '''
+        Returns list of Workitems for given list of item ids.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/list?view=azure-devops-rest-6.0
+
+        Args:
+            item_ids (List[int] | List[str] | int | str): list of ids of workitems to get
+            item_fields (List[str]): list of requested fields of workitems
+            expand (str): The expand parameters for work item attributes. Possible options are { None, Relations, Fields, Links, All }. Default: All
+            batch_size (int): batch size
+
+        Returns:
+            List or workitems: List[Workitem]
+
+        Raises:
+            ClientError with information about exception
+        '''
+
+        if not item_ids:
+            raise ClientError('WorkitemClient::get_workitems: item ids can\'t be None')
 
         if isinstance(item_ids, int):
             item_ids = [item_ids]
         if isinstance(item_ids, str):
             item_ids = [int(item_ids)]
 
         # Http Query Params
@@ -76,28 +89,50 @@
             query_params['ids'] = ','.join(map(str, items))
 
             workitems += self._get_items(self._WORKITEM_URL, query_params=query_params)
         
         return workitems
 
     def get_single_workitem(self, item_id, item_fields: List[str] = None) -> Workitem:
-        """
-        Get TFS workitem
-        """
+        '''
+        Get single TFS/Azure workitem. Calls get_workitems().
+        
+        Args:
+            item_id (int| str): workitem id
+            item_fields (List[str]): list of requested fields of workitems. Default: all fields
+
+        Returns:
+            Workitem instance
+        
+        Raises:
+            ClientError with information about exception
+        '''
         
-        assert item_id, 'WorkitemClient::get_single_workitem: item_id can\'t be None'
+        if not item_id:
+            raise ClientError('WorkitemClient::get_single_workitem: item_id can\'t be None')
 
-        return self.get_workitems(item_ids=item_id, item_fields=item_fields)[0]
+        items = self.get_workitems(item_ids=item_id, item_fields=item_fields)
+        return items[0] if items else None
 
     def get_workitem_changes(self, item_id: Union[int, Workitem], skip: int = 0, top: int = -1) -> List[WorkitemChange]:
         '''
-        Get Workitem history changes (updates)
+        Get Workitem history changes (updates).
+
+        Args:
+            item_id (int, Workitem): workitem instance
+
+        Returns:
+            List of changes of workitem: List[WorkitemChange]
+
+        Raises:
+            ClientError with information about exception
         '''
         
-        assert item_id, 'WorkitemClient::get_workitem_history: item_id can\'t be None'
+        if not item_id:
+            raise ClientError('WorkitemClient::get_workitem_history: item_id can\'t be None')
         
         if isinstance(item_id, Workitem):
             item_id = item_id.id
         if not isinstance(item_id, int):
             raise ClientError('WorkitemClient::get_workitem_history: item_id should be instance of int or Workitem')
         
         request_url = f'{self.client_connection.api_url}{self._WORKITEM_URL}/{item_id}/updates'
@@ -136,36 +171,52 @@
             return changes
         except Exception as ex:
             raise ClientError(f'WorkitemClient::get_workitem_history: exception raised. Msg: {ex}', ex)
 
     # return dictonary with standart query params
     @staticmethod
     def _make_query_params(expand: str, bypass_rules: bool, suppress_notifications: bool, validate_only: bool) -> dict:
-        """
+        '''
         Return dictonary with standart query params
-        """
+        '''
 
         return {
             'api-version' : BaseClient.api_version,
             '$expand' : expand,
             'bypassRules' : str(bypass_rules),
             'suppressNotifications' : str(bypass_rules),
             'validateOnly' : str(validate_only)
         }
     
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/create?view=azure-devops-rest-6.0
     def create_workitem(self, type_name: str, \
         item_fields: Dict[str, str] = None, item_relations: List[WorkitemRelation] = None, \
         expand: str = 'All', bypass_rules: bool = False, \
         suppress_notifications: bool = False, validate_only: bool = False) -> Workitem:
-        """
-        Creates workitem of given type, properties and relations
-        """
+        '''
+        Creates workitem of given type, properties and relations.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/create?view=azure-devops-rest-6.0
+
+        Args:
+            type_name (str): The work item type of the work item to create. Ex: Task, Change request
+            item_fields (Dict[str, str]): created workitems fields values
+            item_relations (List[WorkitemRelation]): workitem relations
+            expand (str): The expand parameters for work item attributes. Possible options are { None, Relations, Fields, Links, All }.
+            bypass_rules (bool): Do not enforce the work item type rules on this update
+            suppress_notifications (bool): Do not fire any notifications for this change
+            validate_only (bool): Indicate if you only want to validate the changes without saving the work item
 
-        assert type_name, 'WorkitemClient::create_workitem: item type name can\'t be None'
+        Returns:    
+            Workitem instance
+
+        Raises:
+            ClientError with information about exception
+        '''
+
+        if not type_name:
+            raise ClientError('WorkitemClient::create_workitem: item type name can\'t be None')
 
         # request url
         request_url = f'{self.client_connection.project_url}/{self._WORKITEM_URL}/${type_name}'
 
         # query params
         query_params = WorkitemClient._make_query_params(expand, bypass_rules, suppress_notifications, validate_only)
 
@@ -192,20 +243,33 @@
             if http_response:
                 return Workitem.from_json(self, http_response.json())
             else:
                 raise ClientError('WorkitemClient::create_workitem: can\'t create workitem')
         except Exception as ex:
             raise ClientError(f'WorkitemClient::create_workitem: EXCEPTION raised. Msg: {ex}', ex)
 
-    def copy_workitem(self, source_item, item_fields: List[str] = None, item_ignore_fileds: List[str] = None) -> Workitem:
-        """
-        Creates copy of given workitem
-        """
+    def copy_workitem(self, source_item, item_fields: List[str] = None, \
+                      item_ignore_fileds: List[str] = None) -> Workitem:
+        '''
+        Creates copy of given workitem.
+
+        Args:
+            source_item (int | Workitem): source workitem
+            item_fields (List[str]): fields of source workitem to copy. Default: None (all fields).
+            item_ignore_fileds (List[str]): fields of source workitem to ignore. Default: None
+
+        Returns:
+            Copied workitem instance
+        
+        Raises:
+            ClientError with information about exception
+        '''
 
-        assert source_item, 'WorkitemClient::copy_workitem: source_item can\'t be None'
+        if not source_item:
+            raise ClientError('WorkitemClient::copy_workitem: source_item can\'t be None')
 
         if isinstance(source_item, int):
             source_item = self.get_single_workitem(source_item)
         
         if (not isinstance(source_item, Workitem)) or (source_item is None):
             raise ClientError('WorkitemClient::copy_workitem: source item is None')
         
@@ -259,24 +323,41 @@
         item_type_name = source_item.type_name
 
         try:
             return self.create_workitem(item_type_name, item_fields=fields)
         except Exception as ex:
             raise ClientError(f'WorkitemClient::copy_workitem: EXCEPTION raised. Msg: {ex}', ex)
 
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/update?view=azure-devops-rest-6.0
     def update_workitem_fields(self, workitem, item_fields: Dict[str, str], \
         expand: str='All', bypass_rules: bool = False, \
         suppress_notifications: bool = False, validate_only: bool = False) -> Workitem:
-        """
-        Updates fields values for given workitem
-        """
+        '''
+        Updates fields values for given workitem.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/update?view=azure-devops-rest-6.0
 
-        assert workitem, 'WorkitemClient::update_workitem_fields: workitem can\'t be None'
-        assert item_fields, 'WorkitemClient::update_workitem_fields: item_fields can\'t be None'
+        Args:
+            workitem (int, Workitem): workitem to update
+            item_fields: (Dict[str, str]) dictonary with values of updated fields
+            expand: The expand parameters for work item attributes. Possible options are { None, Relations, Fields, Links, All }.
+            bypass_rules: Do not enforce the work item type rules on this update
+            suppress_notifications: Do not fire any notifications for this change
+            validate_only: Indicate if you only want to validate the changes without saving the work item
+
+        Returns:
+            Workitem instance with updated fields
+        
+        Raises:
+            ClientError with information about exception
+        '''
+
+        if not workitem:
+            raise ClientError('WorkitemClient::update_workitem_fields: workitem can\'t be None')
+        
+        if not item_fields:
+            raise ClientError ('WorkitemClient::update_workitem_fields: item_fields can\'t be None')
         
         if isinstance(workitem, int):
             workitem = self.get_single_workitem(workitem)
 
         if (not isinstance(workitem, Workitem)) or (workitem is None):
             raise ClientError('WorkitemClient::update_workitem_fields: workitem is None')
         
@@ -304,26 +385,47 @@
             else:
                 raise ClientError('WorkitemClient::update_workitem_fields: can\'t update workitem fields. Response has error')
         except Exception as ex:
             raise ClientError(f'WorkitemClient::update_workitem_fields: EXCEPTION raised. Msg: {ex}', ex)
 
     ### REGION MANAGING RELATIONS ###
 
-    # https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/update?view=azure-devops-rest-6.0#add-a-link
     def add_relation(self, source_workitem, destination_workitem, relation_type_name: str, \
         relation_attributes = None, \
         expand: str = 'All', bypass_rules: bool = False, \
         suppress_notifications: bool = False, validate_only: bool = False) -> Workitem:
-        """
-        Add relation link of given type for given workitem to another workitem
-        """
-
-        assert source_workitem, 'WorkitemClient::add_relation: source workitem can\'t be None'
-        assert destination_workitem, 'WorkitemClient::add_relation: destination workitem can\'t be None'
-        assert relation_type_name, 'WorkitemClient::add_relation: relation type name can\'t be None'
+        '''
+        Adds relation link of given type for given workitem to another workitem.
+        Docs: https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/work-items/update?view=azure-devops-rest-6.0#add-a-link
+
+        Args:
+            source_workitem (int, Workitem): source workitem
+            destination_workitem (int, Workitem): destination workitem
+            relation_type_name: relation type name (see RelationMap for default relations)
+            relation_attributes: relation attributes
+            expand: The expand parameters for work item attributes. Possible options are { None, Relations, Fields, Links, All }.
+            bypass_rules: Do not enforce the work item type rules on this update
+            suppress_notifications: Do not fire any notifications for this change
+            validate_only: Indicate if you only want to validate the changes without saving the work item
+        
+        Returns:
+            Workitem with added relation
+        
+        Raises:
+            ClientError with information about exception
+        '''
+
+        if not source_workitem:
+            raise ClientError('WorkitemClient::add_relation: source workitem can\'t be None')
+        
+        if not destination_workitem:
+            raise ClientError('WorkitemClient::add_relation: destination workitem can\'t be None')
+        
+        if not relation_type_name:
+            raise ClientError('WorkitemClient::add_relation: relation type name can\'t be None')
 
         if isinstance(source_workitem, Workitem):
             source_workitem = source_workitem.id
         
         if (not isinstance(source_workitem, int)):
             raise ClientError('WorkitemClient::add_relation: can\'t get id of source workitem')
         
@@ -361,20 +463,24 @@
             raise ClientError(f'TfsWorkitemClient::add_relation: response is not json. Msg: {ex}', ex)
         except Exception as ex:
             raise ClientError(f'TfsWorkitemClient::add_relation: EXCEPTION raised. Msg: {ex}', ex)
 
     def remove_relation(self, workitem: Workitem, relation: WorkitemRelation, \
         expand='All', bypass_rules=False, \
         suppress_notifications=False, validate_only=False) -> Workitem:
-        """
-        Remove relation from given workitem. jFYI: Tfs api can remove relation only for given index
-        """
+        '''
+        Removes relation from given workitem.
+        TFS/Azure api can remove relation only for given index
+        '''
 
-        assert workitem, 'WorkitemClient::remove_relation: workitem can\'t be None'
-        assert relation, 'WorkitemClient::remove_relation: relation can\'t be None'
+        if not workitem:
+            raise ClientError('WorkitemClient::remove_relation: workitem can\'t be None')
+        
+        if not relation:
+            raise ClientError('WorkitemClient::remove_relation: relation can\'t be None')
 
         # Find relation index
         relation_idx = -1
         for idx, rel in enumerate(workitem.relations):
             if (rel.relation_name == relation.relation_name) and (rel.destination_id == relation.destination_id):
                 relation_idx = idx
                 break
@@ -415,19 +521,29 @@
 
     ### END REGION MANAGING RELATIONS ###
 
     ### REGION QUERIES (WIQL) ###
 
     # https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/queries/get?view=azure-devops-rest-6.0
     def run_saved_query(self, query_id: str) -> WiqlResult:
-        """
+        '''
         Retrieves an individual query and its children
-        """
 
-        assert query_id, 'WorkitemClient::run_saved_query: query id can\'t be None'
+        Args:
+            query_id (str): query id (GUID)
+        
+        Returns:
+            Query result: WiqlResult
+        
+        Raises:
+            ClientError with information about exception
+        '''
+
+        if not query_id:
+            raise ClientError('WorkitemClient::run_saved_query: query id can\'t be None')
 
         if not isinstance(query_id, str):
             raise ClientError('WorkitemClient::run_saved_query: query_id must be string')
         
         # request url
         request_url = f'{self.client_connection.project_url}/{self._QUERY_URL}/{query_id}'
 
@@ -451,19 +567,29 @@
         except ValueError as ex:
             raise ClientError(f'WorkitemClient::run_saved_query: response is not json. Msg: {ex}', ex)
         except Exception as ex:
             raise ClientError(f'WorkitemClient::run_saved_query: EXCEPTION raised. Msg: {ex}', ex)
 
     # https://docs.microsoft.com/en-us/rest/api/azure/devops/wit/wiql/query-by-wiql?view=azure-devops-rest-6.0
     def run_wiql(self, query: str, max_top: int = -1) -> WiqlResult:
-        """
-        Gets the results of the query given its WIQL
-        """
+        '''
+        Runs WIQL query.
+
+        Args:
+            query (str): WIQL query
+        
+        Returns:
+            Query result: WiqlResult
+        
+        Raises:
+            ClientError with information about exception
+        '''
 
-        assert query, 'WorkitemClient::run_wiql: query can\'t be None'
+        if not query:
+            raise ClientError('WorkitemClient::run_wiql: query can\'t be None')
 
         # request url
         request_url = f'{self.client_connection.project_url}/{self._WIQL_URL}'
 
         # query params
         query_params = {
             'api-version' : self.api_version
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/tfs_client_factory.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_client_factory.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/tfs_project_client.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_project_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .tfs_client import TfsBaseClient, TfsClientError
 from .tfs_project_model import TeamMember, TfsProject, TfsTeam
 from typing import List
 
 from .client_factory import ClientFactory
 from .services.project_client.project_client import ProjectClient
-from .models.project.tfs_project import TfsProject as TProject
-from .models.project.tfs_team import TfsTeam as TTeam
+from .models.project.tfs_project import Project as TProject
+from .models.project.tfs_team import Team as TTeam
 
 ### DEPRECATED IN NEXT VERSIONS ####
 
 class TfsProjectClient:
     def __init__(self, client: TfsBaseClient) -> None:
         self.__client: TfsBaseClient = client
         self.__prj_client: ProjectClient = ClientFactory.get_project_client(client.client_connection)
```

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/tfs_project_model.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_project_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/tfs_wiql_model.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_wiql_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/tfs_workitem_client.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_client.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/src/pytfsclient/tfs_workitem_model.py` & `PyTfsClient-1.5.0/src/pytfsclient/tfs_workitem_model.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/test/test_backward_compatibility.py` & `PyTfsClient-1.5.0/test/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/test/test_client_connection.py` & `PyTfsClient-1.5.0/test/test_client_connection.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/test/test_http_client_auth.py` & `PyTfsClient-1.5.0/test/test_http_client_auth.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/test/test_http_client_basic.py` & `PyTfsClient-1.5.0/test/test_http_client_basic.py`

 * *Files identical despite different names*

### Comparing `PyTfsClient-1.4.0/test/test_integration.py` & `PyTfsClient-1.5.0/test/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pytfsclient.client_connection import ClientConnection
 from pytfsclient.client_factory import ClientFactory
 from pytfsclient.services.project_client.project_client import ProjectClient
 from pytfsclient.services.workitem_client.workitem_client import WorkitemClient
 from pytfsclient.models.workitems.tfs_workitem_relation import WorkitemRelation, RelationTypes, RelationMap
 from pytfsclient.models.workitems.tfs_workitem import UpdateFieldsResult
 from pytfsclient.models.workitems.tfs_workitem_changes import WorkitemChange, FieldChange, WorkitemRelationChanges
-from pytfsclient.models.project.tfs_team_member import TfsTeamMember
+from pytfsclient.models.project.tfs_team_member import TeamMember
 
 ### ^^^ ADDED EXTRA PATHS BELOW ^^^
 ### https://pytest-docs-ru.readthedocs.io/ru/latest/fixture.html
 
 @pytest.fixture(scope="module")
 def server_url() -> str:
     return os.environ['ENV_SERVER_URL']
```

