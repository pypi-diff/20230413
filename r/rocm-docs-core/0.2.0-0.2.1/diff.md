# Comparing `tmp/rocm-docs-core-0.2.0.tar.gz` & `tmp/rocm-docs-core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocm-docs-core-0.2.0.tar", last modified: Tue Apr  4 23:52:26 2023, max compression
+gzip compressed data, was "rocm-docs-core-0.2.1.tar", last modified: Thu Apr 13 16:04:17 2023, max compression
```

## Comparing `rocm-docs-core-0.2.0.tar` & `rocm-docs-core-0.2.1.tar`

### file list

```diff
@@ -1,94 +1,98 @@
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)    17097 2023-03-22 20:27:06.000000 rocm-docs-core-0.2.0/LICENSE.txt
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1728 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/PKG-INFO
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1239 2023-03-22 20:27:06.000000 rocm-docs-core-0.2.0/README.md
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      721 2023-04-04 23:52:20.000000 rocm-docs-core-0.2.0/pyproject.toml
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      755 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/setup.cfg
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.918069 rocm-docs-core-0.2.0/src/
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.918069 rocm-docs-core-0.2.0/src/rocm_docs/
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)    15323 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/__init__.py
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.918069 rocm-docs-core-0.2.0/src/rocm_docs/data/
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.922069 rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)    72387 2023-03-28 18:29:57.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      112 2023-03-28 18:29:57.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/footer.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1428 2023-03-28 18:29:57.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/header.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)    37264 2023-03-28 18:29:57.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/stylesheet.css
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.922069 rocm-docs-core-0.2.0/src/rocm_docs/data/_images/
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)      924 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_images/amd-header-logo.svg
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)     1759 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_images/rdc-watermark.svg
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    10074 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_images/rocm-logo.png
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.922069 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      831 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/code_word_breaks.js
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1957 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/custom.css
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.918069 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    20756 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    16748 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    21924 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    17872 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    20780 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    16808 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    21876 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    17876 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    20672 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    16756 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    21820 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    17780 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    20172 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    16372 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    21248 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    17384 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    20664 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    16696 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    21520 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    17544 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    27552 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    22132 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    29388 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    23712 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    27592 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    22184 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    29392 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    23824 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    27456 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    22212 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    29224 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    23676 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    26652 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    21516 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    28292 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    22904 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    27376 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    22040 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    28704 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    23168 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    29304 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    23704 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    27520 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    22084 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    21856 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-italic.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    17820 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-italic.woff2
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    20712 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-regular.woff
--rwxrwxr-x   0 samwu103  (1001) samwu103  (1001)    16740 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-regular.woff2
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     9931 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts.css
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     3502 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts.css.map
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1503 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts.scss
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      979 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/rocm_footer.css
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     2106 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_static/rocm_header.css
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/components/
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      390 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/components/copyright.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      121 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/components/left-side-menu.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     2523 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/components/social-links.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      108 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/layout.html
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/sections/
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      318 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/sections/footer-content.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1266 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/sections/footer.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1507 2023-04-04 16:02:59.000000 rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/sections/header.html
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     5592 2023-03-29 16:13:01.000000 rocm-docs-core-0.2.0/src/rocm_docs/util.py
-drwxrwxr-x   0 samwu103  (1001) samwu103  (1001)        0 2023-04-04 23:52:26.926069 rocm-docs-core-0.2.0/src/rocm_docs_core.egg-info/
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     1728 2023-04-04 23:52:26.000000 rocm-docs-core-0.2.0/src/rocm_docs_core.egg-info/PKG-INFO
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)     4998 2023-04-04 23:52:26.000000 rocm-docs-core-0.2.0/src/rocm_docs_core.egg-info/SOURCES.txt
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)        1 2023-04-04 23:52:26.000000 rocm-docs-core-0.2.0/src/rocm_docs_core.egg-info/dependency_links.txt
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)      356 2023-04-04 23:52:26.000000 rocm-docs-core-0.2.0/src/rocm_docs_core.egg-info/requires.txt
--rw-rw-r--   0 samwu103  (1001) samwu103  (1001)       10 2023-04-04 23:52:26.000000 rocm-docs-core-0.2.0/src/rocm_docs_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.683056 rocm-docs-core-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 16:04:17.683056 rocm-docs-core-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:04:17.683056 rocm-docs-core-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    13649 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/
+-rw-r--r--   0 runner    (1001) docker     (123)    72387 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/extra_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)    37264 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/components/social-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.675056 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.683056 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20756 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16748 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21924 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17872 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20780 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16808 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21876 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17876 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20672 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16756 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21820 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17780 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20172 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16372 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21248 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17384 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20664 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16696 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21520 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17544 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27552 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22132 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29388 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23712 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27592 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22184 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29392 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23824 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27456 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22212 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29224 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23676 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26652 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21516 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28292 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22904 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27376 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22040 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28704 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23168 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29304 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23704 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27520 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22084 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21856 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20712 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16740 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.683056 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10074 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-04-13 16:04:08.000000 rocm-docs-core-0.2.1/src/rocm_docs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:04:17.683056 rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-13 16:04:17.000000 rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-13 16:04:17.000000 rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:04:17.000000 rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 16:04:17.000000 rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-13 16:04:17.000000 rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 16:04:17.000000 rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/top_level.txt
```

### Comparing `rocm-docs-core-0.2.0/LICENSE.txt` & `rocm-docs-core-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/PKG-INFO` & `rocm-docs-core-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Core utilities for all ROCm documentation on RTD
-Home-page: https://amd.com
-Author: Lauren Wrubleski
-Author-email: Lauren.Wrubleski@amd.com
-Project-URL: Docs, https://docs.amd.com
+Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
+Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
+Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: api_reference
+Provides-Extra: development
 License-File: LICENSE.txt
 
 # ROCm Documentation Core Utilities
 
 ### Purpose
 This repository is comprised of utilities, styling, scripts, and additional HTML content that is common to all ROCm projects' documentation. This greatly aids in maintaining the documentation, as any change to the appearance only needs to be modified in one location.
