# Comparing `tmp/wc-django-geo-db-0.1.8.tar.gz` & `tmp/wc-django-geo-db-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wc-django-geo-db-0.1.8.tar", last modified: Wed Jul 14 07:47:53 2021, max compression
+gzip compressed data, was "wc-django-geo-db-0.1.9.tar", last modified: Tue Aug  3 11:05:56 2021, max compression
```

## Comparing `wc-django-geo-db-0.1.8.tar` & `wc-django-geo-db-0.1.9.tar`

### file list

```diff
@@ -1,199 +1,201 @@
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1072 2021-06-25 13:47:17.000000 wc-django-geo-db-0.1.8/LICENSE
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2721 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2122 2021-07-14 07:46:24.000000 wc-django-geo-db-0.1.8/README.md
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2021-07-14 07:47:53.843315 wc-django-geo-db-0.1.8/setup.cfg
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1744 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/setup.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.819314 wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2721 2021-07-14 07:47:53.000000 wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/PKG-INFO
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     6611 2021-07-14 07:47:53.000000 wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/SOURCES.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2021-07-14 07:47:53.000000 wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/dependency_links.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      311 2021-07-14 07:47:53.000000 wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/requires.txt
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       30 2021-07-14 07:47:53.000000 wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/top_level.txt
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.819314 wc-django-geo-db-0.1.8/wcd_geo_db/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      137 2021-07-14 07:46:37.000000 wc-django-geo-db-0.1.8/wcd_geo_db/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      242 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      434 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/client.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      265 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2807 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/const.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.819314 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.819314 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       70 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.819314 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       41 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.823314 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/bank/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/bank/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1254 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/bank/divisions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      212 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/bank/geometry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      367 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/bank/places.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      325 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/bank/routes.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.823314 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/names/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       25 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/names/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      279 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/names/divisions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      310 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/apps.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.823314 wc-django-geo-db-0.1.8/wcd_geo_db/management/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/management/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.827314 wc-django-geo-db-0.1.8/wcd_geo_db/management/commands/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/management/commands/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      636 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/management/commands/wcd_geo_fix_divisions_tree.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.827314 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5345 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2849 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0002_auto_20210608_1355.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1134 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0003_auto_20210610_1042.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      329 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0004_remove_division_path.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      369 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0005_rename_path_temp_division_path.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      500 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0006_division_wcd_geo_db_division_path_index.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3423 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0007_auto_20210610_1436.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2863 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0008_auto_20210615_1524.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1171 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0009_auto_20210616_1837.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      982 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0010_codes_import_data.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1318 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0011_codes_to_array_merge.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/migrations/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       63 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/models.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.827314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.827314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       22 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.827314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/client/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       47 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/client/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      286 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/client/client.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3304 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/client/formatter.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      498 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/dtos.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.827314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       63 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.827314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/client/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       47 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/client/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      213 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/client/client.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3933 2021-07-14 07:19:26.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/client/divisions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      142 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1433 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/divisions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1238 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/geometry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1462 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/mixins.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      995 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/places.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      795 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/routes.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      208 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/translations.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      628 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/dtos.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       67 2021-07-14 07:19:24.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      939 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/base.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2594 2021-07-14 07:34:27.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/divisions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1029 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/geometry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      652 2021-07-14 07:18:43.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/search.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/client/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       71 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/client/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      750 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/client/base.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      871 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/client/code_seeker.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      407 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/client/database.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      234 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/admin.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      105 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/builtins.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      158 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/globals.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2977 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     7390 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/query.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      630 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/registry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1611 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/seeker.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       42 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/client/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       47 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/client/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      215 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/client/client.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1024 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/client/divisions.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/db/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       25 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/db/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      974 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/db/divisions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      355 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/dtos.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db_sources/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       66 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       37 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/admin.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      361 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/apps.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      437 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      143 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/discover.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db_sources/management/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/management/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db_sources/management/commands/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/management/commands/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1158 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/management/commands/wcd_geo_runimport.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.831314 wc-django-geo-db-0.1.8/wcd_geo_db_sources/migrations/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1767 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/migrations/0001_initial.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/migrations/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/admin/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       23 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/admin/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1482 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/admin/process.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1257 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/code_mapper.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2674 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/code_seeker.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      182 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4823 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/divisions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      550 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/dtos.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1789 2021-07-09 12:38:51.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/merger.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      116 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/cases/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       19 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/cases/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1252 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/cases/run.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      296 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/conf.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      634 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/const.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      477 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/exceptions.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      594 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/globals.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3009 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/models.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/query.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1084 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/registry.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     5374 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/runner.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       77 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/tasks.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/tasks/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       22 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/tasks/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      245 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/tasks/celery.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      152 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/tasks/conf.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/__init__.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/_base/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       44 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/_base/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      715 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/_base/const.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      264 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/_base/parser.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/_base/process.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       27 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      152 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/code_seeker.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      124 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/const.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/parsers/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       95 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/parsers/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4261 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/parsers/v1.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3443 2021-07-09 12:59:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/process.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.835315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      134 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/const.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       95 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      872 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/v1.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3125 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/process.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       27 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      150 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/code_seeker.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      264 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/const.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      320 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2132 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/hierarchical_v1.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      116 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      461 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/categories.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1183 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/geo.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      291 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/json.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     4472 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/mappings.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     2196 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/postprocess.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     1770 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/v1.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)     3560 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/process.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      646 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/const.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)    12688 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/diff.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)    10812 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/process.py
-drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-07-14 07:47:53.839315 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/novaposhta/
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       27 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/novaposhta/__init__.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)      892 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/novaposhta/code_seeker.py
--rw-rw-r--   0 preusx    (1000) preusx    (1000)       53 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.8/wcd_geo_db_sources/tasks.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.956256 wc-django-geo-db-0.1.9/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1072 2021-06-25 13:47:17.000000 wc-django-geo-db-0.1.9/LICENSE
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2721 2021-08-03 11:05:56.956256 wc-django-geo-db-0.1.9/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2122 2021-07-14 13:33:53.000000 wc-django-geo-db-0.1.9/README.md
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       79 2021-08-03 11:05:56.956256 wc-django-geo-db-0.1.9/setup.cfg
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1744 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/setup.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.808254 wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2721 2021-08-03 11:05:56.000000 wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/PKG-INFO
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     6715 2021-08-03 11:05:56.000000 wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/SOURCES.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        1 2021-08-03 11:05:56.000000 wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/dependency_links.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      311 2021-08-03 11:05:56.000000 wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/requires.txt
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       30 2021-08-03 11:05:56.000000 wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/top_level.txt
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.812254 wc-django-geo-db-0.1.9/wcd_geo_db/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      137 2021-08-03 11:05:35.000000 wc-django-geo-db-0.1.9/wcd_geo_db/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      242 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      434 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/client.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      265 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2807 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.812254 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.816254 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       70 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.820254 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       41 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.832254 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/bank/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/bank/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1254 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/bank/divisions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      212 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/bank/geometry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      367 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/bank/places.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      325 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/bank/routes.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.840254 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/names/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       25 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/names/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      279 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/names/divisions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      310 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/apps.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.840254 wc-django-geo-db-0.1.9/wcd_geo_db/management/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/management/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.844254 wc-django-geo-db-0.1.9/wcd_geo_db/management/commands/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/management/commands/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      636 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/management/commands/wcd_geo_fix_divisions_tree.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.856254 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5345 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2849 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0002_auto_20210608_1355.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1134 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0003_auto_20210610_1042.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      329 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0004_remove_division_path.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      369 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0005_rename_path_temp_division_path.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      500 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0006_division_wcd_geo_db_division_path_index.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3423 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0007_auto_20210610_1436.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2863 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0008_auto_20210615_1524.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1171 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0009_auto_20210616_1837.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      982 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0010_codes_import_data.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1318 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0011_codes_to_array_merge.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      321 2021-08-03 08:32:32.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0012_trigram_extension_enable.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      722 2021-08-03 11:04:41.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0013_auto_20210803_1103.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/migrations/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       63 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/models.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.856254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.856254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       22 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.860254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/client/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       47 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/client/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      286 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/client/client.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3304 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/client/formatter.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      498 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/dtos.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.860254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       63 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.860254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/client/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       47 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/client/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      213 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/client/client.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3933 2021-07-14 13:33:53.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/client/divisions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.864254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      142 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1850 2021-08-03 11:03:23.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/divisions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1238 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/geometry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1462 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/mixins.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      995 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/places.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      795 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/routes.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      208 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/translations.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      628 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/dtos.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.864254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       67 2021-07-14 13:33:53.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      939 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/base.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3072 2021-08-03 10:53:35.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/divisions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1029 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/geometry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      652 2021-07-14 13:33:53.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/search.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.872254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/client/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       71 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/client/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      750 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/client/base.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      871 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/client/code_seeker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      407 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/client/database.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.876254 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       93 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      234 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/admin.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      105 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/builtins.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      158 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/globals.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2977 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     7390 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/query.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      630 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/registry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1611 2021-07-02 11:04:13.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/seeker.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.884255 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       42 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.888255 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/client/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       47 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/client/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      215 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/client/client.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1024 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/client/divisions.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.888255 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/db/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       25 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/db/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      974 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/db/divisions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      355 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/dtos.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.892255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       66 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       37 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/admin.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      361 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/apps.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      437 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      143 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/discover.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.892255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/management/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/management/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.892255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/management/commands/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/management/commands/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1158 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/management/commands/wcd_geo_runimport.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.896255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/migrations/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1767 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/migrations/0001_initial.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/migrations/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.896255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.896255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/admin/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       23 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/admin/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1482 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/admin/process.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.900255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1257 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/code_mapper.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2674 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/code_seeker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      182 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4823 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/divisions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      550 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/dtos.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1789 2021-07-09 12:38:51.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/merger.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.904255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      116 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.904255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/cases/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       19 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/cases/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1252 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/cases/run.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      296 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/conf.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      634 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/const.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      477 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/exceptions.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      594 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/globals.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3009 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/models.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      474 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/query.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1084 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/registry.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     5374 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/runner.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       77 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/tasks.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.908255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/tasks/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       22 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/tasks/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      245 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/tasks/celery.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      152 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/tasks/conf.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.908255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/__init__.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.924255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/_base/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       44 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/_base/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      715 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/_base/const.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      264 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/_base/parser.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2029 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/_base/process.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.928255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       27 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      152 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/code_seeker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      124 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.932255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/parsers/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       95 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/parsers/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4261 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/parsers/v1.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3443 2021-07-09 12:59:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/process.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.936255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      134 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.936255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       95 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      872 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/v1.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3125 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/process.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.940255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       27 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      150 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/code_seeker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      264 2021-07-02 11:04:14.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/const.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.940255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      320 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2132 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/hierarchical_v1.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.952255 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      116 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      461 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/categories.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1183 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/geo.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      291 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/json.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     4472 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/mappings.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     2196 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/postprocess.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     1770 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/v1.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)     3560 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/process.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.956256 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)        0 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      646 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/const.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    12688 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/diff.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)    10812 2021-07-12 06:16:48.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/process.py
+drwxrwxr-x   0 preusx    (1000) preusx    (1000)        0 2021-08-03 11:05:56.956256 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/novaposhta/
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       27 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/novaposhta/__init__.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)      892 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/novaposhta/code_seeker.py
+-rw-rw-r--   0 preusx    (1000) preusx    (1000)       53 2021-06-25 13:47:18.000000 wc-django-geo-db-0.1.9/wcd_geo_db_sources/tasks.py
```

### Comparing `wc-django-geo-db-0.1.8/LICENSE` & `wc-django-geo-db-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/PKG-INFO` & `wc-django-geo-db-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-geo-db
-Version: 0.1.8
+Version: 0.1.9
 Summary: Geographical database for internal projects.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `wc-django-geo-db-0.1.8/README.md` & `wc-django-geo-db-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/setup.py` & `wc-django-geo-db-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/PKG-INFO` & `wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wc-django-geo-db
-Version: 0.1.8
+Version: 0.1.9
 Summary: Geographical database for internal projects.
 Home-page: UNKNOWN
 Author: WebCase
 Author-email: info@webcase.studio
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `wc-django-geo-db-0.1.8/wc_django_geo_db.egg-info/SOURCES.txt` & `wc-django-geo-db-0.1.9/wc_django_geo_db.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 wcd_geo_db/migrations/0005_rename_path_temp_division_path.py
 wcd_geo_db/migrations/0006_division_wcd_geo_db_division_path_index.py
 wcd_geo_db/migrations/0007_auto_20210610_1436.py
 wcd_geo_db/migrations/0008_auto_20210615_1524.py
 wcd_geo_db/migrations/0009_auto_20210616_1837.py
 wcd_geo_db/migrations/0010_codes_import_data.py
 wcd_geo_db/migrations/0011_codes_to_array_merge.py
