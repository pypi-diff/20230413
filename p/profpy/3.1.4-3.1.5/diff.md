# Comparing `tmp/profpy-3.1.4.tar.gz` & `tmp/profpy-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profpy-3.1.4.tar", last modified: Thu May 19 19:25:13 2022, max compression
+gzip compressed data, was "profpy-3.1.5.tar", last modified: Thu Apr 13 20:37:35 2023, max compression
```

## Comparing `profpy-3.1.4.tar` & `profpy-3.1.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.225376 profpy-3.1.4/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      115 2022-05-19 16:56:11.000000 profpy-3.1.4/.gitignore
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1056 2022-05-19 16:56:11.000000 profpy-3.1.4/LICENSE
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)       37 2022-05-19 16:56:11.000000 profpy-3.1.4/MANIFEST.in
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2037 2022-05-19 19:25:13.225376 profpy-3.1.4/PKG-INFO
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1525 2022-05-19 16:56:11.000000 profpy-3.1.4/README.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 16:56:11.000000 profpy-3.1.4/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.215376 profpy-3.1.4/profpy/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)       22 2022-05-19 19:24:08.000000 profpy-3.1.4/profpy/__init__.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4645 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/__main__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.218709 profpy-3.1.4/profpy/apis/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)    24292 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/BlackBoardLearn.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      948 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/README.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     8783 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/ServiceNowTable.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)    11562 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/TwentyFiveLive.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      254 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.218709 profpy-3.1.4/profpy/apis/docs/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4120 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/docs/Api.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     7721 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/docs/BlackBoardLearn.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     5793 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/docs/ServiceNowTable.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4659 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/docs/TwentyFiveLive.md
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.218709 profpy-3.1.4/profpy/apis/utils/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      734 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/utils/Api.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      960 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/utils/Token.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/utils/__init__.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      353 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/apis/utils/exceptions.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.218709 profpy-3.1.4/profpy/cli/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     3968 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/README.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.218709 profpy-3.1.4/profpy/cli/flask_init/
--rwxr-xr-x   0 hartigan  (1000) hartigan  (1000)    14407 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.222042 profpy-3.1.4/profpy/cli/flask_init/files/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1581 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.Dockerfile
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      541 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.README.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      194 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.SAMPLE.env
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      245 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.asset_config.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      592 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.db_user.ddl.sql
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1534 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.dev.Dockerfile
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      251 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.dev.docker-compose.override.yml
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      398 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.docker-compose.yml
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)    15406 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.favicon.ico
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1884 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.gitignore
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      135 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.index.html
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4433 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.layout.html
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      585 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.main.css
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1114 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.main.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      310 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.prod.docker-compose.override.yml
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)       32 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.requirements.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      685 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.rowan-site.css
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     3644 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.rowan_torch_logo_small.png
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      405 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.setup.sh
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      155 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/flask_init/files/cli.test.docker-compose.override.yml
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.222042 profpy-3.1.4/profpy/cli/logs/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2119 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/logs/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.222042 profpy-3.1.4/profpy/cli/run_app/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1994 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/run_app/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.222042 profpy-3.1.4/profpy/cli/stop_app/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      898 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/cli/stop_app/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.222042 profpy-3.1.4/profpy/db/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)    13973 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/db/README.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      123 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/db/__init__.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.222042 profpy-3.1.4/profpy/db/general/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/db/general/__init__.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)    12857 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/db/general/connections.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     6915 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/db/general/functions.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.225376 profpy-3.1.4/profpy/web/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)    13248 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/web/README.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)       38 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/web/__init__.py
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)    18581 2022-05-19 16:56:11.000000 profpy-3.1.4/profpy/web/web.py
-drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2022-05-19 19:25:13.215376 profpy-3.1.4/profpy.egg-info/
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2037 2022-05-19 19:25:13.000000 profpy-3.1.4/profpy.egg-info/PKG-INFO
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2023 2022-05-19 19:25:13.000000 profpy-3.1.4/profpy.egg-info/SOURCES.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)        1 2022-05-19 19:25:13.000000 profpy-3.1.4/profpy.egg-info/dependency_links.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)       49 2022-05-19 19:25:13.000000 profpy-3.1.4/profpy.egg-info/entry_points.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      114 2022-05-19 19:25:13.000000 profpy-3.1.4/profpy.egg-info/requires.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)        7 2022-05-19 19:25:13.000000 profpy-3.1.4/profpy.egg-info/top_level.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1733 2022-05-19 16:56:11.000000 profpy-3.1.4/pypi.md
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)      114 2022-05-19 19:24:21.000000 profpy-3.1.4/requirements.txt
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)       38 2022-05-19 19:25:13.225376 profpy-3.1.4/setup.cfg
--rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1248 2022-05-19 16:56:11.000000 profpy-3.1.4/setup.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      131 2023-04-13 20:25:35.000000 profpy-3.1.5/.gitignore
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1056 2023-02-09 20:13:48.000000 profpy-3.1.5/LICENSE
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)       37 2023-02-09 20:13:48.000000 profpy-3.1.5/MANIFEST.in
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2000 2023-04-13 20:37:35.922569 profpy-3.1.5/PKG-INFO
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1537 2023-04-13 20:25:35.000000 profpy-3.1.5/README.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2023-02-09 20:13:48.000000 profpy-3.1.5/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.919235 profpy-3.1.5/profpy/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)       22 2023-04-13 20:25:35.000000 profpy-3.1.5/profpy/__init__.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4645 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/__main__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/apis/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)    24292 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/BlackBoardLearn.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      948 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/README.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     8783 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/ServiceNowTable.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)    11562 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/TwentyFiveLive.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      254 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/apis/docs/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4120 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/docs/Api.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     7721 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/docs/BlackBoardLearn.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     5793 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/docs/ServiceNowTable.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4659 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/docs/TwentyFiveLive.md
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/apis/utils/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      734 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/utils/Api.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      960 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/utils/Token.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/utils/__init__.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      353 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/apis/utils/exceptions.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/cli/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     3968 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/README.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/cli/flask_init/
+-rwxr-xr-x   0 hartigan  (1000) hartigan  (1000)    14407 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/cli/flask_init/files/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1581 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.Dockerfile
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      541 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.README.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      194 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.SAMPLE.env
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      245 2023-04-13 20:25:35.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.asset_config.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      592 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.db_user.ddl.sql
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1534 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.dev.Dockerfile
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      251 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.dev.docker-compose.override.yml
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      398 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.docker-compose.yml
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)    15406 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.favicon.ico
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1884 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.gitignore
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      135 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.index.html
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     4433 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.layout.html
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      585 2023-04-13 20:25:35.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.main.css
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1114 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.main.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      310 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.prod.docker-compose.override.yml
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)       32 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.requirements.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      685 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.rowan-site.css
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     3644 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.rowan_torch_logo_small.png
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      405 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.setup.sh
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      155 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/flask_init/files/cli.test.docker-compose.override.yml
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/cli/logs/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2119 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/logs/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/cli/run_app/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1994 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/run_app/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/cli/stop_app/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      898 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/cli/stop_app/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/db/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)    13973 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/db/README.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      123 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/db/__init__.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/db/general/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)        0 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/db/general/__init__.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)    12878 2023-04-13 20:25:35.000000 profpy-3.1.5/profpy/db/general/connections.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     6927 2023-04-13 20:25:35.000000 profpy-3.1.5/profpy/db/general/functions.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.922569 profpy-3.1.5/profpy/web/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)    13248 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/web/README.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)       38 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/web/__init__.py
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)    18581 2023-02-09 20:13:48.000000 profpy-3.1.5/profpy/web/web.py
+drwxr-xr-x   0 hartigan  (1000) hartigan  (1000)        0 2023-04-13 20:37:35.919235 profpy-3.1.5/profpy.egg-info/
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2000 2023-04-13 20:37:35.000000 profpy-3.1.5/profpy.egg-info/PKG-INFO
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     2023 2023-04-13 20:37:35.000000 profpy-3.1.5/profpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)        1 2023-04-13 20:37:35.000000 profpy-3.1.5/profpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)       48 2023-04-13 20:37:35.000000 profpy-3.1.5/profpy.egg-info/entry_points.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      117 2023-04-13 20:37:35.000000 profpy-3.1.5/profpy.egg-info/requires.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)        7 2023-04-13 20:37:35.000000 profpy-3.1.5/profpy.egg-info/top_level.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1733 2023-02-09 20:13:48.000000 profpy-3.1.5/pypi.md
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)      117 2023-04-13 20:25:35.000000 profpy-3.1.5/requirements.txt
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)       38 2023-04-13 20:37:35.922569 profpy-3.1.5/setup.cfg
+-rw-r--r--   0 hartigan  (1000) hartigan  (1000)     1248 2023-02-09 20:13:48.000000 profpy-3.1.5/setup.py
```

### Comparing `profpy-3.1.4/LICENSE` & `profpy-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/PKG-INFO` & `profpy-3.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: profpy
-Version: 3.1.4
-Summary: UNKNOWN
+Version: 3.1.5
 Home-page: https://github.com/rowanuniversity/profpy/
 Author: Connor Hornibrook
 Author-email: hornibrookc@rowan.edu
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # profpy
 ### What is profpy?
 The profpy library is a centralized repository for Rowan's various python scripts to use.