```

### Comparing `rocm-docs-core-0.2.0/README.md` & `rocm-docs-core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/__init__.py` & `rocm-docs-core-0.2.1/src/rocm_docs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,26 +39,19 @@
         "breathe_default_project",
         "myst_enable_extensions",
         "myst_heading_anchors",
         "external_toc_path",
         "external_toc_exclude_missing",
         "intersphinx_mapping",
         "intersphinx_disabled_domains",
-        "templates_path",
         "epub_show_urls",
         "exclude_patterns",
         "html_theme",
         "html_title",
-        "html_static_path",
-        "html_css_files",
-        "html_js_files",
-        "html_extra_path",
         "html_theme_options",
-        "html_show_sphinx",
-        "html_favicon",
         "numfig",
     ]
 
     def __init__(
         self,
         project_name: str,
         docs_folder: MaybePath = None,
@@ -76,21 +69,15 @@
         self.intersphinx_mapping: Dict[str, Tuple[str, None]]
         self.intersphinx_disabled_domains: List[str]
         self.templates_path: List[str]
         self.epub_show_urls: str
         self.exclude_patterns: List[str]
         self.html_theme: str
         self.html_title: str
-        self.html_static_path: List[str]
-        self.html_css_files: List[str]
-        self.html_js_files: List[str]
-        self.html_extra_path: List[str]
-        self.html_theme_options: Dict[str, Union[str, bool, List[str]]]
-        self.html_show_sphinx: bool
-        self.html_favicon: str
+        self.html_theme_options: Dict[str, Union[str, bool, List[str]]] = {}
         self.numfig: bool
         self._docs_folder: Path
         tmp_docs_folder = self.to_path(docs_folder)
         self._docs_folder = (
             tmp_docs_folder if tmp_docs_folder is not None else Path(".")
         )
         self._doxygen_context = _DoxygenContext()
@@ -265,79 +252,48 @@
         toc_in_path = self._docs_folder / "./.sphinx/_toc.yml.in"
         if not (toc_in_path.exists() and toc_in_path.is_file()):
             raise FileNotFoundError(
                 f"Expected input toc file {toc_in_path} to exist and be"
                 " readable."
             )
         format_toc(self._docs_folder)
-        url, branch, edit_page = get_branch(self._docs_folder)
 
         self.external_toc_path = "./.sphinx/_toc.yml"
         self.external_toc_exclude_missing = False
 
         # intersphinx Configuration
         self.intersphinx_mapping = {
             "rtd": ("https://docs.readthedocs.io/en/stable/", None),
             "python": ("https://docs.python.org/3/", None),
             "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
         }
         self.intersphinx_disabled_domains = ["std"]
 
-        # Other configuration
-        self.templates_path = ["_templates"]
-
         # -- Options foself.r EPUB output
         self.epub_show_urls = "footnote"
 
         # List of patterns, relative to source directory, that match files and
         # directories to ignore when looking for source files.
         # This pattern also affects html_static_path and html_extra_path.
         self.exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
         # -- Options for HTML output ------------------------------------------
 
         # The theme to use for HTML and HTML Help pages.  See the documentation
         # for a list of builtin themes.
         #
-        self.html_theme = "sphinx_book_theme"
+        self.html_theme = "rocm_docs_theme"
         self.html_title = self._project_name
-        self.html_static_path = ["_static"]
-        self.html_css_files = [
-            "custom.css",
-            "rocm_header.css",
-            "rocm_footer.css",
-            "fonts.css",
-        ]
-        self.html_js_files = ["code_word_breaks.js"]
-        self.html_extra_path = ["_images"]
-        self.html_theme_options = {
-            "home_page_in_toc": False,
-            "use_edit_page_button": edit_page,
-            "repository_url": url,
-            "repository_branch": branch,
-            "path_to_docs": get_path_to_docs(),
-            "show_navbar_depth": "0",
-            "body_max_width": "none",
-            "show_toc_level": "0",
-            "article_header_start": [
-                "toggle-primary-sidebar.html",
-                "breadcrumbs.html",
-            ],
-            "navbar_center": ["components/left-side-menu.html"],
-        }
-
-        self.html_show_sphinx = False
-        self.html_favicon = "https://www.amd.com/themes/custom/amd/favicon.ico"
 
         self.numfig = True
 
         self.copy_files()
 
     def disable_main_doc_link(self):
-        self.html_theme_options.pop("navbar_center")
+        self.html_theme_options["link_main_doc"] = False
 
     def copy_files(self):
         """Insert additional files into workspace."""
         if self._copied_files:
             return
         self._copied_files = True
 
@@ -389,19 +345,14 @@
     root: Path = Path()
     path: Path = Path()
     doxyfile: str = ""
 
 
 def setup(app: Sphinx) -> None:
     app.setup_extension("notfound.extension")
-    app.add_js_file(
-        "https://download.amd.com/js/analytics/analyticsinit.js",
-        priority=999_999,
-        loading_method="async",
-    )
     app.connect("config-inited", force_notfound_prefix, 300)
 
     # Execute doxysphinx now that sphinx source and output directories are known
     if not hasattr(setup, '_doxygen_context'):
         return
 
     doxygen_context = setup._doxygen_context
```

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css` & `rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/extra_stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/header.html` & `rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/header.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_doxygen/stylesheet.css` & `rocm-docs-core-0.2.1/src/rocm_docs/data/_doxygen/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_images/amd-header-logo.svg` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_images/rdc-watermark.svg` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_images/rocm-logo.png` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/code_word_breaks.js` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/custom.css` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/custom.css`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     transform: translate(-50%, -50%) rotate(-45deg);
     opacity: 10%;
     z-index: 10000;
     max-width: 100%;
     max-height: calc(100% - 200px);
     object-fit: contain;
     width: 45%;
+    opacity: 20%;
 }
 
 ul.bd-breadcrumbs {
     margin-bottom: 0;
     margin-top: 1px;
 }
```

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-300italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-500italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-600italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-700italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-800italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-italic.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-italic.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-regular.woff` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts/open-sans/open-sans-v34-latin-regular.woff2` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts.css` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts.css.map` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts.css.map`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/fonts.scss` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/fonts.scss`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/rocm_footer.css` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css`

 * *Files 6% similar despite different names*

```diff
@@ -53,7 +53,10 @@
 }
 
 .rocm-footer ul li+li {
     margin-left: 10px;
     padding-left: 8px;
 }
 
