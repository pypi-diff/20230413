# Comparing `tmp/EOxServer-1.2.4.tar.gz` & `tmp/EOxServer-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EOxServer-1.2.4.tar", last modified: Thu Mar 30 10:37:55 2023, max compression
+gzip compressed data, was "EOxServer-1.2.5.tar", last modified: Thu Apr 13 11:03:44 2023, max compression
```

## Comparing `EOxServer-1.2.4.tar` & `EOxServer-1.2.5.tar`

### file list

```diff
@@ -1,564 +1,565 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.792377 EOxServer-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/EOxServer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-03-30 10:37:55.000000 EOxServer-1.2.4/EOxServer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21098 2023-03-30 10:37:55.000000 EOxServer-1.2.4/EOxServer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:37:55.000000 EOxServer-1.2.4/EOxServer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:37:55.000000 EOxServer-1.2.4/EOxServer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-30 10:37:55.000000 EOxServer-1.2.4/EOxServer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-30 10:37:55.000000 EOxServer-1.2.4/EOxServer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-30 10:37:35.000000 EOxServer-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-30 10:37:35.000000 EOxServer-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-03-30 10:37:55.792377 EOxServer-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-30 10:37:35.000000 EOxServer-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/backends/keystone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/keystone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/keystone/storage_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/backends/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/management/commands/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/management/commands/storageauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/migrations/0002_storage_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/migrations/0003_nameblank.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/storage_auths.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/storages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/testbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/backends/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/conf/default.conf
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/conf/defaultAttributeDictionary
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/conf/default_formats.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/gdal_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/mapserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/osr.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/vrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/contrib/vsi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/core/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/commands/create_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/core/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/decoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/decoders/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/decoders/kvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/decoders/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/core/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/templates/admin/change_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/templates/eoxserver_index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/core/templates/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/templates/logging/logview.html
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/geotools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/importtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/iteratortools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/multiparttools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/perftools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/timetools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/util/xmltools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/instance_template/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/instance_template/project_name/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/eoxserver.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/formats.conf
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/outline_template_dataset.html
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/outline_template_footer.html
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/outline_template_header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.752376 EOxServer-1.2.4/eoxserver/instance_template/project_name/data/
--rw-r--r--   0 runner    (1001) docker     (123)   879633 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/instance_template/project_name/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/logs/DO-NOT-REMOVE
--rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/instance_template/project_name/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/static/DO-NOT-REMOVE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/500.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.html
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.js
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/instance_template/project_name/wcst_perm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/wcst_perm/DO-NOT-REMOVE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/instance_template/project_name/wcst_temp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/wcst_temp/DO-NOT-REMOVE
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/instance_template/project_name/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.744376 EOxServer-1.2.4/eoxserver/media/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/media/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/media/admin/widgets.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/media/images/
--rw-r--r--   0 runner    (1001) docker     (123)   146838 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/media/images/eoxserver_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   171474 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/media/images/eoxserver_logo_transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/processing/gdal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/gdal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31278 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/gdal/reftools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/gdal/vrt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/processing/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/preprocessing/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/preprocessing/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/preprocessing/georeference.py
--rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/preprocessing/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/processing/preprocessing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/render/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/render/browse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/browse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/browse/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/browse/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/browse/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/browse/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    32830 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/render/coverage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/coverage/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.756376 EOxServer-1.2.4/eoxserver/render/map/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/map/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/map/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/map/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.760376 EOxServer-1.2.4/eoxserver/render/mapserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/mapserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/mapserver/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    32386 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/mapserver/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/render/mapserver/map_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.760376 EOxServer-1.2.4/eoxserver/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.760376 EOxServer-1.2.4/eoxserver/resources/coverages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/crss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/dateline.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.760376 EOxServer-1.2.4/eoxserver/resources/coverages/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.760376 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/browse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/browsetype.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/collectiontype.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/coveragetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/mapcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/masktype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/product.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/producttype.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.760376 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.764376 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py
--rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.764376 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/gsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.764376 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/utils/gsc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.764376 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0006_masktype_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0007_typemodels.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0008_incidence_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0009_begin_time_end_time_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0011_bandstatistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0012_out_of_bounds_data_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43338 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.764376 EOxServer-1.2.4/eoxserver/resources/coverages/registration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/browse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/product.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.764376 EOxServer-1.2.4/eoxserver/resources/coverages/registration/registrators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/registrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/registrators/gdal.py
--rw-r--r--   0 runner    (1001) docker     (123)    30037 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/registration/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/resources/coverages/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.764376 EOxServer-1.2.4/eoxserver/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/scripts/eoxserver-instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/auth/charonpdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/auth/dummypdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/auth/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/auth/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/cis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/cis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/cis/v11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/cis/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/cis/v11/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ecql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/gdal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/gdal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/gdal/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/gdal/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/gml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/gml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/gml/v32/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/gml/v32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/gml/v32/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/management/commands/eoxs_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/management/commands/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/management/commands/wms_options_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/management/commands/wms_options_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/management/commands/wms_options_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/mapserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/mapserver/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/connectors/mosaic_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/connectors/multifile_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/connectors/polygonmask_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/connectors/simple_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/connectors/tileindex_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.768376 EOxServer-1.2.4/eoxserver/services/mapserver/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wcs/base_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wcs/capabilities_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wcs/coverage_description_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wcs/coverage_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/mapserver/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/capabilities_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/feature_info_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/legendgraphic_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/map_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/mapserver/wms/styleapplicators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/styleapplicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/styleapplicators/sld.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/mapserver/wms/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/migrations/0003_service_name_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/native/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/native/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/native/wcs/capabilities_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/native/wcs/coverage_description_renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/opensearch/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/extensions/cql.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/extensions/eo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/extensions/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/extensions/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/opensearch/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/formats/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)    22258 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/formats/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/formats/geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/formats/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/formats/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/opensearch/v11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/v11/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/v11/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/opensearch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.772377 EOxServer-1.2.4/eoxserver/services/ows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/common/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/common/v11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/common/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/common/v11/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/common/v20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/common/v20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/common/v20/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/common/v20/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/dseo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/dseo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/dseo/v10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/dseo/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/dseo/v10/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/dseo/v10/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/basehandlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/describecoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/getcoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/describecoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/getcoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.776377 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/describecoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/describeeocoverageset.py
--rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.780377 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/encodings/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/encodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/encodings/geotiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/getcoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/geteocoverageset.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.780377 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/packages/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/packages/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13005 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wcs11Transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.780377 EOxServer-1.2.4/eoxserver/services/ows/wms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/basehandlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    29074 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/layermapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.780377 EOxServer-1.2.4/eoxserver/services/ows/wms/v10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v10/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v10/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v10/getfeatureinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v10/getmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v10/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.780377 EOxServer-1.2.4/eoxserver/services/ows/wms/v11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v11/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v11/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v11/getfeatureinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v11/getmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v11/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.780377 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getfeatureinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getlegendgraphic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wms/v13/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.780377 EOxServer-1.2.4/eoxserver/services/ows/wps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/allowed_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/bboxdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/complexdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/literaldata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/response_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/ows/wps/processes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/processes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_cloud_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_dem_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_height_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_time_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/test_allowed_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/describeprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/execute_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/process_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_decoder_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_decoder_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v10/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/ows/wps/v20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v20/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v20/describeprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v20/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/ows/wps/v20/getcapabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/subset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.744376 EOxServer-1.2.4/eoxserver/services/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/templates/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/templates/opensearch/result.html
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/templates/opensearch/summary.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/templates/wcs/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/templates/wcs/error_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/services/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/templatetags/services_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/services/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.784377 EOxServer-1.2.4/eoxserver/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/testing/xcomp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.788377 EOxServer-1.2.4/eoxserver/webclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.788377 EOxServer-1.2.4/eoxserver/webclient/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/migrations/0002_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.788377 EOxServer-1.2.4/eoxserver/webclient/static/
--rw-r--r--   0 runner    (1001) docker     (123)   544139 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/static/822268aa1a6cd4dedba8.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)    17842 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/static/EOxServer_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)  4799085 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/static/prism.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.748376 EOxServer-1.2.4/eoxserver/webclient/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.792377 EOxServer-1.2.4/eoxserver/webclient/templates/webclient/
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/templates/webclient/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/templates/webclient/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-03-30 10:37:36.000000 EOxServer-1.2.4/eoxserver/webclient/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-30 10:37:36.000000 EOxServer-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-30 10:37:55.792377 EOxServer-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-03-30 10:37:36.000000 EOxServer-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:37:55.792377 EOxServer-1.2.4/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14419 2023-03-30 10:37:36.000000 EOxServer-1.2.4/tools/eoxserver-atpd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-03-30 10:37:36.000000 EOxServer-1.2.4/tools/eoxserver-preprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3435 2023-03-30 10:37:36.000000 EOxServer-1.2.4/tools/eoxserver-validate_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.367155 EOxServer-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.319153 EOxServer-1.2.5/EOxServer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-13 11:03:44.000000 EOxServer-1.2.5/EOxServer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21154 2023-04-13 11:03:44.000000 EOxServer-1.2.5/EOxServer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:03:44.000000 EOxServer-1.2.5/EOxServer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:03:44.000000 EOxServer-1.2.5/EOxServer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-13 11:03:44.000000 EOxServer-1.2.5/EOxServer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 11:03:44.000000 EOxServer-1.2.5/EOxServer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-13 11:03:23.000000 EOxServer-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 11:03:23.000000 EOxServer-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-13 11:03:44.367155 EOxServer-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-13 11:03:23.000000 EOxServer-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.319153 EOxServer-1.2.5/eoxserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/backends/keystone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/keystone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/keystone/storage_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/backends/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/management/commands/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/management/commands/storageauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/migrations/0002_storage_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/migrations/0003_nameblank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/migrations/0004_storage_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/storage_auths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/storages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/testbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/backends/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/conf/default.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/conf/defaultAttributeDictionary
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/conf/default_formats.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/gdal_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/mapserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/osr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/vrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/contrib/vsi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.323154 EOxServer-1.2.5/eoxserver/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/commands/create_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/core/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/decoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/decoders/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/decoders/kvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/decoders/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/core/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/templates/admin/change_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/templates/eoxserver_index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/core/templates/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/templates/logging/logview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/geotools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/importtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/iteratortools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/multiparttools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/perftools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/timetools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/util/xmltools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/eoxserver.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/formats.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/outline_template_dataset.html
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/outline_template_footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/outline_template_header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   879633 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/logs/DO-NOT-REMOVE
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/static/DO-NOT-REMOVE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/500.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/admin/openlayers_extralayers.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/wcst_perm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/wcst_perm/DO-NOT-REMOVE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/instance_template/project_name/wcst_temp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/wcst_temp/DO-NOT-REMOVE
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/instance_template/project_name/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.315153 EOxServer-1.2.5/eoxserver/media/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.327154 EOxServer-1.2.5/eoxserver/media/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/media/admin/widgets.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/media/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   146838 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/media/images/eoxserver_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   171474 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/media/images/eoxserver_logo_transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/processing/gdal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/gdal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31278 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/gdal/reftools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/gdal/vrt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/processing/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/preprocessing/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/preprocessing/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/preprocessing/georeference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/preprocessing/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/processing/preprocessing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/render/browse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/browse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/browse/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/browse/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9891 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/browse/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/browse/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32830 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/render/coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26071 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/coverage/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/render/map/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/map/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/map/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/map/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/render/mapserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/mapserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/mapserver/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32608 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/mapserver/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/render/mapserver/map_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/resources/coverages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/crss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/dateline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.331154 EOxServer-1.2.5/eoxserver/resources/coverages/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.335154 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/browse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/browsetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/collectiontype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/coveragetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/mapcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/masktype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/producttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.335154 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.335154 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14250 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.335154 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.335154 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/utils/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.339154 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0006_masktype_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0007_typemodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0008_incidence_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0009_begin_time_end_time_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0011_bandstatistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0012_out_of_bounds_data_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43338 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.339154 EOxServer-1.2.5/eoxserver/resources/coverages/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/browse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/product.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.339154 EOxServer-1.2.5/eoxserver/resources/coverages/registration/registrators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/registrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/registrators/gdal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/registration/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/resources/coverages/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.339154 EOxServer-1.2.5/eoxserver/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/scripts/eoxserver-instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.339154 EOxServer-1.2.5/eoxserver/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/auth/charonpdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/auth/dummypdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/auth/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/auth/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/cis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/cis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/cis/v11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/cis/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/cis/v11/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ecql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/gdal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/gdal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/gdal/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/gdal/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/gml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/gml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/gml/v32/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/gml/v32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/gml/v32/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/management/commands/eoxs_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/management/commands/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/management/commands/wms_options_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/management/commands/wms_options_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/management/commands/wms_options_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/mapserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/mapserver/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/connectors/mosaic_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/connectors/multifile_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/connectors/polygonmask_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/connectors/simple_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/connectors/tileindex_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/mapserver/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wcs/base_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wcs/capabilities_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wcs/coverage_description_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wcs/coverage_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/mapserver/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/capabilities_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/feature_info_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.343154 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/legendgraphic_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/map_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/mapserver/wms/styleapplicators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/styleapplicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/styleapplicators/sld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/mapserver/wms/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/migrations/0003_service_name_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/native/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/native/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/native/wcs/capabilities_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/native/wcs/coverage_description_renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/opensearch/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/extensions/cql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/extensions/eo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/extensions/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/extensions/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/opensearch/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/formats/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22258 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/formats/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/formats/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/formats/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/formats/rss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/opensearch/v11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8191 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/v11/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/v11/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/opensearch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/ows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/ows/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/common/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/ows/common/v11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/common/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/common/v11/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.347154 EOxServer-1.2.5/eoxserver/services/ows/common/v20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/common/v20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/common/v20/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/common/v20/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/dseo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/dseo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/dseo/v10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/dseo/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/dseo/v10/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/dseo/v10/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/basehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/describecoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/getcoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/describecoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/getcoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/describecoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/describeeocoverageset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29749 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/encodings/geotiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/getcoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16676 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/geteocoverageset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.351154 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/packages/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/packages/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13005 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wcs11Transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.355154 EOxServer-1.2.5/eoxserver/services/ows/wms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/basehandlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29376 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/layermapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.355154 EOxServer-1.2.5/eoxserver/services/ows/wms/v10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v10/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v10/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v10/getfeatureinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v10/getmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v10/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.355154 EOxServer-1.2.5/eoxserver/services/ows/wms/v11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v11/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v11/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v11/getfeatureinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v11/getmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v11/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.355154 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getfeatureinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getlegendgraphic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wms/v13/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.355154 EOxServer-1.2.5/eoxserver/services/ows/wps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/allowed_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/bboxdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/complexdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/literaldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/response_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/ows/wps/processes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/processes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_cloud_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_dem_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_height_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_time_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/test_allowed_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17124 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/describeprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/execute_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/process_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_decoder_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_decoder_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v10/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/ows/wps/v20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v20/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v20/describeprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v20/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/ows/wps/v20/getcapabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/subset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.319153 EOxServer-1.2.5/eoxserver/services/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/templates/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/templates/opensearch/result.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/templates/opensearch/summary.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/templates/wcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/templates/wcs/error_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/services/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/templatetags/services_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25514 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/services/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/testing/xcomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.359155 EOxServer-1.2.5/eoxserver/webclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.363155 EOxServer-1.2.5/eoxserver/webclient/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/migrations/0002_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.363155 EOxServer-1.2.5/eoxserver/webclient/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   544139 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/static/822268aa1a6cd4dedba8.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17842 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/static/EOxServer_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)  4799085 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/static/prism.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.319153 EOxServer-1.2.5/eoxserver/webclient/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.367155 EOxServer-1.2.5/eoxserver/webclient/templates/webclient/
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/templates/webclient/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/templates/webclient/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-13 11:03:24.000000 EOxServer-1.2.5/eoxserver/webclient/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-13 11:03:24.000000 EOxServer-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-13 11:03:44.367155 EOxServer-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-04-13 11:03:24.000000 EOxServer-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:03:44.367155 EOxServer-1.2.5/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14419 2023-04-13 11:03:24.000000 EOxServer-1.2.5/tools/eoxserver-atpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-04-13 11:03:24.000000 EOxServer-1.2.5/tools/eoxserver-preprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3435 2023-04-13 11:03:24.000000 EOxServer-1.2.5/tools/eoxserver-validate_xml.py
```

### Comparing `EOxServer-1.2.4/EOxServer.egg-info/PKG-INFO` & `EOxServer-1.2.5/EOxServer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOxServer
-Version: 1.2.4
+Version: 1.2.5
 Summary: EOxServer is a server for Earth Observation (EO) data
 Home-page: http://eoxserver.org/
 Author: EOX IT Services GmbH
 Author-email: office@eox.at
 Maintainer: EOX IT Services GmbH
 Maintainer-email: packages@eox.at
 License: EOxServer Open License (MIT-style)
