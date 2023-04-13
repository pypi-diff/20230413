# Comparing `tmp/whoogle-search-0.8.1.tar.gz` & `tmp/whoogle-search-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whoogle-search-0.8.1.tar", last modified: Mon Dec 19 17:59:02 2022, max compression
+gzip compressed data, was "whoogle-search-0.8.2.tar", last modified: Thu Apr 13 20:05:30 2023, max compression
```

## Comparing `whoogle-search-0.8.1.tar` & `whoogle-search-0.8.2.tar`

### file list

```diff
@@ -1,107 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.024000 whoogle-search-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    37058 2022-12-19 17:59:02.024000 whoogle-search-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36503 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.011999 whoogle-search-0.8.1/app/
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24583 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.016000 whoogle-search-0.8.1/app/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/models/g_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.011999 whoogle-search-0.8.1/app/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.016000 whoogle-search-0.8.1/app/static/build/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.016000 whoogle-search-0.8.1/app/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/dark-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/error.css
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/header.css
--rw-r--r--   0 runner    (1001) docker     (123)      793 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/input.css
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/light-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/logo.css
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/main.css
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/search.css
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/css/variables.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.016000 whoogle-search-0.8.1/app/static/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.020000 whoogle-search-0.8.1/app/static/img/favicon/
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (123)    12632 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/apple-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      281 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      787 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/ms-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/ms-icon-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    29292 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon/ms-icon-70x70.png
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    24077 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/img/whoogle.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.020000 whoogle-search-0.8.1/app/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/js/autocomplete.js
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/js/controller.js
--rw-r--r--   0 runner    (1001) docker     (123)      394 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/js/currency.js
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/js/header.js
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/js/keyboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/js/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.020000 whoogle-search-0.8.1/app/static/settings/
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/settings/countries.json
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/settings/header_tabs.json
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/settings/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/settings/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)    53221 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/static/settings/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.024000 whoogle-search-0.8.1/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/display.html
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/imageresults.html
--rw-r--r--   0 runner    (1001) docker     (123)    15877 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/opensearch.xml
--rw-r--r--   0 runner    (1001) docker     (123)      453 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/templates/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.024000 whoogle-search-0.8.1/app/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/utils/bangs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/utils/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/app/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      961 2022-12-19 17:59:02.024000 whoogle-search-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.024000 whoogle-search-0.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/test/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/test/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2022-12-19 17:58:52.000000 whoogle-search-0.8.1/test/test_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:59:02.024000 whoogle-search-0.8.1/whoogle_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37058 2022-12-19 17:59:01.000000 whoogle-search-0.8.1/whoogle_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2022-12-19 17:59:02.000000 whoogle-search-0.8.1/whoogle_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 17:59:01.000000 whoogle-search-0.8.1/whoogle_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2022-12-19 17:59:01.000000 whoogle-search-0.8.1/whoogle_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-19 17:59:01.000000 whoogle-search-0.8.1/whoogle_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-19 17:59:01.000000 whoogle-search-0.8.1/whoogle_search.egg-info/top_level.txt
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/
+-rw-r--r--   0 benbusby  (1000) users      (985)     1066 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/LICENSE
+-rw-r--r--   0 benbusby  (1000) users      (985)      121 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/MANIFEST.in
+-rw-r--r--   0 benbusby  (1000) users      (985)    37366 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/PKG-INFO
+-rw-r--r--   0 benbusby  (1000) users      (985)    36811 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/README.md
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.458581 whoogle-search-0.8.2/app/
+-rw-r--r--   0 benbusby  (1000) users      (985)     6919 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/__init__.py
+-rw-r--r--   0 benbusby  (1000) users      (985)       39 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/__main__.py
+-rw-r--r--   0 benbusby  (1000) users      (985)    24769 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/filter.py
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.458581 whoogle-search-0.8.2/app/models/
+-rw-r--r--   0 benbusby  (1000) users      (985)        0 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/models/__init__.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     7981 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/models/config.py
+-rw-r--r--   0 benbusby  (1000) users      (985)      506 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/models/endpoint.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     1453 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/models/g_classes.py
+-rw-r--r--   0 benbusby  (1000) users      (985)    12415 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/request.py
+-rw-r--r--   0 benbusby  (1000) users      (985)    22526 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/routes.py
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.458581 whoogle-search-0.8.2/app/static/
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.458581 whoogle-search-0.8.2/app/static/build/
+-rw-r--r--   0 benbusby  (1000) users      (985)       14 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/build/.gitignore
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.458581 whoogle-search-0.8.2/app/static/css/
+-rw-r--r--   0 benbusby  (1000) users      (985)     4657 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/dark-theme.css
+-rw-r--r--   0 benbusby  (1000) users      (985)      106 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/error.css
+-rw-r--r--   0 benbusby  (1000) users      (985)     4256 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/header.css
+-rw-r--r--   0 benbusby  (1000) users      (985)      793 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/input.css
+-rw-r--r--   0 benbusby  (1000) users      (985)     4041 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/light-theme.css
+-rw-r--r--   0 benbusby  (1000) users      (985)      187 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/logo.css
+-rw-r--r--   0 benbusby  (1000) users      (985)     2910 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/main.css
+-rw-r--r--   0 benbusby  (1000) users      (985)     1044 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/search.css
+-rw-r--r--   0 benbusby  (1000) users      (985)     1074 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/css/variables.css
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.461915 whoogle-search-0.8.2/app/static/img/
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.461915 whoogle-search-0.8.2/app/static/img/favicon/
+-rw-r--r--   0 benbusby  (1000) users      (985)    10193 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/android-icon-144x144.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    12058 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/android-icon-192x192.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     2505 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/android-icon-36x36.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     3316 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/android-icon-48x48.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     4815 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/android-icon-72x72.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     6446 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/android-icon-96x96.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     7773 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-114x114.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     8257 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-120x120.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    10193 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-144x144.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    11002 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-152x152.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    13463 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-180x180.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     3871 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-57x57.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     4028 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-60x60.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     4815 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-72x72.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     5084 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-76x76.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    12632 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon-precomposed.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    12632 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/apple-icon.png
+-rw-r--r--   0 benbusby  (1000) users      (985)      281 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/browserconfig.xml
+-rw-r--r--   0 benbusby  (1000) users      (985)     1393 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/favicon-16x16.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     2142 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/favicon-32x32.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     6446 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/favicon-96x96.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     1150 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/favicon.ico
+-rw-r--r--   0 benbusby  (1000) users      (985)      787 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/manifest.json
+-rw-r--r--   0 benbusby  (1000) users      (985)    10193 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/ms-icon-144x144.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    10808 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/ms-icon-150x150.png
+-rw-r--r--   0 benbusby  (1000) users      (985)    29292 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/ms-icon-310x310.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     4703 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon/ms-icon-70x70.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     1150 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/favicon.ico
+-rw-r--r--   0 benbusby  (1000) users      (985)    24077 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/logo.png
+-rw-r--r--   0 benbusby  (1000) users      (985)     7199 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/img/whoogle.svg
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.461915 whoogle-search-0.8.2/app/static/js/
+-rw-r--r--   0 benbusby  (1000) users      (985)     4722 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/js/autocomplete.js
+-rw-r--r--   0 benbusby  (1000) users      (985)     2699 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/js/controller.js
+-rw-r--r--   0 benbusby  (1000) users      (985)      394 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/js/currency.js
+-rw-r--r--   0 benbusby  (1000) users      (985)     2238 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/js/header.js
+-rw-r--r--   0 benbusby  (1000) users      (985)     1645 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/js/keyboard.js
+-rw-r--r--   0 benbusby  (1000) users      (985)     2614 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/js/utils.js
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/app/static/settings/
+-rw-r--r--   0 benbusby  (1000) users      (985)    10215 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/settings/countries.json
+-rw-r--r--   0 benbusby  (1000) users      (985)      614 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/settings/header_tabs.json
+-rw-r--r--   0 benbusby  (1000) users      (985)     2991 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/settings/languages.json
+-rw-r--r--   0 benbusby  (1000) users      (985)       42 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/settings/themes.json
+-rw-r--r--   0 benbusby  (1000) users      (985)      260 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/settings/time_periods.json
+-rw-r--r--   0 benbusby  (1000) users      (985)    66113 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/settings/translations.json
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/app/static/widgets/
+-rw-r--r--   0 benbusby  (1000) users      (985)     8519 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/static/widgets/calculator.html
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/app/templates/
+-rw-r--r--   0 benbusby  (1000) users      (985)     2047 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/display.html
+-rw-r--r--   0 benbusby  (1000) users      (985)     1311 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/error.html
+-rw-r--r--   0 benbusby  (1000) users      (985)      334 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/footer.html
+-rw-r--r--   0 benbusby  (1000) users      (985)     7161 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/header.html
+-rw-r--r--   0 benbusby  (1000) users      (985)     8040 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/imageresults.html
+-rw-r--r--   0 benbusby  (1000) users      (985)    16940 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/index.html
+-rw-r--r--   0 benbusby  (1000) users      (985)     7543 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/logo.html
+-rw-r--r--   0 benbusby  (1000) users      (985)     6511 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/opensearch.xml
+-rw-r--r--   0 benbusby  (1000) users      (985)      453 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/templates/search.html
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/app/utils/
+-rw-r--r--   0 benbusby  (1000) users      (985)        0 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/utils/__init__.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     2594 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/utils/bangs.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     2586 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/utils/misc.py
+-rw-r--r--   0 benbusby  (1000) users      (985)    15167 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/utils/results.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     6331 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/utils/search.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     1031 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/utils/session.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     2205 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/utils/widgets.py
+-rw-r--r--   0 benbusby  (1000) users      (985)      157 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/app/version.py
+-rw-r--r--   0 benbusby  (1000) users      (985)       90 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/pyproject.toml
+-rw-r--r--   0 benbusby  (1000) users      (985)      721 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/requirements.txt
+-rw-r--r--   0 benbusby  (1000) users      (985)      961 2023-04-13 20:05:30.468581 whoogle-search-0.8.2/setup.cfg
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/test/
+-rw-r--r--   0 benbusby  (1000) users      (985)      498 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/test/test_autocomplete.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     3024 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/test/test_misc.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     4339 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/test/test_results.py
+-rw-r--r--   0 benbusby  (1000) users      (985)     2349 2023-04-13 19:52:45.000000 whoogle-search-0.8.2/test/test_routes.py
+drwxr-xr-x   0 benbusby  (1000) users      (985)        0 2023-04-13 20:05:30.465248 whoogle-search-0.8.2/whoogle_search.egg-info/
+-rw-r--r--   0 benbusby  (1000) users      (985)    37366 2023-04-13 20:05:30.000000 whoogle-search-0.8.2/whoogle_search.egg-info/PKG-INFO
+-rw-r--r--   0 benbusby  (1000) users      (985)     2882 2023-04-13 20:05:30.000000 whoogle-search-0.8.2/whoogle_search.egg-info/SOURCES.txt
+-rw-r--r--   0 benbusby  (1000) users      (985)        1 2023-04-13 20:05:30.000000 whoogle-search-0.8.2/whoogle_search.egg-info/dependency_links.txt
+-rw-r--r--   0 benbusby  (1000) users      (985)       54 2023-04-13 20:05:30.000000 whoogle-search-0.8.2/whoogle_search.egg-info/entry_points.txt
+-rw-r--r--   0 benbusby  (1000) users      (985)      148 2023-04-13 20:05:30.000000 whoogle-search-0.8.2/whoogle_search.egg-info/requires.txt
+-rw-r--r--   0 benbusby  (1000) users      (985)        4 2023-04-13 20:05:30.000000 whoogle-search-0.8.2/whoogle_search.egg-info/top_level.txt
```

### Comparing `whoogle-search-0.8.1/LICENSE` & `whoogle-search-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/PKG-INFO` & `whoogle-search-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoogle-search
-Version: 0.8.1
+Version: 0.8.2
 Summary: Self-hosted, ad-free, privacy-respecting metasearch engine
 Home-page: https://github.com/benbusby/whoogle-search
 Author: Ben Busby
 Author-email: contact@benbusby.com
 License: MIT
 Keywords: search,metasearch,flask,adblock,degoogle,privacy
 Classifier: Programming Language :: Python :: 3