+.rocm-footer .copyright {
+    text-align: center;
+}
```

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_static/rocm_header.css` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/static/rocm_header.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/components/social-links.html` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/components/social-links.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/sections/footer.html` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/sections/footer.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 <div class="rocm-footer">
     {%- include "components/social-links.html" with context -%}
-    {% include 'components/copyright.html' %}
     <div class="rocm-footer-links">
         <ul>
-            <li><a href="https://www.amd.com/en/corporate/copyright">Terms and Conditions</a></li>
-            <li><a href="https://">ROCm Licenses and Disclaimers</a></li>
-            <li><a href="https://www.amd.com/en/corporate/privacy">Privacy</a></li>
-            <li><a href="https://www.amd.com/en/corporate/trademarks">Trademarks</a></li>
-            <li><a href="https://www.amd.com/system/files/documents/statement-human-trafficking-forced-labor.pdf">Statement on Forced Labor</a></li>
-            <li><a href="https://www.amd.com/en/corporate/competition">Fair and Open Competition</a></li>
-            <li><a href="https://www.amd.com/system/files/documents/amd-uk-tax-strategy.pdf">UK Tax Strategy</a></li>
-            <li><a href="https://www.amd.com/en/corporate/cookies">Cookie Policy</a></li>
+            <li><a href="https://www.amd.com/en/corporate/copyright" target="_blank">Terms and Conditions</a></li>
+            <li><a href="https://rocmdocs.amd.com/projects/alpha/en/develop/release/licensing.html">ROCm Licenses and Disclaimers</a></li>
+            <li><a href="https://www.amd.com/en/corporate/privacy" target="_blank">Privacy</a></li>
+            <li><a href="https://www.amd.com/en/corporate/trademarks" target="_blank">Trademarks</a></li>
+            <li><a href="https://www.amd.com/system/files/documents/statement-human-trafficking-forced-labor.pdf" target="_blank">Statement on Forced Labor</a></li>
+            <li><a href="https://www.amd.com/en/corporate/competition" target="_blank">Fair and Open Competition</a></li>
+            <li><a href="https://www.amd.com/system/files/documents/amd-uk-tax-strategy.pdf" target="_blank">UK Tax Strategy</a></li>
+            <li><a href="https://www.amd.com/en/corporate/cookies" target="_blank">Cookie Policy</a></li>
             <!-- OneTrust Cookies Settings button start -->
             <li><a href="#cookie-settings" id="ot-sdk-btn" class="ot-sdk-show-settings">Cookie Settings</a></li>
             <!-- OneTrust Cookies Settings button end -->        
         </ul>
     </div>