```

### Comparing `EOxServer-1.2.4/EOxServer.egg-info/SOURCES.txt` & `EOxServer-1.2.5/EOxServer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 eoxserver/backends/management/__init__.py
 eoxserver/backends/management/commands/__init__.py
 eoxserver/backends/management/commands/storage.py
 eoxserver/backends/management/commands/storageauth.py
 eoxserver/backends/migrations/0001_initial.py
 eoxserver/backends/migrations/0002_storage_auth.py
 eoxserver/backends/migrations/0003_nameblank.py
+eoxserver/backends/migrations/0004_storage_streaming.py
 eoxserver/backends/migrations/__init__.py
 eoxserver/conf/default.conf
 eoxserver/conf/defaultAttributeDictionary
 eoxserver/conf/default_formats.conf
 eoxserver/contrib/__init__.py
 eoxserver/contrib/gdal.py
 eoxserver/contrib/gdal_array.py
```

### Comparing `EOxServer-1.2.4/LICENSE` & `EOxServer-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/PKG-INFO` & `EOxServer-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EOxServer
-Version: 1.2.4
+Version: 1.2.5
 Summary: EOxServer is a server for Earth Observation (EO) data
 Home-page: http://eoxserver.org/
 Author: EOX IT Services GmbH
 Author-email: office@eox.at
 Maintainer: EOX IT Services GmbH
 Maintainer-email: packages@eox.at
 License: EOxServer Open License (MIT-style)
