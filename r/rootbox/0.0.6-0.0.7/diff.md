# Comparing `tmp/rootbox-0.0.6.tar.gz` & `tmp/rootbox-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootbox-0.0.6.tar", last modified: Mon Apr 10 19:38:28 2023, max compression
+gzip compressed data, was "rootbox-0.0.7.tar", last modified: Thu Apr 13 18:01:59 2023, max compression
```

## Comparing `rootbox-0.0.6.tar` & `rootbox-0.0.7.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.030635 rootbox-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.034635 rootbox-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-10 19:38:20.000000 rootbox-0.0.6/.github/workflows/multi-test.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-10 19:38:20.000000 rootbox-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-10 19:38:20.000000 rootbox-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-10 19:38:20.000000 rootbox-0.0.6/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.034635 rootbox-0.0.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-10 19:38:20.000000 rootbox-0.0.6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-10 19:38:20.000000 rootbox-0.0.6/CREDITS.md
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-10 19:38:20.000000 rootbox-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-10 19:38:20.000000 rootbox-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-10 19:38:28.042636 rootbox-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-10 19:38:20.000000 rootbox-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.034635 rootbox-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-10 19:38:20.000000 rootbox-0.0.6/docs/LXC.md
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-10 19:38:20.000000 rootbox-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-10 19:38:20.000000 rootbox-0.0.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-10 19:38:20.000000 rootbox-0.0.6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.038636 rootbox-0.0.6/rootbox/
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/rootbox/cli/
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_create.py
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/cli/verbose.py
--rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/colorhelper.py
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/download.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/enter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/rootbox/images/
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1596 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images/lxc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/images_cache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/mount.py
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/process.py
--rw-r--r--   0 runner    (1001) docker     (122)     1869 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/rootfs.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/size.py
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/socket.py
--rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/tar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/unshare.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-10 19:38:20.000000 rootbox-0.0.6/rootbox/verbose.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/rootbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1040 2023-04-10 19:38:28.000000 rootbox-0.0.6/rootbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-10 19:38:27.000000 rootbox-0.0.6/rootbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/samples/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-10 19:38:20.000000 rootbox-0.0.6/samples/test.py
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-10 19:38:28.046635 rootbox-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-10 19:38:20.000000 rootbox-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-10 19:38:28.042636 rootbox-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-10 19:38:20.000000 rootbox-0.0.6/tests/test_cmd_pull.py
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-04-10 19:38:20.000000 rootbox-0.0.6/tests/test_image_url.py
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-10 19:38:20.000000 rootbox-0.0.6/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-10 19:38:20.000000 rootbox-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.916169 rootbox-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-13 18:01:51.000000 rootbox-0.0.7/.github/workflows/multi-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-13 18:01:51.000000 rootbox-0.0.7/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2055 2023-04-13 18:01:51.000000 rootbox-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-04-13 18:01:51.000000 rootbox-0.0.7/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-13 18:01:51.000000 rootbox-0.0.7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-04-13 18:01:51.000000 rootbox-0.0.7/CREDITS.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-04-13 18:01:51.000000 rootbox-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 18:01:51.000000 rootbox-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-13 18:01:59.924170 rootbox-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-13 18:01:51.000000 rootbox-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-04-13 18:01:51.000000 rootbox-0.0.7/docs/LXC.md
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-04-13 18:01:51.000000 rootbox-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       54 2023-04-13 18:01:51.000000 rootbox-0.0.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-13 18:01:51.000000 rootbox-0.0.7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.920169 rootbox-0.0.7/rootbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/rootbox/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/colorhelper.py
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/enter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/rootbox/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4313 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images/lxc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/images_cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1562 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/mount.py
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/path.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/process.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/rootfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/size.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/socket.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/tar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/unshare.py
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2023-04-13 18:01:51.000000 rootbox-0.0.7/rootbox/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/rootbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2459 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-13 18:01:59.000000 rootbox-0.0.7/rootbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/samples/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-04-13 18:01:51.000000 rootbox-0.0.7/samples/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-13 18:01:59.924170 rootbox-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-13 18:01:51.000000 rootbox-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 18:01:59.924170 rootbox-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      611 2023-04-13 18:01:51.000000 rootbox-0.0.7/tests/test_cmd_pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1314 2023-04-13 18:01:51.000000 rootbox-0.0.7/tests/test_image_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-04-13 18:01:51.000000 rootbox-0.0.7/tox.ini
```

### Comparing `rootbox-0.0.6/.github/workflows/multi-test.yaml` & `rootbox-0.0.7/.github/workflows/multi-test.yaml`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/.github/workflows/release.yaml` & `rootbox-0.0.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/.gitignore` & `rootbox-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/.pre-commit-config.yaml` & `rootbox-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/LICENSE` & `rootbox-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/PKG-INFO` & `rootbox-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rootbox-0.0.6/README.md` & `rootbox-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/docs/LXC.md` & `rootbox-0.0.7/docs/LXC.md`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/__main__.py` & `rootbox-0.0.7/rootbox/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import typer
 