@@ -47,9 +45,7 @@
 - [web](https://github.com/rowanuniversity/profpy/tree/master/profpy/web)
 
 
 ### Dependencies
 - Python 3.6.7 or above
 - Oracle Instant Client
 
-
-
```

### Comparing `profpy-3.1.4/README.md` & `profpy-3.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,39 +3,37 @@
 The profpy library is a centralized repository for Rowan's various python scripts to use.
 
 
 ### Why use it?
 Many of Rowan's python scripts/programs utilize similar or congruent functions and classes that end up getting rewritten or even
 copy/pasted wherever needed. Rather than continue this trend of untracked code, profpy allows us to have overhead control over these common functions
 and classes. If a program or script needs to use a class or function, it can just import it from profpy rather than rewrite it. This will allow us
-to standardize some of our code practices moving forward. 
+to standardize some of our code practices moving forward.
 
 ### Installation
 ```bash
 pip3 install profpy
 ```
 
 ### CLI
 
 For details on the ```profpy``` command line interface, [read the docs](./profpy/cli).
 
 ### Submodules
 The profpy library is organized into submodules: ```db```, ```web```, and ```apis```. The ```db``` submodule makes accessing
-Oracle databases with cx_Oracle and or Sql-Alchemy simpler. The ```apis``` submodule 
+Oracle databases with oracledb (formerly cx_Oracle) and or Sql-Alchemy simpler. The ```apis``` submodule
 contains wrapper-classes for some commonly used web APIs. The ```web``` submodule contains code for making easy,
 database-backed Flask apps, configured with CAS and role-based security.
 
 All three of these submodules can be used to cut back on duplicated code, as well as make the development process much less
-time consuming.  
+time consuming.
 
 
 For in-depth documentation, explore the submodules individually:
 - [db](./profpy/db)
 - [apis](./profpy/apis)
 - [web](profpy/web)
 
 
-
 ### Dependencies
-- Python 3.6.7 or above
+- Python 3.8 or above
 - Oracle Instant Client
-
```

### Comparing `profpy-3.1.4/profpy/__main__.py` & `profpy-3.1.5/profpy/__main__.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/BlackBoardLearn.py` & `profpy-3.1.5/profpy/apis/BlackBoardLearn.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/README.md` & `profpy-3.1.5/profpy/apis/README.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/ServiceNowTable.py` & `profpy-3.1.5/profpy/apis/ServiceNowTable.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/TwentyFiveLive.py` & `profpy-3.1.5/profpy/apis/TwentyFiveLive.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/docs/Api.md` & `profpy-3.1.5/profpy/apis/docs/Api.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/docs/BlackBoardLearn.md` & `profpy-3.1.5/profpy/apis/docs/BlackBoardLearn.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/docs/ServiceNowTable.md` & `profpy-3.1.5/profpy/apis/docs/ServiceNowTable.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/docs/TwentyFiveLive.md` & `profpy-3.1.5/profpy/apis/docs/TwentyFiveLive.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/utils/Api.py` & `profpy-3.1.5/profpy/apis/utils/Api.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/apis/utils/Token.py` & `profpy-3.1.5/profpy/apis/utils/Token.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/README.md` & `profpy-3.1.5/profpy/cli/README.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/__init__.py` & `profpy-3.1.5/profpy/cli/flask_init/__init__.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.Dockerfile` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.Dockerfile`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.README.md` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.README.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.db_user.ddl.sql` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.db_user.ddl.sql`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.dev.Dockerfile` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.dev.Dockerfile`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.favicon.ico` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.favicon.ico`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.gitignore` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.gitignore`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.layout.html` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.layout.html`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.main.css` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.main.css`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.main.py` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.main.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.rowan-site.css` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.rowan-site.css`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/flask_init/files/cli.rowan_torch_logo_small.png` & `profpy-3.1.5/profpy/cli/flask_init/files/cli.rowan_torch_logo_small.png`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/logs/__init__.py` & `profpy-3.1.5/profpy/cli/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/run_app/__init__.py` & `profpy-3.1.5/profpy/cli/run_app/__init__.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/cli/stop_app/__init__.py` & `profpy-3.1.5/profpy/cli/stop_app/__init__.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/db/README.md` & `profpy-3.1.5/profpy/db/README.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/db/general/connections.py` & `profpy-3.1.5/profpy/db/general/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import cx_Oracle
+import oracledb as cx_Oracle
 import os
 import re
 import functools
 from sqlalchemy import create_engine, MetaData
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 short_form_regex = re.compile(r"^[a-zA-Z]+[a-zA-Z0-9_]*@[a-zA-Z_]+$")
@@ -37,15 +37,15 @@
                 dsn = cx_Oracle.makedsn(host, port, service_name=service)
             except IndexError:
                 raise Exception("Invalid login string.")
 
         self.__username = username
         self.__password = password
         self.__dsn = dsn
-        self.__engine_string = f"oracle://{username}:{password}@{dsn}"
+        self.__engine_string = f"oracle+oracledb://{username}:{password}@{dsn}"
 
     def get_cx_oracle_connection(self):
         """
         :return: A cx_Oracle connection object
         """
         return cx_Oracle.connect(user=self.__username, password=self.__password, dsn=self.__dsn)
```

### Comparing `profpy-3.1.4/profpy/db/general/functions.py` & `profpy-3.1.5/profpy/db/general/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import cx_Oracle
+import oracledb as cx_Oracle
 import re
 
 DEFAULT_ARRAY_SIZE = 1000
 
 
 def execute_statement(cursor, sql, params=None):
     """
```

### Comparing `profpy-3.1.4/profpy/web/README.md` & `profpy-3.1.5/profpy/web/README.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy/web/web.py` & `profpy-3.1.5/profpy/web/web.py`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/profpy.egg-info/PKG-INFO` & `profpy-3.1.5/profpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: profpy
-Version: 3.1.4
-Summary: UNKNOWN
+Version: 3.1.5
 Home-page: https://github.com/rowanuniversity/profpy/
 Author: Connor Hornibrook
 Author-email: hornibrookc@rowan.edu
 License: MIT
-Platform: UNKNOWN
 Requires-Python: >=3.6.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # profpy
 ### What is profpy?
 The profpy library is a centralized repository for Rowan's various python scripts to use.
@@ -47,9 +45,7 @@
 - [web](https://github.com/rowanuniversity/profpy/tree/master/profpy/web)
 
 
 ### Dependencies
 - Python 3.6.7 or above
 - Oracle Instant Client
 
-
-
```

### Comparing `profpy-3.1.4/profpy.egg-info/SOURCES.txt` & `profpy-3.1.5/profpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/pypi.md` & `profpy-3.1.5/pypi.md`

 * *Files identical despite different names*

### Comparing `profpy-3.1.4/setup.py` & `profpy-3.1.5/setup.py`

 * *Files identical despite different names*