+wcd_geo_db/migrations/0012_trigram_extension_enable.py
+wcd_geo_db/migrations/0013_auto_20210803_1103.py
 wcd_geo_db/migrations/__init__.py
 wcd_geo_db/modules/__init__.py
 wcd_geo_db/modules/addresses/__init__.py
 wcd_geo_db/modules/addresses/dtos.py
 wcd_geo_db/modules/addresses/client/__init__.py
 wcd_geo_db/modules/addresses/client/client.py
 wcd_geo_db/modules/addresses/client/formatter.py
```

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/const.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/const.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/contrib/admin/admin/bank/divisions.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/contrib/admin/admin/bank/divisions.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/management/commands/wcd_geo_fix_divisions_tree.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/management/commands/wcd_geo_fix_divisions_tree.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0001_initial.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0002_auto_20210608_1355.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0002_auto_20210608_1355.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0003_auto_20210610_1042.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0003_auto_20210610_1042.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0007_auto_20210610_1436.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0007_auto_20210610_1436.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0008_auto_20210615_1524.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0008_auto_20210615_1524.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0009_auto_20210616_1837.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0009_auto_20210616_1837.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0010_codes_import_data.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0010_codes_import_data.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/migrations/0011_codes_to_array_merge.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/migrations/0011_codes_to_array_merge.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/addresses/client/formatter.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/addresses/client/formatter.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/client/divisions.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/client/divisions.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/divisions.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/divisions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.db import models
+from django.contrib.postgres.indexes import GistIndex
 from django.utils.translation import pgettext_lazy
 
 from pxd_tree.hierarchy import Tree, tree_indexes
 from wcd_geo_db.const import DivisionLevel
 from wcd_geo_db.modules.code_seeker.models import (
     create_codes_model, CodesDefinableMixin, codes_mixin_indexes
 )
@@ -18,15 +19,26 @@
 class Division(Tree, NamedMixin, SynonymizedMixin, WithGeometryMixin, CodesDefinableMixin):
     Levels = DivisionLevel
     objects: models.Manager[DivisionsQuerySet] = DivisionsQuerySet.as_manager()
 
     class Meta:
         verbose_name = pgettext_lazy('wcd_geo_db', 'Division')
         verbose_name_plural = pgettext_lazy('wcd_geo_db', 'Divisions')
-        indexes = tree_indexes() + codes_mixin_indexes()
+        indexes = tree_indexes() + codes_mixin_indexes() + [
+            GistIndex(
+                name='%(app_label)s_%(class)s_name_idx',
+                fields=['name'],
+                opclasses=['gist_trgm_ops'],
+            ),
+            GistIndex(
+                name='%(app_label)s_%(class)s_syn_idx',
+                fields=['synonyms'],
+                opclasses=['gist_trgm_ops'],
+            ),
+        ]
 
     id = models.BigAutoField(
         primary_key=True, verbose_name=pgettext_lazy('wcd_geo_db', 'ID')
     )
     level = models.SmallIntegerField(
         verbose_name=pgettext_lazy('wcd_geo_db', 'Division level'),
         choices=Levels.choices, null=False, blank=False
```

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/geometry.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/geometry.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/mixins.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/mixins.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/places.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/places.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/db/routes.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/db/routes.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/dtos.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/dtos.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/base.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/base.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/divisions.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/divisions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, List, Optional, Sequence, TypeVar
 from django.db import models