-from .cli import cmd_create, cmd_exec, cmd_lxc, cmd_pull, cmd_run, verbose
+from .cli import cmd_create, cmd_exec, cmd_lxc, cmd_pull, cmd_run, main
 
+app = typer.Typer(short_help="Utility to manage rootbox containers")
 
-def main():
-    app = typer.Typer(short_help="Utility to manage a pypy.org metadata cache")
+app.command(help="Create a container instance")(cmd_create.create)
+app.command(help="Execute a command in an existing instance")(cmd_exec.exec)
+app.command(help="Pull an image into the local cache")(cmd_pull.pull)
+app.command(help="Run a command in an ephemeral instance")(cmd_run.run)
+app.add_typer(
+    cmd_lxc.app, name="lxc", help="Get information about available LCX images"
+)
+
+app.callback()(main.rootbox)
 
-    app.command(help="Create a container instance")(cmd_create.create)
-    app.command(help="Execute a command in an existing instance")(cmd_exec.exec)
-    app.command(help="Pull an image into the local cache")(cmd_pull.pull)
-    app.command(help="Run a command in an ephemeral instance")(cmd_run.run)
-    app.add_typer(
-        cmd_lxc.app, name="lxc", help="Get information about available LCX images"
-    )
 
-    app.callback()(verbose.verbose)
+def main():
     app()
 
 
 if __name__ == "__main__":
-    main()
+    app()
```

### Comparing `rootbox-0.0.6/rootbox/cli/cmd_create.py` & `rootbox-0.0.7/rootbox/cli/cmd_create.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/cli/cmd_pull.py` & `rootbox-0.0.7/rootbox/cli/cmd_pull.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/cli/cmd_run.py` & `rootbox-0.0.7/rootbox/cli/cmd_run.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 from typing import Optional
 
 import typer
 
 from ..download import download_image
 from ..images import parse_image_url
 from ..rootfs import prepare_rootfs
+from ..unshare import CLONE_NEWNET, unshare
 
 
 def run(
     image_name: str = typer.Argument(...),
     no_shell: bool = typer.Option(False, "--no-sh"),
+    no_net: bool = typer.Option(
+        False, "--no-network", "-N", help="Disable network in the container"
+    ),
     command: Optional[str] = typer.Argument("/bin/sh", help="Command to be run"),
     only_from_cache: bool = typer.Option(False, "--only-from-cache"),
 ):
     image = parse_image_url(image_name)
     image_fname = download_image(image, only_from_cache=only_from_cache)
     prepare_rootfs(image_fname, in_memory=True, perform_chroot=True)
+    if no_net:
+        unshare(CLONE_NEWNET)
     if no_shell:
         command = command.split()
         os.execvp(command[0], command[:])
     else:
         os.execvp("/bin/sh", ["sh", "-c", command])