+    {% include 'components/copyright.html' %}
+</div>
+
+<div id="rdc-watermark-container">
+    <img id="rdc-watermark" src="{{ pathto('_static/images/alpha-watermark.svg',1) }}" alt="DRAFT watermark"/>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-{%- include "components/social-links.html" with context -%} {% include
-'components/copyright.html' %}
+{%- include "components/social-links.html" with context -%}
     * Terms_and_Conditions
     * ROCm_Licenses_and_Disclaimers
     * Privacy
     * Trademarks
     * Statement_on_Forced_Labor
     * Fair_and_Open_Competition
     * UK_Tax_Strategy
     * Cookie_Policy
     * Cookie_Settings
+{% include 'components/copyright.html' %}
+[DRAFT watermark]
```

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/data/_templates/sections/header.html` & `rocm-docs-core-0.2.1/src/rocm_docs/rocm_docs_theme/sections/header.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 <div class="rocm-header">
     <div class="rocm-header-buttons">
-        <a href="https://www.amd.com" class="rocm-header-link">
-            <img id="amd-logo" alt="Advanced Micro Devices, Inc." src="{{ pathto('rocm-logo.png',1) }}"></img>
+        <a href="https://www.amd.com" target="_blank" class="rocm-header-link">
+            <img id="amd-logo" alt="Advanced Micro Devices, Inc." src="{{ pathto('_static/images/rocm-logo.png',1) }}"></img>
             <div class="glow-wrap">
                 <i class="glow"></i>
             </div>
         </a>
-        <a href="{{ theme_repository_url }}" class="rocm-header-link">
+        <a href="{{ theme_repository_url }}" target="_blank" class="rocm-header-link">
             <div class="rocm-link-box">
                 <p>GitHub</p>
             </div>
             <div class="glow-wrap">
                 <i class="glow"></i>
             </div>
         </a>
-        <a href="https://github.com/RadeonOpenCompute/ROCm/discussions" class="rocm-header-link">
+        <a href="https://github.com/RadeonOpenCompute/ROCm/discussions" target="_blank" class="rocm-header-link">
             <div class="rocm-link-box">
                 <p>Community</p>
             </div>
             <div class="glow-wrap">
                 <i class="glow"></i>
             </div>
         </a>
-        <a href="https://github.com/RadeonOpenCompute/ROCm/issues/new" class="rocm-header-link">
+        <a href="https://github.com/RadeonOpenCompute/ROCm/issues/new" target="_blank" class="rocm-header-link">
             <div class="rocm-link-box">
                 <p>Support</p>
             </div>
             <div class="glow-wrap">
                 <i class="glow"></i>
             </div>
         </a>
-        <a href="https://www.amd.com/en/technologies/infinity-hub" class="rocm-header-link">
+        <a href="https://www.amd.com/en/technologies/infinity-hub" target="_blank" class="rocm-header-link">
             <div class="rocm-link-box">
                 <p>Infinity Hub</p>
             </div>
             <div class="glow-wrap">
                 <i class="glow"></i>
             </div>
         </a>
```

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs/util.py` & `rocm-docs-core-0.2.1/src/rocm_docs/util.py`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.2.0/src/rocm_docs_core.egg-info/PKG-INFO` & `rocm-docs-core-0.2.1/src/rocm_docs_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Core utilities for all ROCm documentation on RTD
-Home-page: https://amd.com
-Author: Lauren Wrubleski
-Author-email: Lauren.Wrubleski@amd.com
-Project-URL: Docs, https://docs.amd.com
+Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
+Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
+Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: api_reference
+Provides-Extra: development
 License-File: LICENSE.txt
 
 # ROCm Documentation Core Utilities
 
 ### Purpose
 This repository is comprised of utilities, styling, scripts, and additional HTML content that is common to all ROCm projects' documentation. This greatly aids in maintaining the documentation, as any change to the appearance only needs to be modified in one location.
```

