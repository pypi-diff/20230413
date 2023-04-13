# Comparing `tmp/paramiko-stat-0.1.tar.gz` & `tmp/paramiko-stat-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paramiko-stat-0.1.tar", last modified: Thu Apr 13 16:00:42 2023, max compression
+gzip compressed data, was "paramiko-stat-0.2.tar", last modified: Thu Apr 13 17:58:45 2023, max compression
```

## Comparing `paramiko-stat-0.1.tar` & `paramiko-stat-0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.254804 paramiko-stat-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.250804 paramiko-stat-0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.250804 paramiko-stat-0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/dependabot.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/init.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      129 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/release_message.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/rename_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.250804 paramiko-stat-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.github/workflows/rename_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-13 16:00:38.000000 paramiko-stat-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 16:00:38.000000 paramiko-stat-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 16:00:38.000000 paramiko-stat-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-13 16:00:38.000000 paramiko-stat-0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-13 16:00:42.254804 paramiko-stat-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 16:00:38.000000 paramiko-stat-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.250804 paramiko-stat-0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-13 16:00:38.000000 paramiko-stat-0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 16:00:38.000000 paramiko-stat-0.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.250804 paramiko-stat-0.1/paramiko_stat/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 16:00:38.000000 paramiko-stat-0.1/paramiko_stat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-04-13 16:00:38.000000 paramiko-stat-0.1/paramiko_stat/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-13 16:00:38.000000 paramiko-stat-0.1/paramiko_stat/sftp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-13 16:00:38.000000 paramiko-stat-0.1/paramiko_stat/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.254804 paramiko-stat-0.1/paramiko_stat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-13 16:00:42.000000 paramiko-stat-0.1/paramiko_stat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 16:00:42.000000 paramiko-stat-0.1/paramiko_stat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:00:42.000000 paramiko-stat-0.1/paramiko_stat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 16:00:42.000000 paramiko-stat-0.1/paramiko_stat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 16:00:42.000000 paramiko-stat-0.1/paramiko_stat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 16:00:38.000000 paramiko-stat-0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 16:00:38.000000 paramiko-stat-0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:00:42.254804 paramiko-stat-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 16:00:38.000000 paramiko-stat-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:42.254804 paramiko-stat-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 16:00:38.000000 paramiko-stat-0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-13 16:00:38.000000 paramiko-stat-0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-13 16:00:38.000000 paramiko-stat-0.1/tests/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-13 16:00:38.000000 paramiko-stat-0.1/tests/stub_sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-13 16:00:38.000000 paramiko-stat-0.1/tests/test_rsa.key
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-13 16:00:38.000000 paramiko-stat-0.1/tests/test_stat_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 16:00:38.000000 paramiko-stat-0.1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.306776 paramiko-stat-0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.302776 paramiko-stat-0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.302776 paramiko-stat-0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/dependabot.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2309 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/init.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      129 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/release_message.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      933 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/rename_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.302776 paramiko-stat-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.github/workflows/rename_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-13 17:58:41.000000 paramiko-stat-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-13 17:58:41.000000 paramiko-stat-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 17:58:41.000000 paramiko-stat-0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-13 17:58:41.000000 paramiko-stat-0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-13 17:58:45.306776 paramiko-stat-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-13 17:58:41.000000 paramiko-stat-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.302776 paramiko-stat-0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-13 17:58:41.000000 paramiko-stat-0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 17:58:41.000000 paramiko-stat-0.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.302776 paramiko-stat-0.2/paramiko_stat/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 17:58:41.000000 paramiko-stat-0.2/paramiko_stat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-13 17:58:41.000000 paramiko-stat-0.2/paramiko_stat/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-13 17:58:41.000000 paramiko-stat-0.2/paramiko_stat/sftp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-13 17:58:41.000000 paramiko-stat-0.2/paramiko_stat/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.302776 paramiko-stat-0.2/paramiko_stat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-13 17:58:45.000000 paramiko-stat-0.2/paramiko_stat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 17:58:45.000000 paramiko-stat-0.2/paramiko_stat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:58:45.000000 paramiko-stat-0.2/paramiko_stat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 17:58:45.000000 paramiko-stat-0.2/paramiko_stat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 17:58:45.000000 paramiko-stat-0.2/paramiko_stat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 17:58:41.000000 paramiko-stat-0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 17:58:41.000000 paramiko-stat-0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:58:45.306776 paramiko-stat-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-13 17:58:41.000000 paramiko-stat-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:45.306776 paramiko-stat-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:58:41.000000 paramiko-stat-0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-13 17:58:41.000000 paramiko-stat-0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-13 17:58:41.000000 paramiko-stat-0.2/tests/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-13 17:58:41.000000 paramiko-stat-0.2/tests/stub_sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-13 17:58:41.000000 paramiko-stat-0.2/tests/test_rsa.key
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-13 17:58:41.000000 paramiko-stat-0.2/tests/test_stat_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-13 17:58:41.000000 paramiko-stat-0.2/tests/util.py
```

### Comparing `paramiko-stat-0.1/.github/FUNDING.yml` & `paramiko-stat-0.2/.github/FUNDING.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # These are supported funding model platforms
 