```

### Comparing `rootbox-0.0.6/rootbox/colorhelper.py` & `rootbox-0.0.7/rootbox/colorhelper.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/download.py` & `rootbox-0.0.7/rootbox/download.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/enter.py` & `rootbox-0.0.7/rootbox/enter.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/http.py` & `rootbox-0.0.7/rootbox/http.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/images/__init__.py` & `rootbox-0.0.7/rootbox/images/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         lxc:distro[:version][:variant]
         docker:image[:tag]
         docker:[repository/]image[:tag]
         https://url.tar.g
         /path/to/file.tar.gz
         /path/to/directory
     """
-
     if ":" not in image_url:
         return local_url(image_url)
 
     handler, url = image_url.split(":", 1)
 
     if handler == "lxc":
         return LXCImage(*url.split(":"))
```

### Comparing `rootbox-0.0.6/rootbox/images/docker.py` & `rootbox-0.0.7/rootbox/images/docker.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 @dataclass
 class DockerImage:
     registry: str
     image_name: str
     image_tag: str = "latest"
 
     def as_url(self) -> str:
-        return url_to_filename(
-            f"docker_{self.registry}_{self.image_name}_{self.image_tag}"
-        )
+        registry = self.registry.replace(".", "_")
+        return url_to_filename(f"docker_{registry}_{self.image_name}_{self.image_tag}")
 
     def download(self):
         return pull_docker_image(self.registry, self.image_name, self.image_tag)
 
 
 def pull_docker_image(registry, repository, tag):
     source_reference = f"{registry}/{repository}:{tag}"
```

### Comparing `rootbox-0.0.6/rootbox/images/lxc.py` & `rootbox-0.0.7/rootbox/images/lxc.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/images_cache.py` & `rootbox-0.0.7/rootbox/images_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,10 @@
                 return find
         return default
 
     def put(self, filename, cache_key):
         """put a file into cache"""
         cached_fname = CACHE_PATH.joinpath(cache_key)
         if ".tar" not in cached_fname.suffixes:
-            cached_fname = cached_fname.with_suffix(".tar.gz")
+            cached_fname = Path(f"{cached_fname}.tar.gz")
         shutil.move(filename, cached_fname)
         return cached_fname
```

### Comparing `rootbox-0.0.6/rootbox/mount.py` & `rootbox-0.0.7/rootbox/mount.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/process.py` & `rootbox-0.0.7/rootbox/process.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/rootfs.py` & `rootbox-0.0.7/rootbox/rootfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,11 +43,10 @@
     if perform_chroot:
         if restore_path:
             target_restore_path = Path(mount_dir, restore_path[1:])
             target_restore_path.mkdir(parents=True)
             mount(restore_path, target_restore_path, None, MS_BIND | MS_REC)
         else:
             target_restore_path = "/"
-        mount("/etc/resolv.conf", f"{mount_dir}/etc/resolv.conf", None, MS_BIND)
         os.chroot(mount_dir)
         os.chdir(restore_path or "/")
     return mount_dir
```

### Comparing `rootbox-0.0.6/rootbox/size.py` & `rootbox-0.0.7/rootbox/size.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox/socket.py` & `rootbox-0.0.7/rootbox/socket.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import socket
 import time
 from pathlib import Path
 
 import xdg
 
-SOCKETS_DIR = Path(xdg.xdg_runtime_dir(), "rootbox")
+SOCKETS_DIR = Path(xdg.xdg_runtime_dir() or "/tmp", "rootbox")
 
 
 def create_socket_bind():
     my_pid = os.getpid()
     SOCKETS_DIR.mkdir(parents=True, exist_ok=True)
     sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
     socket_path = Path(SOCKETS_DIR, f"rootbox.{my_pid}.sock")
```

### Comparing `rootbox-0.0.6/rootbox/unshare.py` & `rootbox-0.0.7/rootbox/unshare.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/rootbox.egg-info/PKG-INFO` & `rootbox-0.0.7/rootbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rootbox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Portable reproducible environments for Linux applications
 Home-page: https://github.com/joaompinto/rootbox
 Author: João Pinto
 Author-email: lamego.pinto@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rootbox-0.0.6/rootbox.egg-info/SOURCES.txt` & `rootbox-0.0.7/rootbox.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 rootbox.egg-info/requires.txt
 rootbox.egg-info/top_level.txt
 rootbox/cli/cmd_create.py
 rootbox/cli/cmd_exec.py
 rootbox/cli/cmd_lxc.py
 rootbox/cli/cmd_pull.py
 rootbox/cli/cmd_run.py
-rootbox/cli/verbose.py
+rootbox/cli/main.py
 rootbox/images/__init__.py
 rootbox/images/docker.py
 rootbox/images/lxc.py
 samples/test.py
 tests/test_cmd_pull.py
-tests/test_image_url.py
-tests/test_version.py
+tests/test_image_url.py
```

### Comparing `rootbox-0.0.6/samples/test.py` & `rootbox-0.0.7/samples/test.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/setup.py` & `rootbox-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `rootbox-0.0.6/tests/test_image_url.py` & `rootbox-0.0.7/tests/test_image_url.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     assert isinstance(result, Path)
 
 
 def test_lxc_url():
     result = parse_image_url("lxc:archlinux")
     assert isinstance(result, LXCImage)
     assert result.name == "archlinux"
-    assert result.version == "latest"
+    assert result.version is None
 
     result = parse_image_url("lxc:alpine:edge")
     assert isinstance(result, LXCImage)
     assert result.name == "alpine"
     assert result.version == "edge"
```

