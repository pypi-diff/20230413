# Comparing `tmp/heizer-999999.dev1679944487.tar.gz` & `tmp/heizer-999999.dev1681350078.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heizer-999999.dev1679944487.tar", last modified: Mon Mar 27 19:14:56 2023, max compression
+gzip compressed data, was "heizer-999999.dev1681350078.tar", last modified: Thu Apr 13 01:41:26 2023, max compression
```

## Comparing `heizer-999999.dev1679944487.tar` & `heizer-999999.dev1681350078.tar`

### file list

```diff
@@ -1,73 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.690633 heizer-999999.dev1679944487/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.678633 heizer-999999.dev1679944487/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.678633 heizer-999999.dev1679944487/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/.github/workflows/deploy-latest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-27 19:14:56.690633 heizer-999999.dev1679944487/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.682633 heizer-999999.dev1679944487/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/img1.png
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.682633 heizer-999999.dev1679944487/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.682633 heizer-999999.dev1679944487/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.682633 heizer-999999.dev1679944487/docs/source/_static/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/_static/websocket/create-topic.png
--rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/_static/websocket/message-in-browser.png
--rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/_static/websocket/publish-kafka-msg.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.682633 heizer-999999.dev1679944487/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/heizer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.682633 heizer-999999.dev1679944487/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/tutorial/consumer.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/tutorial/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/tutorial/prepare.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/docs/source/tutorial/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.686633 heizer-999999.dev1679944487/heizer/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 19:14:47.000000 heizer-999999.dev1679944487/heizer/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.686633 heizer-999999.dev1679944487/heizer/_source/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/_source/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/_source/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/_source/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/_source/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.686633 heizer-999999.dev1679944487/heizer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/config.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/heizer/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.686633 heizer-999999.dev1679944487/heizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-27 19:14:56.000000 heizer-999999.dev1679944487/heizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-03-27 19:14:56.000000 heizer-999999.dev1679944487/heizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 19:14:56.000000 heizer-999999.dev1679944487/heizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-27 19:14:56.000000 heizer-999999.dev1679944487/heizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-27 19:14:56.000000 heizer-999999.dev1679944487/heizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.686633 heizer-999999.dev1679944487/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/samples/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.686633 heizer-999999.dev1679944487/samples/websockets/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/samples/websockets/client.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/samples/websockets/server.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 19:14:56.690633 heizer-999999.dev1679944487/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:56.686633 heizer-999999.dev1679944487/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-03-27 19:14:42.000000 heizer-999999.dev1679944487/tests/test_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.306465 heizer-999999.dev1681350078/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.306465 heizer-999999.dev1681350078/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/.github/workflows/deploy-latest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.306465 heizer-999999.dev1681350078/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   940058 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/img1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.306465 heizer-999999.dev1681350078/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.306465 heizer-999999.dev1681350078/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.306465 heizer-999999.dev1681350078/docs/source/_static/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)   231431 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/_static/websocket/create-topic.png
+-rw-r--r--   0 runner    (1001) docker     (123)   157758 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/_static/websocket/message-in-browser.png
+-rw-r--r--   0 runner    (1001) docker     (123)   232265 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/_static/websocket/publish-kafka-msg.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/heizer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/tutorial/consumer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/tutorial/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/tutorial/prepare.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/docs/source/tutorial/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/heizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 01:41:18.000000 heizer-999999.dev1681350078/heizer/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/heizer/_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/_source/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/_source/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/_source/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/_source/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/heizer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/heizer/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/heizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-04-13 01:41:26.000000 heizer-999999.dev1681350078/heizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-13 01:41:26.000000 heizer-999999.dev1681350078/heizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 01:41:26.000000 heizer-999999.dev1681350078/heizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 01:41:26.000000 heizer-999999.dev1681350078/heizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 01:41:26.000000 heizer-999999.dev1681350078/heizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/samples/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/samples/websockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/samples/websockets/client.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/samples/websockets/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:26.310465 heizer-999999.dev1681350078/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-13 01:41:16.000000 heizer-999999.dev1681350078/tests/test_consumer.py
```

### Comparing `heizer-999999.dev1679944487/.github/workflows/deploy-latest.yml` & `heizer-999999.dev1681350078/.github/workflows/deploy-latest.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/.github/workflows/main.yml` & `heizer-999999.dev1681350078/.github/workflows/main.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 name: "Heizer CI Tests"
 
 on: [push]
 
 jobs:
-  tests:
+  tests-3-10:
     runs-on: ubuntu-latest
     services:
       zookeeper:
         image: confluentinc/cp-zookeeper:latest
         env:
           ZOOKEEPER_CLIENT_PORT: 2181
           ZOOKEEPER_TICK_TIME: 2000
@@ -29,30 +29,64 @@
     - name: Set up Python 3.10
       uses: actions/setup-python@v3
       with:
         python-version: "3.10"
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install -r requirements.txt
-        pip install -r tests/requirements.txt
+        pip install -e .[all,test,dev]
 
     - name: Lint
       run: |
-        pip install pre-commit
         pre-commit install
         pre-commit run --all-files
 
     - name: Test with pytest
       env:
         KAFKA_SERVER: "localhost:9092"
       run: |
         python -m pytest -s tests --cov=heizer --cov-report=xml  --junit-xml=report.xml
 
 
+  tests-3-7:
+    runs-on: ubuntu-latest
+    services:
+      zookeeper:
+        image: confluentinc/cp-zookeeper:latest
+        env:
+          ZOOKEEPER_CLIENT_PORT: 2181
+          ZOOKEEPER_TICK_TIME: 2000
+      kafka:
+        image: confluentinc/cp-kafka:latest
+        ports:
+          - 9092:9092
+        env:
+          KAFKA_BROKER_ID: 1
+          KAFKA_ZOOKEEPER_CONNECT: zookeeper:2181
+          KAFKA_ADVERTISED_LISTENERS: PLAINTEXT://kafka:29092,PLAINTEXT_HOST://localhost:9092
+          KAFKA_LISTENER_SECURITY_PROTOCOL_MAP: PLAINTEXT:PLAINTEXT,PLAINTEXT_HOST:PLAINTEXT
+          KAFKA_INTER_BROKER_LISTENER_NAME: PLAINTEXT
+          KAFKA_OFFSETS_TOPIC_REPLICATION_FACTOR: 1
+
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python 3.7
+      uses: actions/setup-python@v3
+      with:
+        python-version: "3.7"
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        pip install -e .[all,test,dev]
+    - name: Test with pytest
+      env:
+        KAFKA_SERVER: "localhost:9092"
+      run: |
+        python -m pytest -s tests --cov=heizer --cov-report=xml  --junit-xml=report.xml
+
   test_build_doc:
     runs-on: ubuntu-latest
     services:
       zookeeper:
         image: confluentinc/cp-zookeeper:latest
         env:
           ZOOKEEPER_CLIENT_PORT: 2181
@@ -77,16 +111,15 @@
         uses: actions/setup-python@v3
         with:
           python-version: "3.10"
       - name: Build Docs
         run: |
           sudo apt-get install -y zip gzip tar
           python -m pip install --upgrade pip
-          pip install -r requirements.txt
-          pip install -r docs/requirements.txt
+          pip install -e .[all,doc]
           sphinx-multiversion ./docs/source ./doc/
           zip -r doc.zip doc/
       - name: Upload Artifact
         uses: actions/upload-artifact@v3
         with:
           name: doc_zip
           path: doc.zip
