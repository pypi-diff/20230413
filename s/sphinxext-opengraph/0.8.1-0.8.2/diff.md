# Comparing `tmp/sphinxext-opengraph-0.8.1.tar.gz` & `tmp/sphinxext-opengraph-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sphinxext-opengraph/sphinxext-opengraph/dist/.tmp-h2z7oqsm/sphinxext-opengraph-0.8.1.tar", last modified: Thu Feb  9 04:07:48 2023, max compression
+gzip compressed data, was "/home/runner/work/sphinxext-opengraph/sphinxext-opengraph/dist/.tmp-47iiha98/sphinxext-opengraph-0.8.2.tar", last modified: Thu Apr 13 13:34:17 2023, max compression
```

## Comparing `sphinxext-opengraph-0.8.1.tar` & `sphinxext-opengraph-0.8.2.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/docs/script/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/script/generate_social_card_previews.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/source/_static/og-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/docs/source/socialcards.md
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/_static/
--rw-r--r--   0 runner    (1001) docker     (123)  1755856 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/_static/Roboto-Flex.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/_static/sphinx-logo-shadow.png
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/descriptionparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/metaparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/socialcards.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/sphinxext/opengraph/titleparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-arbitrary-tags/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-arbitrary-tags/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-arbitrary-tags/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-custom-tags/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-custom-tags/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-custom-tags/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-description-length/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-description-length/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-description-length/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-double-spacing/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-double-spacing/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-double-spacing/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-first-image/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-first-image/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-first-image/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-first-image-no-image/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-first-image-no-image/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-first-image-no-image/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/img/
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/img/sample.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/sub/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/sub/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-list/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-list/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-list/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-local-image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-local-image/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-local-image/_static/sample.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-local-image/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-local-image/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description-manual-description/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description-manual-description/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description-manual-description/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description-manual-og-description/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description-manual-og-description/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-meta-name-description-manual-og-description/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-nested-lists/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-nested-lists/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-nested-lists/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-overrides-complex/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-overrides-complex/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-overrides-complex/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-overrides-simple/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-overrides-simple/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-overrides-simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-quotation-marks/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-quotation-marks/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-quotation-marks/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-rtd-default/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-rtd-default/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-rtd-default/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-rtd-invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-rtd-invalid/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-rtd-invalid/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-simple/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-simple/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-simple/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-sitename/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-sitename/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-sitename/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-sitename-from-project/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-sitename-from-project/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-sitename-from-project/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-admonitions/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-admonitions/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-admonitions/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-code-block/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-code-block/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-code-block/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-comments/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-comments/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-comments/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-raw/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-raw/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-raw/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-title/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-title/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-skip-title/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-social-cards-svg/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-social-cards-svg/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-social-cards-svg/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:48.000000 sphinxext-opengraph-0.8.1/tests/roots/test-type/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-type/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/roots/test-type/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-02-09 04:07:16.000000 sphinxext-opengraph-0.8.1/tests/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/docs/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/script/generate_social_card_previews.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/source/_static/og-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/docs/source/socialcards.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)  1755856 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/_static/Roboto-Flex.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/_static/sphinx-logo-shadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/descriptionparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/metaparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/socialcards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/sphinxext/opengraph/titleparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-arbitrary-tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-arbitrary-tags/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-arbitrary-tags/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-custom-tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-custom-tags/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-custom-tags/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-description-length/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-description-length/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-description-length/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-double-spacing/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-double-spacing/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-double-spacing/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-first-image/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-first-image/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-first-image/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-first-image-no-image/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-first-image-no-image/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-first-image-no-image/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/img/sample.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/sub/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/sub/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-list/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-list/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-list/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-local-image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-local-image/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8377 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-local-image/_static/sample.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-local-image/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-local-image/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description-manual-description/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description-manual-description/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description-manual-description/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description-manual-og-description/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description-manual-og-description/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-meta-name-description-manual-og-description/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-nested-lists/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-nested-lists/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-nested-lists/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-overrides-complex/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-overrides-complex/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-overrides-complex/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-overrides-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-overrides-simple/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-overrides-simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-quotation-marks/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-quotation-marks/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-quotation-marks/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-rtd-default/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-rtd-default/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-rtd-default/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-rtd-invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-rtd-invalid/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-rtd-invalid/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-simple/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-simple/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-sitename/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-sitename/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-sitename/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-sitename-from-project/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-sitename-from-project/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-sitename-from-project/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-admonitions/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-admonitions/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-admonitions/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-code-block/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-code-block/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-code-block/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-comments/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-comments/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-comments/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-raw/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-raw/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-title/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-title/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-skip-title/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-social-cards-svg/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-social-cards-svg/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-social-cards-svg/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:34:17.000000 sphinxext-opengraph-0.8.2/tests/roots/test-type/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-type/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/roots/test-type/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-04-13 13:33:44.000000 sphinxext-opengraph-0.8.2/tests/test_options.py
```

### Comparing `sphinxext-opengraph-0.8.1/.github/workflows/workflow.yml` & `sphinxext-opengraph-0.8.2/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/.gitignore` & `sphinxext-opengraph-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/LICENSE.md` & `sphinxext-opengraph-0.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/PKG-INFO` & `sphinxext-opengraph-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxext-opengraph
-Version: 0.8.1
+Version: 0.8.2
 Summary: Sphinx Extension to enable OGP support
 Home-page: https://github.com/wpilibsuite/sphinxext-opengraph
 Author: Itay Ziv
 Author-email: itay220204@gmail.com
 License: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `sphinxext-opengraph-0.8.1/README.md` & `sphinxext-opengraph-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/docs/Makefile` & `sphinxext-opengraph-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/docs/make.bat` & `sphinxext-opengraph-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/docs/script/generate_social_card_previews.py` & `sphinxext-opengraph-0.8.2/docs/script/generate_social_card_previews.py`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/docs/source/_static/og-logo.png` & `sphinxext-opengraph-0.8.2/docs/source/_static/og-logo.png`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/docs/source/conf.py` & `sphinxext-opengraph-0.8.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/docs/source/socialcards.md` & `sphinxext-opengraph-0.8.2/docs/source/socialcards.md`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/noxfile.py` & `sphinxext-opengraph-0.8.2/noxfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,24 +15,25 @@
 
 nox.options.reuse_existing_virtualenvs = True
 
 
 @nox.session
 def docs(session):
     """Build the documentation. Use `-- live` to build with a live server."""