-from django.contrib.postgres.search import SearchVector, SearchQuery, SearchRank
+from django.db.models.functions import Cast
+from django.contrib.postgres.search import TrigramSimilarity
 
 from wcd_geo_db.const import DivisionLevel
 from wcd_geo_db.modules.code_seeker.query import CodeSeekerQuerySet
 from pxd_tree.hierarchy import TreeQuerySet
 
 from ..dtos import DivisionDTO, GeometryDTO
 from .base import QuerySet
@@ -40,40 +41,50 @@
 class DivisionsQuerySet(
     WithGeometryQuerySet,
     CodeSeekerQuerySet,
     TreeQuerySet,
     SearchQuerySet,
     QuerySet
 ):
-    SEARCH_QUERY_MIN_LENGTH: int = 2
+    SEARCH_QUERY_MIN_LENGTH: int = 1
+    SEARCH_QUERY_MIN_RANK: float = 0.1
     SEARCH_QUERY_RANK_WEIGHTS: Sequence[float] = [0.2, 0.4, 0.8, 1]
 
     def search(self: QT, query: SearchQueryParam) -> QT:
         q = query.get('query')
+        min_rank = query.get('min_rank', self.SEARCH_QUERY_MIN_RANK)
 
         if not q or len(q) < self.SEARCH_QUERY_MIN_LENGTH:
             return self
 