```

### Comparing `heizer-999999.dev1679944487/.github/workflows/release.yml` & `heizer-999999.dev1681350078/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/.gitignore` & `heizer-999999.dev1681350078/.gitignore`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/LICENSE` & `heizer-999999.dev1681350078/LICENSE`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/PKG-INFO` & `heizer-999999.dev1681350078/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1679944487
+Version: 999999.dev1681350078
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,19 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: socket
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 # Heizer
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/heizer.svg)](https://pypi.org/project/heizer/)
 [![Package Status](https://img.shields.io/pypi/status/heizer.svg)](https://pypi.org/project/heizer/)
 [![License](https://img.shields.io/pypi/l/heizer.svg)](https://github.com/claudezss/heizer/blob/main/LICENSE)
```

### Comparing `heizer-999999.dev1679944487/README.md` & `heizer-999999.dev1681350078/README.md`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docker-compose.yaml` & `heizer-999999.dev1681350078/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/Makefile` & `heizer-999999.dev1681350078/docs/Makefile`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/img1.png` & `heizer-999999.dev1681350078/docs/img1.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/make.bat` & `heizer-999999.dev1681350078/docs/make.bat`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/source/_static/websocket/create-topic.png` & `heizer-999999.dev1681350078/docs/source/_static/websocket/create-topic.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/source/_static/websocket/message-in-browser.png` & `heizer-999999.dev1681350078/docs/source/_static/websocket/message-in-browser.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/source/_static/websocket/publish-kafka-msg.png` & `heizer-999999.dev1681350078/docs/source/_static/websocket/publish-kafka-msg.png`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/source/_templates/versions.html` & `heizer-999999.dev1681350078/docs/source/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/source/conf.py` & `heizer-999999.dev1681350078/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/docs/source/tutorial/consumer.rst` & `heizer-999999.dev1681350078/docs/source/tutorial/consumer.rst`

 * *Files 12% similar despite different names*

```diff
@@ -25,38 +25,40 @@
         }
     )
 
 2. Create the topic
 
 .. ipython:: python
 
-    topics = [HeizerTopic(name="my.topic1")]
+    topics = [HeizerTopic(name="my.topic1.consumer.example")]
 
 3. Create producer
 
 .. ipython:: python
 
     @producer(
         topics=topics,
-        config=producer_config
+        config=producer_config,
+        key_alias="key",
+        headers_alias="headers",
     )
     def produce_data(status: str, result: str):
         return {
             "status": status,
             "result": result,
+            "key": "my_key",
+            "headers": {"my_header": "my_header_value"},
         }
 
 4. Publish messages
 
 .. ipython:: python
 
     produce_data("start", "1")
 
-    produce_data("start", "1")
-
     produce_data("loading", "2")
 
     produce_data("success", "3")
 
     produce_data("postprocess", "4")
 
 5. Create consumer
@@ -78,12 +80,13 @@
         topics=topics,
         config=consumer_config,
         stopper=stopper,
     )
     def consume_data(message: HeizerMessage):
         data = json.loads(message.value)
         print(data)
+        print(message.key)
+        print(message.headers)
         return data["result"]
 
     result = consume_data()
-
     print("Expected Result:", result)
```

### Comparing `heizer-999999.dev1679944487/docs/source/tutorial/websockets.rst` & `heizer-999999.dev1681350078/docs/source/tutorial/websockets.rst`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/heizer/_source/__init__.py` & `heizer-999999.dev1681350078/heizer/_source/__init__.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/heizer/_source/consumer.py` & `heizer-999999.dev1681350078/heizer/_source/consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,91 @@
 import asyncio
 import functools
 import logging
-from typing import Any, Awaitable, Callable, Concatenate, Coroutine, List, Optional, ParamSpec, Type, TypeVar, Union
 from uuid import uuid4
 
 from confluent_kafka import Consumer
 from pydantic import BaseModel
 
 from heizer._source import get_logger
 from heizer._source.message import HeizerMessage
 from heizer._source.topic import HeizerTopic
 from heizer.config import HeizerConfig
-from heizer.types import Stopper
+from heizer.types import (
+    Any,
+    Awaitable,
+    Callable,
+    Concatenate,
+    Coroutine,
+    List,
+    Optional,
+    ParamSpec,
+    Stopper,
+    Type,
+    TypeVar,
+    Union,
+)
 
 R = TypeVar("R")
 F = TypeVar("F", bound=Callable[..., Any])
 P = ParamSpec("P")
 T = TypeVar("T")
 
 logger = get_logger(__name__)
 
 
 class consumer(object):
     """A decorator to create a consumer"""
 
     __id__: str
+    name: Optional[str]
 
     topics: List[HeizerTopic]
     config: HeizerConfig = HeizerConfig()
     call_once: bool = False
     stopper: Optional[Stopper] = None
     deserializer: Optional[Type[BaseModel]] = None
 
     is_async: bool = False
+    poll_timeout: int = 1
 
     def __init__(
         self,
         *,
         topics: List[HeizerTopic],
         config: HeizerConfig = HeizerConfig(),
         call_once: bool = False,
         stopper: Optional[Stopper] = None,
         deserializer: Optional[Type[BaseModel]] = None,
         is_async: bool = False,
+        name: Optional[str] = None,
+        poll_timeout: Optional[int] = None,
     ):
         self.topics = topics
         self.config = config
         self.call_once = call_once
         self.stopper = stopper
         self.deserializer = deserializer
         self.__id__ = str(uuid4())
+        self.name = name or self.__id__
         self.is_async = is_async
+        self.poll_timeout = poll_timeout or 1
 
     async def __run__(
         self,
         func: Callable[Concatenate[HeizerMessage, P], Union[T, Awaitable[T]]],
         c: Consumer,
         is_async: bool,
         *args: P.args,
         **kwargs: P.kwargs,
     ) -> Union[Optional[T]]:  # ignore type
         """Run the consumer"""
 
         while True:
-            msg = c.poll(1)
+            msg = c.poll(self.poll_timeout)
 
             if msg is None:
                 continue
 
             if msg.error():
                 logger.error(f"Consumer error: {msg.error()}")
                 continue
```

### Comparing `heizer-999999.dev1679944487/heizer/_source/message.py` & `heizer-999999.dev1681350078/heizer/_source/message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Any, List, Optional, Tuple
-
 from confluent_kafka import Message
 
+from heizer.types import Any, Dict, List, Optional, Tuple, Union
+
 
 class HeizerMessage:
     # initialized properties
     message: Message
     topic: Optional[str]
     partition: int
-    headers: Optional[dict[str, str]]
+    headers: Optional[Dict[str, str]]
     key: Optional[str]
     value: Optional[str]
 
     formatted_value: Optional[Any] = None
 
     def __init__(self, message: Message):
         self.message = message
@@ -23,33 +23,33 @@
         self.value = self._parse_value(message.value())
 
     @staticmethod
     def __bytes_to_str(b: bytes) -> str:
         """Convert bytes to string"""
         return str(b, "utf-8")
 
-    def _parse_topic(self, topic: str | bytes) -> Optional[str]:
+    def _parse_topic(self, topic: Union[str, bytes]) -> Optional[str]:
         """Parse topic to string"""
         if topic is None:
             return None
         return self.__bytes_to_str(topic) if isinstance(topic, bytes) else topic
 
-    def _parse_headers(self, headers: Optional[List[Tuple[str, bytes]]]) -> Optional[dict[str, str]]:
+    def _parse_headers(self, headers: Optional[List[Tuple[str, bytes]]]) -> Optional[Dict[str, str]]:
         """Parse headers to dict"""
         parsed_headers = {}
         if headers is None:
             return None
         for k, v in headers:
             parsed_headers.update({k: v if isinstance(v, str) else self.__bytes_to_str(v)})
         return parsed_headers
 
-    def _parse_key(self, key: str | bytes) -> Optional[str]:
+    def _parse_key(self, key: Union[str, bytes]) -> Optional[str]:
         """Parse key to string"""
         if key is None:
             return None
         return self.__bytes_to_str(key) if isinstance(key, bytes) else key
 
-    def _parse_value(self, value: str | bytes) -> Optional[str]:
+    def _parse_value(self, value: Union[str, bytes]) -> Optional[str]:
         """Parse value to string"""
         if value is None:
             return None
         return self.__bytes_to_str(value) if isinstance(value, bytes) else value
```

### Comparing `heizer-999999.dev1679944487/heizer/_source/producer.py` & `heizer-999999.dev1681350078/heizer/_source/producer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,92 @@
 import functools
 import json
-from logging import getLogger
-from typing import Any, Callable, Dict, List, Optional, TypeVar, Union, cast
+from uuid import uuid4
 
 from confluent_kafka import Message, Producer
 
+from heizer._source import get_logger
 from heizer._source.topic import HeizerTopic
 from heizer.config import HeizerConfig
+from heizer.types import Any, Callable, Dict, List, Optional, TypeVar, Union, cast
 
-logger = getLogger(__name__)
-PRODUCER_LIST = []
+logger = get_logger(__name__)
 
 R = TypeVar("R")
-F = TypeVar("F", bound=Callable[..., Any])
+F = TypeVar("F", bound=Callable[..., Dict[str, str]])
 
 
-def _default_encoder(value: Union[Dict[Any, Any], str, bytes]) -> bytes:
+def _default_serializer(value: Union[Dict[Any, Any], str, bytes]) -> bytes:
     """
     :param value:
     :return: bytes
 
-    Default Kafka message encoder, which will encode inputs to bytes
+    Default Kafka message serializer, which will encode inputs to bytes
 
     """
     if isinstance(value, dict):
         return json.dumps(value).encode("utf-8")
     elif isinstance(value, str):
         return value.encode("utf-8")
     elif isinstance(value, bytes):
         return value
     else:
         raise ValueError(f"Input type is not supported: {type(value).__name__}")
 
 
 class producer(object):
+
+    """
+    A decorator to create a producer
+    """
+
+    __id__: str
+    name: str
+
     # args
     config: HeizerConfig = HeizerConfig()
     topics: List[HeizerTopic]
-    message_encoder: Callable[..., bytes] = _default_encoder
+    serializer: Callable[..., bytes] = _default_serializer
     call_back: Optional[Callable[..., Any]] = None
-    key: Optional[str] = None
-    headers: Optional[Dict[str, str]] = None
+
+    default_key: Optional[str] = None
+    default_headers: Optional[Dict[str, str]] = None
+
+    key_alias: str = "key"
+    headers_alias: str = "headers"
 
     # private properties
     _producer_instance: Optional[Producer] = None
 
     def __init__(
         self,
         topics: List[HeizerTopic],
         config: HeizerConfig = HeizerConfig(),
-        message_encoder: Callable[..., bytes] = _default_encoder,
+        serializer: Callable[..., bytes] = _default_serializer,
         call_back: Optional[Callable[..., Any]] = None,
-        key: Optional[str] = None,
-        headers: Optional[Dict[str, str]] = None,
+        default_key: Optional[str] = None,
+        default_headers: Optional[Dict[str, str]] = None,
+        key_alias: Optional[str] = None,
+        headers_alias: Optional[str] = None,
+        name: Optional[str] = None,
     ):
         self.topics = topics
         self.config = config
-        self.message_encoder = message_encoder
+        self.serializer = serializer
         self.call_back = call_back
-        self.key = key
-        self.headers = headers
+        self.default_key = default_key
+        self.default_headers = default_headers
+
+        if key_alias:
+            self.key_alias = key_alias
+        if headers_alias:
+            self.headers_alias = headers_alias
 
-        PRODUCER_LIST.append(self)
+        self.__id__ = str(uuid4())
+        self.name = name or self.__id__
 
     @property
     def _producer(self) -> Producer:
         if not self._producer_instance:
             self._producer_instance = Producer(self.config.value)
         return self._producer_instance
 
@@ -73,47 +94,63 @@
         @functools.wraps(func)
         def decorator(*args: Any, **kwargs: Any) -> Any:
             try:
                 result = func(*args, **kwargs)
             except Exception as e:
                 raise e
 
-            msg = self.message_encoder(result)
+            try:
+                key = result.get(self.key_alias, self.default_key)
+            except Exception as e:
+                logger.debug(f"Failed to get key from result. {str(e)}")
+                key = self.default_key
+
+            try:
+                headers = result.get(self.headers_alias, self.default_headers)
+            except Exception as e:
+                logger.debug(
+                    f"Failed to get headers from result. {str(e)}",
+                )
+                headers = self.default_headers
+
+            headers = cast(Dict[str, str], headers)
+
+            msg = self.serializer(result)
 
-            self._produce_message(message=msg)
+            self._produce_message(message=msg, key=key, headers=headers)
 
             return result
 
         return cast(F, decorator)
 
-    def _produce_message(self, message: bytes) -> None:
+    def _produce_message(self, message: bytes, key: Optional[str], headers: Optional[Dict[str, str]]) -> None:
         for topic in self.topics:
             for partition in topic.partitions:
                 try:
                     self._producer.poll(0)
                     self._producer.produce(
                         topic=topic.name,
                         value=message,
                         partition=partition,
-                        key=self.key,
-                        headers=self.headers,
+                        key=key,
+                        headers=headers,
                         on_delivery=self.call_back,
                     )
                     self._producer.flush()
                 except Exception as e:
-                    logger.error(f"Failed to produce msg. {str(e)}")
+                    logger.exception(f"Failed to produce msg to topic: {topic.name}", exc_info=e)
                     raise e
 
 
 def delivery_report(err: str, msg: Message) -> None:
     """
     Called once for each message produced to indicate delivery result.
     Triggered by poll() or flush().
 
     :param msg:
     :param err:
     :return:
     """
     if err is not None:
-        print("Message delivery failed: {}".format(err))
+        logger.error("Message delivery failed: {}".format(err))
     else:
-        print("Message delivered to {} [{}]".format(msg.topic(), msg.partition()))
+        logger.debug("Message delivered to {} [{}]".format(msg.topic(), msg.partition()))
```

### Comparing `heizer-999999.dev1679944487/heizer/_source/topic.py` & `heizer-999999.dev1681350078/heizer/_source/topic.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/heizer/config.py` & `heizer-999999.dev1681350078/heizer/config.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/heizer.egg-info/PKG-INFO` & `heizer-999999.dev1681350078/heizer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heizer
-Version: 999999.dev1679944487
+Version: 999999.dev1681350078
 Summary: A python library to easily create kafka producer and consumer
 Author-email: Yan Zhang <dev.claude.yan.zhang@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yan Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,14 +31,19 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: socket
+Provides-Extra: dev
+Provides-Extra: doc
+Provides-Extra: test
 License-File: LICENSE
 
 # Heizer
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/heizer.svg)](https://pypi.org/project/heizer/)
 [![Package Status](https://img.shields.io/pypi/status/heizer.svg)](https://pypi.org/project/heizer/)
 [![License](https://img.shields.io/pypi/l/heizer.svg)](https://github.com/claudezss/heizer/blob/main/LICENSE)
```

### Comparing `heizer-999999.dev1679944487/heizer.egg-info/SOURCES.txt` & `heizer-999999.dev1681350078/heizer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 .gitignore
 .pre-commit-config.yaml
-.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.md
-dev-requirements.txt
 docker-compose.yaml
 pyproject.toml
-requirements.txt
 setup.py
 .github/dependabot.yml
 .github/workflows/deploy-latest.yml
 .github/workflows/main.yml
 .github/workflows/release.yml
 docs/Makefile
 docs/img1.png
 docs/make.bat
-docs/requirements.txt
 docs/source/conf.py
 docs/source/heizer.rst
 docs/source/index.rst
 docs/source/_static/.gitkeep
 docs/source/_static/websocket/create-topic.png
 docs/source/_static/websocket/message-in-browser.png
 docs/source/_static/websocket/publish-kafka-msg.png
@@ -47,9 +43,8 @@
 heizer/_source/topic.py
 heizer/bin/__init__.py
 samples/requirements.txt
 samples/websockets/client.html
 samples/websockets/server.py
 tests/__init__.py
 tests/conftest.py
-tests/requirements.txt
 tests/test_consumer.py
```

### Comparing `heizer-999999.dev1679944487/samples/websockets/client.html` & `heizer-999999.dev1681350078/samples/websockets/client.html`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/samples/websockets/server.py` & `heizer-999999.dev1681350078/samples/websockets/server.py`

 * *Files identical despite different names*

### Comparing `heizer-999999.dev1679944487/tests/test_consumer.py` & `heizer-999999.dev1681350078/tests/test_consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,22 +22,26 @@
 )
 
 
 def test_consumer_stopper() -> None:
     @producer(
         topics=[HeizerTopic(name="heizer.test.result")],
         config=Producer_Config,
+        key_alias="myKey",
+        headers_alias="myHeaders",
     )
     def produce_data(status: str, result_value: str) -> Dict[str, Any]:
         return {
             "key1": 1,
             "key2": "2",
             "key3": True,
             "status": status,
             "result": result_value,
+            "myKey": "id1",
+            "myHeaders": {"header1": "value1", "header2": "value2"},
         }
 
     def stopper(msg: HeizerMessage) -> bool:
         data = json.loads(msg.value)
         if data["status"] == "success":
             return True
         return False
@@ -45,14 +49,18 @@
     @consumer(
         topics=[HeizerTopic(name="heizer.test.result")],
         config=Consumer_Config,
         stopper=stopper,
     )
     def consume_data(msg, *args, **kwargs) -> str:
         data = json.loads(msg.value)
+
+        assert msg.key == "id1"
+        assert msg.headers == {"header1": "value1", "header2": "value2"}
+
         return cast(str, data["result"])
 
     produce_data("start", "waiting")
     produce_data("loading", "waiting")
     produce_data("success", "finished")
     produce_data("postprocess", "postprocess")
```