-    session.install("-e", ".")
     session.install("-r", "docs/requirements.txt")
+    session.install("-e", ".")
     if "live" in session.posargs:
         session.install("ipython")
         session.install("sphinx-autobuild")
         session.run(*split("sphinx-autobuild -b html docs/source docs/build/html"))
     else:
         session.run(
             *split("sphinx-build -nW --keep-going -b html docs/source docs/build/html")
         )
 
 
 @nox.session
 def test(session):
     """Run the test suite."""
-    session.install(".")
+    session.install("-e", ".")
+    session.install("-r", "dev-requirements.txt")
     session.run(*(["pytest"] + session.posargs))
```

### Comparing `sphinxext-opengraph-0.8.1/setup.py` & `sphinxext-opengraph-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/sphinxext/opengraph/__init__.py` & `sphinxext-opengraph-0.8.2/sphinxext/opengraph/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -132,16 +132,14 @@
 
     # Decide whether to add social media card images for each page.
     # Only do this as a fallback if the user hasn't given any configuration
     # to add other images.
     config_social = DEFAULT_SOCIAL_CONFIG.copy()
     social_card_user_options = app.config.ogp_social_cards or {}
     config_social.update(social_card_user_options)
-
-    # This will only be False if the user explicitly sets it
     if (
         not (image_url or ogp_use_first_image)
         and config_social.get("enable") is not False
     ):
         # Description
         description_max_length = config_social.get(
             "description_max_length", DEFAULT_DESCRIPTION_LENGTH_SOCIAL_CARDS - 3
@@ -181,14 +179,21 @@
 
         # Link the image in our page metadata
         # We use os.path.sep to standardize behavior acros *nix and Windows
         url = app.config.ogp_site_url.strip("/")
         image_path = str(image_path).replace(os.path.sep, "/").strip("/")
         image_url = f"{url}/{image_path}"
 
+        # If the social card objects have been added we add special metadata for them
+        # These are the dimensions *in pixels* of the card
+        # They were chosen by looking at the image pixel dimensions on disk
+        tags["og:image:width"] = "1146"
+        tags["og:image:height"] = "600"
+        meta_tags["twitter:card"] = "summary_large_image"
+
     fields.pop("og:image:alt", None)
 
     first_image = None
     if ogp_use_first_image:
         # Use the first image that is defined in the current page
         first_image = doctree.next_node(nodes.image)
         if (
@@ -220,20 +225,14 @@
         if isinstance(ogp_image_alt, str):
             tags["og:image:alt"] = ogp_image_alt
         elif ogp_image_alt is None and site_name:
             tags["og:image:alt"] = site_name
         elif ogp_image_alt is None and title:
             tags["og:image:alt"] = title
 
-        if "ogp_social_card_tags" in context:
-            # Add social media metadata if we've activated preview cards
-            tags["og:image:width"] = meta["width"]
-            tags["og:image:height"] = meta["height"]
-            meta_tags["twitter:card"] = "summary_large_image"
-
     # arbitrary tags and overrides
     tags.update({k: v for k, v in fields.items() if k.startswith("og:")})
 
     return (
         "\n".join(
             [make_tag(p, c) for p, c in tags.items()]
             + [make_tag(p, c, "name") for p, c in meta_tags.items()]
```

### Comparing `sphinxext-opengraph-0.8.1/sphinxext/opengraph/_static/Roboto-Flex.ttf` & `sphinxext-opengraph-0.8.2/sphinxext/opengraph/_static/Roboto-Flex.ttf`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/sphinxext/opengraph/_static/sphinx-logo-shadow.png` & `sphinxext-opengraph-0.8.2/sphinxext/opengraph/_static/sphinx-logo-shadow.png`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/sphinxext/opengraph/descriptionparser.py` & `sphinxext-opengraph-0.8.2/sphinxext/opengraph/descriptionparser.py`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/sphinxext/opengraph/metaparser.py` & `sphinxext-opengraph-0.8.2/sphinxext/opengraph/metaparser.py`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/sphinxext/opengraph/socialcards.py` & `sphinxext-opengraph-0.8.2/sphinxext/opengraph/socialcards.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,20 +96,20 @@
     for img in ["image_mini", "image"]:
         impath = kwargs_fig.get(img)
         if not impath:
             continue
 
         # If image is an SVG replace it with None
         if impath.suffix.lower() == ".svg":
-            LOGGER.warn(f"[Social card] {img} cannot be an SVG image, skipping...")
+            LOGGER.warning(f"[Social card] %s cannot be an SVG image, skipping...", img)
             kwargs_fig[img] = None
 
         # If image doesn't exist, throw a warning and replace with none
         if not impath.exists():
-            LOGGER.warn(f"[Social card]: {img} file doesn't exist, skipping...")
+            LOGGER.warning(f"[Social card]: %s file doesn't exist, skipping...", img)
             kwargs_fig[img] = None
 
     # These are passed directly from the user configuration to our plotting function
     pass_through_config = ["text_color", "line_color", "background_color", "font"]
     for config in pass_through_config:
         if config_social.get(config):
             kwargs_fig[config] = config_social.get(config)
```

### Comparing `sphinxext-opengraph-0.8.1/sphinxext/opengraph/titleparser.py` & `sphinxext-opengraph-0.8.2/sphinxext/opengraph/titleparser.py`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/PKG-INFO` & `sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxext-opengraph
-Version: 0.8.1
+Version: 0.8.2
 Summary: Sphinx Extension to enable OGP support
 Home-page: https://github.com/wpilibsuite/sphinxext-opengraph
 Author: Itay Ziv
 Author-email: itay220204@gmail.com
 License: LICENSE.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `sphinxext-opengraph-0.8.1/sphinxext_opengraph.egg-info/SOURCES.txt` & `sphinxext-opengraph-0.8.2/sphinxext_opengraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/tests/conftest.py` & `sphinxext-opengraph-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/tests/roots/test-image-rel-paths/img/sample.jpg` & `sphinxext-opengraph-0.8.2/tests/roots/test-image-rel-paths/img/sample.jpg`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/tests/roots/test-local-image/_static/sample.jpg` & `sphinxext-opengraph-0.8.2/tests/roots/test-local-image/_static/sample.jpg`

 * *Files identical despite different names*

### Comparing `sphinxext-opengraph-0.8.1/tests/test_options.py` & `sphinxext-opengraph-0.8.2/tests/test_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
 from sphinx.application import Sphinx
 import conftest
 
 
-def get_tag(tags, tag_type):
-    return [tag for tag in tags if tag.get("property") == f"og:{tag_type}"][0]
+def get_tag(tags, tag_type, kind="property", prefix="og"):
+    return [tag for tag in tags if tag.get(kind) == f"{prefix}:{tag_type}"][0]
 
 
-def get_tag_content(tags, tag_type):
+def get_tag_content(tags, tag_type, kind="property", prefix="og"):
     # Gets the content of a specific ogp tag
-    return get_tag(tags, tag_type).get("content", "")
+    return get_tag(tags, tag_type, kind, prefix).get("content", "")
 
 
 def get_meta_description(tags):
     return [tag for tag in tags if tag.get("name") == "description"][0].get(
         "content", ""
     )
 
@@ -95,25 +95,29 @@
 
 @pytest.mark.sphinx("html", testroot="image")
 def test_image_alt(og_meta_tags):
     assert get_tag_content(og_meta_tags, "image:alt") == "Example's Docs!"
 
 
 @pytest.mark.sphinx("html", testroot="simple")
-def test_image_social_cards(og_meta_tags):
+def test_image_social_cards(meta_tags):
     """Social cards should automatically be added if no og:image is given."""
     # Asserting `in` instead of `==` because of the hash that is generated
     assert (
         "http://example.org/en/latest/_images/social_previews/summary_index"
-        in get_tag_content(og_meta_tags, "image")
+        in get_tag_content(meta_tags, "image")
     )
     # Image alt text should be taken from page content.
     assert (
         "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
-        in get_tag_content(og_meta_tags, "image:alt")
+        in get_tag_content(meta_tags, "image:alt")
+    )
+    # Make sure the extra tags are in the HTML
+    assert "summary_large_image" in get_tag_content(
+        meta_tags, "card", kind="name", prefix="twitter"
     )
 
 
 @pytest.mark.sphinx("html", testroot="type")
 def test_type(og_meta_tags):
     assert get_tag_content(og_meta_tags, "type") == "article"
```