-        vector = (
-            SearchVector('name', weight='A')
-            +
-            SearchVector('synonyms', weight='B')
+        name_similarity = TrigramSimilarity(
+            'name', Cast(models.Value(q), output_field=models.TextField()),
+            function='strict_word_similarity'
         )
-        sql_query = SearchQuery(q, search_type='websearch')
-        rank = SearchRank(
-            vector, sql_query, weights=self.SEARCH_QUERY_RANK_WEIGHTS
+        synonyms_similarity = TrigramSimilarity(
+            'synonyms', Cast(models.Value(q), output_field=models.TextField()),
+            function='strict_word_similarity'
         )
 
-        return (
+        queryset = (
             self
-            .annotate(search=vector, rank=rank)
-            .filter(search=sql_query)
-            .order_by('-rank')
+            .annotate(
+                name_similarity=name_similarity,
+                synonyms_similarity=synonyms_similarity,
+            )
+            .filter(
+                models.Q(name_similarity__gt=min_rank)
+                |
+                models.Q(synonyms_similarity__gt=min_rank)
+            )
+            .order_by('-name_similarity', '-synonyms_similarity')
         )
 
+        return queryset
+
     def as_dtos(self) -> List[DivisionDTO]:
         return [as_dto(values) for values in self.values(*VALUES_NAMES)]
 
     def general_filter(
         self: QT,
         parent_ids: Optional[Sequence[int]] = None,
         levels: Optional[Sequence[DivisionLevel]] = None,
```

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/geometry.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/geometry.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/bank/query/search.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/bank/query/search.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/client/base.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/client/base.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/client/code_seeker.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/client/code_seeker.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/models.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/models.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/query.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/query.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/registry.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/registry.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/code_seeker/seeker.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/code_seeker/seeker.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/client/divisions.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/client/divisions.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db/modules/names/db/divisions.py` & `wc-django-geo-db-0.1.9/wcd_geo_db/modules/names/db/divisions.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/management/commands/wcd_geo_runimport.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/management/commands/wcd_geo_runimport.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/migrations/0001_initial.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/admin/process.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/admin/process.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/code_mapper.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/code_mapper.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/code_seeker.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/code_seeker.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/divisions.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/divisions.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/dtos.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/dtos.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/merger/merger.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/merger/merger.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/cases/run.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/cases/run.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/const.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/const.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/globals.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/globals.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/models.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/models.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/registry.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/registry.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/modules/process/runner.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/modules/process/runner.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/_base/const.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/_base/const.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/_base/process.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/_base/process.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/parsers/v1.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/parsers/v1.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg/process.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg/process.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/v1.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/parsers/v1.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/katottg_to_koatuu/process.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/katottg_to_koatuu/process.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/hierarchical_v1.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/hierarchical_v1.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/geo.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/geo.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/mappings.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/mappings.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/shared/postprocess.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/shared/postprocess.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/parsers/v1.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/parsers/v1.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu/process.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu/process.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/const.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/const.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/diff.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/diff.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/koatuu_diff/process.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/koatuu_diff/process.py`

 * *Files identical despite different names*

### Comparing `wc-django-geo-db-0.1.8/wcd_geo_db_sources/sources/novaposhta/code_seeker.py` & `wc-django-geo-db-0.1.9/wcd_geo_db_sources/sources/novaposhta/code_seeker.py`

 * *Files identical despite different names*