-github: [rochacbruno]
+github: [wbarnha]
 patreon: # Replace with a single Patreon username
 open_collective: # Replace with a single Open Collective username
 ko_fi: # Replace with a single Ko-fi username
 tidelift: # Replace with a single Tidelift platform-name/package-name e.g., npm/babel
 community_bridge: # Replace with a single Community Bridge project-name e.g., cloud-foundry
 liberapay: # Replace with a single Liberapay username
 issuehunt: # Replace with a single IssueHunt username
```

### Comparing `paramiko-stat-0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `paramiko-stat-0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `paramiko-stat-0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/.github/init.sh` & `paramiko-stat-0.2/.github/init.sh`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/.github/rename_project.sh` & `paramiko-stat-0.2/.github/rename_project.sh`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/.github/workflows/main.yml` & `paramiko-stat-0.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/.github/workflows/release.yml` & `paramiko-stat-0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/.github/workflows/rename_project.yml` & `paramiko-stat-0.2/.github/workflows/rename_project.yml`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/.gitignore` & `paramiko-stat-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/Makefile` & `paramiko-stat-0.2/Makefile`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/PKG-INFO` & `paramiko-stat-0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: paramiko-stat
-Version: 0.1
-Summary: Wrapper for paramiko with extra stat methods
-Home-page: https://github.com/wbarnha/paramiko-stat/
-Author: William Barnhart, Gordon P. Hemsley
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
 
 ---
 # paramiko-stat
 This is just a wrapper for paramiko with changes included from https://github.com/paramiko/paramiko/pull/1259/files.
 
 
 ## Install it from PyPI
@@ -28,8 +17,17 @@
 
 ssh = SSHClient()
 ssh.connect("127.0.0.1", username="user", ...)
 sftp = ssh.open_sftp()
 sftp.mkdir("path", mode=700)
 
 ```
+Alternatively, a much better practice:
 
+```py
+from paramiko import SSHClient
+from paramiko_stat import Transport
+
+ssh = SSHClient()
+ssh.connect("127.0.0.1", username="user", ..., transport_factory=Transport)
+
+```
```

### Comparing `paramiko-stat-0.1/paramiko_stat/client.py` & `paramiko-stat-0.2/paramiko_stat/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+# Copyright (C) 2006-2007  Robey Pointer <robeypointer@gmail.com>
+#
+# This file is part of paramiko.
+#
+# Paramiko is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free
+# Software Foundation; either version 2.1 of the License, or (at your option)
+# any later version.
+#
+# Paramiko is distributed in the hope that it will be useful, but WITHOUT ANY
+# WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
+# A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
+# details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with Paramiko; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA.
+
 import getpass
 import socket
 from errno import ECONNREFUSED, EHOSTUNREACH
 
 from paramiko.client import SSHClient as _SSHClient
 from paramiko.config import SSH_PORT
 from paramiko.ssh_exception import BadHostKeyException, NoValidConnectionsError
```

### Comparing `paramiko-stat-0.1/paramiko_stat.egg-info/SOURCES.txt` & `paramiko-stat-0.2/paramiko_stat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/setup.py` & `paramiko-stat-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/tests/conftest.py` & `paramiko-stat-0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/tests/loop.py` & `paramiko-stat-0.2/tests/loop.py`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/tests/stub_sftp.py` & `paramiko-stat-0.2/tests/stub_sftp.py`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/tests/test_rsa.key` & `paramiko-stat-0.2/tests/test_rsa.key`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/tests/test_stat_methods.py` & `paramiko-stat-0.2/tests/test_stat_methods.py`

 * *Files identical despite different names*

### Comparing `paramiko-stat-0.1/tests/util.py` & `paramiko-stat-0.2/tests/util.py`

 * *Files identical despite different names*