@@ -31,25 +31,25 @@
   </tr>
 </table>
 
 Get Google search results, but without any ads, javascript, AMP links, cookies, or IP address tracking. Easily deployable in one click as a Docker app, and customizable with a single config file. Quick and simple to implement as a primary search engine replacement on both desktop and mobile.
 
 Contents
 1. [Features](#features)
-2. [Dependencies](#dependencies)
-3. [Install/Deploy](#install)
-    1. [Heroku Quick Deploy](#a-heroku-quick-deploy)
-    2. [Repl.it](#b-replit)
-    3. [Fly.io](#c-flyio)
-    4. [pipx](#d-pipx)
-    5. [pip](#e-pip)
-    6. [Manual](#f-manual)
-    7. [Docker](#g-manual-docker)
-    8. [Arch/AUR](#arch-linux--arch-based-distributions)
-    9. [Helm/Kubernetes](#helm-chart-for-kubernetes)
+3. [Install/Deploy Options](#install)
+    1. [Heroku Quick Deploy](#heroku-quick-deploy)
+    1. [Repl.it](#replit)
+    1. [Fly.io](#flyio)
+    1. [Koyeb](#koyeb)
+    1. [pipx](#pipx)
+    1. [pip](#pip)
+    1. [Manual](#manual)
+    1. [Docker](#manual-docker)
+    1. [Arch/AUR](#arch-linux--arch-based-distributions)
+    1. [Helm/Kubernetes](#helm-chart-for-kubernetes)
 4. [Environment Variables and Configuration](#environment-variables)
 5. [Usage](#usage)
 6. [Extra Steps](#extra-steps)
     1. [Set Primary Search Engine](#set-whoogle-as-your-primary-search-engine)
     2. [Prevent Downtime (Heroku Only)](#prevent-downtime-heroku-only)
     3. [Manual HTTPS Enforcement](#https-enforcement)
     4. [Using with Firefox Containers](#using-with-firefox-containers)
@@ -81,75 +81,86 @@
 
 <sup>*No third party JavaScript. Whoogle can be used with JavaScript disabled, but if enabled, uses JavaScript for things like presenting search suggestions.</sup>
 
 <sup>**No third party cookies. Whoogle uses server side cookies (sessions) to store non-sensitive configuration settings such as theme, language, etc. Just like with JavaScript, cookies can be disabled and not affect Whoogle's search functionality.</sup>
 
 <sup>***If deployed to a remote server, or configured to send requests through a VPN, Tor, proxy, etc.</sup>
 
-## Dependencies
-If using Heroku Quick Deploy, **you can skip this section**.
-
-- Docker ([Windows](https://docs.docker.com/docker-for-windows/install/), [macOS](https://docs.docker.com/docker-for-mac/install/), [Ubuntu](https://docs.docker.com/engine/install/ubuntu/), [other Linux distros](https://docs.docker.com/engine/install/binaries/))
-  - Only needed if you intend on deploying the app as a Docker image
-- [Python3](https://www.python.org/downloads/)
-- `libcurl4-openssl-dev` and `libssl-dev`
-  - macOS: `brew install openssl curl-openssl`
-  - Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev`
-  - Arch: `pacman -S curl openssl`
-
 ## Install
 There are a few different ways to begin using the app, depending on your preferences:
 
-### A) [Heroku Quick Deploy](https://heroku.com/about)
+___
+
+### [Heroku Quick Deploy](https://heroku.com/about)
 [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/benbusby/whoogle-search/tree/main)
 
 Provides:
 - Easy Deployment of App
 - A HTTPS url (https://\<your app name\>.herokuapp.com)
 
 Notes:
 - Requires a **PAID** Heroku Account.
 - Sometimes has issues with auto-redirecting to `https`. Make sure to navigate to the `https` version of your app before adding as a default search engine.
 
-### B) [Repl.it](https://repl.it)
+___
+
+### [Repl.it](https://repl.it)
 [![Run on Repl.it](https://repl.it/badge/github/benbusby/whoogle-search)](https://repl.it/github/benbusby/whoogle-search)
 
 *Note: Requires a (free) Replit account*
 
 Provides:
 - Free deployment of app
 - Free HTTPS url (https://\<app name\>.\<username\>\.repl\.co)
     - Supports custom domains
 - Downtime after periods of inactivity \([solution 1](https://repl.it/talk/ask/use-this-pingmat1replco-just-enter/28821/101298), [solution 2](https://repl.it/talk/learn/How-to-use-and-setup-UptimeRobot/9003)\)
 
-### C) [Fly.io](https://fly.io)
+___
+
+### [Fly.io](https://fly.io)
 
 You will need a **PAID** [Fly.io](https://fly.io) account to deploy Whoogle.
 
 #### Install the CLI: https://fly.io/docs/hands-on/installing/
 
 #### Deploy the app
 
 ```bash
 flyctl auth login
 flyctl launch --image benbusby/whoogle-search:latest
 ```
 
+The first deploy won't succeed because the default `internal_port` is wrong.
+To fix this, open the generated `fly.toml` file, set `services.internal_port` to `5000` and run `flyctl launch` again.
+
 Your app is now available at `https://<app-name>.fly.dev`.
 
-### D) [pipx](https://github.com/pipxproject/pipx#install-pipx)
+___
+
+### [Koyeb](https://www.koyeb.com)
+
+Use one of the following guides to install Whoogle on Koyeb:
+
+1. Using GitHub: https://www.koyeb.com/docs/quickstart/deploy-with-git
+2. Using Docker: https://www.koyeb.com/docs/quickstart/deploy-a-docker-application
+
+___
+
+### [pipx](https://github.com/pipxproject/pipx#install-pipx)
 Persistent install:
 
 `pipx install git+https://github.com/benbusby/whoogle-search.git`
 
 Sandboxed temporary instance:
 
 `pipx run --spec git+https://github.com/benbusby/whoogle-search.git whoogle-search`
 
-### E) pip
+___
+
+### pip
 `pip install whoogle-search`
 
 ```bash
 $ whoogle-search --help
 usage: whoogle-search [-h] [--port <port number>] [--host <ip address>] [--debug] [--https-only] [--userpass <username:password>]
                       [--proxyauth <username:password>] [--proxytype <socks4|socks5|http>] [--proxyloc <location:port>]
 
@@ -168,18 +179,29 @@
   --proxytype <socks4|socks5|http>
                         Sets a proxy type for all connections (default None)
   --proxyloc <location:port>
                         Sets a proxy location for all connections (default None)
 ```
 See the [available environment variables](#environment-variables) for additional configuration.
 
-### F) Manual
+___
+
+### Manual
 
 *Note: `Content-Security-Policy` headers can be sent by Whoogle if you set `WHOOGLE_CSP`.*
 
+#### Dependencies
+- [Python3](https://www.python.org/downloads/)
+- `libcurl4-openssl-dev` and `libssl-dev`
+  - macOS: `brew install openssl curl-openssl`
+  - Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev`
+  - Arch: `pacman -S curl openssl`
+
+#### Install
+
 Clone the repo and run the following commands to start the app in a local-only environment:
 
 ```bash
 git clone https://github.com/benbusby/whoogle-search.git
 cd whoogle-search
 python3 -m venv venv
 source venv/bin/activate
@@ -205,15 +227,14 @@
 #Environment=WHOOGLE_PROXY_TYPE=<proxy type (http|https|proxy4|proxy5)
 #Environment=WHOOGLE_PROXY_LOC=<proxy host/ip>
 # Site alternative configurations, uncomment to enable
 # Note: If not set, the feature will still be available
 # with default values.
 #Environment=WHOOGLE_ALT_TW=farside.link/nitter
 #Environment=WHOOGLE_ALT_YT=farside.link/invidious
-#Environment=WHOOGLE_ALT_IG=farside.link/bibliogram/u
 #Environment=WHOOGLE_ALT_RD=farside.link/libreddit
 #Environment=WHOOGLE_ALT_MD=farside.link/scribe
 #Environment=WHOOGLE_ALT_TL=farside.link/lingva
 #Environment=WHOOGLE_ALT_IMG=farside.link/rimgo
 #Environment=WHOOGLE_ALT_WIKI=farside.link/wikiless
 #Environment=WHOOGLE_ALT_IMDB=farside.link/libremdb
 #Environment=WHOOGLE_ALT_QUORA=farside.link/quetre
@@ -285,15 +306,17 @@
        - `chmod 400 control.conf`
 
     5. Finally set the Tor environment variable and use password variable to 1, `WHOOGLE_CONFIG_TOR` and `WHOOGLE_TOR_USE_PASS`. Refer to the [Environment Variables](#environment-variables) section for more details.
        - These may be added to the systemd unit file or env file:
           - `WHOOGLE_CONFIG_TOR=1`
           - `WHOOGLE_TOR_USE_PASS=1`
 
-### G) Manual (Docker)
+___
+
+### Manual (Docker)
 1. Ensure the Docker daemon is running, and is accessible by your user account
   - To add user permissions, you can execute `sudo usermod -aG docker yourusername`
   - Running `docker ps` should return something besides an error. If you encounter an error saying the daemon isn't running, try `sudo systemctl start docker` (Linux) or ensure the docker tool is running (Windows/macOS).
 2. Clone and deploy the docker app using a method below:
 
 #### Docker CLI
 
@@ -346,24 +369,30 @@
 heroku container:release web
 heroku open
 ```
 
 This series of commands can take a while, but once you run it once, you shouldn't have to run it again. The final command, `heroku open` will launch a tab in your web browser, where you can test out Whoogle and even [set it as your primary search engine](https://github.com/benbusby/whoogle#set-whoogle-as-your-primary-search-engine).
 You may also edit environment variables from your app’s Settings tab in the Heroku Dashboard.
 
-#### Arch Linux & Arch-based Distributions
+___
+
+### Arch Linux & Arch-based Distributions
 There is an [AUR package available](https://aur.archlinux.org/packages/whoogle-git/), as well as a pre-built and daily updated package available at [Chaotic-AUR](https://chaotic.cx).
 
-#### Helm chart for Kubernetes
+___
+
+### Helm chart for Kubernetes
 To use the Kubernetes Helm Chart:
 1. Ensure you have [Helm](https://helm.sh/docs/intro/install/) `>=3.0.0` installed
 2. Clone this repository
 3. Update [charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired
 4. Run `helm install whoogle ./charts/whoogle`
 
+___
+
 #### Using your own server, or alternative container deployment
 There are other methods for deploying docker containers that are well outlined in [this article](https://rollout.io/blog/the-shortlist-of-docker-hosting/), but there are too many to describe set up for each here. Generally it should be about the same amount of effort as the Heroku deployment.
 
 Depending on your preferences, you can also deploy the app yourself on your own infrastructure. This route would require a few extra steps:
   - A server (I personally recommend [Digital Ocean](https://www.digitalocean.com/pricing/) or [Linode](https://www.linode.com/pricing/), their cheapest tiers will work fine)
   - Your own URL (I suppose this is optional, but recommended)
   - SSL certificates (free through [Let's Encrypt](https://letsencrypt.org/getting-started/))
@@ -386,15 +415,14 @@
 | WHOOGLE_PROXY_PASS   | The password of the proxy server.                                                         |
 | WHOOGLE_PROXY_TYPE   | The type of the proxy server. Can be "socks5", "socks4", or "http".                       |
 | WHOOGLE_PROXY_LOC    | The location of the proxy server (host or ip).                                            |
 | EXPOSE_PORT          | The port where Whoogle will be exposed.                                                   |
 | HTTPS_ONLY           | Enforce HTTPS. (See [here](https://github.com/benbusby/whoogle-search#https-enforcement)) |
 | WHOOGLE_ALT_TW       | The twitter.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_YT       | The youtube.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
-| WHOOGLE_ALT_IG       | The instagram.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_RD       | The reddit.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_TL       | The Google Translate alternative to use. This is used for all "translate ____" searches.  Set to "" to disable. |
 | WHOOGLE_ALT_MD       | The medium.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_IMG      | The imgur.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_WIKI     | The wikipedia.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_IMDB     | The imdb.com alternative to use when site alternatives are enabled in the config. Set to "" to disable.  |
 | WHOOGLE_ALT_QUORA    | The quora.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
@@ -412,14 +440,16 @@
 | Variable                             | Description                                                     |
 | ------------------------------------ | --------------------------------------------------------------- |
 | WHOOGLE_CONFIG_DISABLE               | Hide config from UI and disallow changes to config by client    |
 | WHOOGLE_CONFIG_COUNTRY               | Filter results by hosting country                               |
 | WHOOGLE_CONFIG_LANGUAGE              | Set interface language                                          |
 | WHOOGLE_CONFIG_SEARCH_LANGUAGE       | Set search result language                                      |
 | WHOOGLE_CONFIG_BLOCK                 | Block websites from search results (use comma-separated list)   |
+| WHOOGLE_CONFIG_BLOCK_TITLE           | Block search result with a REGEX filter on title                |
+| WHOOGLE_CONFIG_BLOCK_URL             | Block search result with a REGEX filter on URL                  |
 | WHOOGLE_CONFIG_THEME                 | Set theme mode (light, dark, or system)                         |
 | WHOOGLE_CONFIG_SAFE                  | Enable safe searches                                            |
 | WHOOGLE_CONFIG_ALTS                  | Use social media site alternatives (nitter, invidious, etc)     |
 | WHOOGLE_CONFIG_NEAR                  | Restrict results to only those near a particular city           |
 | WHOOGLE_CONFIG_TOR                   | Use Tor routing (if available)                                  |
 | WHOOGLE_CONFIG_NEW_TAB               | Always open results in new tab                                  |
 | WHOOGLE_CONFIG_VIEW_IMAGE            | Enable View Image option                                        |
@@ -606,29 +636,31 @@
 | [https://search.garudalinux.org](https://search.garudalinux.org) | 🇫🇮 FI | Multi-choice | ✅ |
 | [https://search.dr460nf1r3.org](https://search.dr460nf1r3.org) | 🇩🇪 DE | Multi-choice | ✅ |
 | [https://s.tokhmi.xyz](https://s.tokhmi.xyz) | 🇺🇸 US | Multi-choice | ✅ |
 | [https://search.sethforprivacy.com](https://search.sethforprivacy.com) | 🇩🇪 DE | English | |
 | [https://whoogle.dcs0.hu](https://whoogle.dcs0.hu) | 🇭🇺 HU | Multi-choice | |
 | [https://whoogle.esmailelbob.xyz](https://whoogle.esmailelbob.xyz) | 🇨🇦 CA | Multi-choice | |
 | [https://gowogle.voring.me](https://gowogle.voring.me) | 🇺🇸 US | Multi-choice | |
-| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | 🇺🇸 US | English | |
+| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | 🇳🇱 NL | English | |
 | [https://wg.vern.cc](https://wg.vern.cc) | 🇺🇸 US | English |  |
-| [https://www.indexia.gq](https://www.indexia.gq) | 🇨🇦 CA | Multi-choice | ✅ |
+| [https://whoogle.hxvy0.gq](https://whoogle.hxvy0.gq) | 🇨🇦 CA | Turkish Only | ✅ |
 | [https://whoogle.hostux.net](https://whoogle.hostux.net) | 🇫🇷 FR | Multi-choice | |
+| [https://whoogle.lunar.icu](https://whoogle.lunar.icu) | 🇩🇪 DE | Multi-choice | ✅ |
+| [https://wgl.frail.duckdns.org](https://wgl.frail.duckdns.org) | 🇧🇷 BR | Multi-choice | |
 
 * A checkmark in the "Cloudflare" category here refers to the use of the reverse proxy, [Cloudflare](https://cloudflare.com). The checkmark will not be listed for a site which uses Cloudflare DNS but rather the proxying service which grants Cloudflare the ability to monitor traffic to the website.
 
 #### Onion Instances
 
 | Website | Country | Language |
 |-|-|-|
 | [http://whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion](http://whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion) | 🇺🇸 US |  Multi-choice
 | [http://nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion](http://nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion) | 🇩🇪 DE |  English
 | [http://whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/) | 🇺🇸 US | English |
-| [http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) | 🇺🇸 US | English |
+| [http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) | 🇳🇱 NL | English |
 
 #### I2P Instances
 
 | Website | Country | Language |
 |-|-|-|
 | [http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p](http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p) | 🇺🇸 US | English |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: whoogle-search Version: 0.8.1 Summary: Self-hosted,
+Metadata-Version: 2.1 Name: whoogle-search Version: 0.8.2 Summary: Self-hosted,
 ad-free, privacy-respecting metasearch engine Home-page: https://github.com/
 benbusby/whoogle-search Author: Ben Busby Author-email: contact@benbusby.com
 License: MIT Keywords: search,metasearch,flask,adblock,degoogle,privacy
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
 dev License-File: LICENSE ![Whoogle Search](docs/banner.png) [![Latest Release]
@@ -18,110 +18,110 @@
 benbusby-shoogle-master) [![Docker Pulls](https://img.shields.io/docker/pulls/
 benbusby/whoogle-search)](https://hub.docker.com/r/benbusby/whoogle-search)
 SourceHut GitHub
 Get Google search results, but without any ads, javascript, AMP links, cookies,
 or IP address tracking. Easily deployable in one click as a Docker app, and
 customizable with a single config file. Quick and simple to implement as a
 primary search engine replacement on both desktop and mobile. Contents 1.
-[Features](#features) 2. [Dependencies](#dependencies) 3. [Install/Deploy]
-(#install) 1. [Heroku Quick Deploy](#a-heroku-quick-deploy) 2. [Repl.it](#b-
-replit) 3. [Fly.io](#c-flyio) 4. [pipx](#d-pipx) 5. [pip](#e-pip) 6. [Manual]
-(#f-manual) 7. [Docker](#g-manual-docker) 8. [Arch/AUR](#arch-linux--arch-
-based-distributions) 9. [Helm/Kubernetes](#helm-chart-for-kubernetes) 4.
-[Environment Variables and Configuration](#environment-variables) 5. [Usage]
-(#usage) 6. [Extra Steps](#extra-steps) 1. [Set Primary Search Engine](#set-
-whoogle-as-your-primary-search-engine) 2. [Prevent Downtime (Heroku Only)]
-(#prevent-downtime-heroku-only) 3. [Manual HTTPS Enforcement](#https-
-enforcement) 4. [Using with Firefox Containers](#using-with-firefox-containers)
-5. [Reverse Proxying](#reverse-proxying) 1. [Nginx](#nginx) 7. [Contributing]
-(#contributing) 8. [FAQ](#faq) 9. [Public Instances](#public-instances) 10.
-[Screenshots](#screenshots) ## Features - No ads or sponsored content - No
-JavaScript\* - No cookies\*\* - No tracking/linking of your personal IP
-address\*\*\* - No AMP links - No URL tracking tags (i.e. utm=%s) - No referrer
-header - Tor and HTTP/SOCKS proxy support - Autocomplete/search suggestions -
-POST request search and suggestion queries (when possible) - View images at
-full res without site redirect (currently mobile only) - Light/Dark/System
-theme modes (with support for [custom CSS theming](https://github.com/benbusby/
-whoogle-search/wiki/User-Contributed-CSS-Themes)) - Randomly generated User
-Agent - Easy to install/deploy - DDG-style bang (i.e. `! `) searches - Optional
-location-based searching (i.e. results near \
+[Features](#features) 3. [Install/Deploy Options](#install) 1. [Heroku Quick
+Deploy](#heroku-quick-deploy) 1. [Repl.it](#replit) 1. [Fly.io](#flyio) 1.
+[Koyeb](#koyeb) 1. [pipx](#pipx) 1. [pip](#pip) 1. [Manual](#manual) 1.
+[Docker](#manual-docker) 1. [Arch/AUR](#arch-linux--arch-based-distributions)
+1. [Helm/Kubernetes](#helm-chart-for-kubernetes) 4. [Environment Variables and
+Configuration](#environment-variables) 5. [Usage](#usage) 6. [Extra Steps]
+(#extra-steps) 1. [Set Primary Search Engine](#set-whoogle-as-your-primary-
+search-engine) 2. [Prevent Downtime (Heroku Only)](#prevent-downtime-heroku-
+only) 3. [Manual HTTPS Enforcement](#https-enforcement) 4. [Using with Firefox
+Containers](#using-with-firefox-containers) 5. [Reverse Proxying](#reverse-
+proxying) 1. [Nginx](#nginx) 7. [Contributing](#contributing) 8. [FAQ](#faq) 9.
+[Public Instances](#public-instances) 10. [Screenshots](#screenshots) ##
+Features - No ads or sponsored content - No JavaScript\* - No cookies\*\* - No
+tracking/linking of your personal IP address\*\*\* - No AMP links - No URL
+tracking tags (i.e. utm=%s) - No referrer header - Tor and HTTP/SOCKS proxy
+support - Autocomplete/search suggestions - POST request search and suggestion
+queries (when possible) - View images at full res without site redirect
+(currently mobile only) - Light/Dark/System theme modes (with support for
+[custom CSS theming](https://github.com/benbusby/whoogle-search/wiki/User-
+Contributed-CSS-Themes)) - Randomly generated User Agent - Easy to install/
+deploy - DDG-style bang (i.e. `! `) searches - Optional location-based
+searching (i.e. results near \
 >) - Optional NoJS mode to view search results in a separate window with
 JavaScript blocked *No third party JavaScript. Whoogle can be used with
 JavaScript disabled, but if enabled, uses JavaScript for things like presenting
 search suggestions. **No third party cookies. Whoogle uses server side cookies
 (sessions) to store non-sensitive configuration settings such as theme,
 language, etc. Just like with JavaScript, cookies can be disabled and not
 affect Whoogle's search functionality. ***If deployed to a remote server, or
-configured to send requests through a VPN, Tor, proxy, etc. ## Dependencies If
-using Heroku Quick Deploy, **you can skip this section**. - Docker ([Windows]
-(https://docs.docker.com/docker-for-windows/install/), [macOS](https://
-docs.docker.com/docker-for-mac/install/), [Ubuntu](https://docs.docker.com/
-engine/install/ubuntu/), [other Linux distros](https://docs.docker.com/engine/
-install/binaries/)) - Only needed if you intend on deploying the app as a
-Docker image - [Python3](https://www.python.org/downloads/) - `libcurl4-
-openssl-dev` and `libssl-dev` - macOS: `brew install openssl curl-openssl` -
-Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev` - Arch:
-`pacman -S curl openssl` ## Install There are a few different ways to begin
-using the app, depending on your preferences: ### A) [Heroku Quick Deploy]
-(https://heroku.com/about) [![Deploy](https://www.herokucdn.com/deploy/
-button.svg)](https://heroku.com/deploy?template=https://github.com/benbusby/
-whoogle-search/tree/main) Provides: - Easy Deployment of App - A HTTPS url
-(https://\
+configured to send requests through a VPN, Tor, proxy, etc. ## Install There
+are a few different ways to begin using the app, depending on your preferences:
+___ ### [Heroku Quick Deploy](https://heroku.com/about) [![Deploy](https://
+www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https:
+//github.com/benbusby/whoogle-search/tree/main) Provides: - Easy Deployment of
+App - A HTTPS url (https://\
 >.herokuapp.com) Notes: - Requires a **PAID** Heroku Account. - Sometimes has
 issues with auto-redirecting to `https`. Make sure to navigate to the `https`
-version of your app before adding as a default search engine. ### B) [Repl.it]
+version of your app before adding as a default search engine. ___ ### [Repl.it]
 (https://repl.it) [![Run on Repl.it](https://repl.it/badge/github/benbusby/
 whoogle-search)](https://repl.it/github/benbusby/whoogle-search) *Note:
 Requires a (free) Replit account* Provides: - Free deployment of app - Free
 HTTPS url (https://\
 >.\
 >\.repl\.co) - Supports custom domains - Downtime after periods of inactivity \
 ([solution 1](https://repl.it/talk/ask/use-this-pingmat1replco-just-enter/
 28821/101298), [solution 2](https://repl.it/talk/learn/How-to-use-and-setup-
-UptimeRobot/9003)\) ### C) [Fly.io](https://fly.io) You will need a **PAID**
+UptimeRobot/9003)\) ___ ### [Fly.io](https://fly.io) You will need a **PAID**
 [Fly.io](https://fly.io) account to deploy Whoogle. #### Install the CLI:
 https://fly.io/docs/hands-on/installing/ #### Deploy the app ```bash flyctl
-auth login flyctl launch --image benbusby/whoogle-search:latest ``` Your app is
-now available at `https://.fly.dev`. ### D) [pipx](https://github.com/
-pipxproject/pipx#install-pipx) Persistent install: `pipx install git+https://
-github.com/benbusby/whoogle-search.git` Sandboxed temporary instance: `pipx run
---spec git+https://github.com/benbusby/whoogle-search.git whoogle-search` ###
-E) pip `pip install whoogle-search` ```bash $ whoogle-search --help usage:
-whoogle-search [-h] [--port ] [--host ] [--debug] [--https-only] [--userpass ]
-[--proxyauth ] [--proxytype
+auth login flyctl launch --image benbusby/whoogle-search:latest ``` The first
+deploy won't succeed because the default `internal_port` is wrong. To fix this,
+open the generated `fly.toml` file, set `services.internal_port` to `5000` and
+run `flyctl launch` again. Your app is now available at `https://.fly.dev`. ___
+### [Koyeb](https://www.koyeb.com) Use one of the following guides to install
+Whoogle on Koyeb: 1. Using GitHub: https://www.koyeb.com/docs/quickstart/
+deploy-with-git 2. Using Docker: https://www.koyeb.com/docs/quickstart/deploy-
+a-docker-application ___ ### [pipx](https://github.com/pipxproject/
+pipx#install-pipx) Persistent install: `pipx install git+https://github.com/
+benbusby/whoogle-search.git` Sandboxed temporary instance: `pipx run --spec
+git+https://github.com/benbusby/whoogle-search.git whoogle-search` ___ ### pip
+`pip install whoogle-search` ```bash $ whoogle-search --help usage: whoogle-
+search [-h] [--port ] [--host ] [--debug] [--https-only] [--userpass ] [--
+proxyauth ] [--proxytype
 socks5|http>] [--proxyloc ] Whoogle Search console runner optional arguments: -
 h, --help Show this help message and exit --port  Specifies a port to run on
 (default 5000) --host  Specifies the host address to use (default 127.0.0.1) --
 debug Activates debug mode for the server (default False) --https-only Enforces
 HTTPS redirects for all requests --userpass  Sets a username/password basic
 auth combo (default None) --proxyauth  Sets a username/password for a HTTP/
 SOCKS proxy (default None) --proxytype
 socks5|http> Sets a proxy type for all connections (default None) --proxyloc
 Sets a proxy location for all connections (default None) ``` See the [available
 environment variables](#environment-variables) for additional configuration.
-### F) Manual *Note: `Content-Security-Policy` headers can be sent by Whoogle
-if you set `WHOOGLE_CSP`.* Clone the repo and run the following commands to
-start the app in a local-only environment: ```bash git clone https://
-github.com/benbusby/whoogle-search.git cd whoogle-search python3 -m venv venv
-source venv/bin/activate pip install -r requirements.txt ./run ``` See the
-[available environment variables](#environment-variables) for additional
-configuration. #### systemd Configuration After building the virtual
-environment, you can add something like the following to `/lib/systemd/system/
-whoogle.service` to set up a Whoogle Search systemd service: ```ini [Unit]
-Description=Whoogle [Service] # Basic auth configuration, uncomment to enable
-#Environment=WHOOGLE_USER= #Environment=WHOOGLE_PASS= # Proxy configuration,
-uncomment to enable #Environment=WHOOGLE_PROXY_USER=
-#Environment=WHOOGLE_PROXY_PASS= #Environment=WHOOGLE_PROXY_TYPE=
+___ ### Manual *Note: `Content-Security-Policy` headers can be sent by Whoogle
+if you set `WHOOGLE_CSP`.* #### Dependencies - [Python3](https://
+www.python.org/downloads/) - `libcurl4-openssl-dev` and `libssl-dev` - macOS:
+`brew install openssl curl-openssl` - Ubuntu: `sudo apt-get install -
+y libcurl4-openssl-dev libssl-dev` - Arch: `pacman -S curl openssl` ####
+Install Clone the repo and run the following commands to start the app in a
+local-only environment: ```bash git clone https://github.com/benbusby/whoogle-
+search.git cd whoogle-search python3 -m venv venv source venv/bin/activate pip
+install -r requirements.txt ./run ``` See the [available environment variables]
+(#environment-variables) for additional configuration. #### systemd
+Configuration After building the virtual environment, you can add something
+like the following to `/lib/systemd/system/whoogle.service` to set up a Whoogle
+Search systemd service: ```ini [Unit] Description=Whoogle [Service] # Basic
+auth configuration, uncomment to enable #Environment=WHOOGLE_USER=
+#Environment=WHOOGLE_PASS= # Proxy configuration, uncomment to enable
+#Environment=WHOOGLE_PROXY_USER= #Environment=WHOOGLE_PROXY_PASS=
+#Environment=WHOOGLE_PROXY_TYPE=
 http|https|proxy4|proxy5) #Environment=WHOOGLE_PROXY_LOC=
 p> # Site alternative configurations, uncomment to enable # Note: If not set,
 the feature will still be available # with default values.
 #Environment=WHOOGLE_ALT_TW=farside.link/nitter
 #Environment=WHOOGLE_ALT_YT=farside.link/invidious
-#Environment=WHOOGLE_ALT_IG=farside.link/bibliogram/
-u #Environment=WHOOGLE_ALT_RD=farside.link/libreddit
+#Environment=WHOOGLE_ALT_RD=farside.link/libreddit
 #Environment=WHOOGLE_ALT_MD=farside.link/scribe
 #Environment=WHOOGLE_ALT_TL=farside.link/lingva
 #Environment=WHOOGLE_ALT_IMG=farside.link/rimgo
 #Environment=WHOOGLE_ALT_WIKI=farside.link/wikiless
 #Environment=WHOOGLE_ALT_IMDB=farside.link/libremdb
 #Environment=WHOOGLE_ALT_QUORA=farside.link/quetre # Load values from dotenv
 only #Environment=WHOOGLE_DOTENV=1 Type=simple User= # If installed as a
@@ -159,15 +159,15 @@
 the `WHOOGLE_TOR_CONF` environment variable. Refer to the [Environment
 Variables](#environment-variables) section for more details. 4. Heavily
 restrict access to control.conf to only be readable by the user running
 whoogle: - `chmod 400 control.conf` 5. Finally set the Tor environment variable
 and use password variable to 1, `WHOOGLE_CONFIG_TOR` and
 `WHOOGLE_TOR_USE_PASS`. Refer to the [Environment Variables](#environment-
 variables) section for more details. - These may be added to the systemd unit
-file or env file: - `WHOOGLE_CONFIG_TOR=1` - `WHOOGLE_TOR_USE_PASS=1` ### G)
+file or env file: - `WHOOGLE_CONFIG_TOR=1` - `WHOOGLE_TOR_USE_PASS=1` ___ ###
 Manual (Docker) 1. Ensure the Docker daemon is running, and is accessible by
 your user account - To add user permissions, you can execute `sudo usermod -aG
 docker yourusername` - Running `docker ps` should return something besides an
 error. If you encounter an error saying the daemon isn't running, try `sudo
 systemctl start docker` (Linux) or ensure the docker tool is running (Windows/
 macOS). 2. Clone and deploy the docker app using a method below: #### Docker
 CLI Through Docker Hub: ```bash docker pull benbusby/whoogle-search docker run
@@ -188,22 +188,22 @@
 https://github.com/benbusby/whoogle-search.git cd whoogle-search heroku create
 heroku container:push web heroku container:release web heroku open ``` This
 series of commands can take a while, but once you run it once, you shouldn't
 have to run it again. The final command, `heroku open` will launch a tab in
 your web browser, where you can test out Whoogle and even [set it as your
 primary search engine](https://github.com/benbusby/whoogle#set-whoogle-as-your-
 primary-search-engine). You may also edit environment variables from your
-appâs Settings tab in the Heroku Dashboard. #### Arch Linux & Arch-based
+appâs Settings tab in the Heroku Dashboard. ___ ### Arch Linux & Arch-based
 Distributions There is an [AUR package available](https://aur.archlinux.org/
 packages/whoogle-git/), as well as a pre-built and daily updated package
-available at [Chaotic-AUR](https://chaotic.cx). #### Helm chart for Kubernetes
-To use the Kubernetes Helm Chart: 1. Ensure you have [Helm](https://helm.sh/
-docs/intro/install/) `>=3.0.0` installed 2. Clone this repository 3. Update
-[charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired 4. Run
-`helm install whoogle ./charts/whoogle` #### Using your own server, or
+available at [Chaotic-AUR](https://chaotic.cx). ___ ### Helm chart for
+Kubernetes To use the Kubernetes Helm Chart: 1. Ensure you have [Helm](https://
+helm.sh/docs/intro/install/) `>=3.0.0` installed 2. Clone this repository 3.
+Update [charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired 4.
+Run `helm install whoogle ./charts/whoogle` ___ #### Using your own server, or
 alternative container deployment There are other methods for deploying docker
 containers that are well outlined in [this article](https://rollout.io/blog/
 the-shortlist-of-docker-hosting/), but there are too many to describe set up
 for each here. Generally it should be about the same amount of effort as the
 Heroku deployment. Depending on your preferences, you can also deploy the app
 yourself on your own infrastructure. This route would require a few extra
 steps: - A server (I personally recommend [Digital Ocean](https://
@@ -228,23 +228,21 @@
 proxy server. Can be "socks5", "socks4", or "http". | | WHOOGLE_PROXY_LOC | The
 location of the proxy server (host or ip). | | EXPOSE_PORT | The port where
 Whoogle will be exposed. | | HTTPS_ONLY | Enforce HTTPS. (See [here](https://
 github.com/benbusby/whoogle-search#https-enforcement)) | | WHOOGLE_ALT_TW | The
 twitter.com alternative to use when site alternatives are enabled in the
 config. Set to "" to disable. | | WHOOGLE_ALT_YT | The youtube.com alternative
 to use when site alternatives are enabled in the config. Set to "" to disable.
-| | WHOOGLE_ALT_IG | The instagram.com alternative to use when site
-alternatives are enabled in the config. Set to "" to disable. | |
-WHOOGLE_ALT_RD | The reddit.com alternative to use when site alternatives are
-enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_TL | The Google
-Translate alternative to use. This is used for all "translate ____" searches.
-Set to "" to disable. | | WHOOGLE_ALT_MD | The medium.com alternative to use
-when site alternatives are enabled in the config. Set to "" to disable. | |
-WHOOGLE_ALT_IMG | The imgur.com alternative to use when site alternatives are
-enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_WIKI | The
+| | WHOOGLE_ALT_RD | The reddit.com alternative to use when site alternatives
+are enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_TL | The
+Google Translate alternative to use. This is used for all "translate ____"
+searches. Set to "" to disable. | | WHOOGLE_ALT_MD | The medium.com alternative
+to use when site alternatives are enabled in the config. Set to "" to disable.
+| | WHOOGLE_ALT_IMG | The imgur.com alternative to use when site alternatives
+are enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_WIKI | The
 wikipedia.com alternative to use when site alternatives are enabled in the
 config. Set to "" to disable. | | WHOOGLE_ALT_IMDB | The imdb.com alternative
 to use when site alternatives are enabled in the config. Set to "" to disable.
 | | WHOOGLE_ALT_QUORA | The quora.com alternative to use when site alternatives
 are enabled in the config. Set to "" to disable. | | WHOOGLE_AUTOCOMPLETE |
 Controls visibility of autocomplete/search suggestions. Default on -- use '0'
 to disable. | | WHOOGLE_MINIMAL | Remove everything except basic result cards
@@ -261,15 +259,17 @@
 instance to the same config state every time. | Variable | Description | | ----
 -------------------------------- | --------------------------------------------
 ------------------- | | WHOOGLE_CONFIG_DISABLE | Hide config from UI and
 disallow changes to config by client | | WHOOGLE_CONFIG_COUNTRY | Filter
 results by hosting country | | WHOOGLE_CONFIG_LANGUAGE | Set interface language
 | | WHOOGLE_CONFIG_SEARCH_LANGUAGE | Set search result language | |
 WHOOGLE_CONFIG_BLOCK | Block websites from search results (use comma-separated
-list) | | WHOOGLE_CONFIG_THEME | Set theme mode (light, dark, or system) | |
+list) | | WHOOGLE_CONFIG_BLOCK_TITLE | Block search result with a REGEX filter
+on title | | WHOOGLE_CONFIG_BLOCK_URL | Block search result with a REGEX filter
+on URL | | WHOOGLE_CONFIG_THEME | Set theme mode (light, dark, or system) | |
 WHOOGLE_CONFIG_SAFE | Enable safe searches | | WHOOGLE_CONFIG_ALTS | Use social
 media site alternatives (nitter, invidious, etc) | | WHOOGLE_CONFIG_NEAR |
 Restrict results to only those near a particular city | | WHOOGLE_CONFIG_TOR |
 Use Tor routing (if available) | | WHOOGLE_CONFIG_NEW_TAB | Always open results
 in new tab | | WHOOGLE_CONFIG_VIEW_IMAGE | Enable View Image option | |
 WHOOGLE_CONFIG_GET_ONLY | Search using GET requests only | | WHOOGLE_CONFIG_URL
 | The root url of the instance (`https:///`) | | WHOOGLE_CONFIG_STYLE | The
@@ -429,34 +429,37 @@
 search.dr460nf1r3.org) | ð©ðª DE | Multi-choice | â | | [https://
 s.tokhmi.xyz](https://s.tokhmi.xyz) | ðºð¸ US | Multi-choice | â | |
 [https://search.sethforprivacy.com](https://search.sethforprivacy.com) |
 ð©ðª DE | English | | | [https://whoogle.dcs0.hu](https://whoogle.dcs0.hu)
 | ð­ðº HU | Multi-choice | | | [https://whoogle.esmailelbob.xyz](https://
 whoogle.esmailelbob.xyz) | ð¨ð¦ CA | Multi-choice | | | [https://
 gowogle.voring.me](https://gowogle.voring.me) | ðºð¸ US | Multi-choice | |
-| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | ðºð¸
-US | English | | | [https://wg.vern.cc](https://wg.vern.cc) | ðºð¸ US |
-English | | | [https://www.indexia.gq](https://www.indexia.gq) | ð¨ð¦ CA |
-Multi-choice | â | | [https://whoogle.hostux.net](https://whoogle.hostux.net)
-|Â ð«ð· FR | Multi-choice | | * A checkmark in the "Cloudflare" category
-here refers to the use of the reverse proxy, [Cloudflare](https://
-cloudflare.com). The checkmark will not be listed for a site which uses
-Cloudflare DNS but rather the proxying service which grants Cloudflare the
-ability to monitor traffic to the website. #### Onion Instances | Website |
-Country | Language | |-|-|-| | [http://
+| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | ð³ð±
+NL | English | | | [https://wg.vern.cc](https://wg.vern.cc) | ðºð¸ US |
+English | | | [https://whoogle.hxvy0.gq](https://whoogle.hxvy0.gq) | ð¨ð¦
+CA | Turkish Only | â | | [https://whoogle.hostux.net](https://
+whoogle.hostux.net) |Â ð«ð· FR | Multi-choice | | | [https://
+whoogle.lunar.icu](https://whoogle.lunar.icu) | ð©ðª DE | Multi-choice |
+â | | [https://wgl.frail.duckdns.org](https://wgl.frail.duckdns.org) |
+ð§ð· BR | Multi-choice | | * A checkmark in the "Cloudflare" category here
+refers to the use of the reverse proxy, [Cloudflare](https://cloudflare.com).
+The checkmark will not be listed for a site which uses Cloudflare DNS but
+rather the proxying service which grants Cloudflare the ability to monitor
+traffic to the website. #### Onion Instances | Website | Country | Language |
+|-|-|-| | [http://
 whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion](http://
 whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion) | ðºð¸ US |
 Multi-choice | [http://
 nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion](http://
 nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion) | ð©ðª DE |
 English | [http://
 whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://
 whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/) |
 ðºð¸ US | English | | [http://
 whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://
 whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) |
-ðºð¸ US | English | #### I2P Instances | Website | Country | Language | |-
+ð³ð± NL | English | #### I2P Instances | Website | Country | Language | |-
 |-|-| | [http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p]
 (http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p) |
 ðºð¸ US | English | ## Screenshots #### Desktop ![Whoogle Desktop](docs/
 screenshot_desktop.png) #### Mobile ![Whoogle Mobile](docs/
 screenshot_mobile.png)
```

### Comparing `whoogle-search-0.8.1/README.md` & `whoogle-search-0.8.2/whoogle_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: whoogle-search
+Version: 0.8.2
+Summary: Self-hosted, ad-free, privacy-respecting metasearch engine
+Home-page: https://github.com/benbusby/whoogle-search
+Author: Ben Busby
+Author-email: contact@benbusby.com
+License: MIT
+Keywords: search,metasearch,flask,adblock,degoogle,privacy
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+License-File: LICENSE
+
 ![Whoogle Search](docs/banner.png)
 
 [![Latest Release](https://img.shields.io/github/v/release/benbusby/whoogle-search)](https://github.com/benbusby/shoogle/releases)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/benbusby/whoogle-search/actions/workflows/tests.yml/badge.svg)](https://github.com/benbusby/whoogle-search/actions/workflows/tests.yml)
 [![buildx](https://github.com/benbusby/whoogle-search/actions/workflows/buildx.yml/badge.svg)](https://github.com/benbusby/whoogle-search/actions/workflows/buildx.yml)
 [![codebeat badge](https://codebeat.co/badges/e96cada2-fb6f-4528-8285-7d72abd74e8d)](https://codebeat.co/projects/github-com-benbusby-shoogle-master)
@@ -14,25 +31,25 @@
   </tr>
 </table>
 
 Get Google search results, but without any ads, javascript, AMP links, cookies, or IP address tracking. Easily deployable in one click as a Docker app, and customizable with a single config file. Quick and simple to implement as a primary search engine replacement on both desktop and mobile.
 
 Contents
 1. [Features](#features)
-2. [Dependencies](#dependencies)
-3. [Install/Deploy](#install)
-    1. [Heroku Quick Deploy](#a-heroku-quick-deploy)
-    2. [Repl.it](#b-replit)
-    3. [Fly.io](#c-flyio)
-    4. [pipx](#d-pipx)
-    5. [pip](#e-pip)
-    6. [Manual](#f-manual)
-    7. [Docker](#g-manual-docker)
-    8. [Arch/AUR](#arch-linux--arch-based-distributions)
-    9. [Helm/Kubernetes](#helm-chart-for-kubernetes)
+3. [Install/Deploy Options](#install)
+    1. [Heroku Quick Deploy](#heroku-quick-deploy)
+    1. [Repl.it](#replit)
+    1. [Fly.io](#flyio)
+    1. [Koyeb](#koyeb)
+    1. [pipx](#pipx)
+    1. [pip](#pip)
+    1. [Manual](#manual)
+    1. [Docker](#manual-docker)
+    1. [Arch/AUR](#arch-linux--arch-based-distributions)
+    1. [Helm/Kubernetes](#helm-chart-for-kubernetes)
 4. [Environment Variables and Configuration](#environment-variables)
 5. [Usage](#usage)
 6. [Extra Steps](#extra-steps)
     1. [Set Primary Search Engine](#set-whoogle-as-your-primary-search-engine)
     2. [Prevent Downtime (Heroku Only)](#prevent-downtime-heroku-only)
     3. [Manual HTTPS Enforcement](#https-enforcement)
     4. [Using with Firefox Containers](#using-with-firefox-containers)
@@ -64,75 +81,86 @@
 
 <sup>*No third party JavaScript. Whoogle can be used with JavaScript disabled, but if enabled, uses JavaScript for things like presenting search suggestions.</sup>
 
 <sup>**No third party cookies. Whoogle uses server side cookies (sessions) to store non-sensitive configuration settings such as theme, language, etc. Just like with JavaScript, cookies can be disabled and not affect Whoogle's search functionality.</sup>
 
 <sup>***If deployed to a remote server, or configured to send requests through a VPN, Tor, proxy, etc.</sup>
 
-## Dependencies
-If using Heroku Quick Deploy, **you can skip this section**.
-
-- Docker ([Windows](https://docs.docker.com/docker-for-windows/install/), [macOS](https://docs.docker.com/docker-for-mac/install/), [Ubuntu](https://docs.docker.com/engine/install/ubuntu/), [other Linux distros](https://docs.docker.com/engine/install/binaries/))
-  - Only needed if you intend on deploying the app as a Docker image
-- [Python3](https://www.python.org/downloads/)
-- `libcurl4-openssl-dev` and `libssl-dev`
-  - macOS: `brew install openssl curl-openssl`
-  - Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev`
-  - Arch: `pacman -S curl openssl`
-
 ## Install
 There are a few different ways to begin using the app, depending on your preferences:
 
-### A) [Heroku Quick Deploy](https://heroku.com/about)
+___
+
+### [Heroku Quick Deploy](https://heroku.com/about)
 [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/benbusby/whoogle-search/tree/main)
 
 Provides:
 - Easy Deployment of App
 - A HTTPS url (https://\<your app name\>.herokuapp.com)
 
 Notes:
 - Requires a **PAID** Heroku Account.
 - Sometimes has issues with auto-redirecting to `https`. Make sure to navigate to the `https` version of your app before adding as a default search engine.
 
-### B) [Repl.it](https://repl.it)
+___
+
+### [Repl.it](https://repl.it)
 [![Run on Repl.it](https://repl.it/badge/github/benbusby/whoogle-search)](https://repl.it/github/benbusby/whoogle-search)
 
 *Note: Requires a (free) Replit account*
 
 Provides:
 - Free deployment of app
 - Free HTTPS url (https://\<app name\>.\<username\>\.repl\.co)
     - Supports custom domains
 - Downtime after periods of inactivity \([solution 1](https://repl.it/talk/ask/use-this-pingmat1replco-just-enter/28821/101298), [solution 2](https://repl.it/talk/learn/How-to-use-and-setup-UptimeRobot/9003)\)
 
-### C) [Fly.io](https://fly.io)
+___
+
+### [Fly.io](https://fly.io)
 
 You will need a **PAID** [Fly.io](https://fly.io) account to deploy Whoogle.
 
 #### Install the CLI: https://fly.io/docs/hands-on/installing/
 
 #### Deploy the app
 
 ```bash
 flyctl auth login
 flyctl launch --image benbusby/whoogle-search:latest
 ```
 
+The first deploy won't succeed because the default `internal_port` is wrong.
+To fix this, open the generated `fly.toml` file, set `services.internal_port` to `5000` and run `flyctl launch` again.
+
 Your app is now available at `https://<app-name>.fly.dev`.
 
-### D) [pipx](https://github.com/pipxproject/pipx#install-pipx)
+___
+
+### [Koyeb](https://www.koyeb.com)
+
+Use one of the following guides to install Whoogle on Koyeb:
+
+1. Using GitHub: https://www.koyeb.com/docs/quickstart/deploy-with-git
+2. Using Docker: https://www.koyeb.com/docs/quickstart/deploy-a-docker-application
+
+___
+
+### [pipx](https://github.com/pipxproject/pipx#install-pipx)
 Persistent install:
 
 `pipx install git+https://github.com/benbusby/whoogle-search.git`
 
 Sandboxed temporary instance:
 
 `pipx run --spec git+https://github.com/benbusby/whoogle-search.git whoogle-search`
 
-### E) pip
+___
+
+### pip
 `pip install whoogle-search`
 
 ```bash
 $ whoogle-search --help
 usage: whoogle-search [-h] [--port <port number>] [--host <ip address>] [--debug] [--https-only] [--userpass <username:password>]
                       [--proxyauth <username:password>] [--proxytype <socks4|socks5|http>] [--proxyloc <location:port>]
 
@@ -151,18 +179,29 @@
   --proxytype <socks4|socks5|http>
                         Sets a proxy type for all connections (default None)
   --proxyloc <location:port>
                         Sets a proxy location for all connections (default None)
 ```
 See the [available environment variables](#environment-variables) for additional configuration.
 
-### F) Manual
+___
+
+### Manual
 
 *Note: `Content-Security-Policy` headers can be sent by Whoogle if you set `WHOOGLE_CSP`.*
 
+#### Dependencies
+- [Python3](https://www.python.org/downloads/)
+- `libcurl4-openssl-dev` and `libssl-dev`
+  - macOS: `brew install openssl curl-openssl`
+  - Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev`
+  - Arch: `pacman -S curl openssl`
+
+#### Install
+
 Clone the repo and run the following commands to start the app in a local-only environment:
 
 ```bash
 git clone https://github.com/benbusby/whoogle-search.git
 cd whoogle-search
 python3 -m venv venv
 source venv/bin/activate
@@ -188,15 +227,14 @@
 #Environment=WHOOGLE_PROXY_TYPE=<proxy type (http|https|proxy4|proxy5)
 #Environment=WHOOGLE_PROXY_LOC=<proxy host/ip>
 # Site alternative configurations, uncomment to enable
 # Note: If not set, the feature will still be available
 # with default values.
 #Environment=WHOOGLE_ALT_TW=farside.link/nitter
 #Environment=WHOOGLE_ALT_YT=farside.link/invidious
-#Environment=WHOOGLE_ALT_IG=farside.link/bibliogram/u
 #Environment=WHOOGLE_ALT_RD=farside.link/libreddit
 #Environment=WHOOGLE_ALT_MD=farside.link/scribe
 #Environment=WHOOGLE_ALT_TL=farside.link/lingva
 #Environment=WHOOGLE_ALT_IMG=farside.link/rimgo
 #Environment=WHOOGLE_ALT_WIKI=farside.link/wikiless
 #Environment=WHOOGLE_ALT_IMDB=farside.link/libremdb
 #Environment=WHOOGLE_ALT_QUORA=farside.link/quetre
@@ -268,15 +306,17 @@
        - `chmod 400 control.conf`
 
     5. Finally set the Tor environment variable and use password variable to 1, `WHOOGLE_CONFIG_TOR` and `WHOOGLE_TOR_USE_PASS`. Refer to the [Environment Variables](#environment-variables) section for more details.
        - These may be added to the systemd unit file or env file:
           - `WHOOGLE_CONFIG_TOR=1`
           - `WHOOGLE_TOR_USE_PASS=1`
 
-### G) Manual (Docker)
+___
+
+### Manual (Docker)
 1. Ensure the Docker daemon is running, and is accessible by your user account
   - To add user permissions, you can execute `sudo usermod -aG docker yourusername`
   - Running `docker ps` should return something besides an error. If you encounter an error saying the daemon isn't running, try `sudo systemctl start docker` (Linux) or ensure the docker tool is running (Windows/macOS).
 2. Clone and deploy the docker app using a method below:
 
 #### Docker CLI
 
@@ -329,24 +369,30 @@
 heroku container:release web
 heroku open
 ```
 
 This series of commands can take a while, but once you run it once, you shouldn't have to run it again. The final command, `heroku open` will launch a tab in your web browser, where you can test out Whoogle and even [set it as your primary search engine](https://github.com/benbusby/whoogle#set-whoogle-as-your-primary-search-engine).
 You may also edit environment variables from your app’s Settings tab in the Heroku Dashboard.
 
-#### Arch Linux & Arch-based Distributions
+___
+
+### Arch Linux & Arch-based Distributions
 There is an [AUR package available](https://aur.archlinux.org/packages/whoogle-git/), as well as a pre-built and daily updated package available at [Chaotic-AUR](https://chaotic.cx).
 
-#### Helm chart for Kubernetes
+___
+
+### Helm chart for Kubernetes
 To use the Kubernetes Helm Chart:
 1. Ensure you have [Helm](https://helm.sh/docs/intro/install/) `>=3.0.0` installed
 2. Clone this repository
 3. Update [charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired
 4. Run `helm install whoogle ./charts/whoogle`
 
+___
+
 #### Using your own server, or alternative container deployment
 There are other methods for deploying docker containers that are well outlined in [this article](https://rollout.io/blog/the-shortlist-of-docker-hosting/), but there are too many to describe set up for each here. Generally it should be about the same amount of effort as the Heroku deployment.
 
 Depending on your preferences, you can also deploy the app yourself on your own infrastructure. This route would require a few extra steps:
   - A server (I personally recommend [Digital Ocean](https://www.digitalocean.com/pricing/) or [Linode](https://www.linode.com/pricing/), their cheapest tiers will work fine)
   - Your own URL (I suppose this is optional, but recommended)
   - SSL certificates (free through [Let's Encrypt](https://letsencrypt.org/getting-started/))
@@ -369,15 +415,14 @@
 | WHOOGLE_PROXY_PASS   | The password of the proxy server.                                                         |
 | WHOOGLE_PROXY_TYPE   | The type of the proxy server. Can be "socks5", "socks4", or "http".                       |
 | WHOOGLE_PROXY_LOC    | The location of the proxy server (host or ip).                                            |
 | EXPOSE_PORT          | The port where Whoogle will be exposed.                                                   |
 | HTTPS_ONLY           | Enforce HTTPS. (See [here](https://github.com/benbusby/whoogle-search#https-enforcement)) |
 | WHOOGLE_ALT_TW       | The twitter.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_YT       | The youtube.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
-| WHOOGLE_ALT_IG       | The instagram.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_RD       | The reddit.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_TL       | The Google Translate alternative to use. This is used for all "translate ____" searches.  Set to "" to disable. |
 | WHOOGLE_ALT_MD       | The medium.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_IMG      | The imgur.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_WIKI     | The wikipedia.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_IMDB     | The imdb.com alternative to use when site alternatives are enabled in the config. Set to "" to disable.  |
 | WHOOGLE_ALT_QUORA    | The quora.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
@@ -395,14 +440,16 @@
 | Variable                             | Description                                                     |
 | ------------------------------------ | --------------------------------------------------------------- |
 | WHOOGLE_CONFIG_DISABLE               | Hide config from UI and disallow changes to config by client    |
 | WHOOGLE_CONFIG_COUNTRY               | Filter results by hosting country                               |
 | WHOOGLE_CONFIG_LANGUAGE              | Set interface language                                          |
 | WHOOGLE_CONFIG_SEARCH_LANGUAGE       | Set search result language                                      |
 | WHOOGLE_CONFIG_BLOCK                 | Block websites from search results (use comma-separated list)   |
+| WHOOGLE_CONFIG_BLOCK_TITLE           | Block search result with a REGEX filter on title                |
+| WHOOGLE_CONFIG_BLOCK_URL             | Block search result with a REGEX filter on URL                  |
 | WHOOGLE_CONFIG_THEME                 | Set theme mode (light, dark, or system)                         |
 | WHOOGLE_CONFIG_SAFE                  | Enable safe searches                                            |
 | WHOOGLE_CONFIG_ALTS                  | Use social media site alternatives (nitter, invidious, etc)     |
 | WHOOGLE_CONFIG_NEAR                  | Restrict results to only those near a particular city           |
 | WHOOGLE_CONFIG_TOR                   | Use Tor routing (if available)                                  |
 | WHOOGLE_CONFIG_NEW_TAB               | Always open results in new tab                                  |
 | WHOOGLE_CONFIG_VIEW_IMAGE            | Enable View Image option                                        |
@@ -589,29 +636,31 @@
 | [https://search.garudalinux.org](https://search.garudalinux.org) | 🇫🇮 FI | Multi-choice | ✅ |
 | [https://search.dr460nf1r3.org](https://search.dr460nf1r3.org) | 🇩🇪 DE | Multi-choice | ✅ |
 | [https://s.tokhmi.xyz](https://s.tokhmi.xyz) | 🇺🇸 US | Multi-choice | ✅ |
 | [https://search.sethforprivacy.com](https://search.sethforprivacy.com) | 🇩🇪 DE | English | |
 | [https://whoogle.dcs0.hu](https://whoogle.dcs0.hu) | 🇭🇺 HU | Multi-choice | |
 | [https://whoogle.esmailelbob.xyz](https://whoogle.esmailelbob.xyz) | 🇨🇦 CA | Multi-choice | |
 | [https://gowogle.voring.me](https://gowogle.voring.me) | 🇺🇸 US | Multi-choice | |
-| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | 🇺🇸 US | English | |
+| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | 🇳🇱 NL | English | |
 | [https://wg.vern.cc](https://wg.vern.cc) | 🇺🇸 US | English |  |
-| [https://www.indexia.gq](https://www.indexia.gq) | 🇨🇦 CA | Multi-choice | ✅ |
+| [https://whoogle.hxvy0.gq](https://whoogle.hxvy0.gq) | 🇨🇦 CA | Turkish Only | ✅ |
 | [https://whoogle.hostux.net](https://whoogle.hostux.net) | 🇫🇷 FR | Multi-choice | |
+| [https://whoogle.lunar.icu](https://whoogle.lunar.icu) | 🇩🇪 DE | Multi-choice | ✅ |
+| [https://wgl.frail.duckdns.org](https://wgl.frail.duckdns.org) | 🇧🇷 BR | Multi-choice | |
 
 * A checkmark in the "Cloudflare" category here refers to the use of the reverse proxy, [Cloudflare](https://cloudflare.com). The checkmark will not be listed for a site which uses Cloudflare DNS but rather the proxying service which grants Cloudflare the ability to monitor traffic to the website.
 
 #### Onion Instances
 
 | Website | Country | Language |
 |-|-|-|
 | [http://whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion](http://whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion) | 🇺🇸 US |  Multi-choice
 | [http://nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion](http://nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion) | 🇩🇪 DE |  English
 | [http://whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/) | 🇺🇸 US | English |
-| [http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) | 🇺🇸 US | English |
+| [http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) | 🇳🇱 NL | English |
 
 #### I2P Instances
 
 | Website | Country | Language |
 |-|-|-|
 | [http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p](http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p) | 🇺🇸 US | English |
```

#### html2text {}

```diff
@@ -1,120 +1,127 @@
-![Whoogle Search](docs/banner.png) [![Latest Release](https://img.shields.io/
-github/v/release/benbusby/whoogle-search)](https://github.com/benbusby/shoogle/
-releases) [![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT) [![tests](https://github.com/
-benbusby/whoogle-search/actions/workflows/tests.yml/badge.svg)](https://
-github.com/benbusby/whoogle-search/actions/workflows/tests.yml) [![buildx]
-(https://github.com/benbusby/whoogle-search/actions/workflows/buildx.yml/
+Metadata-Version: 2.1 Name: whoogle-search Version: 0.8.2 Summary: Self-hosted,
+ad-free, privacy-respecting metasearch engine Home-page: https://github.com/
+benbusby/whoogle-search Author: Ben Busby Author-email: contact@benbusby.com
+License: MIT Keywords: search,metasearch,flask,adblock,degoogle,privacy
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
+dev License-File: LICENSE ![Whoogle Search](docs/banner.png) [![Latest Release]
+(https://img.shields.io/github/v/release/benbusby/whoogle-search)](https://
+github.com/benbusby/shoogle/releases) [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![tests]
+(https://github.com/benbusby/whoogle-search/actions/workflows/tests.yml/
 badge.svg)](https://github.com/benbusby/whoogle-search/actions/workflows/
-buildx.yml) [![codebeat badge](https://codebeat.co/badges/e96cada2-fb6f-4528-
-8285-7d72abd74e8d)](https://codebeat.co/projects/github-com-benbusby-shoogle-
-master) [![Docker Pulls](https://img.shields.io/docker/pulls/benbusby/whoogle-
-search)](https://hub.docker.com/r/benbusby/whoogle-search)
+tests.yml) [![buildx](https://github.com/benbusby/whoogle-search/actions/
+workflows/buildx.yml/badge.svg)](https://github.com/benbusby/whoogle-search/
+actions/workflows/buildx.yml) [![codebeat badge](https://codebeat.co/badges/
+e96cada2-fb6f-4528-8285-7d72abd74e8d)](https://codebeat.co/projects/github-com-
+benbusby-shoogle-master) [![Docker Pulls](https://img.shields.io/docker/pulls/
+benbusby/whoogle-search)](https://hub.docker.com/r/benbusby/whoogle-search)
 SourceHut GitHub
 Get Google search results, but without any ads, javascript, AMP links, cookies,
 or IP address tracking. Easily deployable in one click as a Docker app, and
 customizable with a single config file. Quick and simple to implement as a
 primary search engine replacement on both desktop and mobile. Contents 1.
-[Features](#features) 2. [Dependencies](#dependencies) 3. [Install/Deploy]
-(#install) 1. [Heroku Quick Deploy](#a-heroku-quick-deploy) 2. [Repl.it](#b-
-replit) 3. [Fly.io](#c-flyio) 4. [pipx](#d-pipx) 5. [pip](#e-pip) 6. [Manual]
-(#f-manual) 7. [Docker](#g-manual-docker) 8. [Arch/AUR](#arch-linux--arch-
-based-distributions) 9. [Helm/Kubernetes](#helm-chart-for-kubernetes) 4.
-[Environment Variables and Configuration](#environment-variables) 5. [Usage]
-(#usage) 6. [Extra Steps](#extra-steps) 1. [Set Primary Search Engine](#set-
-whoogle-as-your-primary-search-engine) 2. [Prevent Downtime (Heroku Only)]
-(#prevent-downtime-heroku-only) 3. [Manual HTTPS Enforcement](#https-
-enforcement) 4. [Using with Firefox Containers](#using-with-firefox-containers)
-5. [Reverse Proxying](#reverse-proxying) 1. [Nginx](#nginx) 7. [Contributing]
-(#contributing) 8. [FAQ](#faq) 9. [Public Instances](#public-instances) 10.
-[Screenshots](#screenshots) ## Features - No ads or sponsored content - No
-JavaScript\* - No cookies\*\* - No tracking/linking of your personal IP
-address\*\*\* - No AMP links - No URL tracking tags (i.e. utm=%s) - No referrer
-header - Tor and HTTP/SOCKS proxy support - Autocomplete/search suggestions -
-POST request search and suggestion queries (when possible) - View images at
-full res without site redirect (currently mobile only) - Light/Dark/System
-theme modes (with support for [custom CSS theming](https://github.com/benbusby/
-whoogle-search/wiki/User-Contributed-CSS-Themes)) - Randomly generated User
-Agent - Easy to install/deploy - DDG-style bang (i.e. `! `) searches - Optional
-location-based searching (i.e. results near \
+[Features](#features) 3. [Install/Deploy Options](#install) 1. [Heroku Quick
+Deploy](#heroku-quick-deploy) 1. [Repl.it](#replit) 1. [Fly.io](#flyio) 1.
+[Koyeb](#koyeb) 1. [pipx](#pipx) 1. [pip](#pip) 1. [Manual](#manual) 1.
+[Docker](#manual-docker) 1. [Arch/AUR](#arch-linux--arch-based-distributions)
+1. [Helm/Kubernetes](#helm-chart-for-kubernetes) 4. [Environment Variables and
+Configuration](#environment-variables) 5. [Usage](#usage) 6. [Extra Steps]
+(#extra-steps) 1. [Set Primary Search Engine](#set-whoogle-as-your-primary-
+search-engine) 2. [Prevent Downtime (Heroku Only)](#prevent-downtime-heroku-
+only) 3. [Manual HTTPS Enforcement](#https-enforcement) 4. [Using with Firefox
+Containers](#using-with-firefox-containers) 5. [Reverse Proxying](#reverse-
+proxying) 1. [Nginx](#nginx) 7. [Contributing](#contributing) 8. [FAQ](#faq) 9.
+[Public Instances](#public-instances) 10. [Screenshots](#screenshots) ##
+Features - No ads or sponsored content - No JavaScript\* - No cookies\*\* - No
+tracking/linking of your personal IP address\*\*\* - No AMP links - No URL
+tracking tags (i.e. utm=%s) - No referrer header - Tor and HTTP/SOCKS proxy
+support - Autocomplete/search suggestions - POST request search and suggestion
+queries (when possible) - View images at full res without site redirect
+(currently mobile only) - Light/Dark/System theme modes (with support for
+[custom CSS theming](https://github.com/benbusby/whoogle-search/wiki/User-
+Contributed-CSS-Themes)) - Randomly generated User Agent - Easy to install/
+deploy - DDG-style bang (i.e. `! `) searches - Optional location-based
+searching (i.e. results near \
 >) - Optional NoJS mode to view search results in a separate window with
 JavaScript blocked *No third party JavaScript. Whoogle can be used with
 JavaScript disabled, but if enabled, uses JavaScript for things like presenting
 search suggestions. **No third party cookies. Whoogle uses server side cookies
 (sessions) to store non-sensitive configuration settings such as theme,
 language, etc. Just like with JavaScript, cookies can be disabled and not
 affect Whoogle's search functionality. ***If deployed to a remote server, or
-configured to send requests through a VPN, Tor, proxy, etc. ## Dependencies If
-using Heroku Quick Deploy, **you can skip this section**. - Docker ([Windows]
-(https://docs.docker.com/docker-for-windows/install/), [macOS](https://
-docs.docker.com/docker-for-mac/install/), [Ubuntu](https://docs.docker.com/
-engine/install/ubuntu/), [other Linux distros](https://docs.docker.com/engine/
-install/binaries/)) - Only needed if you intend on deploying the app as a
-Docker image - [Python3](https://www.python.org/downloads/) - `libcurl4-
-openssl-dev` and `libssl-dev` - macOS: `brew install openssl curl-openssl` -
-Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev` - Arch:
-`pacman -S curl openssl` ## Install There are a few different ways to begin
-using the app, depending on your preferences: ### A) [Heroku Quick Deploy]
-(https://heroku.com/about) [![Deploy](https://www.herokucdn.com/deploy/
-button.svg)](https://heroku.com/deploy?template=https://github.com/benbusby/
-whoogle-search/tree/main) Provides: - Easy Deployment of App - A HTTPS url
-(https://\
+configured to send requests through a VPN, Tor, proxy, etc. ## Install There
+are a few different ways to begin using the app, depending on your preferences:
+___ ### [Heroku Quick Deploy](https://heroku.com/about) [![Deploy](https://
+www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https:
+//github.com/benbusby/whoogle-search/tree/main) Provides: - Easy Deployment of
+App - A HTTPS url (https://\
 >.herokuapp.com) Notes: - Requires a **PAID** Heroku Account. - Sometimes has
 issues with auto-redirecting to `https`. Make sure to navigate to the `https`
-version of your app before adding as a default search engine. ### B) [Repl.it]
+version of your app before adding as a default search engine. ___ ### [Repl.it]
 (https://repl.it) [![Run on Repl.it](https://repl.it/badge/github/benbusby/
 whoogle-search)](https://repl.it/github/benbusby/whoogle-search) *Note:
 Requires a (free) Replit account* Provides: - Free deployment of app - Free
 HTTPS url (https://\
 >.\
 >\.repl\.co) - Supports custom domains - Downtime after periods of inactivity \
 ([solution 1](https://repl.it/talk/ask/use-this-pingmat1replco-just-enter/
 28821/101298), [solution 2](https://repl.it/talk/learn/How-to-use-and-setup-
-UptimeRobot/9003)\) ### C) [Fly.io](https://fly.io) You will need a **PAID**
+UptimeRobot/9003)\) ___ ### [Fly.io](https://fly.io) You will need a **PAID**
 [Fly.io](https://fly.io) account to deploy Whoogle. #### Install the CLI:
 https://fly.io/docs/hands-on/installing/ #### Deploy the app ```bash flyctl
-auth login flyctl launch --image benbusby/whoogle-search:latest ``` Your app is
-now available at `https://.fly.dev`. ### D) [pipx](https://github.com/
-pipxproject/pipx#install-pipx) Persistent install: `pipx install git+https://
-github.com/benbusby/whoogle-search.git` Sandboxed temporary instance: `pipx run
---spec git+https://github.com/benbusby/whoogle-search.git whoogle-search` ###
-E) pip `pip install whoogle-search` ```bash $ whoogle-search --help usage:
-whoogle-search [-h] [--port ] [--host ] [--debug] [--https-only] [--userpass ]
-[--proxyauth ] [--proxytype
+auth login flyctl launch --image benbusby/whoogle-search:latest ``` The first
+deploy won't succeed because the default `internal_port` is wrong. To fix this,
+open the generated `fly.toml` file, set `services.internal_port` to `5000` and
+run `flyctl launch` again. Your app is now available at `https://.fly.dev`. ___
+### [Koyeb](https://www.koyeb.com) Use one of the following guides to install
+Whoogle on Koyeb: 1. Using GitHub: https://www.koyeb.com/docs/quickstart/
+deploy-with-git 2. Using Docker: https://www.koyeb.com/docs/quickstart/deploy-
+a-docker-application ___ ### [pipx](https://github.com/pipxproject/
+pipx#install-pipx) Persistent install: `pipx install git+https://github.com/
+benbusby/whoogle-search.git` Sandboxed temporary instance: `pipx run --spec
+git+https://github.com/benbusby/whoogle-search.git whoogle-search` ___ ### pip
+`pip install whoogle-search` ```bash $ whoogle-search --help usage: whoogle-
+search [-h] [--port ] [--host ] [--debug] [--https-only] [--userpass ] [--
+proxyauth ] [--proxytype
 socks5|http>] [--proxyloc ] Whoogle Search console runner optional arguments: -
 h, --help Show this help message and exit --port  Specifies a port to run on
 (default 5000) --host  Specifies the host address to use (default 127.0.0.1) --
 debug Activates debug mode for the server (default False) --https-only Enforces
 HTTPS redirects for all requests --userpass  Sets a username/password basic
 auth combo (default None) --proxyauth  Sets a username/password for a HTTP/
 SOCKS proxy (default None) --proxytype
 socks5|http> Sets a proxy type for all connections (default None) --proxyloc
 Sets a proxy location for all connections (default None) ``` See the [available
 environment variables](#environment-variables) for additional configuration.
-### F) Manual *Note: `Content-Security-Policy` headers can be sent by Whoogle
-if you set `WHOOGLE_CSP`.* Clone the repo and run the following commands to
-start the app in a local-only environment: ```bash git clone https://
-github.com/benbusby/whoogle-search.git cd whoogle-search python3 -m venv venv
-source venv/bin/activate pip install -r requirements.txt ./run ``` See the
-[available environment variables](#environment-variables) for additional
-configuration. #### systemd Configuration After building the virtual
-environment, you can add something like the following to `/lib/systemd/system/
-whoogle.service` to set up a Whoogle Search systemd service: ```ini [Unit]
-Description=Whoogle [Service] # Basic auth configuration, uncomment to enable
-#Environment=WHOOGLE_USER= #Environment=WHOOGLE_PASS= # Proxy configuration,
-uncomment to enable #Environment=WHOOGLE_PROXY_USER=
-#Environment=WHOOGLE_PROXY_PASS= #Environment=WHOOGLE_PROXY_TYPE=
+___ ### Manual *Note: `Content-Security-Policy` headers can be sent by Whoogle
+if you set `WHOOGLE_CSP`.* #### Dependencies - [Python3](https://
+www.python.org/downloads/) - `libcurl4-openssl-dev` and `libssl-dev` - macOS:
+`brew install openssl curl-openssl` - Ubuntu: `sudo apt-get install -
+y libcurl4-openssl-dev libssl-dev` - Arch: `pacman -S curl openssl` ####
+Install Clone the repo and run the following commands to start the app in a
+local-only environment: ```bash git clone https://github.com/benbusby/whoogle-
+search.git cd whoogle-search python3 -m venv venv source venv/bin/activate pip
+install -r requirements.txt ./run ``` See the [available environment variables]
+(#environment-variables) for additional configuration. #### systemd
+Configuration After building the virtual environment, you can add something
+like the following to `/lib/systemd/system/whoogle.service` to set up a Whoogle
+Search systemd service: ```ini [Unit] Description=Whoogle [Service] # Basic
+auth configuration, uncomment to enable #Environment=WHOOGLE_USER=
+#Environment=WHOOGLE_PASS= # Proxy configuration, uncomment to enable
+#Environment=WHOOGLE_PROXY_USER= #Environment=WHOOGLE_PROXY_PASS=
+#Environment=WHOOGLE_PROXY_TYPE=
 http|https|proxy4|proxy5) #Environment=WHOOGLE_PROXY_LOC=
 p> # Site alternative configurations, uncomment to enable # Note: If not set,
 the feature will still be available # with default values.
 #Environment=WHOOGLE_ALT_TW=farside.link/nitter
 #Environment=WHOOGLE_ALT_YT=farside.link/invidious
-#Environment=WHOOGLE_ALT_IG=farside.link/bibliogram/
-u #Environment=WHOOGLE_ALT_RD=farside.link/libreddit
+#Environment=WHOOGLE_ALT_RD=farside.link/libreddit
 #Environment=WHOOGLE_ALT_MD=farside.link/scribe
 #Environment=WHOOGLE_ALT_TL=farside.link/lingva
 #Environment=WHOOGLE_ALT_IMG=farside.link/rimgo
 #Environment=WHOOGLE_ALT_WIKI=farside.link/wikiless
 #Environment=WHOOGLE_ALT_IMDB=farside.link/libremdb
 #Environment=WHOOGLE_ALT_QUORA=farside.link/quetre # Load values from dotenv
 only #Environment=WHOOGLE_DOTENV=1 Type=simple User= # If installed as a
@@ -152,15 +159,15 @@
 the `WHOOGLE_TOR_CONF` environment variable. Refer to the [Environment
 Variables](#environment-variables) section for more details. 4. Heavily
 restrict access to control.conf to only be readable by the user running
 whoogle: - `chmod 400 control.conf` 5. Finally set the Tor environment variable
 and use password variable to 1, `WHOOGLE_CONFIG_TOR` and
 `WHOOGLE_TOR_USE_PASS`. Refer to the [Environment Variables](#environment-
 variables) section for more details. - These may be added to the systemd unit
-file or env file: - `WHOOGLE_CONFIG_TOR=1` - `WHOOGLE_TOR_USE_PASS=1` ### G)
+file or env file: - `WHOOGLE_CONFIG_TOR=1` - `WHOOGLE_TOR_USE_PASS=1` ___ ###
 Manual (Docker) 1. Ensure the Docker daemon is running, and is accessible by
 your user account - To add user permissions, you can execute `sudo usermod -aG
 docker yourusername` - Running `docker ps` should return something besides an
 error. If you encounter an error saying the daemon isn't running, try `sudo
 systemctl start docker` (Linux) or ensure the docker tool is running (Windows/
 macOS). 2. Clone and deploy the docker app using a method below: #### Docker
 CLI Through Docker Hub: ```bash docker pull benbusby/whoogle-search docker run
@@ -181,22 +188,22 @@
 https://github.com/benbusby/whoogle-search.git cd whoogle-search heroku create
 heroku container:push web heroku container:release web heroku open ``` This
 series of commands can take a while, but once you run it once, you shouldn't
 have to run it again. The final command, `heroku open` will launch a tab in
 your web browser, where you can test out Whoogle and even [set it as your
 primary search engine](https://github.com/benbusby/whoogle#set-whoogle-as-your-
 primary-search-engine). You may also edit environment variables from your
-appâs Settings tab in the Heroku Dashboard. #### Arch Linux & Arch-based
+appâs Settings tab in the Heroku Dashboard. ___ ### Arch Linux & Arch-based
 Distributions There is an [AUR package available](https://aur.archlinux.org/
 packages/whoogle-git/), as well as a pre-built and daily updated package
-available at [Chaotic-AUR](https://chaotic.cx). #### Helm chart for Kubernetes
-To use the Kubernetes Helm Chart: 1. Ensure you have [Helm](https://helm.sh/
-docs/intro/install/) `>=3.0.0` installed 2. Clone this repository 3. Update
-[charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired 4. Run
-`helm install whoogle ./charts/whoogle` #### Using your own server, or
+available at [Chaotic-AUR](https://chaotic.cx). ___ ### Helm chart for
+Kubernetes To use the Kubernetes Helm Chart: 1. Ensure you have [Helm](https://
+helm.sh/docs/intro/install/) `>=3.0.0` installed 2. Clone this repository 3.
+Update [charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired 4.
+Run `helm install whoogle ./charts/whoogle` ___ #### Using your own server, or
 alternative container deployment There are other methods for deploying docker
 containers that are well outlined in [this article](https://rollout.io/blog/
 the-shortlist-of-docker-hosting/), but there are too many to describe set up
 for each here. Generally it should be about the same amount of effort as the
 Heroku deployment. Depending on your preferences, you can also deploy the app
 yourself on your own infrastructure. This route would require a few extra
 steps: - A server (I personally recommend [Digital Ocean](https://
@@ -221,23 +228,21 @@
 proxy server. Can be "socks5", "socks4", or "http". | | WHOOGLE_PROXY_LOC | The
 location of the proxy server (host or ip). | | EXPOSE_PORT | The port where
 Whoogle will be exposed. | | HTTPS_ONLY | Enforce HTTPS. (See [here](https://
 github.com/benbusby/whoogle-search#https-enforcement)) | | WHOOGLE_ALT_TW | The
 twitter.com alternative to use when site alternatives are enabled in the
 config. Set to "" to disable. | | WHOOGLE_ALT_YT | The youtube.com alternative
 to use when site alternatives are enabled in the config. Set to "" to disable.
-| | WHOOGLE_ALT_IG | The instagram.com alternative to use when site
-alternatives are enabled in the config. Set to "" to disable. | |
-WHOOGLE_ALT_RD | The reddit.com alternative to use when site alternatives are
-enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_TL | The Google
-Translate alternative to use. This is used for all "translate ____" searches.
-Set to "" to disable. | | WHOOGLE_ALT_MD | The medium.com alternative to use
-when site alternatives are enabled in the config. Set to "" to disable. | |
-WHOOGLE_ALT_IMG | The imgur.com alternative to use when site alternatives are
-enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_WIKI | The
+| | WHOOGLE_ALT_RD | The reddit.com alternative to use when site alternatives
+are enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_TL | The
+Google Translate alternative to use. This is used for all "translate ____"
+searches. Set to "" to disable. | | WHOOGLE_ALT_MD | The medium.com alternative
+to use when site alternatives are enabled in the config. Set to "" to disable.
+| | WHOOGLE_ALT_IMG | The imgur.com alternative to use when site alternatives
+are enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_WIKI | The
 wikipedia.com alternative to use when site alternatives are enabled in the
 config. Set to "" to disable. | | WHOOGLE_ALT_IMDB | The imdb.com alternative
 to use when site alternatives are enabled in the config. Set to "" to disable.
 | | WHOOGLE_ALT_QUORA | The quora.com alternative to use when site alternatives
 are enabled in the config. Set to "" to disable. | | WHOOGLE_AUTOCOMPLETE |
 Controls visibility of autocomplete/search suggestions. Default on -- use '0'
 to disable. | | WHOOGLE_MINIMAL | Remove everything except basic result cards
@@ -254,15 +259,17 @@
 instance to the same config state every time. | Variable | Description | | ----
 -------------------------------- | --------------------------------------------
 ------------------- | | WHOOGLE_CONFIG_DISABLE | Hide config from UI and
 disallow changes to config by client | | WHOOGLE_CONFIG_COUNTRY | Filter
 results by hosting country | | WHOOGLE_CONFIG_LANGUAGE | Set interface language
 | | WHOOGLE_CONFIG_SEARCH_LANGUAGE | Set search result language | |
 WHOOGLE_CONFIG_BLOCK | Block websites from search results (use comma-separated
-list) | | WHOOGLE_CONFIG_THEME | Set theme mode (light, dark, or system) | |
+list) | | WHOOGLE_CONFIG_BLOCK_TITLE | Block search result with a REGEX filter
+on title | | WHOOGLE_CONFIG_BLOCK_URL | Block search result with a REGEX filter
+on URL | | WHOOGLE_CONFIG_THEME | Set theme mode (light, dark, or system) | |
 WHOOGLE_CONFIG_SAFE | Enable safe searches | | WHOOGLE_CONFIG_ALTS | Use social
 media site alternatives (nitter, invidious, etc) | | WHOOGLE_CONFIG_NEAR |
 Restrict results to only those near a particular city | | WHOOGLE_CONFIG_TOR |
 Use Tor routing (if available) | | WHOOGLE_CONFIG_NEW_TAB | Always open results
 in new tab | | WHOOGLE_CONFIG_VIEW_IMAGE | Enable View Image option | |
 WHOOGLE_CONFIG_GET_ONLY | Search using GET requests only | | WHOOGLE_CONFIG_URL
 | The root url of the instance (`https:///`) | | WHOOGLE_CONFIG_STYLE | The
@@ -422,34 +429,37 @@
 search.dr460nf1r3.org) | ð©ðª DE | Multi-choice | â | | [https://
 s.tokhmi.xyz](https://s.tokhmi.xyz) | ðºð¸ US | Multi-choice | â | |
 [https://search.sethforprivacy.com](https://search.sethforprivacy.com) |
 ð©ðª DE | English | | | [https://whoogle.dcs0.hu](https://whoogle.dcs0.hu)
 | ð­ðº HU | Multi-choice | | | [https://whoogle.esmailelbob.xyz](https://
 whoogle.esmailelbob.xyz) | ð¨ð¦ CA | Multi-choice | | | [https://
 gowogle.voring.me](https://gowogle.voring.me) | ðºð¸ US | Multi-choice | |
-| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | ðºð¸
-US | English | | | [https://wg.vern.cc](https://wg.vern.cc) | ðºð¸ US |
-English | | | [https://www.indexia.gq](https://www.indexia.gq) | ð¨ð¦ CA |
-Multi-choice | â | | [https://whoogle.hostux.net](https://whoogle.hostux.net)
-|Â ð«ð· FR | Multi-choice | | * A checkmark in the "Cloudflare" category
-here refers to the use of the reverse proxy, [Cloudflare](https://
-cloudflare.com). The checkmark will not be listed for a site which uses
-Cloudflare DNS but rather the proxying service which grants Cloudflare the
-ability to monitor traffic to the website. #### Onion Instances | Website |
-Country | Language | |-|-|-| | [http://
+| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | ð³ð±
+NL | English | | | [https://wg.vern.cc](https://wg.vern.cc) | ðºð¸ US |
+English | | | [https://whoogle.hxvy0.gq](https://whoogle.hxvy0.gq) | ð¨ð¦
+CA | Turkish Only | â | | [https://whoogle.hostux.net](https://
+whoogle.hostux.net) |Â ð«ð· FR | Multi-choice | | | [https://
+whoogle.lunar.icu](https://whoogle.lunar.icu) | ð©ðª DE | Multi-choice |
+â | | [https://wgl.frail.duckdns.org](https://wgl.frail.duckdns.org) |
+ð§ð· BR | Multi-choice | | * A checkmark in the "Cloudflare" category here
+refers to the use of the reverse proxy, [Cloudflare](https://cloudflare.com).
+The checkmark will not be listed for a site which uses Cloudflare DNS but
+rather the proxying service which grants Cloudflare the ability to monitor
+traffic to the website. #### Onion Instances | Website | Country | Language |
+|-|-|-| | [http://
 whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion](http://
 whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion) | ðºð¸ US |
 Multi-choice | [http://
 nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion](http://
 nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion) | ð©ðª DE |
 English | [http://
 whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://
 whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/) |
 ðºð¸ US | English | | [http://
 whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://
 whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) |
-ðºð¸ US | English | #### I2P Instances | Website | Country | Language | |-
+ð³ð± NL | English | #### I2P Instances | Website | Country | Language | |-
 |-|-| | [http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p]
 (http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p) |
 ðºð¸ US | English | ## Screenshots #### Desktop ![Whoogle Desktop](docs/
 screenshot_desktop.png) #### Mobile ![Whoogle Mobile](docs/
 screenshot_mobile.png)
```

### Comparing `whoogle-search-0.8.1/app/__init__.py` & `whoogle-search-0.8.2/app/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from app.filter import clean_query
 from app.request import send_tor_signal
 from app.utils.session import generate_key
 from app.utils.bangs import gen_bangs_json
 from app.utils.misc import gen_file_hash, read_config_bool
 from base64 import b64encode
+from bs4 import MarkupResemblesLocatorWarning
 from datetime import datetime, timedelta
+from dotenv import load_dotenv
 from flask import Flask
 import json
 import logging.config
 import os
 from stem import Signal
 import threading
-from dotenv import load_dotenv
+import warnings
 
 from werkzeug.middleware.proxy_fix import ProxyFix
 
 from app.utils.misc import read_config_bool
 from app.version import __version__
 
 app = Flask(__name__, static_folder=os.path.dirname(
@@ -24,15 +26,15 @@
 app.wsgi_app = ProxyFix(app.wsgi_app)
 
 dot_env_path = (
     os.path.join(os.path.dirname(os.path.abspath(__file__)),
     '../whoogle.env'))
 
 # Load .env file if enabled
-if read_config_bool('WHOOGLE_DOTENV'):
+if os.path.exists(dot_env_path):
     load_dotenv(dot_env_path)
 
 app.enc_key = generate_key()
 
 if read_config_bool('HTTPS_ONLY'):
     app.config['SESSION_COOKIE_NAME'] = '__Secure-session'
     app.config['SESSION_COOKIE_SECURE'] = True
@@ -49,14 +51,17 @@
 app.config['CACHE_BUSTING_MAP'] = {}
 app.config['LANGUAGES'] = json.load(open(
     os.path.join(app.config['STATIC_FOLDER'], 'settings/languages.json'),
     encoding='utf-8'))
 app.config['COUNTRIES'] = json.load(open(
     os.path.join(app.config['STATIC_FOLDER'], 'settings/countries.json'),
     encoding='utf-8'))
+app.config['TIME_PERIODS'] = json.load(open(
+    os.path.join(app.config['STATIC_FOLDER'], 'settings/time_periods.json'),
+    encoding='utf-8'))
 app.config['TRANSLATIONS'] = json.load(open(
     os.path.join(app.config['STATIC_FOLDER'], 'settings/translations.json'),
     encoding='utf-8'))
 app.config['THEMES'] = json.load(open(
     os.path.join(app.config['STATIC_FOLDER'], 'settings/themes.json'),
     encoding='utf-8'))
 app.config['HEADER_TABS'] = json.load(open(
@@ -167,14 +172,17 @@
 app.jinja_env.globals.update(clean_query=clean_query)
 app.jinja_env.globals.update(
     cb_url=lambda f: app.config['CACHE_BUSTING_MAP'][f])
 
 # Attempt to acquire tor identity, to determine if Tor config is available
 send_tor_signal(Signal.HEARTBEAT)
 
+# Suppress spurious warnings from BeautifulSoup
+warnings.simplefilter('ignore', MarkupResemblesLocatorWarning)
+
 from app import routes  # noqa
 
 # Disable logging from imported modules
 logging.config.dictConfig({
     'version': 1,
     'disable_existing_loggers': True,
 })
```

### Comparing `whoogle-search-0.8.1/app/filter.py` & `whoogle-search-0.8.2/app/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,16 @@
 
         # Update default footer and header
         footer = self.soup.find('footer')
         if footer:
             # Remove divs that have multiple links beyond just page navigation
             [_.decompose() for _ in footer.find_all('div', recursive=False)
              if len(_.find_all('a', href=True)) > 3]
+            for link in footer.find_all('a', href=True):
+                link['href'] = f'{link["href"]}&preferences={self.config.preferences}'
 
         header = self.soup.find('header')
         if header:
             header.decompose()
         self.remove_site_blocks(self.soup)
         return self.soup
 
@@ -219,24 +221,24 @@
             div_ads = [_ for _ in div.find_all('span', recursive=True)
                        if has_ad_content(_.text)]
             _ = div.decompose() if len(div_ads) else None
 
     def remove_block_titles(self) -> None:
         if not self.main_divs or not self.config.block_title:
             return
-        block_title = re.compile(self.block_title)
+        block_title = re.compile(self.config.block_title)
         for div in [_ for _ in self.main_divs.find_all('div', recursive=True)]:
             block_divs = [_ for _ in div.find_all('h3', recursive=True)
                           if block_title.search(_.text) is not None]
             _ = div.decompose() if len(block_divs) else None
 
     def remove_block_url(self) -> None:
         if not self.main_divs or not self.config.block_url:
             return
-        block_url = re.compile(self.block_url)
+        block_url = re.compile(self.config.block_url)
         for div in [_ for _ in self.main_divs.find_all('div', recursive=True)]:
             block_divs = [_ for _ in div.find_all('a', recursive=True)
                           if block_url.search(_.attrs['href']) is not None]
             _ = div.decompose() if len(block_divs) else None
 
     def remove_block_tabs(self) -> None:
         if self.main_divs:
@@ -455,15 +457,15 @@
         else:
             link_netloc = parsed_link.netloc
 
         # Remove any elements that direct to unsupported Google pages
         if any(url in link_netloc for url in unsupported_g_pages):
             # FIXME: The "Shopping" tab requires further filtering (see #136)
             # Temporarily removing all links to that tab for now.
-            
+
             # Replaces the /url google unsupported link to the direct url
             link['href'] = link_netloc
             parent = link.parent
 
             if 'google.com/preferences?hl=' in link_netloc:
                 # Handle case where a search is performed in a different
                 # language than what is configured. This usually returns a
@@ -584,18 +586,17 @@
                 link_str = str(link_desc)
 
                 # Medium links should be handled differently, since 'medium.com'
                 # is a common substring of domain names, but shouldn't be
                 # replaced (i.e. 'philomedium.com' should stay as it is).
                 if 'medium.com' in link_str:
                     if link_str.startswith('medium.com') or '.medium.com' in link_str:
-                        new_desc.string = link_str.replace(
-                            'medium.com', 'farside.link/scribe')
-                    else:
-                        new_desc.string = link_str
+                        link_str = 'farside.link/scribe' + link_str[
+                            link_str.find('medium.com') + len('medium.com'):]
+                    new_desc.string = link_str
                 else:
                     new_desc.string = link_str.replace(site, alt)
 
                 link_desc.replace_with(new_desc)
 
     def view_image(self, soup) -> BeautifulSoup:
         """Replaces the soup with a new one that handles mobile results and
@@ -606,21 +607,23 @@
 
         Returns:
             BeautifulSoup: The new BeautifulSoup object
         """
 
         # get some tags that are unchanged between mobile and pc versions
         cor_suggested = soup.find_all('table', attrs={'class': "By0U9"})
-        next_pages = soup.find_all('table', attrs={'class': "uZgmoc"})[0]
+        next_pages = soup.find('table', attrs={'class': "uZgmoc"})
 
         results = []
         # find results div
-        results_div = soup.find_all('div', attrs={'class': "nQvrDb"})[0]
-        # find all the results
-        results_all = results_div.find_all('div', attrs={'class': "lIMUZd"})
+        results_div = soup.find('div', attrs={'class': "nQvrDb"})
+        # find all the results (if any)
+        results_all = []
+        if results_div:
+            results_all = results_div.find_all('div', attrs={'class': "lIMUZd"})
 
         for item in results_all:
             urls = item.find('a')['href'].split('&imgrefurl=')
 
             # Skip urls that are not two-element lists
             if len(urls) != 2:
                 continue
```

### Comparing `whoogle-search-0.8.1/app/models/config.py` & `whoogle-search-0.8.2/app/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             'WHOOGLE_CONFIG_STYLE',
             open(os.path.join(app_config['STATIC_FOLDER'],
                               'css/variables.css')).read())
         self.block = os.getenv('WHOOGLE_CONFIG_BLOCK', '')
         self.block_title = os.getenv('WHOOGLE_CONFIG_BLOCK_TITLE', '')
         self.block_url = os.getenv('WHOOGLE_CONFIG_BLOCK_URL', '')
         self.country = os.getenv('WHOOGLE_CONFIG_COUNTRY', '')
+        self.tbs = os.getenv('WHOOGLE_CONFIG_TIME_PERIOD', '')
         self.theme = os.getenv('WHOOGLE_CONFIG_THEME', 'system')
         self.safe = read_config_bool('WHOOGLE_CONFIG_SAFE')
         self.dark = read_config_bool('WHOOGLE_CONFIG_DARK')  # deprecated
         self.alts = read_config_bool('WHOOGLE_CONFIG_ALTS')
         self.nojs = read_config_bool('WHOOGLE_CONFIG_NOJS')
         self.tor = read_config_bool('WHOOGLE_CONFIG_TOR')
         self.near = os.getenv('WHOOGLE_CONFIG_NEAR', '')
@@ -48,15 +49,16 @@
             'alts',
             'new_tab',
             'view_image',
             'block',
             'safe',
             'nojs',
             'anon_view',
-            'preferences_encrypted'
+            'preferences_encrypted',
+            'tbs'
         ]
 
         # Skip setting custom config if there isn't one
         if kwargs:
             mutable_attrs = self.get_mutable_attrs()
             for attr in mutable_attrs:
                 if attr in kwargs.keys():
```

### Comparing `whoogle-search-0.8.1/app/models/g_classes.py` & `whoogle-search-0.8.2/app/models/g_classes.py`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/request.py` & `whoogle-search-0.8.2/app/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 
     # Use :past(hour/day/week/month/year) if available
     # example search "new restaurants :past month"
     lang = ''
     if ':past' in query and 'tbs' not in args:
         time_range = str.strip(query.split(':past', 1)[-1])
         param_dict['tbs'] = '&tbs=' + ('qdr:' + str.lower(time_range[0]))
-    elif 'tbs' in args:
-        result_tbs = args.get('tbs')
+    elif 'tbs' in args or 'tbs' in config:
+        result_tbs = args.get('tbs') if 'tbs' in args else config['tbs']
         param_dict['tbs'] = '&tbs=' + result_tbs
 
         # Occasionally the 'tbs' param provided by google also contains a
         # field for 'lr', but formatted strangely. This is a rough solution
         # for this.
         #
         # Example:
```

### Comparing `whoogle-search-0.8.1/app/routes.py` & `whoogle-search-0.8.2/app/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from app.models.endpoint import Endpoint
 from app.request import Request, TorError
 from app.utils.bangs import resolve_bang
 from app.utils.misc import get_proxy_host_url
 from app.filter import Filter
 from app.utils.misc import read_config_bool, get_client_ip, get_request_url, \
     check_for_update
-from app.utils.results import add_ip_card, bold_search_terms,\
+from app.utils.widgets import *
+from app.utils.results import bold_search_terms,\
     add_currency_card, check_currency, get_tabs_content
 from app.utils.search import Search, needs_https, has_captcha
 from app.utils.session import valid_user_session
 from bs4 import BeautifulSoup as bsoup
 from flask import jsonify, make_response, request, redirect, render_template, \
     send_file, session, url_for, g
 from requests import exceptions
@@ -43,23 +44,32 @@
         if tab['tbm'] == tbm:
             return tab['name']
 
 
 def auth_required(f):
     @wraps(f)
     def decorated(*args, **kwargs):
+        # do not ask password if cookies already present
+        if (
+            valid_user_session(session)
+            and 'cookies_disabled' not in request.args
+            and session['auth']
+        ):
+            return f(*args, **kwargs)
+
         auth = request.authorization
 
         # Skip if username/password not set
         whoogle_user = os.getenv('WHOOGLE_USER', '')
         whoogle_pass = os.getenv('WHOOGLE_PASS', '')
         if (not whoogle_user or not whoogle_pass) or (
                 auth
                 and whoogle_user == auth.username
                 and whoogle_pass == auth.password):
+            session['auth'] = True
             return f(*args, **kwargs)
         else:
             return make_response('Not logged in', 401, {
                 'WWW-Authenticate': 'Basic realm="Login Required"'})
 
     return decorated
 
@@ -135,14 +145,15 @@
         if os.path.exists(app.config['DEFAULT_CONFIG']) else {}
 
     # Generate session values for user if unavailable
     if not valid_user_session(session):
         session['config'] = default_config
         session['uuid'] = str(uuid.uuid4())
         session['key'] = app.enc_key
+        session['auth'] = False
 
     # Establish config values per user session
     g.user_config = Config(**session['config'])
 
     # Update user config if specified in search args
     g.user_config = g.user_config.from_params(g.request_params)
 
@@ -201,14 +212,15 @@
         session['error_message'] = ''
         return render_template('error.html', error_message=error_message)
 
     return render_template('index.html',
                            has_update=app.config['HAS_UPDATE'],
                            languages=app.config['LANGUAGES'],
                            countries=app.config['COUNTRIES'],
+                           time_periods=app.config['TIME_PERIODS'],
                            themes=app.config['THEMES'],
                            autocomplete_enabled=autocomplete_enabled,
                            translation=app.config['TRANSLATIONS'][
                                g.user_config.get_localization_lang()
                            ],
                            logo=render_template(
                                'logo.html',
@@ -235,16 +247,15 @@
         'User-Agent')
 
     return render_template(
         'opensearch.xml',
         main_url=opensearch_url,
         request_type='' if get_only else 'method="post"',
         search_type=request.args.get('tbm'),
-        search_name=get_search_name(request.args.get('tbm')),
-        preferences=g.user_config.preferences
+        search_name=get_search_name(request.args.get('tbm'))
     ), 200, {'Content-Type': 'application/xml'}
 
 
 @app.route(f'/{Endpoint.search_html}', methods=['GET'])
 def search_html():
     search_url = g.app_location
     if search_url.endswith('/'):
@@ -279,15 +290,14 @@
     # Note: If Tor is enabled, this returns nothing, as the request is
     # almost always rejected
     return jsonify([
         q,
         g.user_request.autocomplete(q) if not g.user_config.tor else []
     ])
 
-
 @app.route(f'/{Endpoint.search}', methods=['GET', 'POST'])
 @session_required
 @auth_required
 def search():
     search_util = Search(request, g.user_config, g.session_key)
     query = search_util.new_search_query()
 
@@ -314,47 +324,62 @@
 
     # If the user is attempting to translate a string, determine the correct
     # string for formatting the lingva.ml url
     localization_lang = g.user_config.get_localization_lang()
     translation = app.config['TRANSLATIONS'][localization_lang]
     translate_to = localization_lang.replace('lang_', '')
 
+    # removing st-card to only use whoogle time selector
+    soup = bsoup(response, "html.parser");
+    for x in soup.find_all(attrs={"id": "st-card"}):
+        x.replace_with("")
+
+    response = str(soup)
+
     # Return 503 if temporarily blocked by captcha
     if has_captcha(str(response)):
+        app.logger.error('503 (CAPTCHA)')
         return render_template(
             'error.html',
             blocked=True,
             error_message=translation['ratelimit'],
             translation=translation,
             farside='https://farside.link',
             config=g.user_config,
             query=urlparse.unquote(query),
             params=g.user_config.to_params(keys=['preferences'])), 503
+
     response = bold_search_terms(response, query)
 
-    # Feature to display IP address
-    if search_util.check_kw_ip():
+    # check for widgets and add if requested
+    if search_util.widget != '':
         html_soup = bsoup(str(response), 'html.parser')
-        response = add_ip_card(html_soup, get_client_ip(request))
+        if search_util.widget == 'ip':
+            response = add_ip_card(html_soup, get_client_ip(request))
+        elif search_util.widget == 'calculator' and not 'nojs' in request.args:
+            response = add_calculator_card(html_soup)
 
     # Update tabs content
     tabs = get_tabs_content(app.config['HEADER_TABS'],
                             search_util.full_query,
                             search_util.search_type,
                             g.user_config.preferences,
                             translation)
 
     # Feature to display currency_card
+    # Since this is determined by more than just the
+    # query is it not defined as a standard widget
     conversion = check_currency(str(response))
     if conversion:
         html_soup = bsoup(str(response), 'html.parser')
         response = add_currency_card(html_soup, conversion)
 
     preferences = g.user_config.preferences
     home_url = f"home?preferences={preferences}" if preferences else "home"
+    cleanresponse = str(response).replace("andlt;","&lt;").replace("andgt;","&gt;")
 
     return render_template(
         'display.html',
         has_update=app.config['HAS_UPDATE'],
         query=urlparse.unquote(query),
         search_type=search_util.search_type,
         search_name=get_search_name(search_util.search_type),
@@ -367,28 +392,29 @@
             'translate', ''
         ).replace(
             translation['translate'], ''
         ),
         is_translation=any(
             _ in query.lower() for _ in [translation['translate'], 'translate']
         ) and not search_util.search_type,  # Standard search queries only
-        response=response,
+        response=cleanresponse,
         version_number=app.config['VERSION_NUMBER'],
         search_header=render_template(
             'header.html',
             home_url=home_url,
             config=g.user_config,
             translation=translation,
             languages=app.config['LANGUAGES'],
             countries=app.config['COUNTRIES'],
+            time_periods=app.config['TIME_PERIODS'],
             logo=render_template('logo.html', dark=g.user_config.dark),
             query=urlparse.unquote(query),
             search_type=search_util.search_type,
             mobile=g.user_request.mobile,
-            tabs=tabs))
+            tabs=tabs)).replace("  ", "")
 
 
 @app.route(f'/{Endpoint.config}', methods=['GET', 'POST', 'PUT'])
 @session_required
 @auth_required
 def config():
     config_disabled = (
@@ -527,14 +553,19 @@
         response=results,
         translation=app.config['TRANSLATIONS'][
             g.user_config.get_localization_lang()
         ]
     )
 
 
+@app.errorhandler(404)
+def page_not_found(e):
+    return render_template('error.html', error_message=str(e)), 404
+
+
 def run_app() -> None:
     parser = argparse.ArgumentParser(
         description='Whoogle Search console runner')
     parser.add_argument(
         '--port',
         default=5000,
         metavar='<port number>',
```

### Comparing `whoogle-search-0.8.1/app/static/css/dark-theme.css` & `whoogle-search-0.8.2/app/static/css/dark-theme.css`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/css/header.css` & `whoogle-search-0.8.2/app/static/css/header.css`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/css/input.css` & `whoogle-search-0.8.2/app/static/css/input.css`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/css/light-theme.css` & `whoogle-search-0.8.2/app/static/css/light-theme.css`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/css/main.css` & `whoogle-search-0.8.2/app/static/css/main.css`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/css/search.css` & `whoogle-search-0.8.2/app/static/css/search.css`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/css/variables.css` & `whoogle-search-0.8.2/app/static/css/variables.css`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/android-icon-144x144.png` & `whoogle-search-0.8.2/app/static/img/favicon/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/android-icon-192x192.png` & `whoogle-search-0.8.2/app/static/img/favicon/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/android-icon-36x36.png` & `whoogle-search-0.8.2/app/static/img/favicon/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/android-icon-48x48.png` & `whoogle-search-0.8.2/app/static/img/favicon/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/android-icon-72x72.png` & `whoogle-search-0.8.2/app/static/img/favicon/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/android-icon-96x96.png` & `whoogle-search-0.8.2/app/static/img/favicon/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-114x114.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-120x120.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-144x144.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-152x152.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-180x180.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-57x57.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-60x60.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-72x72.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-76x76.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon-precomposed.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/apple-icon.png` & `whoogle-search-0.8.2/app/static/img/favicon/apple-icon.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/favicon-16x16.png` & `whoogle-search-0.8.2/app/static/img/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/favicon-32x32.png` & `whoogle-search-0.8.2/app/static/img/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/favicon-96x96.png` & `whoogle-search-0.8.2/app/static/img/favicon/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/favicon.ico` & `whoogle-search-0.8.2/app/static/img/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/manifest.json` & `whoogle-search-0.8.2/app/static/img/favicon/manifest.json`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/ms-icon-144x144.png` & `whoogle-search-0.8.2/app/static/img/favicon/ms-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/ms-icon-150x150.png` & `whoogle-search-0.8.2/app/static/img/favicon/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/ms-icon-310x310.png` & `whoogle-search-0.8.2/app/static/img/favicon/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon/ms-icon-70x70.png` & `whoogle-search-0.8.2/app/static/img/favicon/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/favicon.ico` & `whoogle-search-0.8.2/app/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/logo.png` & `whoogle-search-0.8.2/app/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/img/whoogle.svg` & `whoogle-search-0.8.2/app/static/img/whoogle.svg`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/js/autocomplete.js` & `whoogle-search-0.8.2/app/static/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/js/controller.js` & `whoogle-search-0.8.2/app/static/js/controller.js`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/js/header.js` & `whoogle-search-0.8.2/app/static/js/header.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,46 @@
 document.addEventListener("DOMContentLoaded", () => {
     const advSearchToggle = document.getElementById("adv-search-toggle");
     const advSearchDiv = document.getElementById("adv-search-div");
     const searchBar = document.getElementById("search-bar");
     const countrySelect = document.getElementById("result-country");
+    const timePeriodSelect = document.getElementById("result-time-period");
     const arrowKeys = [37, 38, 39, 40];
     let searchValue = searchBar.value;
 
     countrySelect.onchange = () => {
         let str = window.location.href;
         n = str.lastIndexOf("/search");
         if (n > 0) {
-            str = str.substring(0, n) +
-                `/search?q=${searchBar.value}&country=${countrySelect.value}`;
+            str = str.substring(0, n) + `/search?q=${searchBar.value}`;
+            str = tackOnParams(str);
             window.location.href = str;
         }
     }
 
+    timePeriodSelect.onchange = () => {
+        let str = window.location.href;
+        n = str.lastIndexOf("/search");
+        if (n > 0) {
+            str = str.substring(0, n) + `/search?q=${searchBar.value}`;
+            str = tackOnParams(str);
+            window.location.href = str;
+        }
+    }
+
+    function tackOnParams(str) {
+        if (timePeriodSelect.value != "") {
+            str = str + `&tbs=${timePeriodSelect.value}`;
+        }
+        if (countrySelect.value != "") {
+            str = str + `&country=${countrySelect.value}`;
+        }
+        return str;
+    }
+
     const toggleAdvancedSearch = on => {
         if (on) {
             advSearchDiv.style.maxHeight = "70px";
         } else {
             advSearchDiv.style.maxHeight = "0px";
         }
         localStorage.advSearchToggled = on;
```

### Comparing `whoogle-search-0.8.1/app/static/js/keyboard.js` & `whoogle-search-0.8.2/app/static/js/keyboard.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -52,11 +52,15 @@
             block: 'center',
             inline: 'nearest'
         });
         results[activeIdx].focus();
     }
 
     function focusSearch() {
+        if (window.usingCalculator) {
+            // if this function exists, it means the calculator widget has been displayed
+            if (usingCalculator()) return;
+        }
         activeIdx = -1;
         searchBar.focus();
     }
 }());
```

### Comparing `whoogle-search-0.8.1/app/static/js/utils.js` & `whoogle-search-0.8.2/app/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/settings/countries.json` & `whoogle-search-0.8.2/app/static/settings/countries.json`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/settings/header_tabs.json` & `whoogle-search-0.8.2/app/static/settings/header_tabs.json`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/static/settings/languages.json` & `whoogle-search-0.8.2/app/static/settings/languages.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9811320754716981%*

 * *Differences: {'insert': "[(5, OrderedDict([('name', 'Azerbaijani (Azərbaycanca)'), ('value', 'lang_az')]))]"}*

```diff
@@ -16,14 +16,18 @@
         "value": "lang_ar"
     },
     {
         "name": "Armenian (\u0570\u0561\u0575\u0565\u0580\u0565\u0576)",
         "value": "lang_hy"
     },
     {
+        "name": "Azerbaijani (Az\u0259rbaycanca)",
+        "value": "lang_az"
+    },
+    {
         "name": "Belarusian (\u0411\u0435\u043b\u0430\u0440\u0443\u0441\u043a\u0430\u044f)",
         "value": "lang_be"
     },
     {
         "name": "Bulgarian (\u0431\u044a\u043b\u0433\u0430\u0440\u0441\u043a\u0438)",
         "value": "lang_bg"
     },
```

### Comparing `whoogle-search-0.8.1/app/static/settings/translations.json` & `whoogle-search-0.8.2/app/static/settings/translations.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8095813204508858%*

 * *Differences: {"'lang_az'": "OrderedDict([('', '--'), ('search', 'Axtar'), ('config', 'Konfiqurasiya'), "*

 * *              "('config-country', 'Ölkə'), ('config-lang', 'İnterfeys dili'), "*

 * *              "('config-lang-search', 'Axtarış dili'), ('config-near', 'Yaxın'), "*

 * *              "('config-near-help', 'Şəhər Adı'), ('config-block', 'Blok'), ('config-block-help', "*

 * *              "'Vergüllə ayrılmış sayt siyahısı'), ('config-block-title', 'Başlığa görə "*

 * *              "bloklayın'), ('config-block-title-help', 'Regex isti […]*

```diff
@@ -1,16 +1,73 @@
 {
+    "lang_az": {
+        "": "--",
+        "all": "Ham\u0131s\u0131",
+        "anon-view": "Anonim Bax\u0131\u015f",
+        "apply": "T\u0259tbiq edin",
+        "books": "Kitablar",
+        "config": "Konfiqurasiya",
+        "config-alts": "Sosial Media Linkl\u0259rini d\u0259yi\u015fdirin",
+        "config-alts-help": "Twitter/YouTube/s. linkl\u0259ri alternativl\u0259r\u0259 uy\u011fun m\u0259xfilikl\u0259 \u0259v\u0259z edir.",
+        "config-anon-view": "Anonim Bax\u0131\u015f Linkl\u0259rini g\u00f6st\u0259rin",
+        "config-block": "Blok",
+        "config-block-help": "Verg\u00fcll\u0259 ayr\u0131lm\u0131\u015f sayt siyah\u0131s\u0131",
+        "config-block-title": "Ba\u015fl\u0131\u011fa g\u00f6r\u0259 bloklay\u0131n",
+        "config-block-title-help": "Regex istifad\u0259 edin",
+        "config-block-url": "URL il\u0259 bloklay\u0131n",
+        "config-block-url-help": "Regex istifad\u0259 edin",
+        "config-country": "\u00d6lk\u0259",
+        "config-css": "F\u0259rdi CSS",
+        "config-dark": "Qaranl\u0131q rejim",
+        "config-get-only": "Yaln\u0131z GET Sor\u011fular\u0131",
+        "config-images": "Tam \u00f6l\u00e7\u00fcl\u00fc \u015e\u0259kil Axtar\u0131\u015f\u0131",
+        "config-images-help": "(Eksperimental) Masa\u00fcst\u00fc \u015f\u0259kil axtar\u0131\u015flar\u0131na '\u015e\u0259kil\u0259 Bax' se\u00e7imini \u0259lav\u0259 edir. Bu, \u015f\u0259kil n\u0259tic\u0259si miniat\u00fcrl\u0259rinin daha a\u015fa\u011f\u0131 ay\u0131rdetm\u0259 keyfiyy\u0259tin\u0259 s\u0259b\u0259b olacaq.",
+        "config-lang": "\u0130nterfeys dili",
+        "config-lang-search": "Axtar\u0131\u015f dili",
+        "config-near": "Yax\u0131n",
+        "config-near-help": "\u015e\u0259h\u0259r Ad\u0131",
+        "config-new-tab": "Linkl\u0259ri Yeni Tabda a\u00e7\u0131n",
+        "config-nojs": "Anonim G\u00f6r\u00fcn\u00fc\u015fd\u0259 Javascript-i silin",
+        "config-pref-encryption": "Encrypt T\u0259rcihl\u0259ri",
+        "config-pref-help": "WHOOGLE_CONFIG_PREFERENCES_KEY t\u0259l\u0259b edir, \u0259ks halda bu n\u0259z\u0259r\u0259 al\u0131nmayacaq.",
+        "config-pref-url": "URL T\u0259rcihl\u0259ri",
+        "config-safe": "T\u0259hl\u00fck\u0259siz axtar\u0131\u015f",
+        "config-theme": "M\u00f6vzu",
+        "config-time-period": "M\u00fcdd\u0259t",
+        "config-tor": "Tor-dan istifad\u0259 edin",
+        "config-url": "K\u00f6k URL",
+        "continue-search": "Axtar\u0131\u015f\u0131n\u0131z\u0131 Farside il\u0259 davam etdirin",
+        "dark": "qaranl\u0131q",
+        "github-link": "GitHub-da bax\u0131n",
+        "images": "\u015e\u0259kill\u0259r",
+        "light": "i\u015f\u0131ql\u0131",
+        "load": "Y\u00fckl\u0259",
+        "maps": "X\u0259rit\u0259l\u0259r",
+        "news": "X\u0259b\u0259rl\u0259r",
+        "qdr:d": "Ke\u00e7\u0259n 24 saat",
+        "qdr:h": "Ke\u00e7\u0259n saat",
+        "qdr:m": "Ke\u00e7\u0259n ay",
+        "qdr:w": "Ke\u00e7\u0259n h\u0259ft\u0259",
+        "qdr:y": "Ke\u00e7\u0259n il",
+        "ratelimit": "N\u00fcmun\u0259 d\u0259r\u0259c\u0259si m\u0259hdudla\u015fd\u0131r\u0131l\u0131b",
+        "save-as": "F\u0259rqli Saxla...",
+        "search": "Axtar",
+        "system": "sistem",
+        "translate": "t\u0259rc\u00fcm\u0259",
+        "videos": "Videolar"
+    },
     "lang_bg": {
+        "": "--",
         "all": "\u0412\u0441\u0438\u0447\u043ao",
         "anon-view": "\u0410\u043d\u043e\u043d\u0438\u043c\u0435\u043d \u0438\u0437\u0433\u043b\u0435\u0434",
         "apply": "\u041f\u0440\u0438\u043b\u043e\u0436\u0438",
         "books": "\u041a\u043d\u0438\u0433\u0438",
         "config": "\u041a\u043e\u043d\u0444\u0438\u0433\u0443\u0440\u0430\u0446\u0438\u044f",
         "config-alts": "\u0417\u0430\u043c\u0435\u043d\u0435\u0442\u0435 \u0432\u0440\u044a\u0437\u043a\u0438\u0442\u0435 \u043a\u044a\u043c \u0441\u043e\u0446\u0438\u0430\u043b\u043d\u0438\u0442\u0435 \u043c\u0435\u0434\u0438\u0438",
-        "config-alts-help": "\u0417\u0430\u043c\u0435\u043d\u044f \u0432\u0440\u044a\u0437\u043a\u0438\u0442\u0435 \u043d\u0430 Twitter/YouTube/Instagram \u0438 \u0442.\u043d. \u0441 \u0437\u0430\u0449\u0438\u0442\u0435\u043d\u0438 \u0430\u043b\u0442\u0435\u0440\u043d\u0430\u0442\u0438\u0432\u043d\u0438 \u043f\u043e\u0432\u0435\u0440\u0438\u0442\u0435\u043b\u043d\u0438 \u0432\u0440\u044a\u0437\u043a\u0438.",
+        "config-alts-help": "\u0417\u0430\u043c\u0435\u043d\u044f \u0432\u0440\u044a\u0437\u043a\u0438\u0442\u0435 \u043d\u0430 Twitter/YouTube \u0438 \u0442.\u043d. \u0441 \u0437\u0430\u0449\u0438\u0442\u0435\u043d\u0438 \u0430\u043b\u0442\u0435\u0440\u043d\u0430\u0442\u0438\u0432\u043d\u0438 \u043f\u043e\u0432\u0435\u0440\u0438\u0442\u0435\u043b\u043d\u0438 \u0432\u0440\u044a\u0437\u043a\u0438.",
         "config-anon-view": "\u041f\u043e\u043a\u0430\u0437\u0432\u0430\u043d\u0435 \u043d\u0430 \u0430\u043d\u043e\u043d\u0438\u043c\u043d\u0438 \u0432\u0440\u044a\u0437\u043a\u0438 \u0437\u0430 \u043f\u0440\u0435\u0433\u043b\u0435\u0434",
         "config-block": "\u0411\u043b\u043e\u043a\u0438\u0440\u0430\u043d\u0438 \u0441\u0430\u0439\u0442\u043e\u0432\u0435",
         "config-block-help": "\u0421\u043f\u0438\u0441\u044a\u043a \u0441\u0430\u0439\u0442\u043e\u0432\u0435, \u0440\u0430\u0437\u0434\u0435\u043b\u0435\u043d\u0438 \u0441\u044a\u0441 \u0437\u0430\u043f\u0435\u0442\u0430\u044f",
         "config-block-title": "\u0411\u043b\u043e\u043a\u0438\u0440\u0430\u043d\u0435 \u043f\u043e \u0437\u0430\u0433\u043b\u0430\u0432\u0438\u0435",
         "config-block-title-help": "\u0418\u0437\u043f\u043e\u043b\u0437\u0432\u0430\u0439\u0442\u0435 \u0440\u0435\u0433\u0443\u043b\u044f\u0440\u043d\u043e \u0438\u0437\u0440\u0430\u0436\u0435\u043d\u0438\u0435",
         "config-block-url": "\u0411\u043b\u043e\u043a\u0438\u0440\u0430\u043d\u0435 \u043f\u043e url",
         "config-block-url-help": "\u0418\u0437\u043f\u043e\u043b\u0437\u0432\u0430\u0439\u0442\u0435 \u0440\u0435\u0433\u0443\u043b\u044f\u0440\u043d\u043e \u0438\u0437\u0440\u0430\u0436\u0435\u043d\u0438\u0435",
@@ -27,39 +84,46 @@
         "config-new-tab": "\u041e\u0442\u0432\u0430\u0440\u044f\u043d\u0435 \u043d\u0430 \u0432\u0440\u044a\u0437\u043a\u0438\u0442\u0435 \u0432 \u043d\u043e\u0432 \u0440\u0430\u0437\u0434\u0435\u043b",
         "config-nojs": "\u041f\u0440\u0435\u043c\u0430\u0445\u043d\u0435\u0442\u0435 Javascript \u0432 \u0430\u043d\u043e\u043d\u0438\u043c\u0435\u043d \u0438\u0437\u0433\u043b\u0435\u0434",
         "config-pref-encryption": "\u0428\u0438\u0444\u0440\u043e\u0432\u0430\u043d\u0435 \u043d\u0430 \u043f\u0440\u0435\u0434\u043f\u043e\u0447\u0438\u0442\u0430\u043d\u0438\u044f\u0442\u0430",
         "config-pref-help": "\u0418\u0437\u0438\u0441\u043a\u0432\u0430 WHOOGLE_CONFIG_PREFERENCES_KEY, \u0432 \u043f\u0440\u043e\u0442\u0438\u0432\u0435\u043d \u0441\u043b\u0443\u0447\u0430\u0439 \u0442\u043e\u0432\u0430 \u0449\u0435 \u0431\u044a\u0434\u0435 \u0438\u0433\u043d\u043e\u0440\u0438\u0440\u0430\u043d\u043e.",
         "config-pref-url": "URL \u0430\u0434\u0440\u0435\u0441 \u043d\u0430 \u043f\u0440\u0435\u0434\u043f\u043e\u0447\u0438\u0442\u0430\u043d\u0438\u044f\u0442\u0430",
         "config-safe": "\u0411\u0435\u0437\u043e\u043f\u0430\u0441\u043d\u043e \u0442\u044a\u0440\u0441\u0435\u043d\u0435",
         "config-theme": "\u0421\u0442\u0438\u043b",
+        "config-time-period": "\u0412\u0440\u0435\u043c\u0435\u0432\u0438 \u043f\u0435\u0440\u0438\u043e\u0434",
         "config-tor": "\u0418\u0437\u043f\u043e\u043b\u0437\u0432\u0430\u0439\u0442\u0435 Tor",
         "config-url": "\u041e\u0441\u043d\u043e\u0432\u0435\u043d URL \u0430\u0434\u0440\u0435\u0441",
         "continue-search": "\u041f\u0440\u043e\u0434\u044a\u043b\u0436\u0435\u0442\u0435 \u0442\u044a\u0440\u0441\u0435\u043d\u0435\u0442\u043e \u0441\u0438 \u0441 Farside",
         "dark": "\u0442\u044a\u043c\u043d\u0430",
         "github-link": "\u0412\u0438\u0436\u0442\u0435 \u0432 GitHub",
         "images": "\u0418\u0437\u043e\u0431\u0440\u0430\u0436\u0435\u043d\u0438\u044f",
         "light": "\u0441\u0432\u0435\u0442\u043b\u0430",
         "load": "\u0417\u0430\u0440\u0435\u0434\u0438",
         "maps": "\u0412\u0438\u0434\u0435\u043e\u043a\u043b\u0438\u043f\u043e\u0432\u0435",
         "news": "\u041a\u0430\u0440\u0442\u0438",
+        "qdr:d": "\u041f\u043e\u0441\u043b\u0435\u0434\u043d\u0438\u0442\u0435 24 \u0447\u0430\u0441\u0430",
+        "qdr:h": "\u041f\u043e\u0441\u043b\u0435\u0434\u043d\u0438\u044f \u0447\u0430\u0441",
+        "qdr:m": "\u041c\u0438\u043d\u0430\u043b\u0438\u044f \u043c\u0435\u0441\u0435\u0446",
+        "qdr:w": "\u041c\u0438\u043d\u0430\u043b\u0430\u0442\u0430 \u0441\u0435\u0434\u043c\u0438\u0446\u0430",
+        "qdr:y": "\u0418\u0437\u043c\u0438\u043d\u0430\u043b\u0430\u0442\u0430 \u0433\u043e\u0434\u0438\u043d\u0430",
         "ratelimit": "\u0415\u043a\u0437\u0435\u043c\u043f\u043b\u044f\u0440\u044a\u0442 \u0435 \u0441 \u043e\u0433\u0440\u0430\u043d\u0438\u0447\u0435\u043d\u0430 \u0441\u043a\u043e\u0440\u043e\u0441\u0442",
         "save-as": "\u0417\u0430\u043f\u0438\u0441 \u043a\u0430\u0442\u043e...",
         "search": "\u0422\u044a\u0440\u0441\u0435\u043d\u0435",
         "system": "\u0441\u0438\u0441\u0442\u0435\u043c\u043d\u0430",
         "translate": "\u043f\u0440\u0435\u0432\u043e\u0434",
         "videos": "\u041d\u043e\u0432\u0438\u043d\u0438"
     },
     "lang_cs": {
+        "": "--",
         "all": "V\u0161e",
         "anon-view": "Anonymn\u00ed pohled",
         "apply": "Pou\u017e\u00edt",
         "books": "Knihy",
         "config": "Konfigurace",
         "config-alts": "Nahradit odkazy na soci\u00e1ln\u00ed m\u00e9dia",
-        "config-alts-help": "Nahrad\u00ed odkazy na Twitter, YouTube, Instagram atd. alternativami respektuj\u00edc\u00edmi soukrom\u00ed.",
+        "config-alts-help": "Nahrad\u00ed odkazy na Twitter, YouTube, atd. alternativami respektuj\u00edc\u00edmi soukrom\u00ed.",
         "config-anon-view": "Zobrazit odkazy anonymn\u00edho zobrazen\u00ed",
         "config-block": "Blokovat",
         "config-block-help": "\u010c\u00e1rkami odd\u011blen\u00fd seznam str\u00e1nek",
         "config-block-title": "Blokovat podle n\u00e1zvu",
         "config-block-title-help": "Pou\u017eijte regul\u00e1rn\u00ed v\u00fdraz",
         "config-block-url": "Blokovat podle adresy URL",
         "config-block-url-help": "Pou\u017eijte regul\u00e1rn\u00ed v\u00fdraz",
@@ -76,39 +140,46 @@
         "config-new-tab": "Otev\u00edrat odkazy na nov\u00e9m listu",
         "config-nojs": "Odeberte Javascript v anonymn\u00edm zobrazen\u00ed",
         "config-pref-encryption": "P\u0159edvolby \u0161ifrov\u00e1n\u00ed",
         "config-pref-help": "Vy\u017eaduje WHOOGLE_CONFIG_PREFERENCES_KEY, jinak bude ignorov\u00e1na.",
         "config-pref-url": "Adresa URL p\u0159edvoleb",
         "config-safe": "Bezpe\u010dn\u00e9 vyhled\u00e1v\u00e1n\u00ed",
         "config-theme": "Motiv",
+        "config-time-period": "\u010casov\u00fd \u00fasek",
         "config-tor": "Pou\u017e\u00edvat Tor",
         "config-url": "Ko\u0159enov\u00e1 adresa URL",
         "continue-search": "Pokra\u010dujte ve vyhled\u00e1v\u00e1n\u00ed pomoc\u00ed Farside",
         "dark": "Tmav\u00fd",
         "github-link": "Zobrazit na GitHub",
         "images": "Obr\u00e1zky",
         "light": "Sv\u011btl\u00fd",
         "load": "Na\u010d\u00edst",
         "maps": "Mapy",
         "news": "Zpr\u00e1vy",
+        "qdr:d": "Posledn\u00edch 24 hodin",
+        "qdr:h": "Posledn\u00ed hodina",
+        "qdr:m": "Minul\u00fd m\u011bs\u00edc",
+        "qdr:w": "Minul\u00fd t\u00fdden",
+        "qdr:y": "Minul\u00fd rok",
         "ratelimit": "Instance byla omezena sazbou",
         "save-as": "Ulo\u017eit jako...",
         "search": "Hledat",
         "system": "Syst\u00e9mov\u00fd",
         "translate": "P\u0159elo\u017eit",
         "videos": "Videa"
     },
     "lang_cy": {
+        "": "--",
         "all": "Holl",
         "anon-view": "Golwg Anhysbys",
         "apply": "Cymhwyswch",
         "books": "Llyfrau",
         "config": "Cyfluniad",
         "config-alts": "Disodli Cysylltau Cyfryngau Cymdeithasol",
-        "config-alts-help": "Yn Amnewid Cysylltau Twitter/YouTube/Instagram/etc gyda Gwefanau Preifatrwydd.",
+        "config-alts-help": "Yn Amnewid Cysylltau Twitter/YouTube/etc gyda Gwefanau Preifatrwydd.",
         "config-anon-view": "Dangos Cysylltau Golwg Anhysbys",
         "config-block": "Blociwch",
         "config-block-help": "Rhestr Gwahanu Comma o Wefannau",
         "config-block-title": "Blocio yn \u00f4l teitl",
         "config-block-title-help": "Defnyddio regex",
         "config-block-url": "Blocio yn \u00f4l URL",
         "config-block-url-help": "Defnyddio regex",
@@ -125,39 +196,46 @@
         "config-new-tab": "Agor Cysylltau mewn Tab Newydd",
         "config-nojs": "Dileu Javascript mewn Golwg Anhysbys",
         "config-pref-encryption": "Cyfluniad Amgryptio",
         "config-pref-help": "Yn angen WHOOGLE_CONFIG_PREFERENCES_KEY, neu bydd hyn yn cael ei anwybyddu.",
         "config-pref-url": "URL am Dewisiadau",
         "config-safe": "Chwilio'n Ddiogel",
         "config-theme": "Thema",
+        "config-time-period": "Cyfnod Amser",
         "config-tor": "Defnyddiwch Tor",
         "config-url": "URL am Gwraidd",
         "continue-search": "Parhau eich chwiliad gyda Farside",
         "dark": "tywyll",
         "github-link": "Gweld ar GitHub",
         "images": "Delweddau",
         "light": "golau",
         "load": "Llwythwch",
         "maps": "Mapiau",
         "news": "Newyddion",
+        "qdr:d": "24 awr diwethaf",
+        "qdr:h": "Yr awr ddiwethaf",
+        "qdr:m": "Mis diwethaf",
+        "qdr:w": "Yr wythnos ddiwethaf",
+        "qdr:y": "Y flwyddyn ddiwethaf",
         "ratelimit": "Whoogle wedi bod yn gyfyngedig",
         "save-as": "Cadw Fel...",
         "search": "Chwiliwch",
         "system": "system",
         "translate": "cyfieithu",
         "videos": "Fideos"
     },
     "lang_de": {
+        "": "--",
         "all": "Alle",
         "anon-view": "Anonyme Ansicht",
         "apply": "\u00dcbernehmen",
         "books": "B\u00fccher",
         "config": "Einstellungen",
         "config-alts": "Social-Media-Links ersetzen",
-        "config-alts-help": "Ersetzt Twitter/YouTube/Instagram/etc Links mit Alternativen, welche die Privatsph\u00e4re respektieren.",
+        "config-alts-help": "Ersetzt Twitter/YouTube/etc Links mit Alternativen, welche die Privatsph\u00e4re respektieren.",
         "config-anon-view": "Anonyme Ansichtslinks anzeigen",
         "config-block": "Block",
         "config-block-help": "Komma-getrennte Liste von Seiten",
         "config-block-title": "Nach Titel blockieren",
         "config-block-title-help": "Regex verwenden",
         "config-block-url": "Nach URL blockieren",
         "config-block-url-help": "Regex verwenden",
@@ -174,39 +252,102 @@
         "config-new-tab": "Links in neuen Tabs \u00f6ffnen",
         "config-nojs": "Entfernen Sie Javascript in der anonymen Ansicht",
         "config-pref-encryption": "Einstellungen verschl\u00fcsseln",
         "config-pref-help": "Erfordert WHOOGLE_CONFIG_PREFERENCES_KEY, sonst wird dies ignoriert.",
         "config-pref-url": "Einstellungs URL",
         "config-safe": "Sicheres Suchen",
         "config-theme": "Thema",
+        "config-time-period": "Zeitraum",
         "config-tor": "Tor benutzen",
         "config-url": "Root URL",
         "continue-search": "Setzen Sie Ihre Suche fort mit Farside",
         "dark": "dunkel",
         "github-link": "Auf GitHub \u00f6ffnen",
         "images": "Bilder",
         "light": "hell",
         "load": "Laden",
         "maps": "Maps",
         "news": "Nachrichten",
+        "qdr:d": "Vergangene 24 Stunden",
+        "qdr:h": "Letzte Stunde",
+        "qdr:m": "Letzten Monat",
+        "qdr:w": "Letzte Woche",
+        "qdr:y": "Vergangenes Jahr",
         "ratelimit": "Instanz wurde ratenbegrenzt",
         "save-as": "Speichern unter...",
         "search": "Suchen",
         "system": "Systemeinstellung",
         "translate": "\u00dcbersetzen",
         "videos": "Videos"
     },
+    "lang_el": {
+        "": "--",
+        "all": "All",
+        "anon-view": "\u0391\u03bd\u03ce\u03bd\u03c5\u03bc\u03b7 \u03a0\u03c1\u03bf\u03b2\u03bf\u03bb\u03ae",
+        "apply": "Apply",
+        "books": "Books",
+        "config": "\u03a1\u03c5\u03b8\u03bc\u03ae\u03c3\u03b5\u03b9\u03c2",
+        "config-alts": "Replace Social Media Links",
+        "config-alts-help": "Replaces Twitter/YouTube/etc links with privacy respecting alternatives.",
+        "config-anon-view": "Show Anonymous View Links",
+        "config-block": "Block",
+        "config-block-help": "Comma-separated site list",
+        "config-block-title": "Block by Title",
+        "config-block-title-help": "Use regex",
+        "config-block-url": "Block by URL",
+        "config-block-url-help": "Use regex",
+        "config-country": "\u03a7\u03ce\u03c1\u03b1",
+        "config-css": "Custom CSS",
+        "config-dark": "Dark Mode",
+        "config-get-only": "GET Requests Only",
+        "config-images": "Full Size Image Search",
+        "config-images-help": "(Experimental) Adds the 'View Image' option to desktop image searches. This will cause image result thumbnails to be lower resolution.",
+        "config-lang": "\u0393\u03bb\u03ce\u03c3\u03c3\u03b1 \u03a0\u03b5\u03c1\u03b9\u03b2\u03ac\u03bb\u03bb\u03bf\u03bd\u03c4\u03bf\u03c2",
+        "config-lang-search": "\u0393\u03bb\u03ce\u03c3\u03c3\u03b1 \u0391\u03bd\u03b1\u03b6\u03ae\u03c4\u03b7\u03c3\u03b7\u03c2",
+        "config-near": "\u039a\u03bf\u03bd\u03c4\u03ac",
+        "config-near-help": "\u038c\u03bd\u03bf\u03bc\u03b1 \u03a0\u03cc\u03bb\u03b7\u03c2",
+        "config-new-tab": "\u0386\u03bd\u03bf\u03b9\u03b3\u03bc\u03b1 \u03c3\u03c5\u03bd\u03b4\u03ad\u03c3\u03bc\u03bf\u03c5 \u03c3\u03b5 \u03bd\u03ad\u03b1 \u03ba\u03b1\u03c1\u03c4\u03ad\u03bb\u03b1",
+        "config-nojs": "\u0391\u03c6\u03b1\u03af\u03c1\u03b5\u03c3\u03b7 Javascript \u03c3\u03b5 \u03b1\u03bd\u03ce\u03bd\u03c5\u03bc\u03b7 \u03c0\u03c1\u03bf\u03b2\u03bf\u03bb\u03ae",
+        "config-pref-encryption": "Encrypt Preferences",
+        "config-pref-help": "Requires WHOOGLE_CONFIG_PREFERENCES_KEY, otherwise this will be ignored.",
+        "config-pref-url": "Preferences URL",
+        "config-safe": "\u0391\u03c3\u03c6\u03b1\u03bb\u03ae\u03c2 \u0391\u03bd\u03b1\u03b6\u03ae\u03c4\u03b7\u03c3\u03b7",
+        "config-theme": "\u0398\u03ad\u03bc\u03b1",
+        "config-time-period": "Time Period",
+        "config-tor": "\u03a7\u03c1\u03ae\u03c3\u03b7 Tor",
+        "config-url": "Root URL",
+        "continue-search": "Continue your search with Farside",
+        "dark": "dark",
+        "github-link": "View on GitHub",
+        "images": "Images",
+        "light": "light",
+        "load": "Load",
+        "maps": "Maps",
+        "news": "News",
+        "qdr:d": "\u03a4\u03b5\u03bb\u03b5\u03c5\u03c4\u03b1\u03af\u03b5\u03c2 24 \u03ce\u03c1\u03b5\u03c2",
+        "qdr:h": "\u03a4\u03b5\u03bb\u03b5\u03c5\u03c4\u03b1\u03af\u03b1 \u03ce\u03c1\u03b1",
+        "qdr:m": "\u03a4\u03b5\u03bb\u03b5\u03c5\u03c4\u03b1\u03af\u03bf\u03c2 \u039c\u03ae\u03bd\u03b1\u03c2",
+        "qdr:w": "\u03a4\u03b5\u03bb\u03b5\u03c5\u03c4\u03b1\u03af\u03b1 \u0392\u03b4\u03bf\u03bc\u03ac\u03b4\u03b1",
+        "qdr:y": "\u03a4\u03b5\u03bb\u03b5\u03c5\u03c4\u03b1\u03af\u03bf\u03c2 \u03a7\u03c1\u03cc\u03bd\u03bf\u03c2",
+        "ratelimit": "Instance has been ratelimited",
+        "save-as": "Save As...",
+        "search": "\u0391\u03bd\u03b1\u03b6\u03ae\u03c4\u03b7\u03c3\u03b7",
+        "system": "system",
+        "translate": "translate",
+        "videos": "Videos"
+    },
     "lang_en": {
+        "": "--",
         "all": "All",
         "anon-view": "Anonymous View",
         "apply": "Apply",
         "books": "Books",
         "config": "Configuration",
         "config-alts": "Replace Social Media Links",
-        "config-alts-help": "Replaces Twitter/YouTube/Instagram/etc links with privacy respecting alternatives.",
+        "config-alts-help": "Replaces Twitter/YouTube/etc links with privacy respecting alternatives.",
         "config-anon-view": "Show Anonymous View Links",
         "config-block": "Block",
         "config-block-help": "Comma-separated site list",
         "config-block-title": "Block by Title",
         "config-block-title-help": "Use regex",
         "config-block-url": "Block by URL",
         "config-block-url-help": "Use regex",
@@ -223,39 +364,46 @@
         "config-new-tab": "Open Links in New Tab",
         "config-nojs": "Remove Javascript in Anonymous View",
         "config-pref-encryption": "Encrypt Preferences",
         "config-pref-help": "Requires WHOOGLE_CONFIG_PREFERENCES_KEY, otherwise this will be ignored.",
         "config-pref-url": "Preferences URL",
         "config-safe": "Safe Search",
         "config-theme": "Theme",
+        "config-time-period": "Time Period",
         "config-tor": "Use Tor",
         "config-url": "Root URL",
         "continue-search": "Continue your search with Farside",
         "dark": "dark",
         "github-link": "View on GitHub",
         "images": "Images",
         "light": "light",
         "load": "Load",
         "maps": "Maps",
         "news": "News",
+        "qdr:d": "Past 24 hours",
+        "qdr:h": "Past hour",
+        "qdr:m": "Past month",
+        "qdr:w": "Past week",
+        "qdr:y": "Past year",
         "ratelimit": "Instance has been ratelimited",
         "save-as": "Save As...",
         "search": "Search",
         "system": "system",
         "translate": "translate",
         "videos": "Videos"
     },
     "lang_es": {
+        "": "--",
         "all": "Todo",
         "anon-view": "Vista An\u00f3nima",
         "apply": "Aplicar",
         "books": "Libros",
         "config": "Configuraci\u00f3n",
         "config-alts": "Reemplazar Enlaces de Redes Sociales",
-        "config-alts-help": "Reemplaza los enlaces de Twitter/YouTube/Instagram/etc con alternativas que respetan la privacidad.",
+        "config-alts-help": "Reemplaza los enlaces de Twitter/YouTube/etc con alternativas que respetan la privacidad.",
         "config-anon-view": "Mostrar enlaces de vista an\u00f3nima",
         "config-block": "Bloquear",
         "config-block-help": "Lista de sitios separados por comas",
         "config-block-title": "Bloquear por t\u00edtulo",
         "config-block-title-help": "Usar expresiones regulares",
         "config-block-url": "Bloquear por URL",
         "config-block-url-help": "Usar expresiones regulares",
@@ -272,32 +420,39 @@
         "config-new-tab": "Abrir enlaces en una pesta\u00f1a nueva",
         "config-nojs": "Eliminar Javascript en vista an\u00f3nima",
         "config-pref-encryption": "Cifrar preferencias",
         "config-pref-help": "Requiere WHOOGLE_CONFIG_PREFERENCES_KEY; de lo contrario, se ignorar\u00e1.",
         "config-pref-url": "URL de preferencias",
         "config-safe": "B\u00fasqueda Segura",
         "config-theme": "Tema",
+        "config-time-period": "Periodo de tiempo",
         "config-tor": "Usa Tor",
         "config-url": "URL ra\u00edz",
         "continue-search": "Contin\u00fae su b\u00fasqueda con Farside",
         "dark": "oscuro",
         "github-link": "Ver en GitHub",
         "images": "Im\u00e1genes",
         "light": "brillante",
         "load": "Cargar",
         "maps": "Maps",
         "news": "Noticias",
+        "qdr:d": "\u00faltimas 24 horas",
+        "qdr:h": "Hora pasada",
+        "qdr:m": "El mes pasado",
+        "qdr:w": "Semana pasada",
+        "qdr:y": "A\u00f1o pasado",
         "ratelimit": "La instancia ha sido ratelimited",
         "save-as": "Guardar como...",
         "search": "Buscar",
         "system": "configuraci\u00f3n del sistema",
         "translate": "traducir",
         "videos": "V\u00eddeos"
     },
     "lang_fa": {
+        "": "--",
         "all": "\u0647\u0645\u0647",
         "anon-view": "\u0646\u0645\u0627\u06cc \u0646\u0627\u0634\u0646\u0627\u0633",
         "apply": "\u062a\u0627\u06cc\u06cc\u062f",
         "books": "\u06a9\u062a\u0627\u0628\u200c\u0647\u0627",
         "config": "\u067e\u06cc\u06a9\u0631\u0628\u0646\u062f\u06cc",
         "config-alts": "\u062c\u0627\u06cc\u06af\u0632\u06cc\u0646\u06cc \u067e\u06cc\u0648\u0646\u062f\u200c\u0647\u0627\u06cc \u0634\u0628\u06a9\u0647\u200c\u0647\u0627\u06cc \u0627\u062c\u062a\u0645\u0627\u0639\u06cc",
         "config-alts-help": "\u0644\u06cc\u0646\u06a9\u200c\u0647\u0627\u06cc \u062a\u0648\u06cc\u06cc\u062a\u0631\u060c \u06cc\u0648\u062a\u06cc\u0648\u0628\u060c \u0627\u06cc\u0646\u0633\u062a\u0627\u06af\u0631\u0627\u0645 \u0648... \u0631\u0627 \u0628\u0627 \u062c\u0627\u06cc\u06af\u0632\u06cc\u0646\u200c\u0647\u0627\u06cc\u06cc \u06a9\u0647 \u0628\u0647 \u062d\u0631\u06cc\u0645 \u062e\u0635\u0648\u0635\u06cc \u0627\u062d\u062a\u0631\u0627\u0645 \u0645\u06cc\u200c\u06af\u0630\u0627\u0631\u0646\u062f \u062c\u0627\u06cc\u06af\u0632\u06cc\u0646 \u0645\u06cc\u200c\u06a9\u0646\u062f.",
@@ -321,39 +476,46 @@
         "config-new-tab": "\u0628\u0627\u0632 \u06a9\u0631\u062f\u0646 \u067e\u06cc\u0648\u0646\u062f\u200c\u0647\u0627 \u062f\u0631 \u062a\u0628 \u062c\u062f\u06cc\u062f",
         "config-nojs": "\u062c\u0627\u0648\u0627 \u0627\u0633\u06a9\u0631\u06cc\u067e\u062a \u0631\u0627 \u062f\u0631 \u0646\u0645\u0627\u06cc \u0646\u0627\u0634\u0646\u0627\u0633 \u062d\u0630\u0641 \u06a9\u0646\u06cc\u062f",
         "config-pref-encryption": "\u0631\u0645\u0632\u06af\u0630\u0627\u0631\u06cc \u062a\u0646\u0638\u06cc\u0645\u0627\u062a \u0628\u0631\u06af\u0632\u06cc\u062f\u0647",
         "config-pref-help": "\u0628\u0647 WHOOGLE_CONFIG_PREFERENCES_KEY \u0646\u06cc\u0627\u0632 \u062f\u0627\u0631\u062f\u060c \u062f\u0631 \u063a\u06cc\u0631 \u0627\u06cc\u0646 \u0635\u0648\u0631\u062a \u0646\u0627\u062f\u06cc\u062f\u0647 \u06af\u0631\u0641\u062a\u0647 \u062e\u0648\u0627\u0647\u062f \u0634\u062f.",
         "config-pref-url": "URL \u062a\u0646\u0638\u06cc\u0645\u0627\u062a \u0628\u0631\u06af\u0632\u06cc\u062f\u0647",
         "config-safe": "\u062c\u0633\u062a\u062c\u0648\u06cc \u0627\u0645\u0646",
         "config-theme": "\u067e\u0648\u0633\u062a\u0647",
+        "config-time-period": "\u0628\u0627\u0632\u0647 \u0632\u0645\u0627\u0646\u06cc",
         "config-tor": "\u0627\u0633\u062a\u0641\u0627\u062f\u0647 \u0627\u0632 \u062a\u0648\u0631",
         "config-url": "\u0622\u062f\u0631\u0633 \u0631\u06cc\u0634\u0647\u200c\u06cc \u0633\u0627\u06cc\u062a",
         "continue-search": "Farside \u062c\u0633\u062a\u062c\u0648\u06cc \u062e\u0648\u062f \u0631\u0627 \u0628\u0627 ",
         "dark": "\u062a\u06cc\u0631\u0647",
         "github-link": "\u0646\u0645\u0627\u06cc\u0634 \u062f\u0631 \u06af\u06cc\u062a\u200c\u0647\u0627\u0628",
         "images": "\u062a\u0635\u0627\u0648\u06cc\u0631",
         "light": "\u0631\u0648\u0634\u0646",
         "load": "\u0628\u0627\u0631\u06af\u0630\u0627\u0631\u06cc",
         "maps": "\u0646\u0642\u0634\u0647\u200c\u0647\u0627",
         "news": "\u0627\u062e\u0628\u0627\u0631",
+        "qdr:d": "24 \u0633\u0627\u0639\u062a \u06af\u0630\u0634\u062a\u0647",
+        "qdr:h": "\u0633\u0627\u0639\u062a \u06af\u0630\u0634\u062a\u0647",
+        "qdr:m": "\u0645\u0627\u0647 \u06af\u0630\u0634\u062a\u0647",
+        "qdr:w": "\u0647\u0641\u062a\u0647 \u06af\u0630\u0634\u062a\u0647",
+        "qdr:y": "\u0633\u0627\u0644 \u06af\u0630\u0634\u062a\u0647",
         "ratelimit": "\u0646\u0645\u0648\u0646\u0647 \u0628\u0627 \u0646\u0631\u062e \u0645\u062d\u062f\u0648\u062f \u0634\u062f\u0647 \u0627\u0633\u062a",
         "save-as": "\u0630\u062e\u06cc\u0631\u0647 \u0628\u0647 \u0639\u0646\u0648\u0627\u0646...",
         "search": "\u062c\u0633\u062a\u062c\u0648",
         "system": "\u0633\u06cc\u0633\u062a\u0645",
         "translate": "\u062a\u0631\u062c\u0645\u0647",
         "videos": "\u0648\u06cc\u062f\u0626\u0648\u0647\u0627"
     },
     "lang_fr": {
+        "": "--",
         "all": "Tous",
         "anon-view": "Vue anonyme",
         "apply": "Appliquer",
         "books": "Livres",
         "config": "Configuration",
         "config-alts": "Remplacer les liens des r\u00e9seaux sociaux",
-        "config-alts-help": "Remplacer les liens Twitter/YouTube/Instagram/etc avec leurs alternatives respectueuses de la vie priv\u00e9e.",
+        "config-alts-help": "Remplacer les liens Twitter/YouTube/etc avec leurs alternatives respectueuses de la vie priv\u00e9e.",
         "config-anon-view": "Afficher les liens de vue anonymes",
         "config-block": "Bloquer",
         "config-block-help": "Liste de sites s\u00e9par\u00e9s pas des virgules",
         "config-block-title": "Bloquer par titre",
         "config-block-title-help": "Utiliser l'expression r\u00e9guli\u00e8re",
         "config-block-url": "Bloquer par URL",
         "config-block-url-help": "Utiliser l'expression r\u00e9guli\u00e8re",
@@ -370,32 +532,39 @@
         "config-new-tab": "Ouvrir les Liens dans un Nouveau Onglet",
         "config-nojs": "Supprimer Javascript dans la vue anonyme",
         "config-pref-encryption": "Chiffrer les pr\u00e9f\u00e9rences",
         "config-pref-help": "N\u00e9cessite WHOOGLE_CONFIG_PREFERENCES_KEY, sinon cela sera ignor\u00e9.",
         "config-pref-url": "URL des pr\u00e9f\u00e9rences",
         "config-safe": "Recherche s\u00e9curis\u00e9e",
         "config-theme": "Theme",
+        "config-time-period": "P\u00e9riode de temps",
         "config-tor": "Utiliser Tor",
         "config-url": "URL de la racine",
         "continue-search": "Continuez votre recherche avec Farside",
         "dark": "sombre",
         "github-link": "Voir sur GitHub",
         "images": "Images",
         "light": "clair",
         "load": "Charger",
         "maps": "Maps",
         "news": "Actualit\u00e9s",
+        "qdr:d": "Derni\u00e8res 24 heures",
+        "qdr:h": "Heure pass\u00e9e",
+        "qdr:m": "Mois pass\u00e9",
+        "qdr:w": "La semaine derni\u00e8re",
+        "qdr:y": "L'ann\u00e9e pass\u00e9e",
         "ratelimit": "Le d\u00e9bit de l'instance a \u00e9t\u00e9 limit\u00e9",
         "save-as": "Sauvegarder comme...",
         "search": "Chercher",
         "system": "syst\u00e8me",
         "translate": "Traduire",
         "videos": "Vid\u00e9os"
     },
     "lang_hi": {
+        "": "--",
         "all": "\u0938\u092d\u0940",
         "anon-view": "\u0905\u0928\u093e\u092e \u0926\u0943\u0936\u094d\u092f",
         "apply": "\u0932\u093e\u0917\u0942 \u0915\u0930\u0928\u093e",
         "books": "\u0915\u093f\u0924\u093e\u092c\u0947\u0902",
         "config": "\u0915\u0949\u0928\u094d\u092b\u093c\u093f\u0917\u0930\u0947\u0936\u0928",
         "config-alts": "\u0938\u094b\u0936\u0932 \u092e\u0940\u0921\u093f\u092f\u093e \u0932\u093f\u0902\u0915 \u092c\u0926\u0932\u0947\u0902",
         "config-alts-help": "\u0917\u094b\u092a\u0928\u0940\u092f\u0924\u093e \u0915\u093e \u0938\u092e\u094d\u092e\u093e\u0928 \u0915\u0930\u0928\u0947 \u0935\u093e\u0932\u0947 \u0935\u093f\u0915\u0932\u094d\u092a\u094b\u0902 \u0915\u0947 \u0938\u093e\u0925 \u091f\u094d\u0935\u093f\u091f\u0930/\u092f\u0942\u091f\u094d\u092f\u0942\u092c/\u0907\u0902\u0938\u094d\u091f\u093e\u0917\u094d\u0930\u093e\u092e/\u0906\u0926\u093f \u0932\u093f\u0902\u0915 \u0915\u094b \u092c\u0926\u0932 \u0926\u0947\u0924\u093e \u0939\u0948\u0964",
@@ -419,39 +588,102 @@
         "config-new-tab": "\u0928\u090f \u091f\u0948\u092c \u092e\u0947\u0902 \u0932\u093f\u0902\u0915 \u0916\u094b\u0932\u0947\u0902",
         "config-nojs": "\u0905\u0928\u093e\u092e \u0926\u0943\u0936\u094d\u092f \u092e\u0947\u0902 \u091c\u093e\u0935\u093e\u0938\u094d\u0915\u094d\u0930\u093f\u092a\u094d\u091f \u0928\u093f\u0915\u093e\u0932\u0947\u0902",
         "config-pref-encryption": "\u090f\u0928\u094d\u0915\u094d\u0930\u093f\u092a\u094d\u091f \u092a\u094d\u0930\u093e\u0925\u092e\u093f\u0915\u0924\u093e\u090f\u0902",
         "config-pref-help": "WHOOGLE_CONFIG_PREFERENCES_KEY \u0915\u0940 \u0906\u0935\u0936\u094d\u092f\u0915\u0924\u093e \u0939\u0948, \u0905\u0928\u094d\u092f\u0925\u093e \u0907\u0938\u0947 \u0905\u0928\u0926\u0947\u0916\u093e \u0915\u0930 \u0926\u093f\u092f\u093e \u091c\u093e\u090f\u0917\u093e\u0964",
         "config-pref-url": "\u0935\u0930\u0940\u092f\u0924\u093e\u090f\u0901 URL",
         "config-safe": "\u0938\u0941\u0930\u0915\u094d\u0937\u093f\u0924 \u0916\u094b\u091c",
         "config-theme": "\u0935\u093f\u0937\u092f",
+        "config-time-period": "\u0938\u092e\u092f \u0938\u0940\u092e\u093e",
         "config-tor": "TOR \u0915\u093e \u092a\u094d\u0930\u092f\u094b\u0917 \u0915\u0930\u0947\u0902",
         "config-url": "\u0930\u0942\u091f \u092f\u0942\u0906\u0930\u090f\u0932",
         "continue-search": "\u0915\u0947 \u0938\u093e\u0925 \u0905\u092a\u0928\u0940 \u0916\u094b\u091c \u091c\u093e\u0930\u0940 \u0930\u0916\u0947\u0902 Farside",
         "dark": "\u0905\u0902\u0927\u0947\u0930\u093e",
         "github-link": "\u0917\u093f\u091f\u0939\u092c \u092a\u0930 \u0926\u0947\u0916\u0947\u0902",
         "images": "\u0907\u092e\u0947\u091c",
         "light": "\u0930\u094b\u0936\u0928\u0940",
         "load": "\u092d\u093e\u0930",
         "maps": "\u0935\u0940\u0921\u093f\u092f\u094b",
         "news": "\u0938\u092e\u093e\u091a\u093e\u0930",
+        "qdr:d": "\u092a\u093f\u091b\u0932\u0947 24 \u0918\u0902\u091f\u0947",
+        "qdr:h": "\u092a\u093f\u091b\u0932\u0947 \u0918\u0902\u091f\u0947",
+        "qdr:m": "\u092a\u093f\u091b\u0932\u0947 \u092e\u0939\u0940\u0928\u0947",
+        "qdr:w": "\u092a\u093f\u091b\u0932\u0947 \u0938\u092a\u094d\u0924\u093e\u0939",
+        "qdr:y": "\u092a\u093f\u091b\u0932\u093e \u0935\u0930\u094d\u0937",
         "ratelimit": "\u0907\u0902\u0938\u094d\u091f\u0947\u0902\u0938 \u0915\u094b \u0938\u0940\u092e\u093f\u0924 \u0915\u0930 \u0926\u093f\u092f\u093e \u0917\u092f\u093e \u0939\u0948",
         "save-as": "\u0915\u0947 \u0930\u0942\u092a \u0930\u0915\u094d\u0937\u093f\u0924 \u0915\u0930\u0947\u0902...",
         "search": "\u0916\u094b\u091c",
         "system": "\u092a\u094d\u0930\u0923\u093e\u0932\u0940",
         "translate": "\u0905\u0928\u0941\u0935\u093e\u0926 \u0915\u0930\u0928\u093e",
         "videos": "\u092e\u0948\u092a"
     },
+    "lang_id": {
+        "": "--",
+        "all": "Semua",
+        "anon-view": "Tampilan Anonim",
+        "apply": "Terapkan",
+        "books": "Buku",
+        "config": "Konfigurasi",
+        "config-alts": "Ganti Tautan Media Sosial",
+        "config-alts-help": "Mengganti tautan Twitter/YouTube/dll dengan alternatif yang lebih menjaga privasi.",
+        "config-anon-view": "Tampilkan Tautan Tampilan Anonim",
+        "config-block": "Blokir",
+        "config-block-help": "Daftar situs yang dipisahkan dengan koma",
+        "config-block-title": "Blokir berdasarkan Judul",
+        "config-block-title-help": "Gunakan regex",
+        "config-block-url": "Blokir berdasarkan URL",
+        "config-block-url-help": "Gunakan regex",
+        "config-country": "Negara",
+        "config-css": "CSS Kustom",
+        "config-dark": "Mode Gelap",
+        "config-get-only": "Hanya Gunakan GET",
+        "config-images": "Pencarian Gambar Ukuran Penuh",
+        "config-images-help": "(Eksperimental) Menambahkan opsi 'Lihat Gambar' ke pencarian gambar desktop. Ini akan menyebabkan resolusi thumbnail hasil gambar menjadi lebih rendah.",
+        "config-lang": "Bahasa Antarmuka",
+        "config-lang-search": "Bahasa Penelusuran",
+        "config-near": "Dekat",
+        "config-near-help": "Nama Kota",
+        "config-new-tab": "Buka Tautan dalam Tab Baru",
+        "config-nojs": "Hapus Javascript dalam Tampilan Anonim",
+        "config-pref-encryption": "Enkripsi Preferensi",
+        "config-pref-help": "Memerlukan WHOOGLE_CONFIG_PREFERENCES_KEY, jika tidak akan diabaikan.",
+        "config-pref-url": "URL Preferensi",
+        "config-safe": "Pencarian Aman",
+        "config-theme": "Tema",
+        "config-time-period": "Periode Waktu",
+        "config-tor": "Gunakan Tor",
+        "config-url": "URL Dasar",
+        "continue-search": "Lanjutkan penelusuran Anda dengan Farside",
+        "dark": "gelap",
+        "github-link": "Lihat di GitHub",
+        "images": "Gambar",
+        "light": "terang",
+        "load": "Muat",
+        "maps": "Peta",
+        "news": "Berita",
+        "qdr:d": "24 jam yang lalu",
+        "qdr:h": "1 jam yang lalu",
+        "qdr:m": "1 bulan yang lalu",
+        "qdr:w": "1 minggu yang lalu",
+        "qdr:y": "1 tahun yang lalu",
+        "ratelimit": "Instansi telah ratelimited",
+        "save-as": "Simpan Sebagai...",
+        "search": "Telusuri",
+        "system": "sistem",
+        "translate": "terjemahkan",
+        "videos": "Video"
+    },
     "lang_it": {
+        "": "--",
         "all": "Tutti",
         "anon-view": "Vista Anonima",
         "apply": "Applica",
         "books": "Libri",
         "config": "Impostazioni",
         "config-alts": "Sostituisci link dei social",
-        "config-alts-help": "Sostituisci link di Twitter/YouTube/Instagram/etc con alternative che rispettano la privacy.",
+        "config-alts-help": "Sostituisci link di Twitter/YouTube/etc con alternative che rispettano la privacy.",
         "config-anon-view": "Mostra collegamenti di visualizzazione anonimi",
         "config-block": "Blocca",
         "config-block-help": "Lista di siti separati da virgole",
         "config-block-title": "Blocca per titolo",
         "config-block-title-help": "Usa regex",
         "config-block-url": "Blocca per url",
         "config-block-url-help": "Usa regex",
@@ -468,39 +700,46 @@
         "config-new-tab": "Apri i link in una nuova scheda",
         "config-nojs": "Rimuovere Javascript in visualizzazione anonima",
         "config-pref-encryption": "Crittografa le preferenze",
         "config-pref-help": "Richiede WHOOGLE_CONFIG_PREFERENCES_KEY, altrimenti verr\u00e0 ignorato.",
         "config-pref-url": "URL delle preferenze",
         "config-safe": "Ricerca Sicura",
         "config-theme": "Tema",
+        "config-time-period": "Periodo di tempo",
         "config-tor": "Usa Tor",
         "config-url": "Root URL",
         "continue-search": "Continua la tua ricerca con Farside",
         "dark": "notte",
         "github-link": "Guarda su GitHub",
         "images": "Immagini",
         "light": "luminoso",
         "load": "Carica",
         "maps": "Maps",
         "news": "Notizie",
+        "qdr:d": "Ultime 24 ore",
+        "qdr:h": "Ultima ora",
+        "qdr:m": "Mese scorso",
+        "qdr:w": "Settimana scorsa",
+        "qdr:y": "L'anno scorso",
         "ratelimit": "L'istanza \u00e8 stata limitata alla velocit\u00e0",
         "save-as": "Salva Come...",
         "search": "Cerca",
         "system": "impostazioni di sistema",
         "translate": "tradurre",
         "videos": "Video"
     },
     "lang_ja": {
+        "": "--",
         "all": "\u3059\u3079\u3066",
         "anon-view": "\u533f\u540d\u30d3\u30e5\u30fc",
         "apply": "\u53cd\u6620",
         "books": "\u66f8\u7c4d",
         "config": "\u8a2d\u5b9a",
         "config-alts": "\u30bd\u30fc\u30b7\u30e3\u30eb\u30e1\u30c7\u30a3\u30a2\u306e\u30ea\u30f3\u30af\u3092\u7f6e\u304d\u63db\u3048",
-        "config-alts-help": "Twitter/YouTube/Instagram\u306a\u3069\u306e\u30ea\u30f3\u30af\u3092\u3001\u30d7\u30e9\u30a4\u30d0\u30b7\u30fc\u3092\u5c0a\u91cd\u3057\u305f\u4ee3\u66ff\u30b5\u30a4\u30c8\u306b\u7f6e\u304d\u63db\u3048\u307e\u3059\u3002",
+        "config-alts-help": "Twitter/YouTube\u306a\u3069\u306e\u30ea\u30f3\u30af\u3092\u3001\u30d7\u30e9\u30a4\u30d0\u30b7\u30fc\u3092\u5c0a\u91cd\u3057\u305f\u4ee3\u66ff\u30b5\u30a4\u30c8\u306b\u7f6e\u304d\u63db\u3048\u307e\u3059\u3002",
         "config-anon-view": "\u533f\u540d\u306e\u30d3\u30e5\u30fc\u30ea\u30f3\u30af\u3092\u8868\u793a\u3059\u308b",
         "config-block": "\u30d6\u30ed\u30c3\u30af",
         "config-block-help": "\u30b5\u30a4\u30c8\u306e\u30ea\u30b9\u30c8\u3092\u30b3\u30f3\u30de\u533a\u5207\u308a\u3067\u5165\u529b",
         "config-block-title": "\u30bf\u30a4\u30c8\u30eb\u3067\u30d6\u30ed\u30c3\u30af",
         "config-block-title-help": "\u6b63\u898f\u8868\u73fe\u3092\u4f7f\u7528\u3057\u307e\u3059",
         "config-block-url": "\u3067\u30d6\u30ed\u30c3\u30af",
         "config-block-url-help": "\u6b63\u898f\u8868\u73fe\u3092\u4f7f\u7528",
@@ -517,39 +756,46 @@
         "config-new-tab": "\u65b0\u3057\u3044\u30bf\u30d6\u3067\u30ea\u30f3\u30af\u3092\u958b\u304f",
         "config-nojs": "\u533f\u540d\u30d3\u30e5\u30fc\u3067Javascript\u3092\u524a\u9664\u3059\u308b",
         "config-pref-encryption": "\u8a2d\u5b9a\u3092\u6697\u53f7\u5316\u3059\u308b",
         "config-pref-help": "WHOOGLE_CONFIG_PREFERENCES_KEY \u304c\u5fc5\u8981\u3067\u3059\u3002\u305d\u308c\u4ee5\u5916\u306e\u5834\u5408\u3001\u3053\u308c\u306f\u7121\u8996\u3055\u308c\u307e\u3059\u3002",
         "config-pref-url": "\u8a2d\u5b9a URL",
         "config-safe": "\u30bb\u30fc\u30d5\u30b5\u30fc\u30c1",
         "config-theme": "\u30c6\u30fc\u30de",
+        "config-time-period": "\u671f\u9593",
         "config-tor": "Tor\u3092\u4f7f\u7528",
         "config-url": "\u30eb\u30fc\u30c8URL",
         "continue-search": "\u3067\u691c\u7d22\u3092\u7d9a\u3051\u308b Farside",
         "dark": "\u30c0\u30fc\u30af",
         "github-link": "Github\u3067\u78ba\u8a8d",
         "images": "\u753b\u50cf",
         "light": "\u30e9\u30a4\u30c8",
         "load": "\u8aad\u307f\u8fbc\u307f",
         "maps": "\u5730\u56f3",
         "news": "\u30cb\u30e5\u30fc\u30b9",
+        "qdr:d": "\u904e\u53bb 24 \u6642\u9593",
+        "qdr:h": "\u904e\u53bb 1 \u6642\u9593",
+        "qdr:m": "\u5148\u6708",
+        "qdr:w": "\u3053\u306e1\u9031\u9593",
+        "qdr:y": "\u904e\u5e74\u5ea6",
         "ratelimit": "\u30a4\u30f3\u30b9\u30bf\u30f3\u30b9\u306f\u30ec\u30fc\u30c8\u5236\u9650\u3055\u308c\u3066\u3044\u307e\u3059",
         "save-as": "\u540d\u524d\u3092\u4ed8\u3051\u3066\u4fdd\u5b58",
         "search": "\u691c\u7d22",
         "system": "\u81ea\u52d5",
         "translate": "\u7ffb\u8a33",
         "videos": "\u52d5\u753b"
     },
     "lang_ko": {
+        "": "--",
         "all": "\uc804\uccb4",
         "anon-view": "\uc775\uba85 \ubcf4\uae30",
         "apply": "\uc801\uc6a9",
         "books": "\ub3c4\uc11c",
         "config": "\uad6c\uc131",
         "config-alts": "\uc18c\uc124 \ubbf8\ub514\uc5b4 \uc8fc\uc18c \uc218\uc815",
-        "config-alts-help": "Twitter/YouTube/Instagram \ub4f1\uc758 \ub9c1\ud06c\ub97c \ud504\ub77c\uc774\ubc84\uc2dc\ub97c \uc874\uc911\ud558\ub294 \ub9c1\ud06c\ub85c \ub300\uccb4\ud569\ub2c8\ub2e4",
+        "config-alts-help": "Twitter/YouTube \ub4f1\uc758 \ub9c1\ud06c\ub97c \ud504\ub77c\uc774\ubc84\uc2dc\ub97c \uc874\uc911\ud558\ub294 \ub9c1\ud06c\ub85c \ub300\uccb4\ud569\ub2c8\ub2e4",
         "config-anon-view": "\uc775\uba85 \ubcf4\uae30 \ub9c1\ud06c \ud45c\uc2dc",
         "config-block": "\ucc28\ub2e8",
         "config-block-help": "\uc27c\ud45c\ub85c \uad6c\ubd84\ub41c \uc0ac\uc774\ud2b8 \ubaa9\ub85d",
         "config-block-title": "\uc81c\ubaa9\uc73c\ub85c \ucc28\ub2e8",
         "config-block-title-help": "\uc815\uaddc \ud45c\ud604\uc2dd \uc0ac\uc6a9",
         "config-block-url": "URL\ub85c \ucc28\ub2e8",
         "config-block-url-help": "\uc815\uaddc \ud45c\ud604\uc2dd \uc0ac\uc6a9",
@@ -566,39 +812,46 @@
         "config-new-tab": "\uc0c8 \ud0ed\uc5d0\uc11c \uc5f4\uae30",
         "config-nojs": "\uc775\uba85 \ubcf4\uae30\uc5d0\uc11c Javascript \uc81c\uac70",
         "config-pref-encryption": "\uc554\ud638\ud654 \ud658\uacbd \uc124\uc815",
         "config-pref-help": "WHOOGLE_CONFIG_PREFERENCES_KEY\uc774 \ud544\uc694\ud569\ub2c8\ub2e4. \uadf8\ub807\uc9c0 \uc54a\uc73c\uba74 \ubb34\uc2dc\ub429\ub2c8\ub2e4.",
         "config-pref-url": "\ud658\uacbd\uc124\uc815 URL",
         "config-safe": "\uc138\uc774\ud504\uc11c\uce58",
         "config-theme": "\ud14c\ub9c8",
+        "config-time-period": "\uae30\uac04",
         "config-tor": "Tor \uc0ac\uc6a9",
         "config-url": "\ub8e8\ud2b8 URL",
         "continue-search": "Farside\ub85c \uac80\uc0c9 \uacc4\uc18d\ud558\uae30",
         "dark": "\ub2e4\ud06c",
         "github-link": "\uae43\ud5c8\ube0c\uc5d0\uc11c \ubcf4\uae30",
         "images": "\uc774\ubbf8\uc9c0",
         "light": "\ub77c\uc774\ud2b8",
         "load": "\ubd88\ub7ec\uc624\uae30",
         "maps": "\uc9c0\ub3c4",
         "news": "\ub274\uc2a4",
+        "qdr:d": "\uc9c0\ub09c 24\uc2dc\uac04",
+        "qdr:h": "\uc9c0\ub09c \uc2dc\uac04",
+        "qdr:m": "\uc9c0\ub09c\ub2ec",
+        "qdr:w": "\uc9c0\ub09c \uc8fc",
+        "qdr:y": "\uc9c0\ub09c \ud574",
         "ratelimit": "\uc778\uc2a4\ud134\uc2a4\uac00 \uc18d\ub3c4 \uc81c\ud55c\ub418\uc5c8\uc2b5\ub2c8\ub2e4.",
         "save-as": "\ub2e4\ub978 \uc774\ub984\uc73c\ub85c \uc800\uc7a5...",
         "search": "\uac80\uc0c9",
         "system": "\uc2dc\uc2a4\ud15c",
         "translate": "\ubc88\uc5ed",
         "videos": "\ub3d9\uc601\uc0c1"
     },
     "lang_ku": {
+        "": "--",
         "all": "Hem\u00fb",
         "anon-view": "D\u00eetina Nenas",
         "apply": "Bisep\u00eene",
         "books": "Pirt\u00fbk",
         "config": "Sazkar\u00ee",
         "config-alts": "Gir\u00eadan\u00ean Tora Civak\u00ee Biguher\u00eene",
-        "config-alts-help": "Gir\u00eadan\u00ean Twitter/YouTube/Instagram/hwd biguher\u00eene bi alternat\u00eev\u00ean ku ji taybetiy\u00ea re r\u00eaz\u00ea digrin.",
+        "config-alts-help": "Gir\u00eadan\u00ean Twitter/YouTube/hwd biguher\u00eene bi alternat\u00eev\u00ean ku ji taybetiy\u00ea re r\u00eaz\u00ea digrin.",
         "config-anon-view": "Gir\u00eadan\u00ean Nenas N\u00ee\u015fan bide",
         "config-block": "Astengkirin",
         "config-block-help": "R\u00eazoka malper\u00ea ya ji hev veqetand\u00ee bi riya b\u00eahnok",
         "config-block-title": "Bi ya Sernav\u00ea Asteng bike",
         "config-block-title-help": "regex bi kar b\u00eene",
         "config-block-url": "Bi ya Gir\u00eadan\u00ea asteng bike",
         "config-block-url-help": "regex bi kar b\u00eene",
@@ -615,39 +868,46 @@
         "config-new-tab": "Gir\u00eadanan di R\u00fbgereke N\u00fb de Veke",
         "config-nojs": "Javascript Rake di N\u00ee\u015fandan\u00ean Nenenas de",
         "config-pref-encryption": "Vebij\u00earkan \u015f\u00eefre bike",
         "config-pref-help": "P\u00eadiv\u00ee bi WHOOGLE_CONFIG_PREFERENCES_KEY dike, wek\u00ee din ev \u00ea were pa\u015fguhkirin.",
         "config-pref-url": "Vebij\u00eark\u00ean gir\u00eadan\u00ea",
         "config-safe": "L\u00eager\u00eena Parast\u00ee",
         "config-theme": "R\u00fbkar",
+        "config-time-period": "Dem Period",
         "config-tor": "Tor bi kar b\u00eene",
         "config-url": "R\u00eageha gir\u00eadan\u00ea",
         "continue-search": "L\u00eager\u00eena xwe bi Farside re bidom\u00eene",
         "dark": "tar\u00ee",
         "github-link": "Li ser GitHub N\u00ee\u015fan bide",
         "images": "W\u00eane",
         "light": "ron\u00ee",
         "load": "Bar bike",
         "maps": "Nex\u015fe",
         "news": "N\u00fb\u00e7e",
+        "qdr:d": "24 saet\u00ean bor\u00ee",
+        "qdr:h": "Saet ber\u00ea",
+        "qdr:m": "Meha bor\u00ee",
+        "qdr:w": "Hefteya bor\u00ee",
+        "qdr:y": "Sala bor\u00ee",
         "ratelimit": "M\u00eenak bi r\u00eajeya s\u00eenorkir\u00ee ye",
         "save-as": "Bipar\u00eaze wek\u00ee...",
         "search": "Bigere",
         "system": "pergal",
         "translate": "werger",
         "videos": "V\u00eedyo"
     },
     "lang_nl": {
+        "": "--",
         "all": "Alle",
         "anon-view": "Anonieme Weergave",
         "apply": "Opslaan",
         "books": "Boeken",
         "config": "Instellingen",
         "config-alts": "Social Media Links Vervangen",
-        "config-alts-help": "Vervang Twitter/YouTube/Instagram/etc links met privacy gerespecteerde alternatieve.",
+        "config-alts-help": "Vervang Twitter/YouTube/etc links met privacy gerespecteerde alternatieve.",
         "config-anon-view": "Toon anonieme links bekijken",
         "config-block": "Blok",
         "config-block-help": "Lijst met sites met kommas onderscheiden",
         "config-block-title": "Blokkeren op titel",
         "config-block-title-help": "Gebruik regex",
         "config-block-url": "Blokkeren op URL",
         "config-block-url-help": "Gebruik regex",
@@ -664,39 +924,46 @@
         "config-new-tab": "Open Links in New Tab",
         "config-nojs": "Javascript verwijderen in anonieme weergave",
         "config-pref-encryption": "Versleutel voorkeuren",
         "config-pref-help": "Vereist WHOOGLE_CONFIG_PREFERENCES_KEY, anders wordt dit genegeerd.",
         "config-pref-url": "Voorkeurs URL",
         "config-safe": "Veilig zoeken",
         "config-theme": "Thema",
+        "config-time-period": "Tijdsperiode",
         "config-tor": "Gebruik Tor",
         "config-url": "Root URL",
         "continue-search": "Ga verder met zoeken met Farside",
         "dark": "donker",
         "github-link": "Bekijk op GitHub",
         "images": "Afbeeldingen",
         "light": "helder",
         "load": "Laden",
         "maps": "Maps",
         "news": "Nieuws",
+        "qdr:d": "Afgelopen 24 uur",
+        "qdr:h": "Afgelopen uur",
+        "qdr:m": "Afgelopen maand",
+        "qdr:w": "Vorige week",
+        "qdr:y": "Afgelopen jaar",
         "ratelimit": "Instantie is beperkt in snelheid",
         "save-as": "Opslaan Als...",
         "search": "Zoeken",
         "system": "systeeminstellingen",
         "translate": "vertalen",
         "videos": "Videos"
     },
     "lang_pt": {
+        "": "--",
         "all": "Todas",
         "anon-view": "Visualiza\u00e7\u00e3o An\u00f4nima",
         "apply": "Aplicar",
         "books": "Livros",
         "config": "Configura\u00e7\u00e3o",
         "config-alts": "Substituir Links de Redes Sociais",
-        "config-alts-help": "Substitui os links do Twitter/YouTube/Instagram/etc. por alternativas que respeitam sua privacidade.",
+        "config-alts-help": "Substitui os links do Twitter/YouTube/etc. por alternativas que respeitam sua privacidade.",
         "config-anon-view": "Mostrar links de visualiza\u00e7\u00e3o an\u00f4nimos",
         "config-block": "Bloquear",
         "config-block-help": "Lista de sites separados por v\u00edrgulas",
         "config-block-title": "Bloco por t\u00edtulo",
         "config-block-title-help": "Use regex",
         "config-block-url": "Bloquear por url",
         "config-block-url-help": "Use regex",
@@ -713,39 +980,46 @@
         "config-new-tab": "Abrir Links em Nova Aba",
         "config-nojs": "Remover Javascript na visualiza\u00e7\u00e3o an\u00f4nima",
         "config-pref-encryption": "Criptografar prefer\u00eancias",
         "config-pref-help": "Requer WHOOGLE_CONFIG_PREFERENCES_KEY, caso contr\u00e1rio, ser\u00e1 ignorado.",
         "config-pref-url": "URL de prefer\u00eancias",
         "config-safe": "Pesquisa Segura",
         "config-theme": "Tema",
+        "config-time-period": "Per\u00edodo de tempo",
         "config-tor": "Usar Tor",
         "config-url": "URL Fonte",
         "continue-search": "Continue sua pesquisa com Farside",
         "dark": "escuro",
         "github-link": "Ver no GitHub",
         "images": "Imagens",
         "light": "brilhante",
         "load": "Carregar",
         "maps": "Maps",
         "news": "Not\u00edcias",
+        "qdr:d": "\u00faltimas 24 horas",
+        "qdr:h": "Hora passada",
+        "qdr:m": "M\u00eas passado",
+        "qdr:w": "Semana passada",
+        "qdr:y": "Ano passado",
         "ratelimit": "A inst\u00e2ncia foi limitada pela taxa",
         "save-as": "Guardar Como...",
         "search": "Pesquisar",
         "system": "configura\u00e7\u00e3o de sistema",
         "translate": "traduzir",
         "videos": "V\u00eddeos"
     },
     "lang_ru": {
+        "": "--",
         "all": "\u0412\u0441\u0435",
         "anon-view": "\u0410\u043d\u043e\u043d\u0438\u043c\u043d\u044b\u0439 \u043f\u0440\u043e\u0441\u043c\u043e\u0442\u0440",
         "apply": "\u041f\u0440\u0438\u043c\u0435\u043d\u0438\u0442\u044c",
         "books": "\u041a\u043d\u0438\u0433\u0438",
         "config": "\u041d\u0430\u0441\u0442\u0440\u043e\u0439\u043a\u0430",
         "config-alts": "\u0417\u0430\u043c\u0435\u043d\u0438\u0442\u044c \u0441\u0441\u044b\u043b\u043a\u0438 \u043d\u0430 \u0441\u043e\u0446\u0438\u0430\u043b\u044c\u043d\u044b\u0435 \u0441\u0435\u0442\u0438",
-        "config-alts-help": "\u0417\u0430\u043c\u0435\u043d\u0430 \u0441\u0441\u044b\u043b\u043a\u043e\u043a Twitter, YouTube, Instagram \u0438 \u0442.\u0434. \u043d\u0430 \u0430\u043b\u044c\u0442\u0435\u0440\u043d\u0430\u0442\u0438\u0432\u044b, \u0443\u0432\u0430\u0436\u0430\u044e\u0449\u0438\u0435 \u043a\u043e\u043d\u0444\u0438\u0434\u0435\u043d\u0446\u0438\u0430\u043b\u044c\u043d\u043e\u0441\u0442\u044c.",
+        "config-alts-help": "\u0417\u0430\u043c\u0435\u043d\u0430 \u0441\u0441\u044b\u043b\u043a\u043e\u043a Twitter, YouTube, \u0438 \u0442.\u0434. \u043d\u0430 \u0430\u043b\u044c\u0442\u0435\u0440\u043d\u0430\u0442\u0438\u0432\u044b, \u0443\u0432\u0430\u0436\u0430\u044e\u0449\u0438\u0435 \u043a\u043e\u043d\u0444\u0438\u0434\u0435\u043d\u0446\u0438\u0430\u043b\u044c\u043d\u043e\u0441\u0442\u044c.",
         "config-anon-view": "\u041f\u043e\u043a\u0430\u0437\u0430\u0442\u044c \u0441\u0441\u044b\u043b\u043a\u0438 \u0434\u043b\u044f \u0430\u043d\u043e\u043d\u0438\u043c\u043d\u043e\u0433\u043e \u043f\u0440\u043e\u0441\u043c\u043e\u0442\u0440\u0430",
         "config-block": "\u0411\u043b\u043e\u043a\u0438\u0440\u043e\u0432\u0430\u0442\u044c",
         "config-block-help": "\u0421\u043f\u0438\u0441\u043e\u043a \u0441\u0430\u0439\u0442\u043e\u0432 \u0447\u0435\u0440\u0435\u0437 \u0437\u0430\u043f\u044f\u0442\u0443\u044e",
         "config-block-title": "\u0411\u043b\u043e\u043a\u0438\u0440\u043e\u0432\u0430\u0442\u044c \u043f\u043e \u043d\u0430\u0437\u0432\u0430\u043d\u0438\u044e",
         "config-block-title-help": "\u0418\u0441\u043f\u043e\u043b\u044c\u0437\u0443\u0439\u0442\u0435 regex",
         "config-block-url": "\u0411\u043b\u043e\u043a\u0438\u0440\u043e\u0432\u0430\u0442\u044c \u043f\u043e URL-\u0430\u0434\u0440\u0435\u0441\u0443",
         "config-block-url-help": "\u0418\u0441\u043f\u043e\u043b\u044c\u0437\u0443\u0439\u0442\u0435 regex",
@@ -762,32 +1036,39 @@
         "config-new-tab": "\u041e\u0442\u043a\u0440\u044b\u0432\u0430\u0442\u044c \u0441\u0441\u044b\u043b\u043a\u0438 \u0432 \u043d\u043e\u0432\u043e\u0439 \u0432\u043a\u043b\u0430\u0434\u043a\u0435",
         "config-nojs": "\u0423\u0434\u0430\u043b\u0438\u0442\u044c Javascript \u0432 \u0430\u043d\u043e\u043d\u0438\u043c\u043d\u043e\u043c \u043f\u0440\u043e\u0441\u043c\u043e\u0442\u0440\u0435",
         "config-pref-encryption": "\u0417\u0430\u0448\u0438\u0444\u0440\u043e\u0432\u0430\u0442\u044c \u043d\u0430\u0441\u0442\u0440\u043e\u0439\u043a\u0438",
         "config-pref-help": "\u0422\u0440\u0435\u0431\u0443\u0435\u0442\u0441\u044f WHOOGLE_CONFIG_PREFERENCES_KEY, \u0438\u043d\u0430\u0447\u0435 \u044d\u0442\u043e \u0431\u0443\u0434\u0435\u0442 \u043f\u0440\u043e\u0438\u0433\u043d\u043e\u0440\u0438\u0440\u043e\u0432\u0430\u043d\u043e.",
         "config-pref-url": "URL-\u0430\u0434\u0440\u0435\u0441 \u043d\u0430\u0441\u0442\u0440\u043e\u0435\u043a",
         "config-safe": "\u0411\u0435\u0437\u043e\u043f\u0430\u0441\u043d\u044b\u0439 \u043f\u043e\u0438\u0441\u043a",
         "config-theme": "\u0422\u0435\u043c\u0430",
+        "config-time-period": "\u0412\u0440\u0435\u043c\u0435\u043d\u043d\u043e\u0439 \u043f\u0435\u0440\u0438\u043e\u0434",
         "config-tor": "\u0418\u0441\u043f\u043e\u043b\u044c\u0437\u043e\u0432\u0430\u0442\u044c Tor",
         "config-url": "\u041a\u043e\u0440\u043d\u0435\u0432\u043e\u0439 URL-\u0430\u0434\u0440\u0435\u0441",
         "continue-search": "\u041f\u0440\u043e\u0434\u043e\u043b\u0436\u0438\u0442\u044c \u043f\u043e\u0438\u0441\u043a \u0441 Farside",
         "dark": "\u0442\u0451\u043c\u043d\u0430\u044f",
         "github-link": "\u041f\u043e\u0441\u043c\u043e\u0442\u0440\u0435\u0442\u044c \u043d\u0430 GitHub",
         "images": "\u041a\u0430\u0440\u0442\u0438\u043d\u043a\u0438",
         "light": "\u0441\u0432\u0435\u0442\u043b\u0430\u044f",
         "load": "\u0417\u0430\u0433\u0440\u0443\u0437\u0438\u0442\u044c",
         "maps": "\u041a\u0430\u0440\u0442\u044b",
         "news": "\u041d\u043e\u0432\u043e\u0441\u0442\u0438",
+        "qdr:d": "\u041f\u043e\u0441\u043b\u0435\u0434\u043d\u0438\u0435 24\u00a0\u0447\u0430\u0441\u0430",
+        "qdr:h": "\u041f\u0440\u043e\u0448\u0435\u0434\u0448\u0438\u0439 \u0447\u0430\u0441",
+        "qdr:m": "\u041f\u0440\u043e\u0448\u043b\u044b\u0439 \u043c\u0435\u0441\u044f\u0446",
+        "qdr:w": "\u041d\u0430 \u043f\u0440\u043e\u0448\u043b\u043e\u0439 \u043d\u0435\u0434\u0435\u043b\u0435",
+        "qdr:y": "\u041f\u0440\u043e\u0448\u043b\u044b\u0439 \u0433\u043e\u0434",
         "ratelimit": "\u0418\u043d\u0441\u0442\u0430\u043d\u0441 \u0431\u044b\u043b \u043e\u0433\u0440\u0430\u043d\u0438\u0447\u0435\u043d \u043f\u043e \u043e\u043f\u0435\u0440\u0430\u0446\u0438\u044f\u043c",
         "save-as": "\u0421\u043e\u0445\u0440\u0430\u043d\u0438\u0442\u044c \u043a\u0430\u043a...",
         "search": "\u041f\u043e\u0438\u0441\u043a",
         "system": "\u0441\u0438\u0441\u0442\u0435\u043c\u043d\u0430\u044f",
         "translate": "\u043f\u0435\u0440\u0435\u0432\u0435\u0441\u0442\u0438",
         "videos": "\u0412\u0438\u0434\u0435\u043e"
     },
     "lang_si": {
+        "": "--",
         "all": "\u0dc3\u0dd2\u0dba\u0dbd\u0dca\u0dbd",
         "anon-view": "\u0db1\u0dd2\u0dbb\u0dca\u0db1\u0dcf\u0db8\u0dd2\u0d9a \u0daf\u0dc3\u0dd4\u0db1",
         "apply": "\u0dba\u0ddc\u0daf\u0db1\u0dca\u0db1",
         "books": "\u0db4\u0ddc\u0dad\u0dca",
         "config": "\u0dc0\u0dd2\u0db1\u0dca\u200d\u0dba\u0dcf\u0dc3\u0dba",
         "config-alts": "\u0dc3\u0db8\u0dcf\u0da2 \u0db8\u0dcf\u0db0\u0dca\u200d\u0dba \u0dc3\u0db6\u0dd0\u0db3\u0dd2 \u0db4\u0dca\u200d\u0dbb\u0dad\u0dd2\u0dc3\u0dca\u0dae\u0dcf\u0db4\u0db1\u0dba \u0d9a\u0dbb\u0db1\u0dca\u0db1",
         "config-alts-help": "\u0da7\u0dca\u0dc0\u0dd2\u0da7\u0dbb\u0dca/\u0dba\u0dd6 \u0da7\u0dd2\u0dba\u0dd4\u0db6\u0dca/\u0d89\u0db1\u0dca\u0dc3\u0dca\u0da7\u0d9c\u0dca\u200d\u0dbb\u0dd1\u0db8\u0dca \u0d86\u0daf\u0dd3 \u0dc3\u0db6\u0dd0\u0db3\u0dd2 \u0db4\u0dde\u0daf\u0dca\u0d9c\u0dbd\u0dd2\u0d9a\u0dad\u0dca\u0dc0\u0dba\u0da7 \u0d9c\u0dbb\u0dd4 \u0d9a\u0dbb\u0db1 \u0dc0\u0dd2\u0d9a\u0dbd\u0dca\u0db4 \u0dc3\u0db8\u0d9f \u0db4\u0dca\u200d\u0dbb\u0dad\u0dd2\u0dc3\u0dca\u0dae\u0dcf\u0db4\u0db1\u0dba \u0d9a\u0dbb\u0dba\u0dd2.",
@@ -811,39 +1092,46 @@
         "config-new-tab": "\u0db1\u0dc0 \u0dad\u0dd3\u0dbb\u0dd4\u0dc0\u0d9a\u0dd2\u0db1\u0dca \u0dc3\u0db6\u0dd0\u0db3\u0dd2 \u0dc0\u0dd2\u0dc0\u0dd8\u0dad \u0d9a\u0dbb\u0db1\u0dca\u0db1",
         "config-nojs": "Anonymous View \u0dc4\u0dd2 Javascript \u0d89\u0dc0\u0dad\u0dca \u0d9a\u0dbb\u0db1\u0dca\u0db1",
         "config-pref-encryption": "\u0db8\u0db1\u0dcf\u0db4 \u0dc3\u0d82\u0d9a\u0dda\u0dad\u0db1\u0dba \u0d9a\u0dbb\u0db1\u0dca\u0db1",
         "config-pref-help": "WHOOGLE_CONFIG_PREFERENCES_KEY \u0d85\u0dc0\u0dc1\u0dca\u200d\u0dba \u0dc0\u0dda, \u0d91\u0dc3\u0dda \u0db1\u0ddc\u0db8\u0dd0\u0dad\u0dd2\u0db1\u0db8\u0dca \u0db8\u0dd9\u0dba \u0db1\u0ddc\u0dc3\u0dbd\u0d9a\u0dcf \u0dc4\u0dbb\u0dd2\u0db1\u0dd4 \u0d87\u0dad.",
         "config-pref-url": "\u0db8\u0db1\u0dcf\u0db4 URL",
         "config-safe": "\u0d86\u0dbb\u0d9a\u0dca\u200d\u0dc2\u0dd2\u0dad \u0dc3\u0dd9\u0dc0\u0dd4\u0db8",
         "config-theme": "\u0dad\u0dda\u0db8\u0dcf\u0dc0",
+        "config-time-period": "\u0d9a\u0dcf\u0dbd \u0dc3\u0dd3\u0db8\u0dcf\u0dc0",
         "config-tor": "\u0da7\u0ddd\u0dbb\u0dca \u0db7\u0dcf\u0dc0\u0dd2\u0dad\u0dcf \u0d9a\u0dbb\u0db1\u0dca\u0db1",
         "config-url": "\u0d92.\u0dc3.\u0db1\u0dd2.(URL) \u0db8\u0dd6\u0dbd\u0dba",
         "continue-search": "Farside \u0dc3\u0db8\u0d9f \u0d94\u0db6\u0d9c\u0dda \u0dc3\u0dd9\u0dc0\u0dd4\u0db8 \u0d9a\u0dbb\u0d9c\u0dd9\u0db1 \u0dba\u0db1\u0dca\u0db1",
         "dark": "\u0d85\u0db3\u0dd4\u0dbb\u0dd4",
         "github-link": "\u0d9c\u0dd2\u0da7\u0dca\u0dc4\u0db6\u0dca \u0dc4\u0dd2 \u0db6\u0dbd\u0db1\u0dca\u0db1",
         "images": "\u0dbb\u0dd6\u0db4",
         "light": "\u0daf\u0dd3\u0db4\u0dca\u0dad\u0dd2\u0db8\u0dad\u0dca",
         "load": "\u0db4\u0dd6\u0dbb\u0db1\u0dba \u0d9a\u0dbb\u0db1\u0dca\u0db1",
         "maps": "\u0dc3\u0dd2\u0dad\u0dd2\u0dba\u0db8\u0dca",
         "news": "\u0d85\u0db1\u0dd4\u0dbb\u0dd6\u0db4",
+        "qdr:d": "\u0db4\u0dc3\u0dd4\u0d9c\u0dd2\u0dba \u0db4\u0dd0\u0dba 24",
+        "qdr:h": "\u0db4\u0dc3\u0dd4\u0d9c\u0dd2\u0dba \u0db4\u0dd0\u0dba",
+        "qdr:m": "\u0db4\u0dc3\u0dd4\u0d9c\u0dd2\u0dba \u0db8\u0dcf\u0dc3\u0dba",
+        "qdr:w": "\u0db4\u0dc3\u0dd4\u0d9c\u0dd2\u0dba \u0dc3\u0dad\u0dd2\u0dba",
+        "qdr:y": "\u0db4\u0dc3\u0dd4\u0d9c\u0dd2\u0dba \u0dc0\u0dc3\u0dbb",
         "ratelimit": "\u0dc3\u0dda\u0dc0\u0dcf\u0daf\u0dcf\u0dba\u0d9a\u0dba \u0d85\u0db1\u0dd4\u0db4\u0dcf\u0dad\u0db1\u0dba \u0d9a\u0dbb \u0d87\u0dad",
         "save-as": "...\u0dbd\u0dd9\u0dc3 \u0dc3\u0dd4\u0dbb\u0d9a\u0dd2\u0db1\u0dca\u0db1",
         "search": "\u0dc3\u0ddc\u0dba\u0db1\u0dca\u0db1",
         "system": "\u0db4\u0daf\u0dca\u0db0\u0dad\u0dd2\u0dba",
         "translate": "\u0db4\u0dbb\u0dd2\u0dc0\u0dbb\u0dca\u0dad\u0db1\u0dba \u0d9a\u0dbb\u0db1\u0dca\u0db1",
         "videos": "\u0dc0\u0dd3\u0da9\u0dd2\u0dba\u0ddd"
     },
     "lang_th": {
+        "": "--",
         "all": "\u0e17\u0e31\u0e49\u0e07\u0e2b\u0e21\u0e14",
         "anon-view": "\u0e21\u0e38\u0e21\u0e21\u0e2d\u0e07\u0e17\u0e35\u0e48\u0e44\u0e21\u0e48\u0e23\u0e30\u0e1a\u0e38\u0e15\u0e31\u0e27\u0e15\u0e19",
         "apply": "\u0e22\u0e2d\u0e21\u0e23\u0e31\u0e1a",
         "books": "\u0e2b\u0e19\u0e31\u0e07\u0e2a\u0e37\u0e2d",
         "config": "\u0e01\u0e33\u0e2b\u0e19\u0e14\u0e04\u0e48\u0e32",
         "config-alts": "\u0e41\u0e17\u0e19\u0e17\u0e35\u0e48\u0e25\u0e34\u0e07\u0e01\u0e4c\u0e42\u0e0b\u0e40\u0e0a\u0e35\u0e22\u0e25\u0e21\u0e35\u0e40\u0e14\u0e35\u0e22",
-        "config-alts-help": "\u0e41\u0e17\u0e19\u0e17\u0e35\u0e48\u0e25\u0e34\u0e07\u0e01\u0e4c Twitter/YouTube/Instagram/\u0e2d\u0e37\u0e48\u0e19\u0e46 \u0e15\u0e32\u0e21\u0e04\u0e27\u0e32\u0e21\u0e40\u0e1b\u0e47\u0e19\u0e2a\u0e48\u0e27\u0e19\u0e15\u0e31\u0e27\u0e14\u0e49\u0e27\u0e22\u0e17\u0e32\u0e07\u0e40\u0e25\u0e37\u0e2d\u0e01\u0e2d\u0e37\u0e48\u0e19",
+        "config-alts-help": "\u0e41\u0e17\u0e19\u0e17\u0e35\u0e48\u0e25\u0e34\u0e07\u0e01\u0e4c Twitter/YouTube/\u0e2d\u0e37\u0e48\u0e19\u0e46 \u0e15\u0e32\u0e21\u0e04\u0e27\u0e32\u0e21\u0e40\u0e1b\u0e47\u0e19\u0e2a\u0e48\u0e27\u0e19\u0e15\u0e31\u0e27\u0e14\u0e49\u0e27\u0e22\u0e17\u0e32\u0e07\u0e40\u0e25\u0e37\u0e2d\u0e01\u0e2d\u0e37\u0e48\u0e19",
         "config-anon-view": "\u0e41\u0e2a\u0e14\u0e07\u0e25\u0e34\u0e07\u0e04\u0e4c\u0e43\u0e19\u0e21\u0e38\u0e21\u0e21\u0e2d\u0e07\u0e44\u0e21\u0e48\u0e23\u0e30\u0e1a\u0e38\u0e15\u0e31\u0e27\u0e15\u0e19",
         "config-block": "\u0e1a\u0e25\u0e47\u0e2d\u0e04",
         "config-block-help": "\u0e23\u0e32\u0e22\u0e01\u0e32\u0e23\u0e40\u0e27\u0e47\u0e1a\u0e44\u0e0b\u0e15\u0e4c\u0e04\u0e31\u0e48\u0e19\u0e14\u0e49\u0e27\u0e22\u0e40\u0e04\u0e23\u0e37\u0e48\u0e2d\u0e07\u0e2b\u0e21\u0e32\u0e22\u0e08\u0e38\u0e25\u0e20\u0e32\u0e04(,)",
         "config-block-title": "\u0e1a\u0e25\u0e47\u0e2d\u0e01\u0e15\u0e32\u0e21\u0e2b\u0e31\u0e27\u0e0a\u0e37\u0e48\u0e2d\u0e40\u0e27\u0e47\u0e1a\u0e44\u0e0b\u0e15\u0e4c",
         "config-block-title-help": "\u0e43\u0e0a\u0e49 regex",
         "config-block-url": "\u0e1a\u0e25\u0e47\u0e2d\u0e01\u0e15\u0e32\u0e21 URL",
         "config-block-url-help": "\u0e43\u0e0a\u0e49 regex",
@@ -860,39 +1148,46 @@
         "config-new-tab": "\u0e40\u0e1b\u0e34\u0e14\u0e25\u0e34\u0e07\u0e01\u0e4c\u0e43\u0e19\u0e41\u0e17\u0e47\u0e1a\u0e43\u0e2b\u0e21\u0e48",
         "config-nojs": "\u0e25\u0e1a Javascript \u0e43\u0e19\u0e21\u0e38\u0e21\u0e21\u0e2d\u0e07\u0e17\u0e35\u0e48\u0e44\u0e21\u0e48\u0e23\u0e30\u0e1a\u0e38\u0e15\u0e31\u0e27\u0e15\u0e19",
         "config-pref-encryption": "\u0e40\u0e02\u0e49\u0e32\u0e23\u0e2b\u0e31\u0e2a\u0e01\u0e32\u0e23\u0e15\u0e31\u0e49\u0e07\u0e04\u0e48\u0e32",
         "config-pref-help": "\u0e08\u0e33\u0e40\u0e1b\u0e47\u0e19\u0e15\u0e49\u0e2d\u0e07\u0e21\u0e35 WHOOGLE_CONFIG_PREFERENCES_KEY \u0e44\u0e21\u0e48\u0e40\u0e0a\u0e48\u0e19\u0e19\u0e31\u0e49\u0e19\u0e08\u0e30\u0e16\u0e39\u0e01\u0e25\u0e30\u0e40\u0e27\u0e49\u0e19\u0e44\u0e1b",
         "config-pref-url": "URL \u0e01\u0e32\u0e23\u0e15\u0e31\u0e49\u0e07\u0e04\u0e48\u0e32",
         "config-safe": "\u0e04\u0e49\u0e19\u0e2b\u0e32\u0e41\u0e1a\u0e1a\u0e1b\u0e25\u0e2d\u0e14\u0e20\u0e31\u0e22",
         "config-theme": "\u0e18\u0e35\u0e21",
+        "config-time-period": "\u0e23\u0e30\u0e22\u0e30\u0e40\u0e27\u0e25\u0e32",
         "config-tor": "\u0e43\u0e0a\u0e49 Tor",
         "config-url": "URL \u0e2b\u0e25\u0e31\u0e01",
         "continue-search": "\u0e04\u0e49\u0e19\u0e2b\u0e32\u0e15\u0e48\u0e2d\u0e44\u0e1b\u0e14\u0e49\u0e27\u0e22 Farside",
         "dark": "\u0e21\u0e37\u0e14",
         "github-link": "\u0e14\u0e39\u0e1a\u0e19 GitHub",
         "images": "\u0e23\u0e39\u0e1b\u0e20\u0e32\u0e1e",
         "light": "\u0e2a\u0e27\u0e48\u0e32\u0e07",
         "load": "\u0e42\u0e2b\u0e25\u0e14",
         "maps": "\u0e41\u0e1c\u0e19\u0e17\u0e35\u0e48",
         "news": "\u0e02\u0e48\u0e32\u0e27",
+        "qdr:d": "24 \u0e0a\u0e31\u0e48\u0e27\u0e42\u0e21\u0e07\u0e17\u0e35\u0e48\u0e1c\u0e48\u0e32\u0e19\u0e21\u0e32",
+        "qdr:h": "\u0e0a\u0e31\u0e48\u0e27\u0e42\u0e21\u0e07\u0e17\u0e35\u0e48\u0e1c\u0e48\u0e32\u0e19\u0e21\u0e32",
+        "qdr:m": "\u0e40\u0e14\u0e37\u0e2d\u0e19\u0e17\u0e35\u0e48\u0e1c\u0e48\u0e32\u0e19\u0e21\u0e32",
+        "qdr:w": "\u0e2a\u0e31\u0e1b\u0e14\u0e32\u0e2b\u0e4c\u0e17\u0e35\u0e48\u0e1c\u0e48\u0e32\u0e19\u0e21\u0e32",
+        "qdr:y": "\u0e1b\u0e35\u0e17\u0e35\u0e48\u0e1c\u0e48\u0e32\u0e19\u0e21\u0e32",
         "ratelimit": "\u0e04\u0e33\u0e02\u0e2d\u0e23\u0e49\u0e2d\u0e07\u0e08\u0e30\u0e16\u0e39\u0e01\u0e08\u0e33\u0e01\u0e31\u0e14\u0e08\u0e33\u0e19\u0e27\u0e19",
         "save-as": "\u0e1a\u0e31\u0e19\u0e17\u0e36\u0e01\u0e40\u0e1b\u0e47\u0e19...",
         "search": "\u0e04\u0e49\u0e19\u0e2b\u0e32",
         "system": "\u0e23\u0e30\u0e1a\u0e1a",
         "translate": "\u0e41\u0e1b\u0e25\u0e20\u0e32\u0e29\u0e32",
         "videos": "\u0e27\u0e34\u0e14\u0e35\u0e42\u0e2d"
     },
     "lang_zh-CN": {
+        "": "--",
         "all": "\u5168\u90e8",
         "anon-view": "\u533f\u540d\u89c6\u56fe",
         "apply": "\u5e94\u7528",
         "books": "\u4e66\u7c4d",
         "config": "\u914d\u7f6e",
         "config-alts": "\u66ff\u6362\u793e\u4ea4\u5a92\u4f53\u94fe\u63a5",
-        "config-alts-help": "\u4f7f\u7528\u5c0a\u91cd\u9690\u79c1\u7684\u7b2c\u4e09\u65b9\u7f51\u7ad9\u66ff\u6362 Twitter/YouTube/Instagram \u7b49\u94fe\u63a5\u3002",
+        "config-alts-help": "\u4f7f\u7528\u5c0a\u91cd\u9690\u79c1\u7684\u7b2c\u4e09\u65b9\u7f51\u7ad9\u66ff\u6362 Twitter/YouTube \u7b49\u94fe\u63a5\u3002",
         "config-anon-view": "\u663e\u793a\u533f\u540d\u67e5\u770b\u94fe\u63a5",
         "config-block": "\u5c4f\u853d",
         "config-block-help": "\u9017\u53f7\u5206\u9694\u7684\u7f51\u7ad9\u5217\u8868",
         "config-block-title": "\u6309\u7f51\u7ad9\u6807\u9898\u5c4f\u853d",
         "config-block-title-help": "\u4f7f\u7528\u6b63\u5219\u8868\u8fbe\u5f0f",
         "config-block-url": "\u6309\u7f51\u7ad9\u94fe\u63a5\u5c4f\u853d",
         "config-block-url-help": "\u4f7f\u7528\u6b63\u5219\u8868\u8fbe\u5f0f",
@@ -909,73 +1204,86 @@
         "config-new-tab": "\u5728\u65b0\u6807\u7b7e\u9875\u6253\u5f00\u94fe\u63a5",
         "config-nojs": "\u5728\u533f\u540d\u89c6\u56fe\u4e2d\u5220\u9664 Javascript",
         "config-pref-encryption": "\u52a0\u5bc6\u9996\u9009\u9879",
         "config-pref-help": "\u9700\u8981 WHOOGLE_CONFIG_PREFERENCES_KEY\uff0c\u5426\u5219\u5c06\u88ab\u5ffd\u7565\u3002",
         "config-pref-url": "\u9996\u9009\u9879\u7f51\u5740",
         "config-safe": "\u5b89\u5168\u641c\u7d22",
         "config-theme": "\u4e3b\u9898",
+        "config-time-period": "\u65f6\u95f4\u6bb5",
         "config-tor": "\u4f7f\u7528 Tor",
         "config-url": "\u7ad9\u70b9\u6839 URL",
         "continue-search": "\u7ee7\u7eed\u641c\u7d22 Farside",
         "dark": "\u9ed1\u6697\u7684",
         "github-link": "\u5728 GitHub \u4e0a\u67e5\u770b",
         "images": "\u56fe\u7247",
         "light": "\u660e\u4eae\u7684",
         "load": "\u8f7d\u5165",
         "maps": "\u5730\u56fe",
         "news": "\u65b0\u95fb",
+        "qdr:d": "\u8fc7\u53bb 24 \u5c0f\u65f6",
+        "qdr:h": "\u8fc7\u53bb\u4e00\u5c0f\u65f6",
+        "qdr:m": "\u8fc7\u53bb\u4e00\u4e2a\u6708",
+        "qdr:w": "\u4e0a\u5468",
+        "qdr:y": "\u8fc7\u53bb\u4e00\u5e74",
         "ratelimit": "\u5b9e\u4f8b\u5df2\u88ab\u9650\u901f",
         "save-as": "\u53e6\u5b58\u4e3a...",
         "search": "\u641c\u7d22",
         "system": "\u7cfb\u7edf\u8bbe\u7f6e",
         "translate": "\u7ffb\u8bd1",
         "videos": "\u89c6\u9891"
     },
     "lang_zh-TW": {
+        "": "--",
         "all": "\u5168\u90e8",
         "anon-view": "\u533f\u540d\u6aa2\u8996",
         "apply": "\u5957\u7528",
         "books": "\u66f8\u7c4d",
         "config": "\u8a2d\u5b9a",
         "config-alts": "\u5c07\u793e\u7fa4\u7db2\u7ad9\u9023\u7d50\u66ff\u63db",
-        "config-alts-help": "\u5c07 Twitter/YouTube/Instagram \u7b49\u7db2\u7ad9\u4e4b\u9023\u7d50\u66ff\u63db\u70ba\u5c0a\u91cd\u96b1\u79c1\u7684\u7b2c\u4e09\u65b9\u7db2\u7ad9\u3002",
+        "config-alts-help": "\u5c07 Twitter/YouTube \u7b49\u7db2\u7ad9\u4e4b\u9023\u7d50\u66ff\u63db\u70ba\u5c0a\u91cd\u96b1\u79c1\u7684\u7b2c\u4e09\u65b9\u7db2\u7ad9\u3002",
         "config-anon-view": "\u986f\u793a\u533f\u540d\u6aa2\u8996\u93c8\u63a5",
         "config-block": "\u5c01\u9396",
         "config-block-help": "\u4ee5\u9017\u865f\u5206\u9694\u4e4b\u7db2\u5740\u5217\u8868",
         "config-block-title": "\u6309\u6a19\u984c\u5c01\u9396",
         "config-block-title-help": "\u4f7f\u7528\u6b63\u898f\u8868\u9054\u5f0f",
         "config-block-url": "\u6309\u7db2\u5740\u5c01\u9396",
         "config-block-url-help": "\u4f7f\u7528\u6b63\u898f\u8868\u9054\u5f0f",
         "config-country": "\u8a2d\u5b9a\u570b\u5bb6",
         "config-css": "\u81ea\u5b9a CSS",
         "config-dark": "\u6df1\u8272\u6a21\u5f0f",
         "config-get-only": "\u50c5\u9650\u65bc GET \u8981\u6c42",
         "config-images": "\u5b8c\u6574\u5c3a\u5bf8\u5716\u7247\u641c\u5c0b",
-        "config-images-help": "\uff08\u5be6\u9a57\u6027\uff09\u5728\u684c\u9762\u7248\u5716\u7247\u641c\u5c0b\u4e2d\u589e\u52a0\u300c\u6aa2\u8996\u5716\u7247\u300d\u9078\u9805\u3002\u9019\u6703\u4f7f\u641c\u5c0b\u7d50\u679c\u5716\u7247\u89e3\u6790\u5ea6\u964d\u4f4e",
+        "config-images-help": "\uff08\u5be6\u9a57\u6027\uff09\u5728\u684c\u9762\u7248\u5716\u7247\u641c\u5c0b\u4e2d\u589e\u52a0\u300c\u6aa2\u8996\u5716\u7247\u300d\u9078\u9805\u3002\u9019\u6703\u4f7f\u641c\u5c0b\u7d50\u679c\u5716\u7247\u89e3\u6790\u5ea6\u964d\u4f4e\u3002",
         "config-lang": "\u4ecb\u9762\u8a9e\u8a00",
         "config-lang-search": "\u641c\u5c0b\u8a9e\u8a00",
         "config-near": "\u63a5\u8fd1",
         "config-near-help": "\u57ce\u5e02\u540d\u7a31",
         "config-new-tab": "\u4ee5\u65b0\u5206\u9801\u958b\u555f\u9023\u7d50",
         "config-nojs": "\u65bc\u533f\u540d\u6aa2\u8996\u4e2d\u522a\u9664 JavaScript",
         "config-pref-encryption": "\u52a0\u5bc6\u8a2d\u5b9a",
         "config-pref-help": "\u9700\u8981\u4e00\u4f75\u8a2d\u5b9a WHOOGLE_CONFIG_PREFERENCES_KEY\uff0c\u5426\u5247\u5c07\u6703\u88ab\u5ffd\u7565\u3002",
         "config-pref-url": "\u8a2d\u5b9a\u7db2\u5740",
         "config-safe": "\u5b89\u5168\u641c\u5c0b",
         "config-theme": "\u4e3b\u984c",
+        "config-time-period": "\u6642\u9593\u7bc4\u570d",
         "config-tor": "\u4f7f\u7528 Tor",
         "config-url": "\u9996\u9801\u7db2\u5740",
         "continue-search": "\u7e7c\u7e8c\u641c\u5c0b Farside",
         "dark": "\u9ed1\u6697\u7684",
         "github-link": "\u5728 GitHub \u4e0a\u6aa2\u8996",
         "images": "\u5716\u7247",
         "light": "\u660e\u4eae\u7684",
         "load": "\u8f09\u5165",
         "maps": "\u5730\u5716",
         "news": "\u65b0\u805e",
+        "qdr:d": "\u904e\u53bb 24 \u5c0f\u6642",
+        "qdr:h": "\u904e\u53bb 1 \u5c0f\u6642",
+        "qdr:m": "\u904e\u53bb 1 \u500b\u6708",
+        "qdr:w": "\u904e\u53bb 1 \u9031",
+        "qdr:y": "\u904e\u53bb 1 \u5e74",
         "ratelimit": "\u8a72\u5be6\u4f8b\u5df2\u88ab\u9650\u901f",
         "save-as": "\u53e6\u5b58\u70ba...",
         "search": "\u641c\u5c0b",
         "system": "\u4f9d\u7167\u7cfb\u7d71\u8a2d\u5b9a",
         "translate": "\u7ffb\u8b6f",
         "videos": "\u5f71\u7247"
     }
```

### Comparing `whoogle-search-0.8.1/app/templates/display.html` & `whoogle-search-0.8.2/app/templates/display.html`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/templates/error.html` & `whoogle-search-0.8.2/app/templates/error.html`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/templates/header.html` & `whoogle-search-0.8.2/app/templates/header.html`

 * *Files 8% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                                 name="q"
                                 spellcheck="false"
                                 type="text"
                                 value="{{ clean_query(query) }}"
                                 dir="auto">
                         <input name="tbm" value="{{ search_type }}" style="display: none">
                         <input name="country" value="{{ config.country }}" style="display: none;">
+                        <input name="tbs" value="{{ config.tbs }}" style="display: none;">
                         <input type="submit" style="display: none;">
                         <div class="sc"></div>
                     </div>
                 </div>
             </form>
         </div>
     </header>
@@ -131,11 +132,27 @@
                     %}
                     selected
                     {% endif %}>
                     {{ country.name }}
                 </option>
             {% endfor %}
         </select>
+        <br />
+        <label for="config-time-period">{{ translation['config-time-period'] }}: </label>
+        <select name="tbs" id="result-time-period">
+            {% for time_period in time_periods %}
+                <option value="{{ time_period.value }}"
+                        {% if (
+                            config.tbs != '' and config.tbs in time_period.value
+                        ) or (
+                            config.tbs == '' and time_period.value == '')
+                        %}
+                        selected
+                        {% endif %}>
+                {{ translation[time_period.value] }}
+                </option>
+            {% endfor %}
+        </select>
     </div>
 </div>
 
 <script type="text/javascript" src="{{ cb_url('header.js') }}"></script>
```

### Comparing `whoogle-search-0.8.1/app/templates/imageresults.html` & `whoogle-search-0.8.2/app/templates/imageresults.html`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/templates/index.html` & `whoogle-search-0.8.2/app/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,31 @@
                                             selected
                                             {% endif %}>
                                         {{ country.name }}
                                     </option>
                                 {% endfor %}
                             </select>
                         </div>
+                        <div class="config-div">
+                            <label for="config-time-period">{{ translation['config-time-period'] }}</label>
+                            <select name="tbs" id="config-time-period">
+                                {% for time_period in time_periods %}
+                                    <option value="{{ time_period.value }}"
+                                            {% if (
+                                                config.tbs != '' and config.tbs in time_period.value
+                                            ) or (
+                                                config.tbs == '' and time_period.value == '')
+                                            %}
+                                            selected
+                                            {% endif %}>
+                                    {{ translation[time_period.value] }}
+                                    </option>
+                                {% endfor %}
+                            </select>
+                        </div>
                         <div class="config-div config-div-lang">
                             <label for="config-lang-interface">{{ translation['config-lang'] }}: </label>
                             <select name="lang_interface" id="config-lang-interface">
                                 {% for lang in languages %}
                                     <option value="{{ lang.value }}"
                                             {% if lang.value in config.lang_interface %}
                                             selected
```

#### html2text {}

```diff
@@ -31,14 +31,19 @@
 {% if not config_disabled %}
 {{ translation['config'] }}
 {% for country in countries %}
 % if ( config.country != '' and config.country in country.value ) or
 ( config.country == '' and country.value == '') %} selected {% endif %}> {
 { country.name }}
 {% endfor %}
+{% for time_period in time_periods %}
+% if ( config.tbs != '' and config.tbs in time_period.value ) or ( config.tbs
+== '' and time_period.value == '') %} selected {% endif %}> {{ translation
+[time_period.value] }}
+{% endfor %}
 {% for lang in languages %}
 % if lang.value in config.lang_interface %} selected {% endif %}> {{ lang.name
 }}
 {% endfor %}
 {% for lang in languages %}
 % if lang.value in config.lang_search %} selected {% endif %}> {{ lang.name }}
 {% endfor %}
```

### Comparing `whoogle-search-0.8.1/app/templates/logo.html` & `whoogle-search-0.8.2/app/templates/logo.html`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/templates/opensearch.xml` & `whoogle-search-0.8.2/app/templates/opensearch.xml`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,14 @@
         data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADwAAAA8CAYAAAA6/NlyAAAABGdBTUEAALGPC/xhBQAAAAFzUkdCAK7OHOkAAAAgY0hSTQAAeiYAAICEAAD6AAAAgOgAAHUwAADqYAAAOpgAABdwnLpRPAAAAAZiS0dEAP8A/wD/oL2nkwAAAAlwSFlzAAAASAAAAEgARslrPgAADS9JREFUaN7Nm2lsXNd1x3/nzQxnOMNdJEeUuYjUZu2Lh7IrWZZsy46btN7ioEgRSHZapEybLgHStPDSAqntNg7yIahdyAjgJg4aB66tJDBsy4ocW5QrWzYtUQslUdx3cV9nONt7tx/ekNSQQ84MOTLzB0hg3nbv/55zzzn33HOFm4Sqx58GEcEwHIALpXIQcaNUFmCJPKYQ8aJULyJDgBcRH4ZhHHn1+ZvSL0kZwX/9KTQ3g6bZgFKU2ghsBnYDxUAOkAnYAW2aMAQBLzAK9ALngLPANUQa8Psncbk48soP/jAIV33rBzA8DE5nHkp9CXggQnI14FjkZ8NAT4T4B8BvsNnaMQx15L//bXkIVz3+NFgsQihUDDwEPALcDriWOoizEAIuAb9B5KiIXFFK6Ud+/twXR7jq0JMAuRGSfwXsBGwpJjobBtACvAr8Ap+vhcxMkpV4UoSrDj8FIhpK7UKpfwK+DDhvMtHZ0IEziPwQOAYEk5F2QoSr/u4FGBkBkUyUOgz8A7DmCyY6G4PATxF5EcPowmLhyM+ejfuSJf53wbOhEqAA+Hfge0DhMpMFU7P2AFsQqUWpPs/2fdScP7U0wlWHngSRMuA54DCmW/lDgQBrgW3ANUpLOzwVO6iprV7whfhklXoR+Eq856eglPlPoeZvWASRlIUBAHWIfBvDOLWQes/bYsQSFwAvYEo2bu+UoUAg3elgRX4uK1cVkJuXjcNhR0QIhcJMjHvp7emn9/ogE+NewuEwmqbF+3Si+Bj4C5S6Mh/pmCSqDj8FkIlSLwB/CVgXJKoUIsLKogI2bV3Htp0bcRflk5HhxGqLftUwDPyTAUaGx7h2tYXaz+toberE7w+kSuLHEPlrTBfGbAs+p4Wqw0+B1SqEQn+DKd30eGRdGU7uPOBh710eCtwrkuq4zzvJlUuNHH+nmraWrlSRfgX4W8A3OyafY7Q82/eBUh7gR4A7Htni0iK+9udf4c4DlWRlZyTdYVuajVXFbtbdWk4oFKanqw9dN5ZKfC3Qgq5f8Ow6EGW5owjfEEH9B7BvoS8ahqJibQnf+ObDbNi0Bosl9jwMh3UCgSChYAgFaJoWk0xGposNGyswDIPWli4MXbEEznZgPZr2MXD9RsLTn6x64hkIBsFi+SbwIguoslKK4pIivn74QdasL5tzPxAI0t7aRXNDO91dfYyOjKHrBi5XOgWFeZRVFLN2XRnZuVlzyPt8kxz91TE+PvU5hjG/lU8Q/4WmfRcIThmwGYui62CxlADfikc2MyuDh752/xyyhmHQ0tjB74+fpv5KMxPjXpSa22m7PQ13UQF793vYvWc7TudMc05nOg9+9T7Gx7ycP3t5qar9VQzjdeBk1aEnOfLq86ZKVz3+NBgGiBwCnmBmvRoTB+69nbvu3o1oM53RdZ1TH3zG//7P2zQ1tBEKhqZ97ew/wzAYGR6n/koTA33DlK5ehdM1Q9ruSCNvRTaXLzbgn1yS9c4ADDTtXcCoOX8qQkwp0LQ8zNXPvC5IKcXKogLuuHMX2g1zVinFJx+d462jJxgaHJ13nt4ITRP0sM5nn5zn6K+OMToyHnV/dUUxO27btBTpTuEgSm2e+mGpeuIZU53hYaAKSJvvTRHhnvv3sLNycxShK5caefO1dxkbGUfTkpOGiHC9ux/RhPW3lk8HIZqmkZ7uSIWUs4FOLSPj1G2b7kDDMKbSMg9gqkBMKKVwudJZv7E8qvHJST8fnviYwYHhKBVPBqaGnOXa1Zao6yWrV7FmfVlMO5Ak/tjweotgZq6WApXxOlVYVMDKouiFUktjBw31rYgsPjwUEUZHxqk5cwE9rE9fT0uzUV5RkorQcwewA6XQUIpIwq083lv5Bbk4XdFpqsZrbUz6/EvxmdOkG6+1MTIyFnXdXVSA3Z4GSxOyC6V2EQ6jqXAYzOziggk3ESErOyNqtM3IqDcVKgfA+NgEY6MTUddy87KwO+wLrrwSxG5sNpcmNls6ZpYxLtLTo8dED+tzOrhYiJhWO+APRLfpdGCzJZSniIe1QL6GmWUsTuSNOZIUUr2mZfbcUIYiRQqUCxRrKJUb+RGHLUz6/FGXrFYruXlZKemNUgpbmhWnM1qLvN5JQqFwKprIQKlSDZFCFnBHM3wVw0Oj6PqMFbVaLZSUrUqJlJWCvBU5ZOdED+DgwDD+SX8q2nAgcosW2etJKE812D/MxLgv6tqadWVkZrlSYLgU6zaUk5UVPfa9PQMEg6ElDyhgQ6lcDXOJGNfRaaLR1ztId2dv1PXS1avYvG39ktyGUopCdz6Vf7QtKniZ9PlpbmhLmRcALIl7dDGjqrqL19B1Y2bY0mzcfd8eVpW4MQwj4c/dSNZms7L/3tspK4+2nU2N7TQ3daTUMGqYskl4CGs+uUhrc0fUtbLyW3j0zx6gwL0iKdJKKaxWC/vu3s3eA54oYsFAiE9P1zIx7kslYaUhMoG5ZRkXIsLw0CgnT3xCIBD9yuZt6/nGE4+wZp0Z+6oFFu9KKQzDICPTyZ88cpA/ffTgHB9/6UI9F89dTSVZHRizolQ/5v5sQhCBC+eusvHTi9xx523TblNEuHXzGvLyc/jow884//llhoZGCU4NjALEXAVlZWVQVlHMXffsZuOWtVitc1ek3Z29kUxmqvjiB7qtiAyi1GjihAW/P8BbR9/H7rCzq3JL1P1C9woefux+9t29m7bmTrq7+vBO+DAMA4fDTl5+Dqsriim6pRCHY37nsHe/h9bmTi7W1ie95JwHPkS6rJjS7U3mTRFhcGCEX7/+HjablS3bN0SpnmbRKCjMo6Awb/qaUiQlrdy8bB567D4mxr20NnUueul5A0aADkvl7oMhdH0TcbKUsUh7J3w01reaBN0rSEuzLfB88j3MzslkZVEBTQ1tTEws2XjVIvKKxbNlD5ih5aMk4I9nk56c9FN/uZn21i5cGU5y8rKxWBIL9pVS9PYMMDoyTlZ27GAvLz+HrOwM6i83E4zkyRaJ13E43rF4tu8DM4/1IGY6JCmICEop+q4PcrWukbbmTgKBoLmMFDN3NZXj0nWdgD/IyPAYrc0dnHz/DO/+9gPqLjRQvqaYrOzMmG0UuvPRRGht6iQcDi+GdBB4iXC4zhrRtQaU+hwoWezwaZowPublXE0dF8/Xk+Eypb0iPwdXhhNN0wj4zT2lwYFhxsa85lIwYr3feO1dvn7oQdxF+XO+bbVauOdLe/H7Axx/+9RiApxriJwFsHh27gfDCCNSBNxLgpvk80l7SuL+CLmerl7amrtoae6ks6OHgf4hfD4/RmQ7ZepvoG8I74SX9RsrYtoCi0WjuGQlA31DdHf1JivlX6JpbwCGpaa2Gs+Ou8AsE7oHKFos4VjkRQTRBE2Lzk3Hev56zwCGbrB2/Wos1rnjnmZPo2z1LfT1DtJ3fSBR0oPAsyjVhIgpTc+uA6jR0VGx293AAVJYsJYMDMOgq+M6TqeD0vLimP7X6UqnpGwVLU0djAyPJUL6OCL/iUjoyM+fMwnX1FZTufsgiAwC9wN58b5yMyAihMM67W095OZlsap4ZUx3lpnlIic3m4b61nhr5QngWUyXRM35UzPz1bNzP2K19mMYOcB+lknKIkLAH6S9rZvi0pXkF8Qe+0L3CjIznTQ3thPwB+cj/Q4iP0YkMLUxPk24prYaz9a9AO2YSb1FW+xUkPZ6J+nrHaSsojimjxYRClfm09PdT1fH9ViEe4F/AS7Z3W7OnD4GzA40LBYwjJZI0dfgchEG0801N7bz5mvvMDgwPOd+wB+k+vdnqL/chMxVxhDwEpr2O0T4yY/+fobijU/V1Fbj2bkfoBkzCNnDMqk2mFIc6B/G651kw8YKbJF6EZ/Pz9u/fp/33q7G552MJd33gGdQajxuyUPN+VN4tu8zEKkHtmDmc5cVvT39WKwWVlcUMzo8zltv/o6PPqwhHIoZddUh8o+I1E8ZqgUJA1TuOgC6PoZILbAVKGMZoesG7S1d+LyTfHSyhnM1ddOVQ7PQBnxn5I03Tjq2bk28bAmm6z0A9gIvY27HLDvmIQowgMj3gZ+hlJqvon7e1dGRV58HTYOXn/s/RL6NWfS17JiHbDsi30fkF4iohY4PLBg319RW4+nSQal24DRmBe0altGQxUAd8B3gKEoZ8UqJ4y4Uamqrqdx1AKXrA6Jpp4EsTEO23EWmIcyw8Xtit1ejlEqkbjq5AnFzXrswkwX/DKSkCGMR6AVeAo4A/RCZggkgadW84azDDsw6zMf44uqnJ4D3gZfRtBMoFUr27MPiD3mYxwHsGMYdwCHgIGY4ejPm9xBQDfwSkeNK10cdbjc/+fF3k/7Q0o/xPP40mBtVm1Hqy5jnIHaw9NMtQaABOAH8FpFPEfFiGAmr700hPE185gCIG7OA5DbMQpm1mEnCDMyyCuusdnXMJLkPM5XaDnwGnEXkLCLti1Hdm044irwpdUEpJ5APFKNUKSK3RDbgZ47iwRjQjUgX0AFcR2QcMBI5tJEs/h/GMBxGKn9DKwAAACV0RVh0ZGF0ZTpjcmVhdGUAMjAyMC0wNC0xMlQyMDoyMDo0OSswMDowME0is3UAAAAldEVYdGRhdGU6bW9kaWZ5ADIwMjAtMDQtMTJUMjA6MjA6NDkrMDA6MDA8fwvJAAAARnRFWHRzb2Z0d2FyZQBJbWFnZU1hZ2ljayA2LjcuOC05IDIwMTQtMDUtMTIgUTE2IGh0dHA6Ly93d3cuaW1hZ2VtYWdpY2sub3Jn3IbtAAAAABh0RVh0VGh1bWI6OkRvY3VtZW50OjpQYWdlcwAxp/+7LwAAABh0RVh0VGh1bWI6OkltYWdlOjpoZWlnaHQAMTkyDwByhQAAABd0RVh0VGh1bWI6OkltYWdlOjpXaWR0aAAxOTLTrCEIAAAAGXRFWHRUaHVtYjo6TWltZXR5cGUAaW1hZ2UvcG5nP7JWTgAAABd0RVh0VGh1bWI6Ok1UaW1lADE1ODY3MjI4NDlV2OpiAAAAD3RFWHRUaHVtYjo6U2l6ZQAwQkKUoj7sAAAAVnRFWHRUaHVtYjo6VVJJAGZpbGU6Ly8vbW50bG9nL2Zhdmljb25zLzIwMjAtMDQtMTIvNTdhMDYyNGFhNzAyYzk3ZWU1YTE5MjgwYWEwNTkwZDMuaWNvLnBuZ1EXWHMAAAAASUVORK5CYII=
     </Image>
     <Url type="text/html" {{ request_type|safe }} template="{{ main_url }}/search">
         <Param name="q" value="{searchTerms}"/>
         {% if search_type %}
             <Param name="tbm" value="{{ search_type }}"/>
         {% endif %}
-        {% if preferences %}
-            <Param name="preferences" value="{{ preferences }}"/>
-        {% endif %}
     </Url>
     <Url type="application/x-suggestions+json" {{ request_type|safe }} template="{{ main_url }}/autocomplete">
         <Param name="q" value="{searchTerms}"/>
     </Url>
     <moz:SearchForm>{{ main_url }}/search</moz:SearchForm>
 </OpenSearchDescription>
```

### Comparing `whoogle-search-0.8.1/app/utils/bangs.py` & `whoogle-search-0.8.2/app/utils/bangs.py`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/app/utils/misc.py` & `whoogle-search-0.8.2/app/utils/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from bs4 import BeautifulSoup as bsoup
 from flask import Request
 import hashlib
 import os
+import re
 from requests import exceptions, get
 from urllib.parse import urlparse
 
 
 def gen_file_hash(path: str, static_file: str) -> str:
     file_contents = open(os.path.join(path, static_file), 'rb').read()
     file_hash = hashlib.md5(file_contents).hexdigest()[:8]
@@ -36,16 +37,24 @@
 
     return url
 
 
 def get_proxy_host_url(r: Request, default: str, root=False) -> str:
     scheme = r.headers.get('X-Forwarded-Proto', 'https')
     http_host = r.headers.get('X-Forwarded-Host')
+
+    full_path = r.full_path if not root else ''
+    if full_path.startswith('/'):
+        full_path = f'/{full_path}'
+
     if http_host:
-        return f'{scheme}://{http_host}{r.full_path if not root else "/"}'
+        prefix = os.environ.get('WHOOGLE_URL_PREFIX', '')
+        if prefix:
+            prefix = f'/{re.sub("[^0-9a-zA-Z]+", "", prefix)}'
+        return f'{scheme}://{http_host}{prefix}{full_path}'
 
     return default
 
 
 def check_for_update(version_url: str, current: str) -> int:
     # Check for the latest version of Whoogle
     try:
```

### Comparing `whoogle-search-0.8.1/app/utils/results.py` & `whoogle-search-0.8.2/app/utils/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 import copy
 from flask import current_app
 import html
 import os
 import urllib.parse as urlparse
 from urllib.parse import parse_qs
 import re
+import warnings
 
 SKIP_ARGS = ['ref_src', 'utm']
-SKIP_PREFIX = ['//www.', '//mobile.', '//m.']
+SKIP_PREFIX = ['//www.', '//mobile.', '//m.', 'www.', 'mobile.', 'm.']
 GOOG_STATIC = 'www.gstatic.com'
 G_M_LOGO_URL = 'https://www.gstatic.com/m/images/icons/googleg.gif'
 GOOG_IMG = '/images/branding/searchlogo/1x/googlelogo'
 LOGO_URL = GOOG_IMG + '_desk'
 BLANK_B64 = ('data:image/png;base64,'
              'iVBORw0KGgoAAAANSUhEUgAAAAoAAAAKCAQAAAAnOwc2AAAAD0lEQVR42mNkw'
              'AIYh7IgAAVVAAuInjI5AAAAAElFTkSuQmCC')
@@ -27,27 +28,47 @@
     'Reklam', 'آگهی', 'Reklāma', 'Reklaam', 'Διαφήμιση', 'מודעה', 'Hirdetés',
     'Anúncio', 'Quảng cáo','โฆษณา', 'sponsored', 'patrocinado', 'gesponsert'
 ]
 
 SITE_ALTS = {
     'twitter.com': os.getenv('WHOOGLE_ALT_TW', 'farside.link/nitter'),
     'youtube.com': os.getenv('WHOOGLE_ALT_YT', 'farside.link/invidious'),
-    'instagram.com': os.getenv('WHOOGLE_ALT_IG', 'farside.link/bibliogram/u'),
     'reddit.com': os.getenv('WHOOGLE_ALT_RD', 'farside.link/libreddit'),
     **dict.fromkeys([
         'medium.com',
         'levelup.gitconnected.com'
     ], os.getenv('WHOOGLE_ALT_MD', 'farside.link/scribe')),
     'imgur.com': os.getenv('WHOOGLE_ALT_IMG', 'farside.link/rimgo'),
     'wikipedia.org': os.getenv('WHOOGLE_ALT_WIKI', 'farside.link/wikiless'),
     'imdb.com': os.getenv('WHOOGLE_ALT_IMDB', 'farside.link/libremdb'),
     'quora.com': os.getenv('WHOOGLE_ALT_QUORA', 'farside.link/quetre')
 }
 
 
+def contains_cjko(s: str) -> bool:
+    """This function check whether or not a string contains Chinese, Japanese,
+    or Korean characters. It employs regex and uses the u escape sequence to
+    match any character in a set of Unicode ranges.
+
+    Args:
+        s (str): string to be checked
+
+    Returns:
+        bool: True if the input s contains the characters and False otherwise
+    """
+    unicode_ranges = ('\u4e00-\u9fff' # Chinese characters
+                      '\u3040-\u309f' # Japanese hiragana
+                      '\u30a0-\u30ff' # Japanese katakana
+                      '\u4e00-\u9faf' # Japanese kanji
+                      '\uac00-\ud7af' # Korean hangul syllables
+                      '\u1100-\u11ff' # Korean hangul jamo
+                      )
+    return bool(re.search(fr'[{unicode_ranges}]', s))
+
+
 def bold_search_terms(response: str, query: str) -> BeautifulSoup:
     """Wraps all search terms in bold tags (<b>). If any terms are wrapped
     in quotes, only that exact phrase will be made bold.
 
     Args:
         response: The initial response body for the query
         query: The original search query
@@ -62,20 +83,26 @@
         # the replacement
         if len(element) == len(target_word):
             return
 
         # Ensure target word is escaped for regex
         target_word = re.escape(target_word)
 
+        # Check if the word contains Chinese, Japanese, or Korean characters
+        if contains_cjko(target_word):
+            reg_pattern = fr'((?![{{}}<>-]){target_word}(?![{{}}<>-]))'
+        else:
+            reg_pattern = fr'\b((?![{{}}<>-]){target_word}(?![{{}}<>-]))\b'
+
         if re.match('.*[@_!#$%^&*()<>?/\|}{~:].*', target_word) or (
                 element.parent and element.parent.name == 'style'):
             return
 
         element.replace_with(BeautifulSoup(
-            re.sub(fr'\b((?![{{}}<>-]){target_word}(?![{{}}<>-]))\b',
+            re.sub(reg_pattern,
                    r'<b>\1</b>',
                    element,
                    flags=re.I), 'html.parser')
         )
 
     # Split all words out of query, grouping the ones wrapped in quotes
     for word in re.split(r'\s+(?=[^"]*(?:"[^"]*"[^"]*)*$)', query):
@@ -155,27 +182,32 @@
         # Wikipedia -> Wikiless replacements require the subdomain (if it's
         # a 2-char language code) to be passed as a URL param to Wikiless
         # in order to preserve the language setting.
         params = ''
         if 'wikipedia' in hostname and len(subdomain) == 2:
             hostname = f'{subdomain}.{hostname}'
             params = f'?lang={subdomain}'
+        elif 'medium' in hostname and len(subdomain) > 0:
+            hostname = f'{subdomain}.{hostname}'
 
         parsed_alt = urlparse.urlparse(SITE_ALTS[site_key])
         link = link.replace(hostname, SITE_ALTS[site_key]) + params
 
         # If a scheme is specified in the alternative, this results in a
         # replaced link that looks like "https://http://altservice.tld".
         # In this case, we can remove the original scheme from the result
         # and use the one specified for the alt.
         if parsed_alt.scheme:
             link = '//'.join(link.split('//')[1:])
 
         for prefix in SKIP_PREFIX:
-            link = link.replace(prefix, '//')
+            if parsed_alt.scheme:
+                link = link.replace(prefix, '')
+            else:
+                link = link.replace(prefix, '//')
         break
 
     return link
 
 
 def filter_link_args(link: str) -> str:
     """Filters out unnecessary URL args from a result link
@@ -245,52 +277,14 @@
     translation = current_app.config['TRANSLATIONS'][
        config.get_localization_lang()
     ]
     av_link.string = f'{translation["anon-view"]}'
     av_link['class'] = 'anon-view'
     result.append(av_link)
 
-
-def add_ip_card(html_soup: BeautifulSoup, ip: str) -> BeautifulSoup:
-    """Adds the client's IP address to the search results
-        if query contains keywords
-
-    Args:
-        html_soup: The parsed search result containing the keywords
-        ip: ip address of the client
-
-    Returns:
-        BeautifulSoup
-
-    """
-    main_div = html_soup.select_one('#main')
-    if main_div:
-        # HTML IP card tag
-        ip_tag = html_soup.new_tag('div')
-        ip_tag['class'] = 'ZINbbc xpd O9g5cc uUPGi'
-
-        # For IP Address html tag
-        ip_address = html_soup.new_tag('div')
-        ip_address['class'] = 'kCrYT ip-address-div'
-        ip_address.string = ip
-
-        # Text below the IP address
-        ip_text = html_soup.new_tag('div')
-        ip_text.string = 'Your public IP address'
-        ip_text['class'] = 'kCrYT ip-text-div'
-
-        # Adding all the above html tags to the IP card
-        ip_tag.append(ip_address)
-        ip_tag.append(ip_text)
-
-        # Insert the element at the top of the result list
-        main_div.insert_before(ip_tag)
-    return html_soup
-
-
 def check_currency(response: str) -> dict:
     """Check whether the results have currency conversion
 
     Args:
         response: Search query Result
 
     Returns:
```

### Comparing `whoogle-search-0.8.1/app/utils/search.py` & `whoogle-search-0.8.2/app/utils/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import os
 import re
 from typing import Any
-
 from app.filter import Filter
 from app.request import gen_query
 from app.utils.misc import get_proxy_host_url
 from app.utils.results import get_first_link
 from bs4 import BeautifulSoup as bsoup
 from cryptography.fernet import Fernet, InvalidToken
 from flask import g
@@ -61,14 +60,15 @@
         self.request = request
         self.request_params = request.args if method == 'GET' else request.form
         self.user_agent = request.headers.get('User-Agent')
         self.feeling_lucky = False
         self.config = config
         self.session_key = session_key
         self.query = ''
+        self.widget = ''
         self.cookies_disabled = cookies_disabled
         self.search_type = self.request_params.get(
             'tbm') if 'tbm' in self.request_params else ''
 
     def __getitem__(self, name) -> Any:
         return getattr(self, name)
 
@@ -101,14 +101,19 @@
                 q = Fernet(self.session_key).decrypt(q.encode()).decode()
             except InvalidToken:
                 pass
 
         # Strip leading '! ' for "feeling lucky" queries
         self.feeling_lucky = q.startswith('! ')
         self.query = q[2:] if self.feeling_lucky else q
+        # Check for possible widgets
+        self.widget = "ip" if re.search("([^a-z0-9]|^)my *[^a-z0-9] *(ip|internet protocol)" +
+                        "($|( *[^a-z0-9] *(((addres|address|adres|" +
+                        "adress)|a)? *$)))", self.query.lower()) else self.widget
+        self.widget = 'calculator' if re.search("calculator|calc|calclator|math", self.query.lower()) else self.widget
         return self.query
 
     def generate_response(self) -> str:
         """Generates a response for the user's query
 
         Returns:
             str: A string response to the search query, in the form of a URL
@@ -138,15 +143,16 @@
                       and self.config.view_image
                       and not g.user_request.mobile)
 
         get_body = g.user_request.send(query=full_query,
                                        force_mobile=view_image)
 
         # Produce cleanable html soup from response
-        html_soup = bsoup(get_body.text, 'html.parser')
+        get_body_safed = get_body.text.replace("&lt;","andlt;").replace("&gt;","andgt;")
+        html_soup = bsoup(get_body_safed, 'html.parser')
 
         # Replace current soup if view_image is active
         if view_image:
             html_soup = content_filter.view_image(html_soup)
 
         # Indicate whether or not a Tor connection is active
         if g.user_request.tor_valid:
@@ -167,17 +173,7 @@
                 if 'search?' not in link['href'] or link['href'].index(
                         'search?') > 1:
                     continue
                 link['href'] += param_str
 
             return str(formatted_results)
 
-    def check_kw_ip(self) -> re.Match:
-        """Checks for keywords related to 'my ip' in the query
-
-        Returns:
-            bool
-
-        """
-        return re.search("([^a-z0-9]|^)my *[^a-z0-9] *(ip|internet protocol)" +
-                         "($|( *[^a-z0-9] *(((addres|address|adres|" +
-                         "adress)|a)? *$)))", self.query.lower())
```

### Comparing `whoogle-search-0.8.1/app/utils/session.py` & `whoogle-search-0.8.2/app/utils/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cryptography.fernet import Fernet
 from flask import current_app as app
 
-REQUIRED_SESSION_VALUES = ['uuid', 'config', 'key']
+REQUIRED_SESSION_VALUES = ['uuid', 'config', 'key', 'auth']
 
 
 def generate_key() -> bytes:
     """Generates a key for encrypting searches and element URLs
 
     Args:
         cookies_disabled: Flag for whether or not cookies are disabled by the
```

### Comparing `whoogle-search-0.8.1/requirements.txt` & `whoogle-search-0.8.2/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-attrs==19.3.0
-beautifulsoup4==4.10.0
+attrs==22.2.0
+beautifulsoup4==4.11.2
 brotli==1.0.9
-cachelib==0.4.1
+cachelib==0.10.2
 certifi==2022.12.7
-cffi==1.15.0
-chardet==3.0.4
-click==8.0.3
-cryptography==3.3.2
-cssutils==2.4.0
+cffi==1.15.1
+chardet==5.1.0
+click==8.1.3
+cryptography==3.3.2; platform_machine == 'armv7l'
+cryptography==39.0.1; platform_machine != 'armv7l'
+cssutils==2.6.0
 defusedxml==0.7.1
-Flask==1.1.1
-idna==2.9
-itsdangerous==1.1.0
-Jinja2==2.11.3
-MarkupSafe==1.1.1
-more-itertools==8.3.0
-packaging==20.4
-pluggy==0.13.1
-pycodestyle==2.6.0
+Flask==2.2.3
+idna==3.4
+itsdangerous==2.1.2
+Jinja2==3.1.2
+MarkupSafe==2.1.2
+more-itertools==9.0.0
+packaging==23.0
+pluggy==1.0.0
+pycodestyle==2.10.0
 pycparser==2.21
-pyOpenSSL==19.1.0
-pyparsing==2.4.7
+pyOpenSSL==19.1.0; platform_machine == 'armv7l'
+pyOpenSSL==23.0.0; platform_machine != 'armv7l'
+pyparsing==3.0.9
 PySocks==1.7.1
-pytest==7.2.0
-python-dateutil==2.8.1
-requests==2.25.1
-soupsieve==1.9.5
-stem==1.8.0
-urllib3==1.26.5
+pytest==7.2.1
+python-dateutil==2.8.2
+requests==2.28.2
+soupsieve==2.4
+stem==1.8.1
+urllib3==1.26.14
 waitress==2.1.2
-wcwidth==0.1.9
-Werkzeug==0.16.0
-python-dotenv==0.16.0
+wcwidth==0.2.6
+Werkzeug==2.2.3
+python-dotenv==0.21.1
```

### Comparing `whoogle-search-0.8.1/setup.cfg` & `whoogle-search-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/test/test_misc.py` & `whoogle-search-0.8.2/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/test/test_results.py` & `whoogle-search-0.8.2/test/test_results.py`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/test/test_routes.py` & `whoogle-search-0.8.2/test/test_routes.py`

 * *Files identical despite different names*

### Comparing `whoogle-search-0.8.1/whoogle_search.egg-info/PKG-INFO` & `whoogle-search-0.8.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: whoogle-search
-Version: 0.8.1
-Summary: Self-hosted, ad-free, privacy-respecting metasearch engine
-Home-page: https://github.com/benbusby/whoogle-search
-Author: Ben Busby
-Author-email: contact@benbusby.com
-License: MIT
-Keywords: search,metasearch,flask,adblock,degoogle,privacy
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-License-File: LICENSE
-
 ![Whoogle Search](docs/banner.png)
 
 [![Latest Release](https://img.shields.io/github/v/release/benbusby/whoogle-search)](https://github.com/benbusby/shoogle/releases)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![tests](https://github.com/benbusby/whoogle-search/actions/workflows/tests.yml/badge.svg)](https://github.com/benbusby/whoogle-search/actions/workflows/tests.yml)
 [![buildx](https://github.com/benbusby/whoogle-search/actions/workflows/buildx.yml/badge.svg)](https://github.com/benbusby/whoogle-search/actions/workflows/buildx.yml)
 [![codebeat badge](https://codebeat.co/badges/e96cada2-fb6f-4528-8285-7d72abd74e8d)](https://codebeat.co/projects/github-com-benbusby-shoogle-master)
@@ -31,25 +14,25 @@
   </tr>
 </table>
 
 Get Google search results, but without any ads, javascript, AMP links, cookies, or IP address tracking. Easily deployable in one click as a Docker app, and customizable with a single config file. Quick and simple to implement as a primary search engine replacement on both desktop and mobile.
 
 Contents
 1. [Features](#features)
-2. [Dependencies](#dependencies)
-3. [Install/Deploy](#install)
-    1. [Heroku Quick Deploy](#a-heroku-quick-deploy)
-    2. [Repl.it](#b-replit)
-    3. [Fly.io](#c-flyio)
-    4. [pipx](#d-pipx)
-    5. [pip](#e-pip)
-    6. [Manual](#f-manual)
-    7. [Docker](#g-manual-docker)
-    8. [Arch/AUR](#arch-linux--arch-based-distributions)
-    9. [Helm/Kubernetes](#helm-chart-for-kubernetes)
+3. [Install/Deploy Options](#install)
+    1. [Heroku Quick Deploy](#heroku-quick-deploy)
+    1. [Repl.it](#replit)
+    1. [Fly.io](#flyio)
+    1. [Koyeb](#koyeb)
+    1. [pipx](#pipx)
+    1. [pip](#pip)
+    1. [Manual](#manual)
+    1. [Docker](#manual-docker)
+    1. [Arch/AUR](#arch-linux--arch-based-distributions)
+    1. [Helm/Kubernetes](#helm-chart-for-kubernetes)
 4. [Environment Variables and Configuration](#environment-variables)
 5. [Usage](#usage)
 6. [Extra Steps](#extra-steps)
     1. [Set Primary Search Engine](#set-whoogle-as-your-primary-search-engine)
     2. [Prevent Downtime (Heroku Only)](#prevent-downtime-heroku-only)
     3. [Manual HTTPS Enforcement](#https-enforcement)
     4. [Using with Firefox Containers](#using-with-firefox-containers)
@@ -81,75 +64,86 @@
 
 <sup>*No third party JavaScript. Whoogle can be used with JavaScript disabled, but if enabled, uses JavaScript for things like presenting search suggestions.</sup>
 
 <sup>**No third party cookies. Whoogle uses server side cookies (sessions) to store non-sensitive configuration settings such as theme, language, etc. Just like with JavaScript, cookies can be disabled and not affect Whoogle's search functionality.</sup>
 
 <sup>***If deployed to a remote server, or configured to send requests through a VPN, Tor, proxy, etc.</sup>
 
-## Dependencies
-If using Heroku Quick Deploy, **you can skip this section**.
-
-- Docker ([Windows](https://docs.docker.com/docker-for-windows/install/), [macOS](https://docs.docker.com/docker-for-mac/install/), [Ubuntu](https://docs.docker.com/engine/install/ubuntu/), [other Linux distros](https://docs.docker.com/engine/install/binaries/))
-  - Only needed if you intend on deploying the app as a Docker image
-- [Python3](https://www.python.org/downloads/)
-- `libcurl4-openssl-dev` and `libssl-dev`
-  - macOS: `brew install openssl curl-openssl`
-  - Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev`
-  - Arch: `pacman -S curl openssl`
-
 ## Install
 There are a few different ways to begin using the app, depending on your preferences:
 
-### A) [Heroku Quick Deploy](https://heroku.com/about)
+___
+
+### [Heroku Quick Deploy](https://heroku.com/about)
 [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/benbusby/whoogle-search/tree/main)
 
 Provides:
 - Easy Deployment of App
 - A HTTPS url (https://\<your app name\>.herokuapp.com)
 
 Notes:
 - Requires a **PAID** Heroku Account.
 - Sometimes has issues with auto-redirecting to `https`. Make sure to navigate to the `https` version of your app before adding as a default search engine.
 
-### B) [Repl.it](https://repl.it)
+___
+
+### [Repl.it](https://repl.it)
 [![Run on Repl.it](https://repl.it/badge/github/benbusby/whoogle-search)](https://repl.it/github/benbusby/whoogle-search)
 
 *Note: Requires a (free) Replit account*
 
 Provides:
 - Free deployment of app
 - Free HTTPS url (https://\<app name\>.\<username\>\.repl\.co)
     - Supports custom domains
 - Downtime after periods of inactivity \([solution 1](https://repl.it/talk/ask/use-this-pingmat1replco-just-enter/28821/101298), [solution 2](https://repl.it/talk/learn/How-to-use-and-setup-UptimeRobot/9003)\)
 
-### C) [Fly.io](https://fly.io)
+___
+
+### [Fly.io](https://fly.io)
 
 You will need a **PAID** [Fly.io](https://fly.io) account to deploy Whoogle.
 
 #### Install the CLI: https://fly.io/docs/hands-on/installing/
 
 #### Deploy the app
 
 ```bash
 flyctl auth login
 flyctl launch --image benbusby/whoogle-search:latest
 ```
 
+The first deploy won't succeed because the default `internal_port` is wrong.
+To fix this, open the generated `fly.toml` file, set `services.internal_port` to `5000` and run `flyctl launch` again.
+
 Your app is now available at `https://<app-name>.fly.dev`.
 
-### D) [pipx](https://github.com/pipxproject/pipx#install-pipx)
+___
+
+### [Koyeb](https://www.koyeb.com)
+
+Use one of the following guides to install Whoogle on Koyeb:
+
+1. Using GitHub: https://www.koyeb.com/docs/quickstart/deploy-with-git
+2. Using Docker: https://www.koyeb.com/docs/quickstart/deploy-a-docker-application
+
+___
+
+### [pipx](https://github.com/pipxproject/pipx#install-pipx)
 Persistent install:
 
 `pipx install git+https://github.com/benbusby/whoogle-search.git`
 
 Sandboxed temporary instance:
 
 `pipx run --spec git+https://github.com/benbusby/whoogle-search.git whoogle-search`
 
-### E) pip
+___
+
+### pip
 `pip install whoogle-search`
 
 ```bash
 $ whoogle-search --help
 usage: whoogle-search [-h] [--port <port number>] [--host <ip address>] [--debug] [--https-only] [--userpass <username:password>]
                       [--proxyauth <username:password>] [--proxytype <socks4|socks5|http>] [--proxyloc <location:port>]
 
@@ -168,18 +162,29 @@
   --proxytype <socks4|socks5|http>
                         Sets a proxy type for all connections (default None)
   --proxyloc <location:port>
                         Sets a proxy location for all connections (default None)
 ```
 See the [available environment variables](#environment-variables) for additional configuration.
 
-### F) Manual
+___
+
+### Manual
 
 *Note: `Content-Security-Policy` headers can be sent by Whoogle if you set `WHOOGLE_CSP`.*
 
+#### Dependencies
+- [Python3](https://www.python.org/downloads/)
+- `libcurl4-openssl-dev` and `libssl-dev`
+  - macOS: `brew install openssl curl-openssl`
+  - Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev`
+  - Arch: `pacman -S curl openssl`
+
+#### Install
+
 Clone the repo and run the following commands to start the app in a local-only environment:
 
 ```bash
 git clone https://github.com/benbusby/whoogle-search.git
 cd whoogle-search
 python3 -m venv venv
 source venv/bin/activate
@@ -205,15 +210,14 @@
 #Environment=WHOOGLE_PROXY_TYPE=<proxy type (http|https|proxy4|proxy5)
 #Environment=WHOOGLE_PROXY_LOC=<proxy host/ip>
 # Site alternative configurations, uncomment to enable
 # Note: If not set, the feature will still be available
 # with default values.
 #Environment=WHOOGLE_ALT_TW=farside.link/nitter
 #Environment=WHOOGLE_ALT_YT=farside.link/invidious
-#Environment=WHOOGLE_ALT_IG=farside.link/bibliogram/u
 #Environment=WHOOGLE_ALT_RD=farside.link/libreddit
 #Environment=WHOOGLE_ALT_MD=farside.link/scribe
 #Environment=WHOOGLE_ALT_TL=farside.link/lingva
 #Environment=WHOOGLE_ALT_IMG=farside.link/rimgo
 #Environment=WHOOGLE_ALT_WIKI=farside.link/wikiless
 #Environment=WHOOGLE_ALT_IMDB=farside.link/libremdb
 #Environment=WHOOGLE_ALT_QUORA=farside.link/quetre
@@ -285,15 +289,17 @@
        - `chmod 400 control.conf`
 
     5. Finally set the Tor environment variable and use password variable to 1, `WHOOGLE_CONFIG_TOR` and `WHOOGLE_TOR_USE_PASS`. Refer to the [Environment Variables](#environment-variables) section for more details.
        - These may be added to the systemd unit file or env file:
           - `WHOOGLE_CONFIG_TOR=1`
           - `WHOOGLE_TOR_USE_PASS=1`
 
-### G) Manual (Docker)
+___
+
+### Manual (Docker)
 1. Ensure the Docker daemon is running, and is accessible by your user account
   - To add user permissions, you can execute `sudo usermod -aG docker yourusername`
   - Running `docker ps` should return something besides an error. If you encounter an error saying the daemon isn't running, try `sudo systemctl start docker` (Linux) or ensure the docker tool is running (Windows/macOS).
 2. Clone and deploy the docker app using a method below:
 
 #### Docker CLI
 
@@ -346,24 +352,30 @@
 heroku container:release web
 heroku open
 ```
 
 This series of commands can take a while, but once you run it once, you shouldn't have to run it again. The final command, `heroku open` will launch a tab in your web browser, where you can test out Whoogle and even [set it as your primary search engine](https://github.com/benbusby/whoogle#set-whoogle-as-your-primary-search-engine).
 You may also edit environment variables from your app’s Settings tab in the Heroku Dashboard.
 
-#### Arch Linux & Arch-based Distributions
+___
+
+### Arch Linux & Arch-based Distributions
 There is an [AUR package available](https://aur.archlinux.org/packages/whoogle-git/), as well as a pre-built and daily updated package available at [Chaotic-AUR](https://chaotic.cx).
 
-#### Helm chart for Kubernetes
+___
+
+### Helm chart for Kubernetes
 To use the Kubernetes Helm Chart:
 1. Ensure you have [Helm](https://helm.sh/docs/intro/install/) `>=3.0.0` installed
 2. Clone this repository
 3. Update [charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired
 4. Run `helm install whoogle ./charts/whoogle`
 
+___
+
 #### Using your own server, or alternative container deployment
 There are other methods for deploying docker containers that are well outlined in [this article](https://rollout.io/blog/the-shortlist-of-docker-hosting/), but there are too many to describe set up for each here. Generally it should be about the same amount of effort as the Heroku deployment.
 
 Depending on your preferences, you can also deploy the app yourself on your own infrastructure. This route would require a few extra steps:
   - A server (I personally recommend [Digital Ocean](https://www.digitalocean.com/pricing/) or [Linode](https://www.linode.com/pricing/), their cheapest tiers will work fine)
   - Your own URL (I suppose this is optional, but recommended)
   - SSL certificates (free through [Let's Encrypt](https://letsencrypt.org/getting-started/))
@@ -386,15 +398,14 @@
 | WHOOGLE_PROXY_PASS   | The password of the proxy server.                                                         |
 | WHOOGLE_PROXY_TYPE   | The type of the proxy server. Can be "socks5", "socks4", or "http".                       |
 | WHOOGLE_PROXY_LOC    | The location of the proxy server (host or ip).                                            |
 | EXPOSE_PORT          | The port where Whoogle will be exposed.                                                   |
 | HTTPS_ONLY           | Enforce HTTPS. (See [here](https://github.com/benbusby/whoogle-search#https-enforcement)) |
 | WHOOGLE_ALT_TW       | The twitter.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_YT       | The youtube.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
-| WHOOGLE_ALT_IG       | The instagram.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_RD       | The reddit.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_TL       | The Google Translate alternative to use. This is used for all "translate ____" searches.  Set to "" to disable. |
 | WHOOGLE_ALT_MD       | The medium.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_IMG      | The imgur.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_WIKI     | The wikipedia.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
 | WHOOGLE_ALT_IMDB     | The imdb.com alternative to use when site alternatives are enabled in the config. Set to "" to disable.  |
 | WHOOGLE_ALT_QUORA    | The quora.com alternative to use when site alternatives are enabled in the config. Set to "" to disable. |
@@ -412,14 +423,16 @@
 | Variable                             | Description                                                     |
 | ------------------------------------ | --------------------------------------------------------------- |
 | WHOOGLE_CONFIG_DISABLE               | Hide config from UI and disallow changes to config by client    |
 | WHOOGLE_CONFIG_COUNTRY               | Filter results by hosting country                               |
 | WHOOGLE_CONFIG_LANGUAGE              | Set interface language                                          |
 | WHOOGLE_CONFIG_SEARCH_LANGUAGE       | Set search result language                                      |
 | WHOOGLE_CONFIG_BLOCK                 | Block websites from search results (use comma-separated list)   |
+| WHOOGLE_CONFIG_BLOCK_TITLE           | Block search result with a REGEX filter on title                |
+| WHOOGLE_CONFIG_BLOCK_URL             | Block search result with a REGEX filter on URL                  |
 | WHOOGLE_CONFIG_THEME                 | Set theme mode (light, dark, or system)                         |
 | WHOOGLE_CONFIG_SAFE                  | Enable safe searches                                            |
 | WHOOGLE_CONFIG_ALTS                  | Use social media site alternatives (nitter, invidious, etc)     |
 | WHOOGLE_CONFIG_NEAR                  | Restrict results to only those near a particular city           |
 | WHOOGLE_CONFIG_TOR                   | Use Tor routing (if available)                                  |
 | WHOOGLE_CONFIG_NEW_TAB               | Always open results in new tab                                  |
 | WHOOGLE_CONFIG_VIEW_IMAGE            | Enable View Image option                                        |
@@ -606,29 +619,31 @@
 | [https://search.garudalinux.org](https://search.garudalinux.org) | 🇫🇮 FI | Multi-choice | ✅ |
 | [https://search.dr460nf1r3.org](https://search.dr460nf1r3.org) | 🇩🇪 DE | Multi-choice | ✅ |
 | [https://s.tokhmi.xyz](https://s.tokhmi.xyz) | 🇺🇸 US | Multi-choice | ✅ |
 | [https://search.sethforprivacy.com](https://search.sethforprivacy.com) | 🇩🇪 DE | English | |
 | [https://whoogle.dcs0.hu](https://whoogle.dcs0.hu) | 🇭🇺 HU | Multi-choice | |
 | [https://whoogle.esmailelbob.xyz](https://whoogle.esmailelbob.xyz) | 🇨🇦 CA | Multi-choice | |
 | [https://gowogle.voring.me](https://gowogle.voring.me) | 🇺🇸 US | Multi-choice | |
-| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | 🇺🇸 US | English | |
+| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | 🇳🇱 NL | English | |
 | [https://wg.vern.cc](https://wg.vern.cc) | 🇺🇸 US | English |  |
-| [https://www.indexia.gq](https://www.indexia.gq) | 🇨🇦 CA | Multi-choice | ✅ |
+| [https://whoogle.hxvy0.gq](https://whoogle.hxvy0.gq) | 🇨🇦 CA | Turkish Only | ✅ |
 | [https://whoogle.hostux.net](https://whoogle.hostux.net) | 🇫🇷 FR | Multi-choice | |
+| [https://whoogle.lunar.icu](https://whoogle.lunar.icu) | 🇩🇪 DE | Multi-choice | ✅ |
+| [https://wgl.frail.duckdns.org](https://wgl.frail.duckdns.org) | 🇧🇷 BR | Multi-choice | |
 
 * A checkmark in the "Cloudflare" category here refers to the use of the reverse proxy, [Cloudflare](https://cloudflare.com). The checkmark will not be listed for a site which uses Cloudflare DNS but rather the proxying service which grants Cloudflare the ability to monitor traffic to the website.
 
 #### Onion Instances
 
 | Website | Country | Language |
 |-|-|-|
 | [http://whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion](http://whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion) | 🇺🇸 US |  Multi-choice
 | [http://nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion](http://nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion) | 🇩🇪 DE |  English
 | [http://whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/) | 🇺🇸 US | English |
-| [http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) | 🇺🇸 US | English |
+| [http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) | 🇳🇱 NL | English |
 
 #### I2P Instances
 
 | Website | Country | Language |
 |-|-|-|
 | [http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p](http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p) | 🇺🇸 US | English |
```

#### html2text {}

```diff
@@ -1,127 +1,120 @@
-Metadata-Version: 2.1 Name: whoogle-search Version: 0.8.1 Summary: Self-hosted,
-ad-free, privacy-respecting metasearch engine Home-page: https://github.com/
-benbusby/whoogle-search Author: Ben Busby Author-email: contact@benbusby.com
-License: MIT Keywords: search,metasearch,flask,adblock,degoogle,privacy
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
-dev License-File: LICENSE ![Whoogle Search](docs/banner.png) [![Latest Release]
-(https://img.shields.io/github/v/release/benbusby/whoogle-search)](https://
-github.com/benbusby/shoogle/releases) [![License: MIT](https://img.shields.io/
-badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![tests]
-(https://github.com/benbusby/whoogle-search/actions/workflows/tests.yml/
+![Whoogle Search](docs/banner.png) [![Latest Release](https://img.shields.io/
+github/v/release/benbusby/whoogle-search)](https://github.com/benbusby/shoogle/
+releases) [![License: MIT](https://img.shields.io/badge/License-MIT-
+yellow.svg)](https://opensource.org/licenses/MIT) [![tests](https://github.com/
+benbusby/whoogle-search/actions/workflows/tests.yml/badge.svg)](https://
+github.com/benbusby/whoogle-search/actions/workflows/tests.yml) [![buildx]
+(https://github.com/benbusby/whoogle-search/actions/workflows/buildx.yml/
 badge.svg)](https://github.com/benbusby/whoogle-search/actions/workflows/
-tests.yml) [![buildx](https://github.com/benbusby/whoogle-search/actions/
-workflows/buildx.yml/badge.svg)](https://github.com/benbusby/whoogle-search/
-actions/workflows/buildx.yml) [![codebeat badge](https://codebeat.co/badges/
-e96cada2-fb6f-4528-8285-7d72abd74e8d)](https://codebeat.co/projects/github-com-
-benbusby-shoogle-master) [![Docker Pulls](https://img.shields.io/docker/pulls/
-benbusby/whoogle-search)](https://hub.docker.com/r/benbusby/whoogle-search)
+buildx.yml) [![codebeat badge](https://codebeat.co/badges/e96cada2-fb6f-4528-
+8285-7d72abd74e8d)](https://codebeat.co/projects/github-com-benbusby-shoogle-
+master) [![Docker Pulls](https://img.shields.io/docker/pulls/benbusby/whoogle-
+search)](https://hub.docker.com/r/benbusby/whoogle-search)
 SourceHut GitHub
 Get Google search results, but without any ads, javascript, AMP links, cookies,
 or IP address tracking. Easily deployable in one click as a Docker app, and
 customizable with a single config file. Quick and simple to implement as a
 primary search engine replacement on both desktop and mobile. Contents 1.
-[Features](#features) 2. [Dependencies](#dependencies) 3. [Install/Deploy]
-(#install) 1. [Heroku Quick Deploy](#a-heroku-quick-deploy) 2. [Repl.it](#b-
-replit) 3. [Fly.io](#c-flyio) 4. [pipx](#d-pipx) 5. [pip](#e-pip) 6. [Manual]
-(#f-manual) 7. [Docker](#g-manual-docker) 8. [Arch/AUR](#arch-linux--arch-
-based-distributions) 9. [Helm/Kubernetes](#helm-chart-for-kubernetes) 4.
-[Environment Variables and Configuration](#environment-variables) 5. [Usage]
-(#usage) 6. [Extra Steps](#extra-steps) 1. [Set Primary Search Engine](#set-
-whoogle-as-your-primary-search-engine) 2. [Prevent Downtime (Heroku Only)]
-(#prevent-downtime-heroku-only) 3. [Manual HTTPS Enforcement](#https-
-enforcement) 4. [Using with Firefox Containers](#using-with-firefox-containers)
-5. [Reverse Proxying](#reverse-proxying) 1. [Nginx](#nginx) 7. [Contributing]
-(#contributing) 8. [FAQ](#faq) 9. [Public Instances](#public-instances) 10.
-[Screenshots](#screenshots) ## Features - No ads or sponsored content - No
-JavaScript\* - No cookies\*\* - No tracking/linking of your personal IP
-address\*\*\* - No AMP links - No URL tracking tags (i.e. utm=%s) - No referrer
-header - Tor and HTTP/SOCKS proxy support - Autocomplete/search suggestions -
-POST request search and suggestion queries (when possible) - View images at
-full res without site redirect (currently mobile only) - Light/Dark/System
-theme modes (with support for [custom CSS theming](https://github.com/benbusby/
-whoogle-search/wiki/User-Contributed-CSS-Themes)) - Randomly generated User
-Agent - Easy to install/deploy - DDG-style bang (i.e. `! `) searches - Optional
-location-based searching (i.e. results near \
+[Features](#features) 3. [Install/Deploy Options](#install) 1. [Heroku Quick
+Deploy](#heroku-quick-deploy) 1. [Repl.it](#replit) 1. [Fly.io](#flyio) 1.
+[Koyeb](#koyeb) 1. [pipx](#pipx) 1. [pip](#pip) 1. [Manual](#manual) 1.
+[Docker](#manual-docker) 1. [Arch/AUR](#arch-linux--arch-based-distributions)
+1. [Helm/Kubernetes](#helm-chart-for-kubernetes) 4. [Environment Variables and
+Configuration](#environment-variables) 5. [Usage](#usage) 6. [Extra Steps]
+(#extra-steps) 1. [Set Primary Search Engine](#set-whoogle-as-your-primary-
+search-engine) 2. [Prevent Downtime (Heroku Only)](#prevent-downtime-heroku-
+only) 3. [Manual HTTPS Enforcement](#https-enforcement) 4. [Using with Firefox
+Containers](#using-with-firefox-containers) 5. [Reverse Proxying](#reverse-
+proxying) 1. [Nginx](#nginx) 7. [Contributing](#contributing) 8. [FAQ](#faq) 9.
+[Public Instances](#public-instances) 10. [Screenshots](#screenshots) ##
+Features - No ads or sponsored content - No JavaScript\* - No cookies\*\* - No
+tracking/linking of your personal IP address\*\*\* - No AMP links - No URL
+tracking tags (i.e. utm=%s) - No referrer header - Tor and HTTP/SOCKS proxy
+support - Autocomplete/search suggestions - POST request search and suggestion
+queries (when possible) - View images at full res without site redirect
+(currently mobile only) - Light/Dark/System theme modes (with support for
+[custom CSS theming](https://github.com/benbusby/whoogle-search/wiki/User-
+Contributed-CSS-Themes)) - Randomly generated User Agent - Easy to install/
+deploy - DDG-style bang (i.e. `! `) searches - Optional location-based
+searching (i.e. results near \
 >) - Optional NoJS mode to view search results in a separate window with
 JavaScript blocked *No third party JavaScript. Whoogle can be used with
 JavaScript disabled, but if enabled, uses JavaScript for things like presenting
 search suggestions. **No third party cookies. Whoogle uses server side cookies
 (sessions) to store non-sensitive configuration settings such as theme,
 language, etc. Just like with JavaScript, cookies can be disabled and not
 affect Whoogle's search functionality. ***If deployed to a remote server, or
-configured to send requests through a VPN, Tor, proxy, etc. ## Dependencies If
-using Heroku Quick Deploy, **you can skip this section**. - Docker ([Windows]
-(https://docs.docker.com/docker-for-windows/install/), [macOS](https://
-docs.docker.com/docker-for-mac/install/), [Ubuntu](https://docs.docker.com/
-engine/install/ubuntu/), [other Linux distros](https://docs.docker.com/engine/
-install/binaries/)) - Only needed if you intend on deploying the app as a
-Docker image - [Python3](https://www.python.org/downloads/) - `libcurl4-
-openssl-dev` and `libssl-dev` - macOS: `brew install openssl curl-openssl` -
-Ubuntu: `sudo apt-get install -y libcurl4-openssl-dev libssl-dev` - Arch:
-`pacman -S curl openssl` ## Install There are a few different ways to begin
-using the app, depending on your preferences: ### A) [Heroku Quick Deploy]
-(https://heroku.com/about) [![Deploy](https://www.herokucdn.com/deploy/
-button.svg)](https://heroku.com/deploy?template=https://github.com/benbusby/
-whoogle-search/tree/main) Provides: - Easy Deployment of App - A HTTPS url
-(https://\
+configured to send requests through a VPN, Tor, proxy, etc. ## Install There
+are a few different ways to begin using the app, depending on your preferences:
+___ ### [Heroku Quick Deploy](https://heroku.com/about) [![Deploy](https://
+www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https:
+//github.com/benbusby/whoogle-search/tree/main) Provides: - Easy Deployment of
+App - A HTTPS url (https://\
 >.herokuapp.com) Notes: - Requires a **PAID** Heroku Account. - Sometimes has
 issues with auto-redirecting to `https`. Make sure to navigate to the `https`
-version of your app before adding as a default search engine. ### B) [Repl.it]
+version of your app before adding as a default search engine. ___ ### [Repl.it]
 (https://repl.it) [![Run on Repl.it](https://repl.it/badge/github/benbusby/
 whoogle-search)](https://repl.it/github/benbusby/whoogle-search) *Note:
 Requires a (free) Replit account* Provides: - Free deployment of app - Free
 HTTPS url (https://\
 >.\
 >\.repl\.co) - Supports custom domains - Downtime after periods of inactivity \
 ([solution 1](https://repl.it/talk/ask/use-this-pingmat1replco-just-enter/
 28821/101298), [solution 2](https://repl.it/talk/learn/How-to-use-and-setup-
-UptimeRobot/9003)\) ### C) [Fly.io](https://fly.io) You will need a **PAID**
+UptimeRobot/9003)\) ___ ### [Fly.io](https://fly.io) You will need a **PAID**
 [Fly.io](https://fly.io) account to deploy Whoogle. #### Install the CLI:
 https://fly.io/docs/hands-on/installing/ #### Deploy the app ```bash flyctl
-auth login flyctl launch --image benbusby/whoogle-search:latest ``` Your app is
-now available at `https://.fly.dev`. ### D) [pipx](https://github.com/
-pipxproject/pipx#install-pipx) Persistent install: `pipx install git+https://
-github.com/benbusby/whoogle-search.git` Sandboxed temporary instance: `pipx run
---spec git+https://github.com/benbusby/whoogle-search.git whoogle-search` ###
-E) pip `pip install whoogle-search` ```bash $ whoogle-search --help usage:
-whoogle-search [-h] [--port ] [--host ] [--debug] [--https-only] [--userpass ]
-[--proxyauth ] [--proxytype
+auth login flyctl launch --image benbusby/whoogle-search:latest ``` The first
+deploy won't succeed because the default `internal_port` is wrong. To fix this,
+open the generated `fly.toml` file, set `services.internal_port` to `5000` and
+run `flyctl launch` again. Your app is now available at `https://.fly.dev`. ___
+### [Koyeb](https://www.koyeb.com) Use one of the following guides to install
+Whoogle on Koyeb: 1. Using GitHub: https://www.koyeb.com/docs/quickstart/
+deploy-with-git 2. Using Docker: https://www.koyeb.com/docs/quickstart/deploy-
+a-docker-application ___ ### [pipx](https://github.com/pipxproject/
+pipx#install-pipx) Persistent install: `pipx install git+https://github.com/
+benbusby/whoogle-search.git` Sandboxed temporary instance: `pipx run --spec
+git+https://github.com/benbusby/whoogle-search.git whoogle-search` ___ ### pip
+`pip install whoogle-search` ```bash $ whoogle-search --help usage: whoogle-
+search [-h] [--port ] [--host ] [--debug] [--https-only] [--userpass ] [--
+proxyauth ] [--proxytype
 socks5|http>] [--proxyloc ] Whoogle Search console runner optional arguments: -
 h, --help Show this help message and exit --port  Specifies a port to run on
 (default 5000) --host  Specifies the host address to use (default 127.0.0.1) --
 debug Activates debug mode for the server (default False) --https-only Enforces
 HTTPS redirects for all requests --userpass  Sets a username/password basic
 auth combo (default None) --proxyauth  Sets a username/password for a HTTP/
 SOCKS proxy (default None) --proxytype
 socks5|http> Sets a proxy type for all connections (default None) --proxyloc
 Sets a proxy location for all connections (default None) ``` See the [available
 environment variables](#environment-variables) for additional configuration.
-### F) Manual *Note: `Content-Security-Policy` headers can be sent by Whoogle
-if you set `WHOOGLE_CSP`.* Clone the repo and run the following commands to
-start the app in a local-only environment: ```bash git clone https://
-github.com/benbusby/whoogle-search.git cd whoogle-search python3 -m venv venv
-source venv/bin/activate pip install -r requirements.txt ./run ``` See the
-[available environment variables](#environment-variables) for additional
-configuration. #### systemd Configuration After building the virtual
-environment, you can add something like the following to `/lib/systemd/system/
-whoogle.service` to set up a Whoogle Search systemd service: ```ini [Unit]
-Description=Whoogle [Service] # Basic auth configuration, uncomment to enable
-#Environment=WHOOGLE_USER= #Environment=WHOOGLE_PASS= # Proxy configuration,
-uncomment to enable #Environment=WHOOGLE_PROXY_USER=
-#Environment=WHOOGLE_PROXY_PASS= #Environment=WHOOGLE_PROXY_TYPE=
+___ ### Manual *Note: `Content-Security-Policy` headers can be sent by Whoogle
+if you set `WHOOGLE_CSP`.* #### Dependencies - [Python3](https://
+www.python.org/downloads/) - `libcurl4-openssl-dev` and `libssl-dev` - macOS:
+`brew install openssl curl-openssl` - Ubuntu: `sudo apt-get install -
+y libcurl4-openssl-dev libssl-dev` - Arch: `pacman -S curl openssl` ####
+Install Clone the repo and run the following commands to start the app in a
+local-only environment: ```bash git clone https://github.com/benbusby/whoogle-
+search.git cd whoogle-search python3 -m venv venv source venv/bin/activate pip
+install -r requirements.txt ./run ``` See the [available environment variables]
+(#environment-variables) for additional configuration. #### systemd
+Configuration After building the virtual environment, you can add something
+like the following to `/lib/systemd/system/whoogle.service` to set up a Whoogle
+Search systemd service: ```ini [Unit] Description=Whoogle [Service] # Basic
+auth configuration, uncomment to enable #Environment=WHOOGLE_USER=
+#Environment=WHOOGLE_PASS= # Proxy configuration, uncomment to enable
+#Environment=WHOOGLE_PROXY_USER= #Environment=WHOOGLE_PROXY_PASS=
+#Environment=WHOOGLE_PROXY_TYPE=
 http|https|proxy4|proxy5) #Environment=WHOOGLE_PROXY_LOC=
 p> # Site alternative configurations, uncomment to enable # Note: If not set,
 the feature will still be available # with default values.
 #Environment=WHOOGLE_ALT_TW=farside.link/nitter
 #Environment=WHOOGLE_ALT_YT=farside.link/invidious
-#Environment=WHOOGLE_ALT_IG=farside.link/bibliogram/
-u #Environment=WHOOGLE_ALT_RD=farside.link/libreddit
+#Environment=WHOOGLE_ALT_RD=farside.link/libreddit
 #Environment=WHOOGLE_ALT_MD=farside.link/scribe
 #Environment=WHOOGLE_ALT_TL=farside.link/lingva
 #Environment=WHOOGLE_ALT_IMG=farside.link/rimgo
 #Environment=WHOOGLE_ALT_WIKI=farside.link/wikiless
 #Environment=WHOOGLE_ALT_IMDB=farside.link/libremdb
 #Environment=WHOOGLE_ALT_QUORA=farside.link/quetre # Load values from dotenv
 only #Environment=WHOOGLE_DOTENV=1 Type=simple User= # If installed as a
@@ -159,15 +152,15 @@
 the `WHOOGLE_TOR_CONF` environment variable. Refer to the [Environment
 Variables](#environment-variables) section for more details. 4. Heavily
 restrict access to control.conf to only be readable by the user running
 whoogle: - `chmod 400 control.conf` 5. Finally set the Tor environment variable
 and use password variable to 1, `WHOOGLE_CONFIG_TOR` and
 `WHOOGLE_TOR_USE_PASS`. Refer to the [Environment Variables](#environment-
 variables) section for more details. - These may be added to the systemd unit
-file or env file: - `WHOOGLE_CONFIG_TOR=1` - `WHOOGLE_TOR_USE_PASS=1` ### G)
+file or env file: - `WHOOGLE_CONFIG_TOR=1` - `WHOOGLE_TOR_USE_PASS=1` ___ ###
 Manual (Docker) 1. Ensure the Docker daemon is running, and is accessible by
 your user account - To add user permissions, you can execute `sudo usermod -aG
 docker yourusername` - Running `docker ps` should return something besides an
 error. If you encounter an error saying the daemon isn't running, try `sudo
 systemctl start docker` (Linux) or ensure the docker tool is running (Windows/
 macOS). 2. Clone and deploy the docker app using a method below: #### Docker
 CLI Through Docker Hub: ```bash docker pull benbusby/whoogle-search docker run
@@ -188,22 +181,22 @@
 https://github.com/benbusby/whoogle-search.git cd whoogle-search heroku create
 heroku container:push web heroku container:release web heroku open ``` This
 series of commands can take a while, but once you run it once, you shouldn't
 have to run it again. The final command, `heroku open` will launch a tab in
 your web browser, where you can test out Whoogle and even [set it as your
 primary search engine](https://github.com/benbusby/whoogle#set-whoogle-as-your-
 primary-search-engine). You may also edit environment variables from your
-appâs Settings tab in the Heroku Dashboard. #### Arch Linux & Arch-based
+appâs Settings tab in the Heroku Dashboard. ___ ### Arch Linux & Arch-based
 Distributions There is an [AUR package available](https://aur.archlinux.org/
 packages/whoogle-git/), as well as a pre-built and daily updated package
-available at [Chaotic-AUR](https://chaotic.cx). #### Helm chart for Kubernetes
-To use the Kubernetes Helm Chart: 1. Ensure you have [Helm](https://helm.sh/
-docs/intro/install/) `>=3.0.0` installed 2. Clone this repository 3. Update
-[charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired 4. Run
-`helm install whoogle ./charts/whoogle` #### Using your own server, or
+available at [Chaotic-AUR](https://chaotic.cx). ___ ### Helm chart for
+Kubernetes To use the Kubernetes Helm Chart: 1. Ensure you have [Helm](https://
+helm.sh/docs/intro/install/) `>=3.0.0` installed 2. Clone this repository 3.
+Update [charts/whoogle/values.yaml](./charts/whoogle/values.yaml) as desired 4.
+Run `helm install whoogle ./charts/whoogle` ___ #### Using your own server, or
 alternative container deployment There are other methods for deploying docker
 containers that are well outlined in [this article](https://rollout.io/blog/
 the-shortlist-of-docker-hosting/), but there are too many to describe set up
 for each here. Generally it should be about the same amount of effort as the
 Heroku deployment. Depending on your preferences, you can also deploy the app
 yourself on your own infrastructure. This route would require a few extra
 steps: - A server (I personally recommend [Digital Ocean](https://
@@ -228,23 +221,21 @@
 proxy server. Can be "socks5", "socks4", or "http". | | WHOOGLE_PROXY_LOC | The
 location of the proxy server (host or ip). | | EXPOSE_PORT | The port where
 Whoogle will be exposed. | | HTTPS_ONLY | Enforce HTTPS. (See [here](https://
 github.com/benbusby/whoogle-search#https-enforcement)) | | WHOOGLE_ALT_TW | The
 twitter.com alternative to use when site alternatives are enabled in the
 config. Set to "" to disable. | | WHOOGLE_ALT_YT | The youtube.com alternative
 to use when site alternatives are enabled in the config. Set to "" to disable.
-| | WHOOGLE_ALT_IG | The instagram.com alternative to use when site
-alternatives are enabled in the config. Set to "" to disable. | |
-WHOOGLE_ALT_RD | The reddit.com alternative to use when site alternatives are
-enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_TL | The Google
-Translate alternative to use. This is used for all "translate ____" searches.
-Set to "" to disable. | | WHOOGLE_ALT_MD | The medium.com alternative to use
-when site alternatives are enabled in the config. Set to "" to disable. | |
-WHOOGLE_ALT_IMG | The imgur.com alternative to use when site alternatives are
-enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_WIKI | The
+| | WHOOGLE_ALT_RD | The reddit.com alternative to use when site alternatives
+are enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_TL | The
+Google Translate alternative to use. This is used for all "translate ____"
+searches. Set to "" to disable. | | WHOOGLE_ALT_MD | The medium.com alternative
+to use when site alternatives are enabled in the config. Set to "" to disable.
+| | WHOOGLE_ALT_IMG | The imgur.com alternative to use when site alternatives
+are enabled in the config. Set to "" to disable. | | WHOOGLE_ALT_WIKI | The
 wikipedia.com alternative to use when site alternatives are enabled in the
 config. Set to "" to disable. | | WHOOGLE_ALT_IMDB | The imdb.com alternative
 to use when site alternatives are enabled in the config. Set to "" to disable.
 | | WHOOGLE_ALT_QUORA | The quora.com alternative to use when site alternatives
 are enabled in the config. Set to "" to disable. | | WHOOGLE_AUTOCOMPLETE |
 Controls visibility of autocomplete/search suggestions. Default on -- use '0'
 to disable. | | WHOOGLE_MINIMAL | Remove everything except basic result cards
@@ -261,15 +252,17 @@
 instance to the same config state every time. | Variable | Description | | ----
 -------------------------------- | --------------------------------------------
 ------------------- | | WHOOGLE_CONFIG_DISABLE | Hide config from UI and
 disallow changes to config by client | | WHOOGLE_CONFIG_COUNTRY | Filter
 results by hosting country | | WHOOGLE_CONFIG_LANGUAGE | Set interface language
 | | WHOOGLE_CONFIG_SEARCH_LANGUAGE | Set search result language | |
 WHOOGLE_CONFIG_BLOCK | Block websites from search results (use comma-separated
-list) | | WHOOGLE_CONFIG_THEME | Set theme mode (light, dark, or system) | |
+list) | | WHOOGLE_CONFIG_BLOCK_TITLE | Block search result with a REGEX filter
+on title | | WHOOGLE_CONFIG_BLOCK_URL | Block search result with a REGEX filter
+on URL | | WHOOGLE_CONFIG_THEME | Set theme mode (light, dark, or system) | |
 WHOOGLE_CONFIG_SAFE | Enable safe searches | | WHOOGLE_CONFIG_ALTS | Use social
 media site alternatives (nitter, invidious, etc) | | WHOOGLE_CONFIG_NEAR |
 Restrict results to only those near a particular city | | WHOOGLE_CONFIG_TOR |
 Use Tor routing (if available) | | WHOOGLE_CONFIG_NEW_TAB | Always open results
 in new tab | | WHOOGLE_CONFIG_VIEW_IMAGE | Enable View Image option | |
 WHOOGLE_CONFIG_GET_ONLY | Search using GET requests only | | WHOOGLE_CONFIG_URL
 | The root url of the instance (`https:///`) | | WHOOGLE_CONFIG_STYLE | The
@@ -429,34 +422,37 @@
 search.dr460nf1r3.org) | ð©ðª DE | Multi-choice | â | | [https://
 s.tokhmi.xyz](https://s.tokhmi.xyz) | ðºð¸ US | Multi-choice | â | |
 [https://search.sethforprivacy.com](https://search.sethforprivacy.com) |
 ð©ðª DE | English | | | [https://whoogle.dcs0.hu](https://whoogle.dcs0.hu)
 | ð­ðº HU | Multi-choice | | | [https://whoogle.esmailelbob.xyz](https://
 whoogle.esmailelbob.xyz) | ð¨ð¦ CA | Multi-choice | | | [https://
 gowogle.voring.me](https://gowogle.voring.me) | ðºð¸ US | Multi-choice | |
-| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | ðºð¸
-US | English | | | [https://wg.vern.cc](https://wg.vern.cc) | ðºð¸ US |
-English | | | [https://www.indexia.gq](https://www.indexia.gq) | ð¨ð¦ CA |
-Multi-choice | â | | [https://whoogle.hostux.net](https://whoogle.hostux.net)
-|Â ð«ð· FR | Multi-choice | | * A checkmark in the "Cloudflare" category
-here refers to the use of the reverse proxy, [Cloudflare](https://
-cloudflare.com). The checkmark will not be listed for a site which uses
-Cloudflare DNS but rather the proxying service which grants Cloudflare the
-ability to monitor traffic to the website. #### Onion Instances | Website |
-Country | Language | |-|-|-| | [http://
+| [https://whoogle.privacydev.net](https://whoogle.privacydev.net) | ð³ð±
+NL | English | | | [https://wg.vern.cc](https://wg.vern.cc) | ðºð¸ US |
+English | | | [https://whoogle.hxvy0.gq](https://whoogle.hxvy0.gq) | ð¨ð¦
+CA | Turkish Only | â | | [https://whoogle.hostux.net](https://
+whoogle.hostux.net) |Â ð«ð· FR | Multi-choice | | | [https://
+whoogle.lunar.icu](https://whoogle.lunar.icu) | ð©ðª DE | Multi-choice |
+â | | [https://wgl.frail.duckdns.org](https://wgl.frail.duckdns.org) |
+ð§ð· BR | Multi-choice | | * A checkmark in the "Cloudflare" category here
+refers to the use of the reverse proxy, [Cloudflare](https://cloudflare.com).
+The checkmark will not be listed for a site which uses Cloudflare DNS but
+rather the proxying service which grants Cloudflare the ability to monitor
+traffic to the website. #### Onion Instances | Website | Country | Language |
+|-|-|-| | [http://
 whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion](http://
 whoglqjdkgt2an4tdepberwqz3hk7tjo4kqgdnuj77rt7nshw2xqhqad.onion) | ðºð¸ US |
 Multi-choice | [http://
 nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion](http://
 nuifgsnbb2mcyza74o7illtqmuaqbwu4flam3cdmsrnudwcmkqur37qd.onion) | ð©ðª DE |
 English | [http://
 whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion](http://
 whoogle.vernccvbvyi5qhfzyqengccj7lkove6bjot2xhh5kajhwvidqafczrad.onion/) |
 ðºð¸ US | English | | [http://
 whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion](http://
 whoogle.g4c3eya4clenolymqbpgwz3q3tawoxw56yhzk4vugqrl6dtu3ejvhjid.onion/) |
-ðºð¸ US | English | #### I2P Instances | Website | Country | Language | |-
+ð³ð± NL | English | #### I2P Instances | Website | Country | Language | |-
 |-|-| | [http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p]
 (http://verneks7rfjptpz5fpii7n7nrxilsidi2qxepeuuf66c3tsf4nhq.b32.i2p) |
 ðºð¸ US | English | ## Screenshots #### Desktop ![Whoogle Desktop](docs/
 screenshot_desktop.png) #### Mobile ![Whoogle Mobile](docs/
 screenshot_mobile.png)
```

### Comparing `whoogle-search-0.8.1/whoogle_search.egg-info/SOURCES.txt` & `whoogle-search-0.8.2/whoogle_search.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,17 @@
 app/static/js/header.js
 app/static/js/keyboard.js
 app/static/js/utils.js
 app/static/settings/countries.json
 app/static/settings/header_tabs.json
 app/static/settings/languages.json
 app/static/settings/themes.json
+app/static/settings/time_periods.json
 app/static/settings/translations.json
+app/static/widgets/calculator.html
 app/templates/display.html
 app/templates/error.html
 app/templates/footer.html
 app/templates/header.html
 app/templates/imageresults.html
 app/templates/index.html
 app/templates/logo.html
@@ -76,14 +78,15 @@
 app/templates/search.html
 app/utils/__init__.py
 app/utils/bangs.py
 app/utils/misc.py
 app/utils/results.py
 app/utils/search.py
 app/utils/session.py
+app/utils/widgets.py
 test/test_autocomplete.py
 test/test_misc.py
 test/test_results.py
 test/test_routes.py
 whoogle_search.egg-info/PKG-INFO
 whoogle_search.egg-info/SOURCES.txt
 whoogle_search.egg-info/dependency_links.txt
```

