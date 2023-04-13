# Comparing `tmp/kfsdutils-0.0.90.tar.gz` & `tmp/kfsdutils-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsdutils-0.0.90.tar", last modified: Thu Apr 13 14:44:13 2023, max compression
+gzip compressed data, was "kfsdutils-0.0.91.tar", last modified: Thu Apr 13 14:52:07 2023, max compression
```

## Comparing `kfsdutils-0.0.90.tar` & `kfsdutils-0.0.91.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.955378 kfsdutils-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 14:44:13.955378 kfsdutils-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.947378 kfsdutils-0.0.90/kfsdutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.947378 kfsdutils-0.0.90/kfsdutils/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.947378 kfsdutils-0.0.90/kfsdutils/apps/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/core/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.947378 kfsdutils-0.0.90/kfsdutils/apps/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.947378 kfsdutils-0.0.90/kfsdutils/apps/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/templates/browser.html
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/templates/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/docs/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/tests/test_apibrowserview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/docs/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/docs/views/apibrowser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/endpoints/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/endpoints/handlers/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/handlers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/handlers/core/basehandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/endpoints/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/renderers/kubefacetstext.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/endpoints/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/serializers/basemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/endpoints/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/endpoints/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/endpoints/views/baseview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     9468 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/tokenuser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.951377 kfsdutils-0.0.90/kfsdutils/apps/frontend/permissions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/permissions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/permissions/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.955378 kfsdutils-0.0.90/kfsdutils/apps/frontend/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/views/baseformview.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/views/basetemplateview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/frontend/views/baseview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.955378 kfsdutils-0.0.90/kfsdutils/apps/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/middleware/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/middleware/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/middleware/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.955378 kfsdutils-0.0.90/kfsdutils/apps/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/models/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/models/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/kfsdutils/apps/models/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:44:13.947378 kfsdutils-0.0.90/kfsdutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 14:44:13.000000 kfsdutils-0.0.90/kfsdutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-13 14:44:13.000000 kfsdutils-0.0.90/kfsdutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:44:13.000000 kfsdutils-0.0.90/kfsdutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:44:13.000000 kfsdutils-0.0.90/kfsdutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 14:44:13.000000 kfsdutils-0.0.90/kfsdutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 14:44:13.000000 kfsdutils-0.0.90/kfsdutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:44:13.955378 kfsdutils-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-13 14:44:04.000000 kfsdutils-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.313054 kfsdutils-0.0.91/kfsdutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13707 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/core/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/browser.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/templates/skeleton.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/tests/test_apibrowserview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/docs/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/docs/views/apibrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/basehandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.317054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetstext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/serializers/basemodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/baseview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/tokenuser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseformview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/basetemplateview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/middleware/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/kfsdutils/apps/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/kfsdutils/apps/models/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 14:52:07.313054 kfsdutils-0.0.91/kfsdutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 14:52:07.000000 kfsdutils-0.0.91/kfsdutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 14:52:07.321054 kfsdutils-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-13 14:51:54.000000 kfsdutils-0.0.91/setup.py
```

### Comparing `kfsdutils-0.0.90/LICENSE` & `kfsdutils-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/core/base.py` & `kfsdutils-0.0.91/kfsdutils/apps/core/base.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/core/configuration.py` & `kfsdutils-0.0.91/kfsdutils/apps/core/configuration.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/core/logger.py` & `kfsdutils-0.0.91/kfsdutils/apps/core/logger.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/core/utils.py` & `kfsdutils-0.0.91/kfsdutils/apps/core/utils.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/core/yaml.py` & `kfsdutils-0.0.91/kfsdutils/apps/core/yaml.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/docs/templates/browser.html` & `kfsdutils-0.0.91/kfsdutils/apps/docs/templates/browser.html`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/docs/templates/skeleton.html` & `kfsdutils-0.0.91/kfsdutils/apps/docs/templates/skeleton.html`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/docs/views/apibrowser.py` & `kfsdutils-0.0.91/kfsdutils/apps/docs/views/apibrowser.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/endpoints/exceptions.py` & `kfsdutils-0.0.91/kfsdutils/apps/endpoints/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/endpoints/handlers/core/basehandler.py` & `kfsdutils-0.0.91/kfsdutils/apps/endpoints/handlers/core/basehandler.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py` & `kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsjson.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py` & `kfsdutils-0.0.91/kfsdutils/apps/endpoints/renderers/kubefacetsyaml.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py` & `kfsdutils-0.0.91/kfsdutils/apps/endpoints/tests/endpoints_test_handler.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/endpoints/views/baseview.py` & `kfsdutils-0.0.91/kfsdutils/apps/endpoints/views/baseview.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/apiclient.py` & `kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/apiclient.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/login.py` & `kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         return self.httpGet(verifyTokensUrl, HTTPStatus.OK, self.getApplicationAuthReqHttpHeaders())
     
     def userExists(self, email):
         authHost, userExistsUri, userIdentifierPrefix = self.findConfigs(["auth_api.host", "auth_api.user_exists_url", "auth_api.user_identifier_prefix"])
         userIdentifier = userIdentifierPrefix.format(email)
         userExistsUri = userExistsUri.format(GeneralUtils.genUrlEncode(userIdentifier))
         userExistsUrl = self.formatUrl([authHost, userExistsUri])
-        return self.httpGet(userExistsUrl, HTTPStatus.OK, APIClient.JSON, self.getApplicationAuthReqHttpHeaders())
+        return self.httpGet(userExistsUrl, HTTPStatus.OK, self.getApplicationAuthReqHttpHeaders())
 
     def sendVerifyEmail(self, email, emailType):
         authHost, verifyEmailUri, userIdentifierPrefix = self.findConfigs(["auth_api.host", "auth_api.verify_email_url", "auth_api.user_identifier_prefix"])
         userIdentifier = userIdentifierPrefix.format(email)
         payload = {"user": userIdentifier, "type": emailType}
         verifyEmailUrl = self.formatUrl([authHost, verifyEmailUri])
         return self.httpPost(verifyEmailUrl, [HTTPStatus.CREATED, HTTPStatus.BAD_REQUEST], payload, self.getApplicationAuthReqHttpHeaders())
```

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/frontend/handlers/tokenuser.py` & `kfsdutils-0.0.91/kfsdutils/apps/frontend/handlers/tokenuser.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/frontend/permissions/base.py` & `kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/base.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/frontend/permissions/common.py` & `kfsdutils-0.0.91/kfsdutils/apps/frontend/permissions/common.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/frontend/views/baseformview.py` & `kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseformview.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/frontend/views/baseview.py` & `kfsdutils-0.0.91/kfsdutils/apps/frontend/views/baseview.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/middleware/configuration.py` & `kfsdutils-0.0.91/kfsdutils/apps/middleware/configuration.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils/apps/models/basemodel.py` & `kfsdutils-0.0.91/kfsdutils/apps/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `kfsdutils-0.0.90/kfsdutils.egg-info/SOURCES.txt` & `kfsdutils-0.0.91/kfsdutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