```

### Comparing `EOxServer-1.2.4/README.md` & `EOxServer-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/__init__.py` & `EOxServer-1.2.5/eoxserver/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 # ------------------------------------------------------------------------------
 
 
-__version__ = '1.2.4'
+__version__ = '1.2.5'
 
 
 def get_version():
     return __version__
```

### Comparing `EOxServer-1.2.4/eoxserver/backends/access.py` & `EOxServer-1.2.5/eoxserver/backends/access.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,26 +97,26 @@
             storage, handler_cls = current
             child_storage, _ = child
 
             item_id = _generate_hash(data_item.location, data_item.format)
             tmp_path = cache.relative_path(item_id)
             if not cache.contains(item_id):
                 # actually retrieve the item when not in the cache
-                handler = handler_cls(path or storage.url)
+                handler = handler_cls(path or storage.url, storage.streaming)
                 use_cache, path = handler.retrieve(
                     path or child_storage.url, tmp_path
                 )
                 if not use_cache:
                     cache.add_mapping(path)
             else:
                 path = tmp_path
 
         if storage_handlers:
             storage, handler_cls = storage_handlers[-1]
-            handler = handler_cls(path)
+            handler = handler_cls(path, storage.streaming)
             return handler.retrieve(data_item.location)[1]
 
 
 def open(data_item, cache=None):
     """ Returns a file object pointing to the given location. This function
     works like the builtin function :func:`open() <__builtins__.open>` but on
     a :class:`DataItem <eoxserver.backends.models.DataItem>` and performs a
@@ -155,15 +155,15 @@
     return vsi_path
 
 
 def get_vsi_storage_path(storage, location=None):
     while storage:
         handler_cls = get_handler_class_for_model(storage)
         if handler_cls:
-            handler = handler_cls(storage.url)
+            handler = handler_cls(storage.url, storage.streaming)
             location = handler.get_vsi_path(location or '')
         else:
             raise AccessError(
                 'Unsupported storage type %r' % storage.storage_type
             )
         storage = storage.parent
 
@@ -174,15 +174,15 @@
 def get_vsi_env(storage):
     """
     """
     env = {}
     while storage:
         handler_cls = get_handler_class_for_model(storage)
         if handler_cls:
-            handler = handler_cls(storage.url)
+            handler = handler_cls(storage.url, storage.streaming)
             env.update(handler.get_vsi_env())
         else:
             raise AccessError(
                 'Unsupported storage type %r' % storage.storage_type
             )
 
         if storage.storage_auth:
```

### Comparing `EOxServer-1.2.4/eoxserver/backends/admin.py` & `EOxServer-1.2.5/eoxserver/backends/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/cache.py` & `EOxServer-1.2.5/eoxserver/backends/cache.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/component.py` & `EOxServer-1.2.5/eoxserver/backends/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/config.py` & `EOxServer-1.2.5/eoxserver/backends/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/interfaces.py` & `EOxServer-1.2.5/eoxserver/backends/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/keystone/storage_auth.py` & `EOxServer-1.2.5/eoxserver/backends/keystone/storage_auth.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/management/commands/storage.py` & `EOxServer-1.2.5/eoxserver/backends/management/commands/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,20 @@
             help='The name of the parent storage. Optional.'
         )
         create_parser.add_argument(
             '--storage-auth', '--storage-auth-name', '--auth', '-a',
             dest='storage_auth_name', default=None,
             help='The name of the storage auth to use. Optional',
         )
+        create_parser.add_argument(
+            '--streaming', action="store_true",
+            default=False,
+            help="""If used, respective streaming version of /vsi file 
+            accessor will be used."""
+        )
 
         for parser in [list_parser, env_parser]:
             parser.add_argument(
                 'paths', nargs='*', default=None,
                 help=(
                     'Possible sub-path on that storage. This may include '
                     'specifiers for sub-storages'
@@ -99,15 +105,15 @@
             self.handle_delete(name, *args, **kwargs)
         elif subcommand == "list":
             self.handle_list(name, *args, **kwargs)
         elif subcommand == "env":
             self.handle_env(name, *args, **kwargs)
 
     def handle_create(self, name, url, type_name, parent_name,
-                      storage_auth_name, **kwargs):
+                      storage_auth_name, streaming, **kwargs):
         """ Handle the creation of a new storage.
         """
         url = url[0]
         parent = None
 
         if type_name:
             handler = get_handler_class_by_name(type_name)
@@ -137,15 +143,15 @@
                 name=storage_auth_name
             )
         else:
             storage_auth = None
 
         backends.Storage.objects.create(
             name=name, url=url, storage_type=type_name, parent=parent,
-            storage_auth=storage_auth,
+            storage_auth=storage_auth, streaming=streaming,
         )
 
         self.print_msg(
             'Successfully created storage %s (%s)' % (
                 name or url, type_name
             )
         )
```

### Comparing `EOxServer-1.2.4/eoxserver/backends/management/commands/storageauth.py` & `EOxServer-1.2.5/eoxserver/backends/management/commands/storageauth.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/middleware.py` & `EOxServer-1.2.5/eoxserver/backends/middleware.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/migrations/0001_initial.py` & `EOxServer-1.2.5/eoxserver/backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/migrations/0002_storage_auth.py` & `EOxServer-1.2.5/eoxserver/backends/migrations/0002_storage_auth.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/migrations/0003_nameblank.py` & `EOxServer-1.2.5/eoxserver/backends/migrations/0003_nameblank.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/models.py` & `EOxServer-1.2.5/eoxserver/backends/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     """ Model to symbolize storages that provide file or other types of access
         to data items.
     """
     url = models.CharField(max_length=1024, **mandatory)
     storage_type = models.CharField(max_length=32, **mandatory)
     name = models.CharField(max_length=1024, null=True, blank=True, unique=True)
     storage_auth = models.ForeignKey(StorageAuth, on_delete=models.CASCADE, **optional)
+    streaming = models.BooleanField(null=True, blank=True)
 
     parent = models.ForeignKey("self", on_delete=models.CASCADE, **optional)
 
     def __str__(self):
         return "%s: %s" % (self.storage_type, self.url)
 
     def clean(self):
```

### Comparing `EOxServer-1.2.4/eoxserver/backends/storage_auths.py` & `EOxServer-1.2.5/eoxserver/backends/storage_auths.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/storages.py` & `EOxServer-1.2.5/eoxserver/backends/storages.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,17 +106,18 @@
     name = "ZIP"
 
     allows_child_storages = True
     allows_parent_storage = True
 
     is_local = True
 
-    def __init__(self, package_filename):
+    def __init__(self, package_filename, streaming):
         self.package_filename = package_filename
         self.zipfile = None
+        self.streaming = streaming
 
     def __enter__(self):
         self.zipfile = zipfile.ZipFile(self.package_filename, "r")
         return self
 
     def __exit__(self, type, value, traceback):
         self.zipfile.close()
@@ -149,17 +150,18 @@
     name = "TAR"
 
     allows_child_storages = True
     allows_parent_storage = True
 
     is_local = True
 
-    def __init__(self, package_filename):
+    def __init__(self, package_filename, streaming):
         self.package_filename = package_filename
         self.tarfile = None
+        self.streaming = streaming
 
     def __enter__(self):
         self.tarfile = tarfile.TarFile(self.package_filename, "r")
         return self
 
     def __exit__(self, type, value, traceback):
         self.tarfile.close()
@@ -193,16 +195,17 @@
     name = 'directory'
 
     allows_child_storages = True
     allows_parent_storage = True
 
     is_local = True
 
-    def __init__(self, dirpath):
+    def __init__(self, dirpath, streaming):
         self.dirpath = dirpath
+        self.streaming = streaming
 
     def retrieve(self, location, path):
         return False, os.path.join(self.dirpath, location)
 
     def list_files(self, glob_pattern=None):
         glob_pattern = glob_pattern or '*'
         return glob.glob(os.path.join(self.dirpath, glob_pattern))
@@ -220,23 +223,28 @@
     """
 
     name = 'HTTP'
 
     allows_child_storages = True
     allows_parent_storage = False
 
-    def __init__(self, url):
+    def __init__(self, url, streaming):
         self.url = url
+        self.streaming = streaming
 
     def retrieve(self, location, path):
         request.urlretrieve(parse.urljoin(self.url, location), path)
         return True, path
 
     def get_vsi_path(self, location):
-        return '/vsicurl/%s' % parse.urljoin(self.url, location)
+        if self.streaming:
+            prefix = '/vsicurl_streaming/'
+        else:
+            prefix = '/vsicurl/'
+        return '%s%s' % (prefix, parse.urljoin(self.url, location))
 
     @classmethod
     def test(cls, locator):
         try:
             return urlparse(locator).scheme.lower() in ('http', 'https')
         except:
             return False
@@ -247,18 +255,19 @@
     """
 
     name = 'FTP'
 
     allows_parent_storage = True
     allows_parent_storage = False
 
-    def __init__(self, url):
+    def __init__(self, url, streaming):
         self.url = url
         self.parsed_url = urlparse(url)
         self.ftp = None
+        self.streaming=streaming
 
     def __enter__(self):
         self.ftp = ftplib.FTP()
         self.ftp.connect(self.parsed_url.hostname, self.parsed_url.port)
         self.ftp.login(self.parsed_url.username, self.parsed_url.password)
         return self
 
@@ -281,15 +290,19 @@
             else:
                 raise
         if glob_pattern:
             filenames = fnmatch.filter(filenames, glob_pattern)
         return filenames
 
     def get_vsi_path(self, location):
-        return '/vsicurl/%s' % parse.urljoin(self.url, location)
+        if self.streaming:
+            prefix = '/vsicurl_streaming/'
+        else:
+            prefix = '/vsicurl/'
+        return '%s%s' % (prefix, parse.urljoin(self.url, location))
 
     @classmethod
     def test(cls, locator):
         try:
             return urlparse(locator).scheme.lower() == 'ftp'
         except:
             return False
@@ -297,54 +310,59 @@
 
 class SwiftStorageHandler(BaseStorageHandler):
     name = 'swift'
 
     allows_parent_storage = False
     allows_child_storages = True
 
-    def __init__(self, url):
+    def __init__(self, url, streaming):
         self.container = url
+        self.streaming = streaming
 
     def retrieve(self, location, path):
         pass
 
     def list_files(self, location, glob_pattern=None):
         return []
 
     def get_vsi_path(self, location):
-        return vsi.join('/vsiswift/%s' % self.container, location)
+        if self.streaming:
+            prefix = '/vsiswift_streaming'
+        else:
+            prefix = '/vsiswift'
+        base_path = f'{prefix}/{self.container}' if self.container else prefix
+        return vsi.join(base_path, location)
 
     @classmethod
     def test(cls, locator):
         return False
 
 
 class S3StorageHandler(BaseStorageHandler):
     name = 'S3'
 
     allows_parent_storage = False
     allows_child_storages = True
 
-    def __init__(self, url):
+    def __init__(self, url, streaming):
         self.bucket = url
+        self.streaming = streaming
 
     def retrieve(self, location, path):
         pass
 
     def list_files(self, location, glob_pattern=None):
         return []
 
     def get_vsi_path(self, location):
-        import logging
-        logger = logging.getLogger(__name__)
-
-        # logger.debug()
-
-
-        base_path = '/vsis3/%s' % self.bucket if self.bucket else '/vsis3'
+        if self.streaming:
+            prefix = '/vsis3_streaming'
+        else:
+            prefix = '/vsis3'
+        base_path = f'{prefix}/{self.bucket}' if self.bucket else prefix
         return vsi.join(base_path, location)
 
     @classmethod
     def test(cls, locator):
         return False
```

### Comparing `EOxServer-1.2.4/eoxserver/backends/testbase.py` & `EOxServer-1.2.5/eoxserver/backends/testbase.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/tests.py` & `EOxServer-1.2.5/eoxserver/backends/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/backends/util.py` & `EOxServer-1.2.5/eoxserver/backends/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/conf/default.conf` & `EOxServer-1.2.5/eoxserver/conf/default.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/conf/default_formats.conf` & `EOxServer-1.2.5/eoxserver/conf/default_formats.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/contrib/__init__.py` & `EOxServer-1.2.5/eoxserver/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/contrib/gdal.py` & `EOxServer-1.2.5/eoxserver/contrib/gdal.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/contrib/gdal_array.py` & `EOxServer-1.2.5/eoxserver/contrib/gdal_array.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/contrib/mapserver.py` & `EOxServer-1.2.5/eoxserver/contrib/mapserver.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/contrib/ogr.py` & `EOxServer-1.2.5/eoxserver/contrib/ogr.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/contrib/osr.py` & `EOxServer-1.2.5/eoxserver/contrib/osr.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/contrib/vrt.py` & `EOxServer-1.2.5/eoxserver/contrib/vrt.py`

 * *Files 2% similar despite different names*

```diff
@@ -494,29 +494,35 @@
                 x_size=x_size, y_size=y_size,
             ), "new_vrt_sources")
 
             out_index += 1
 
     return out_ds
 
+def sign_abs(x):
+    return 0.0 if abs(x) == 0 else x / abs(x)
+
 def with_extent(filename, extent, save=None):
     """ Create a VRT and override the underlying files geolocation
     """
     src_ds = gdal.OpenShared(filename)
     width, height = src_ds.RasterXSize, src_ds.RasterYSize
     driver = gdal.GetDriverByName('VRT')
     out_ds = driver.CreateCopy(save, src_ds)
 
     x = extent[0]
     y = extent[3]
 
+    source_geotransform = src_ds.GetGeoTransform()
+    resy_sign_north_up = sign_abs(source_geotransform[5])
+
     resx = abs(extent[2] - extent[0]) / width
     resy = abs(extent[3] - extent[1]) / height
     out_ds.SetGeoTransform([
         x,
         resx,
         0,
         y,
         0,
-        resy,
+        resy_sign_north_up * resy,
     ])
     return out_ds
```

### Comparing `EOxServer-1.2.4/eoxserver/contrib/vsi.py` & `EOxServer-1.2.5/eoxserver/contrib/vsi.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/__init__.py` & `EOxServer-1.2.5/eoxserver/core/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/commands/__init__.py` & `EOxServer-1.2.5/eoxserver/core/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/commands/create_instance.py` & `EOxServer-1.2.5/eoxserver/core/commands/create_instance.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/component.py` & `EOxServer-1.2.5/eoxserver/core/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/config.py` & `EOxServer-1.2.5/eoxserver/core/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/decoders/__init__.py` & `EOxServer-1.2.5/eoxserver/core/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/decoders/base.py` & `EOxServer-1.2.5/eoxserver/core/decoders/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/decoders/config.py` & `EOxServer-1.2.5/eoxserver/core/decoders/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/decoders/kvp.py` & `EOxServer-1.2.5/eoxserver/core/decoders/kvp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/decoders/xml.py` & `EOxServer-1.2.5/eoxserver/core/decoders/xml.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/instance.py` & `EOxServer-1.2.5/eoxserver/core/instance.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/management.py` & `EOxServer-1.2.5/eoxserver/core/management.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/models.py` & `EOxServer-1.2.5/eoxserver/core/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/templates/admin/change_confirmation.html` & `EOxServer-1.2.5/eoxserver/core/templates/admin/change_confirmation.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/templates/eoxserver_index.html` & `EOxServer-1.2.5/eoxserver/core/templates/eoxserver_index.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/templates/logging/logview.html` & `EOxServer-1.2.5/eoxserver/core/templates/logging/logview.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/tests.py` & `EOxServer-1.2.5/eoxserver/core/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/functools.py` & `EOxServer-1.2.5/eoxserver/core/util/functools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/geotools.py` & `EOxServer-1.2.5/eoxserver/core/util/geotools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/importtools.py` & `EOxServer-1.2.5/eoxserver/core/util/importtools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/iteratortools.py` & `EOxServer-1.2.5/eoxserver/core/util/iteratortools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/multiparttools.py` & `EOxServer-1.2.5/eoxserver/core/util/multiparttools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/perftools.py` & `EOxServer-1.2.5/eoxserver/core/util/perftools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/rect.py` & `EOxServer-1.2.5/eoxserver/core/util/rect.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/timetools.py` & `EOxServer-1.2.5/eoxserver/core/util/timetools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/util/xmltools.py` & `EOxServer-1.2.5/eoxserver/core/util/xmltools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/core/views.py` & `EOxServer-1.2.5/eoxserver/core/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/manage.py` & `EOxServer-1.2.5/eoxserver/instance_template/manage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/eoxserver.conf` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/eoxserver.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/formats.conf` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/formats.conf`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/conf/outline_template_dataset.html` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/conf/outline_template_dataset.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/data/init_spatialite-2.3.sql`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/settings.py` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/settings.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/templates/admin/base_site.html` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/urls.py` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/instance_template/project_name/wsgi.py` & `EOxServer-1.2.5/eoxserver/instance_template/project_name/wsgi.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/media/images/eoxserver_logo.png` & `EOxServer-1.2.5/eoxserver/media/images/eoxserver_logo.png`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/media/images/eoxserver_logo_transparent.png` & `EOxServer-1.2.5/eoxserver/media/images/eoxserver_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/gdal/reftools.py` & `EOxServer-1.2.5/eoxserver/processing/gdal/reftools.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/gdal/vrt.py` & `EOxServer-1.2.5/eoxserver/processing/gdal/vrt.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/preprocessing/__init__.py` & `EOxServer-1.2.5/eoxserver/processing/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/preprocessing/exceptions.py` & `EOxServer-1.2.5/eoxserver/processing/preprocessing/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/preprocessing/format.py` & `EOxServer-1.2.5/eoxserver/processing/preprocessing/format.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/preprocessing/georeference.py` & `EOxServer-1.2.5/eoxserver/processing/preprocessing/georeference.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/preprocessing/optimization.py` & `EOxServer-1.2.5/eoxserver/processing/preprocessing/optimization.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/processing/preprocessing/util.py` & `EOxServer-1.2.5/eoxserver/processing/preprocessing/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/browse/functions.py` & `EOxServer-1.2.5/eoxserver/render/browse/functions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/browse/generate.py` & `EOxServer-1.2.5/eoxserver/render/browse/generate.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/browse/objects.py` & `EOxServer-1.2.5/eoxserver/render/browse/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 # THE SOFTWARE.
 # ------------------------------------------------------------------------------
 
 from typing import List, Tuple, Optional, Union
 
 from django.contrib.gis.geos import Polygon
 from django.contrib.gis.gdal import SpatialReference, CoordTransform, DataSource
+from django.conf import settings
 
 from eoxserver.contrib import gdal
 from eoxserver.backends.access import get_vsi_path, get_vsi_env, gdal_open
 from eoxserver.render.coverage.objects import Coverage
 
 
 BROWSE_MODE_RGB = "rgb"
 BROWSE_MODE_RGBA = "rgba"
 BROWSE_MODE_GRAYSCALE = "grayscale"
+DEFAULT_EOXS_LAYER_SUFFIX_SEPARATOR = '__'
 
 
 OptionalNumeric = Optional[Union[float, int]]
 
 
 class Browse(object):
     def __init__(self, name, filename, env, size, extent, crs, mode, footprint):
@@ -107,18 +109,21 @@
             browse_model.min_x, browse_model.min_y,
             browse_model.max_x, browse_model.max_y
         )
 
         ds = gdal_open(browse_model)
         mode = _get_ds_mode(ds)
         ds = None
-
-        if browse_model.browse_type:
-            name = '%s__%s' % (
-                product_model.identifier, browse_model.browse_type.name
+        suffix_separator = getattr(
+            settings, 'EOXS_LAYER_SUFFIX_SEPARATOR',
+            DEFAULT_EOXS_LAYER_SUFFIX_SEPARATOR
+        )
+        if browse_model.browse_type and browse_model.browse_type.name:
+            name = '%s%s%s' % (
+                product_model.identifier, suffix_separator, browse_model.browse_type.name
             )
         else:
             name = product_model.identifier
 
         return cls(
             name, filename, env, size, extent,
             browse_model.coordinate_reference_system, mode,
```

### Comparing `EOxServer-1.2.4/eoxserver/render/browse/util.py` & `EOxServer-1.2.5/eoxserver/render/browse/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/colors.py` & `EOxServer-1.2.5/eoxserver/render/colors.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/coverage/objects.py` & `EOxServer-1.2.5/eoxserver/render/coverage/objects.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/map/config.py` & `EOxServer-1.2.5/eoxserver/render/map/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/map/objects.py` & `EOxServer-1.2.5/eoxserver/render/map/objects.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/map/renderer.py` & `EOxServer-1.2.5/eoxserver/render/map/renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/mapserver/config.py` & `EOxServer-1.2.5/eoxserver/render/mapserver/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/render/mapserver/factories.py` & `EOxServer-1.2.5/eoxserver/render/mapserver/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from django.conf import settings
 from django.utils.module_loading import import_string
 
 from eoxserver.core.util.iteratortools import pairwise_iterative
 from eoxserver.contrib import mapserver as ms
 from eoxserver.contrib import vsi, vrt, gdal, osr
 from eoxserver.render.browse.objects import (
-    Browse, GeneratedBrowse, BROWSE_MODE_GRAYSCALE
+    Browse, GeneratedBrowse, BROWSE_MODE_GRAYSCALE, BROWSE_MODE_RGBA
 )
 from eoxserver.render.browse.generate import (
     generate_browse, FilenameGenerator
 )
 from eoxserver.render.map.objects import (
     CoverageLayer, CoveragesLayer, MosaicLayer, OutlinedCoveragesLayer,
     BrowseLayer, OutlinedBrowseLayer,
@@ -179,15 +179,15 @@
             extent = (
                 map_extent.minx, map_extent.miny,
                 map_extent.maxx, map_extent.maxy
             )
             sr = osr.SpatialReference(map_obj.getProjection())
 
         layer_objs = _create_raster_layer_objs(
-            map_obj, extent, sr, data, filename_generator
+            map_obj, extent, sr, data, filename_generator, location.env,
         )
 
         for i, layer_obj in enumerate(layer_objs):
             layer_obj.name = '%s__%d' % (coverage.identifier, i)
             layer_obj.setProcessingKey("CLOSE_CONNECTION", "CLOSE")
 
         if num_locations == 1:
@@ -351,19 +351,18 @@
                         map_.bbox,
                         map_.crs,
                         filename_generator,
                         browse.variables,
                     )
                 layer_objs = _create_raster_layer_objs(
                     map_obj, browse.extent, browse.spatial_reference,
-                    creation_info.filename, filename_generator
+                    creation_info.filename, filename_generator, creation_info.env, browse.mode,
                 )
 
                 for layer_obj in layer_objs:
-                    layer_obj.data = creation_info.filename
                     if creation_info.env:
                         ms.set_env(map_obj, creation_info.env, True)
 
                     if creation_info.bands:
                         layer_obj.setProcessingKey('BANDS', ','.join(
                             str(band) for band in creation_info.bands
                         ))
@@ -443,18 +442,16 @@
                                     "SCALE_%d" % i,
                                     "%s,%s" % tuple(range_)
                                 )
 
             elif isinstance(browse, Browse):
                 layer_objs = _create_raster_layer_objs(
                     map_obj, browse.extent, browse.spatial_reference,
-                    browse.filename, filename_generator
+                    browse.filename, filename_generator, browse.env, browse.mode,
                 )
-                for layer_obj in layer_objs:
-                    layer_obj.data = browse.filename
                 ms.set_env(map_obj, browse.env, True)
             elif browse is None:
                 # TODO: figure out why and deal with it?
                 continue
             else:
                 raise TypeError(
                     'Type %s is not supported', type(browse).__name__
@@ -657,23 +654,24 @@
 
 
 # ------------------------------------------------------------------------------
 # utils
 # ------------------------------------------------------------------------------
 
 
-def _create_raster_layer_objs(map_obj, extent, sr, data, filename_generator,
-                              resample=None) -> List[ms.layerObj]:
+def _create_raster_layer_objs(map_obj, extent, sr, data, filename_generator, env,
+                              browse_mode=None, resample=None) -> List[ms.layerObj]:
     layer_obj = ms.layerObj(map_obj)
     layer_obj.type = ms.MS_LAYER_RASTER
     layer_obj.status = ms.MS_ON
 
     layer_obj.data = data
-
-    layer_obj.offsite = ms.colorObj(0, 0, 0)
+    # assumption that RGBA already has transparency in alpha band
+    if browse_mode != BROWSE_MODE_RGBA:
+        layer_obj.offsite = ms.colorObj(0, 0, 0)
 
     if extent:
         layer_obj.setMetaData("wms_extent", "%f %f %f %f" % extent)
         layer_obj.setExtent(*extent)
 
         if sr.srid is not None:
             short_epsg = "EPSG:%d" % sr.srid
@@ -689,18 +687,20 @@
         wrapped_extent = wrap_extent_around_dateline(extent, sr.srid)
 
         wrapped_layer_obj = ms.layerObj(map_obj)
         wrapped_layer_obj.type = ms.MS_LAYER_RASTER
         wrapped_layer_obj.status = ms.MS_ON
 
         wrapped_data = filename_generator.generate()
-        vrt.with_extent(data, wrapped_extent, wrapped_data)
+        with gdal.config_env(env):
+            vrt.with_extent(data, wrapped_extent, wrapped_data)
         wrapped_layer_obj.data = wrapped_data
-
-        wrapped_layer_obj.offsite = ms.colorObj(0, 0, 0)
+        # assumption that RGBA already has transparency in alpha band
+        if browse_mode != BROWSE_MODE_RGBA:
+            wrapped_layer_obj.offsite = ms.colorObj(0, 0, 0)
 
         wrapped_layer_obj.setMetaData("ows_srs", short_epsg)
         wrapped_layer_obj.setMetaData("wms_srs", short_epsg)
         wrapped_layer_obj.setProjection(sr.proj)
 
         wrapped_layer_obj.setExtent(*wrapped_extent)
         wrapped_layer_obj.setMetaData(
```

### Comparing `EOxServer-1.2.4/eoxserver/render/mapserver/map_renderer.py` & `EOxServer-1.2.5/eoxserver/render/mapserver/map_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/admin.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/crss.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/crss.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/dateline.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/dateline.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/formats.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/formats.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/__init__.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/browse.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/browse.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/browsetype.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/browsetype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/collection.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/collection.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/collectiontype.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/collectiontype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/coverage.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/coverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/coveragetype.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/coveragetype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/grid.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/grid.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/id.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/id.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/mapcache.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/mapcache.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/mask.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/mask.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/masktype.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/masktype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/mosaic.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/mosaic.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/product.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/product.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/producttype.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/producttype.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/stac.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/stac.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/management/commands/timeseries.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/management/commands/timeseries.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/component.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/config.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/dimap_general.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/eoom.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/gdal_dataset_envisat.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/gsc.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/inspire.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/landsat8_l1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/native.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/native.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/coverage_formats/native_config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/interfaces.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/__init__.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/gsc.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/gsc.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/landsat8_l1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/sentinel1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/product_formats/sentinel2.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/utils/gsc.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/utils/gsc.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/metadata/utils/landsat8_l1.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0001_initial.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0002_browse_type_fields.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0003_metadata_items_semantic.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0004_auto_20181220_1300.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0005_eo_object_identifier_validator.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0007_typemodels.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0007_typemodels.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0008_incidence_angle.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0008_incidence_angle.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0010_polarisation_channels_expand.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/migrations/0011_bandstatistics.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/migrations/0011_bandstatistics.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/models.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/base.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/browse.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/browse.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/component.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/exceptions.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/interfaces.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/mask.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/mask.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/product.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/product.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/registrators/gdal.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/registrators/gdal.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/stac.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -612,18 +612,26 @@
 
         extent = (min(x_a, x_b), min(y_a, y_b), max(x_a, x_b), max(y_a, y_b))
         browse.min_x, browse.min_y, browse.max_x, browse.max_y = extent
     else:
         ds = gdal_open(browse)
         browse.width = ds.RasterXSize
         browse.height = ds.RasterYSize
-        browse.coordinate_reference_system = ds.GetProjection()
-        extent = gdal.get_extent(ds)
-        browse.min_x, browse.min_y, browse.max_x, browse.max_y = extent
-
+        projection = ds.GetProjection()
+        if projection:
+            browse.coordinate_reference_system = projection
+            extent = gdal.get_extent(ds)
+            browse.min_x, browse.min_y, browse.max_x, browse.max_y = extent
+        elif product.footprint:
+            # unprojected image, attempt to take product footprint bbox
+            srs = osr.SpatialReference()
+            srs.ImportFromEPSG(product.footprint.srid)
+            browse.coordinate_reference_system = srs.ExportToWkt()
+            extent = product.footprint.extent
+            browse.min_x, browse.min_y, browse.max_x, browse.max_y = extent
     browse.full_clean()
     browse.save()
 
 
 @transaction.atomic
 def create_product_type_from_stac_collection(stac_collection,
                                              product_type_name=None):
```

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/registration/timeseries.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/registration/timeseries.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/synchronization.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/synchronization.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/tests.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/urls.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/util.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/resources/coverages/views.py` & `EOxServer-1.2.5/eoxserver/resources/coverages/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/scripts/eoxserver-instance.py` & `EOxServer-1.2.5/eoxserver/scripts/eoxserver-instance.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/admin.py` & `EOxServer-1.2.5/eoxserver/services/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/auth/base.py` & `EOxServer-1.2.5/eoxserver/services/auth/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/auth/charonpdp.py` & `EOxServer-1.2.5/eoxserver/services/auth/charonpdp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/auth/dummypdp.py` & `EOxServer-1.2.5/eoxserver/services/auth/dummypdp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/auth/exceptions.py` & `EOxServer-1.2.5/eoxserver/services/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/auth/interfaces.py` & `EOxServer-1.2.5/eoxserver/services/auth/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/auth/middleware.py` & `EOxServer-1.2.5/eoxserver/services/auth/middleware.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/cis/v11/encoders.py` & `EOxServer-1.2.5/eoxserver/services/cis/v11/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/config.py` & `EOxServer-1.2.5/eoxserver/services/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ecql.py` & `EOxServer-1.2.5/eoxserver/services/ecql.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/exceptions.py` & `EOxServer-1.2.5/eoxserver/services/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/filters.py` & `EOxServer-1.2.5/eoxserver/services/filters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py` & `EOxServer-1.2.5/eoxserver/services/gdal/wcs/referenceable_dataset_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/gml/v32/encoders.py` & `EOxServer-1.2.5/eoxserver/services/gml/v32/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/management/commands/eoxs_filter.py` & `EOxServer-1.2.5/eoxserver/services/management/commands/eoxs_filter.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/management/commands/visibility.py` & `EOxServer-1.2.5/eoxserver/services/management/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/management/commands/wms_options_list.py` & `EOxServer-1.2.5/eoxserver/services/management/commands/wms_options_list.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/management/commands/wms_options_load.py` & `EOxServer-1.2.5/eoxserver/services/management/commands/wms_options_load.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/management/commands/wms_options_set.py` & `EOxServer-1.2.5/eoxserver/services/management/commands/wms_options_set.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/config.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/connectors/__init__.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/connectors/mosaic_connector.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/connectors/mosaic_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/connectors/multifile_connector.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/connectors/multifile_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/connectors/polygonmask_connector.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/connectors/polygonmask_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/connectors/simple_connector.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/connectors/simple_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/connectors/tileindex_connector.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/connectors/tileindex_connector.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/interfaces.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wcs/base_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wcs/base_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wcs/capabilities_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wcs/capabilities_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wcs/coverage_description_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wcs/coverage_description_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wcs/coverage_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wcs/coverage_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/capabilities_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/capabilities_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/feature_info_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/feature_info_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/base.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/colorized_mask_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_bands_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_mask_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_masked_outlines_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/layerfactories/coverage_outlines_layer_factory.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/legendgraphic_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/legendgraphic_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/map_renderer.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/map_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/styleapplicators/sld.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/styleapplicators/sld.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/mapserver/wms/util.py` & `EOxServer-1.2.5/eoxserver/services/mapserver/wms/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/migrations/0001_initial.py` & `EOxServer-1.2.5/eoxserver/services/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py` & `EOxServer-1.2.5/eoxserver/services/migrations/0002_service_visibility_cardinality_uniqueness.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/migrations/0003_service_name_choices.py` & `EOxServer-1.2.5/eoxserver/services/migrations/0003_service_name_choices.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/models.py` & `EOxServer-1.2.5/eoxserver/services/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/native/wcs/capabilities_renderer.py` & `EOxServer-1.2.5/eoxserver/services/native/wcs/capabilities_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/native/wcs/coverage_description_renderer.py` & `EOxServer-1.2.5/eoxserver/services/native/wcs/coverage_description_renderer.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/config.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/extensions/__init__.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/extensions/cql.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/extensions/cql.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/extensions/eo.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/extensions/eo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/extensions/geo.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/extensions/geo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/extensions/time.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/extensions/time.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/formats/__init__.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/formats/atom.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/formats/atom.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/formats/base.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/formats/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/formats/geojson.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/formats/geojson.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/formats/html.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/formats/html.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/formats/kml.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/formats/kml.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/formats/rss.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/formats/rss.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/interfaces.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/urls.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/v11/description.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/v11/description.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/v11/search.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/v11/search.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/opensearch/views.py` & `EOxServer-1.2.5/eoxserver/services/opensearch/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/common/config.py` & `EOxServer-1.2.5/eoxserver/services/ows/common/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/common/v11/encoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/common/v11/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/common/v20/encoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/common/v20/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/common/v20/exceptionhandler.py` & `EOxServer-1.2.5/eoxserver/services/ows/common/v20/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/component.py` & `EOxServer-1.2.5/eoxserver/services/ows/component.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/config.py` & `EOxServer-1.2.5/eoxserver/services/ows/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/decoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/decoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/dispatch.py` & `EOxServer-1.2.5/eoxserver/services/ows/dispatch.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/dseo/v10/encoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/dseo/v10/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/dseo/v10/handlers.py` & `EOxServer-1.2.5/eoxserver/services/ows/dseo/v10/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/interfaces.py` & `EOxServer-1.2.5/eoxserver/services/ows/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/version.py` & `EOxServer-1.2.5/eoxserver/services/ows/version.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/basehandlers.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/basehandlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/config.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/interfaces.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/parameters.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/renderers.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/renderers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/describecoverage.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/describecoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/exceptionhandler.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/getcoverage.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/getcoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/parameters.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v10/util.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v10/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/describecoverage.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/describecoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/exceptionhandler.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/getcoverage.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/getcoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/parameters.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v11/util.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v11/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/describecoverage.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/describecoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/describeeocoverageset.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/describeeocoverageset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/encoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/encodings/__init__.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/encodings/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/encodings/geotiff.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/encodings/geotiff.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/exceptionhandler.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/getcoverage.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/getcoverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/geteocoverageset.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/geteocoverageset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/handlers.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/packages/tar.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/packages/tar.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/packages/zip.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/packages/zip.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/parameters.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs/v20/util.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs/v20/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wcs11Transaction.py` & `EOxServer-1.2.5/eoxserver/services/ows/wcs11Transaction.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/basehandlers.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/basehandlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/exceptions.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/interfaces.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/layermapper.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/layermapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     OutlinesLayer, BrowseLayer, OutlinedBrowseLayer,
     MaskLayer, MaskedBrowseLayer,
     LayerDescription,
 )
 from eoxserver.render.coverage.objects import Coverage as RenderCoverage
 from eoxserver.render.coverage.objects import Mosaic as RenderMosaic
 from eoxserver.render.browse.objects import (
-    Browse, GeneratedBrowse, Mask, MaskedBrowse
+    Browse, GeneratedBrowse, Mask, MaskedBrowse, DEFAULT_EOXS_LAYER_SUFFIX_SEPARATOR
 )
 from eoxserver.resources.coverages import models
 
 
 class UnsupportedObject(Exception):
     pass
 
@@ -55,16 +55,14 @@
 
 
 class NoSuchPrefix(NoSuchLayer):
     code = 'LayerNotDefined'
     locator = 'layer'
 
 
-DEFAULT_EOXS_LAYER_SUFFIX_SEPARATOR = '__'
-
 
 class LayerMapper(object):
     """ Default layer mapper.
     """
 
     def __init__(self, supported_layer_types, suffix_separator=None):
         self.supported_layer_types = supported_layer_types
@@ -548,14 +546,18 @@
                 browse = browses.first()
                 if browse:
                     browse_type = browse.browse_type
                 else:
                     browse_type = models.BrowseType.objects.get(
                         name=name, product_type=product.product_type
                     )
+            # additionally try to filter default browse with name ''
+            elif (browses := browses.filter(browse_type__name='')).count() > 0:
+                browse = browses.first()
+                browse_type = browse.browse_type
             else:
                 browses = browses.filter(browse_type__isnull=True)
                 browse_type = None
 
             # if style:
             #     browses = browses.filter(style=style)
             # else:
@@ -691,15 +693,17 @@
     # only return a browse instance if coverages were found
     if coverages:
         return GeneratedBrowse.from_coverage_models(
             bands,
             ranges or [(None, None)] * len(bands),
             [None] * len(bands),
             fields_and_coverages,
-            product
+            product,
+            variables={},
+            show_out_of_bounds_data=False,
         )
     return None
 
 
 def _lookup_coverages(product, field_names):
     # make a query of all coverages in that product for the given fields
     coverages = product.coverages.filter(
```

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/parsing.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/parsing.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/util.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v10/encoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v10/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v10/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v10/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v10/getfeatureinfo.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v10/getfeatureinfo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v10/getmap.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v10/getmap.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v10/handlers.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v10/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v11/encoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v11/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v11/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v11/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v11/getfeatureinfo.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v11/getfeatureinfo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v11/getmap.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v11/getmap.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v11/handlers.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v11/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v13/encoders.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v13/encoders.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v13/exceptionhandler.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v13/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getfeatureinfo.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getfeatureinfo.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getlegendgraphic.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getlegendgraphic.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v13/getmap.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v13/getmap.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wms/v13/handlers.py` & `EOxServer-1.2.5/eoxserver/services/ows/wms/v13/handlers.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/config.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/config.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/context.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/context.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/exceptions.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/exceptions.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/interfaces.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/interfaces.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/__init__.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/allowed_values.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/allowed_values.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/base.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/bboxdata.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/bboxdata.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/codecs.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/codecs.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/complexdata.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/complexdata.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/crs.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/crs.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/data_types.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/data_types.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/formats.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/formats.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/inputs.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/inputs.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/literaldata.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/literaldata.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/response_form.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/response_form.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/parameters/units.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/parameters/units.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_cloud_coverage.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_cloud_coverage.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_dem_processing.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_dem_processing.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_height_profile.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_height_profile.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_statistics.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_statistics.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/processes/get_time_data.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/processes/get_time_data.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/test_allowed_values.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/test_allowed_values.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/test_data_types.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/test_data_types.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/util.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/describeprocess.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/describeprocess.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/__init__.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/base.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/base.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/capabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/capabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/execute_response.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/execute_response.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/execute_response_raw.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/parameters.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/encoders/process_description.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/encoders/process_description.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/exceptionhandler.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/exceptionhandler.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_decoder_common.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_decoder_common.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_decoder_kvp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_decoder_xml.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_decoder_xml.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/execute_util.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/execute_util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v10/util.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v10/util.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v20/common.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v20/common.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v20/describeprocess.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v20/describeprocess.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v20/execute.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v20/execute.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/ows/wps/v20/getcapabilities.py` & `EOxServer-1.2.5/eoxserver/services/ows/wps/v20/getcapabilities.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/parameters.py` & `EOxServer-1.2.5/eoxserver/services/parameters.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/result.py` & `EOxServer-1.2.5/eoxserver/services/result.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/subset.py` & `EOxServer-1.2.5/eoxserver/services/subset.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/templates/opensearch/result.html` & `EOxServer-1.2.5/eoxserver/services/templates/opensearch/result.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/templates/opensearch/summary.html` & `EOxServer-1.2.5/eoxserver/services/templates/opensearch/summary.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/templatetags/services_extra.py` & `EOxServer-1.2.5/eoxserver/services/templatetags/services_extra.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/tests.py` & `EOxServer-1.2.5/eoxserver/services/tests.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/urls.py` & `EOxServer-1.2.5/eoxserver/services/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/services/views.py` & `EOxServer-1.2.5/eoxserver/services/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/testing/xcomp.py` & `EOxServer-1.2.5/eoxserver/testing/xcomp.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/views.py` & `EOxServer-1.2.5/eoxserver/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/admin.py` & `EOxServer-1.2.5/eoxserver/webclient/admin.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/migrations/0001_initial.py` & `EOxServer-1.2.5/eoxserver/webclient/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/migrations/0002_extra_fields.py` & `EOxServer-1.2.5/eoxserver/webclient/migrations/0002_extra_fields.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/models.py` & `EOxServer-1.2.5/eoxserver/webclient/models.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/static/822268aa1a6cd4dedba8.worker.js` & `EOxServer-1.2.5/eoxserver/webclient/static/822268aa1a6cd4dedba8.worker.js`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/static/EOxServer_logo_small.png` & `EOxServer-1.2.5/eoxserver/webclient/static/EOxServer_logo_small.png`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/static/favicon.ico` & `EOxServer-1.2.5/eoxserver/webclient/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/static/prism.js` & `EOxServer-1.2.5/eoxserver/webclient/static/prism.js`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/templates/webclient/config.json` & `EOxServer-1.2.5/eoxserver/webclient/templates/webclient/config.json`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/templates/webclient/index.html` & `EOxServer-1.2.5/eoxserver/webclient/templates/webclient/index.html`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/urls.py` & `EOxServer-1.2.5/eoxserver/webclient/urls.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/eoxserver/webclient/views.py` & `EOxServer-1.2.5/eoxserver/webclient/views.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/setup.py` & `EOxServer-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/tools/eoxserver-atpd.py` & `EOxServer-1.2.5/tools/eoxserver-atpd.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/tools/eoxserver-preprocess.py` & `EOxServer-1.2.5/tools/eoxserver-preprocess.py`

 * *Files identical despite different names*

### Comparing `EOxServer-1.2.4/tools/eoxserver-validate_xml.py` & `EOxServer-1.2.5/tools/eoxserver-validate_xml.py`

 * *Files identical despite different names*

