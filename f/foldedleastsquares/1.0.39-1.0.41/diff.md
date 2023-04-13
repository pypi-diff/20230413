# Comparing `tmp/foldedleastsquares-1.0.39.tar.gz` & `tmp/foldedleastsquares-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foldedleastsquares-1.0.39.tar", last modified: Wed Apr 12 16:01:56 2023, max compression
+gzip compressed data, was "foldedleastsquares-1.0.41.tar", last modified: Thu Apr 13 17:51:38 2023, max compression
```

## Comparing `foldedleastsquares-1.0.39.tar` & `foldedleastsquares-1.0.41.tar`

### file list

```diff
@@ -1,97 +1,48 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/tutorials/
--rwxrwxrwx   0 martin    (1000) martin    (1000)   205928 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/07 The influence of limb darkening values.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   272427 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/10 Measurement uncertainties.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   277149 2021-01-23 08:20:50.000000 foldedleastsquares-1.0.39/tutorials/12 A comet-like transit from Kepler KIC 12557548 with TLS.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   614539 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/11 A planet from TESS with TLS.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)    56339 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/data_per_t14.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)   333163 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/02 Starter's guide - K2-3b, a red dwarf with a planet.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   229894 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/04 Exploring the TLS spectra and statistics.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)  1116963 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/01 Quick start with synthetic data.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   553194 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/03 Multiple planets - K2-3, a red dwarf with 3 Super-Earths.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)    42518 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/08 Edge effect jitter correction.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   199436 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/06 Comparison between TLS and BLS.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)    99387 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/05 Custom transit shapes - Example of the grazing planet WASP-75.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   124754 2021-01-23 08:28:23.000000 foldedleastsquares-1.0.39/tutorials/13 Flares detection from TESS Proxima Centauri data.ipynb
--rwxrwxrwx   0 martin    (1000) martin    (1000)   568511 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/tutorials/09 Optimal period grid and optimal duration grid.ipynb
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     5220 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       79 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     3263 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      107 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     5220 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/PKG-INFO
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/.github/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 martin    (1000) martin    (1000)      635 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/documentation.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)      604 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/feature_request.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)      530 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1622 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/CONTRIBUTING.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1071 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/LICENSE
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4846 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/docs/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/docs/source/
--rwxrwxrwx   0 martin    (1000) martin    (1000)      906 2020-12-29 16:17:32.000000 foldedleastsquares-1.0.39/docs/source/Installation.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)    22976 2021-01-23 08:21:36.000000 foldedleastsquares-1.0.39/docs/source/Python interface.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)      863 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/conf.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    86868 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/animation.gif
--rwxrwxrwx   0 martin    (1000) martin    (1000)   136291 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/faq_2.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)   144986 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/faq_1.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4608 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/Changelog.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1413 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/Command.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)    41253 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/fig_histo_teff.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)   115484 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/logo.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)      412 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/index.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)     9943 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/FAQ.rst
--rwxrwxrwx   0 martin    (1000) martin    (1000)    68827 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/docs/source/frontpage_rescaled.png
--rwxrwxrwx   0 martin    (1000) martin    (1000)      747 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.travis.yml
--rwxrwxrwx   0 martin    (1000) martin    (1000)      132 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.directory
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1619 2022-05-09 09:54:48.000000 foldedleastsquares-1.0.39/setup.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      101 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/.gitignore
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3332 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/CODE_OF_CONDUCT.md
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/setup.cfg
--rwxrwxrwx   0 martin    (1000) martin    (1000)      349 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/PULL_REQUEST_TEMPLATE.md
--rwxrwxrwx   0 martin    (1000) martin    (1000)       33 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/MANIFEST.in
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/
--rwxrwxrwx   0 martin    (1000) martin    (1000)        0 2020-12-30 08:11:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/__init__.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     6202 2022-06-18 12:59:13.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/tailed_transit_template_generator.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    13229 2023-04-12 15:52:28.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/transit_template_generator.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    17706 2022-06-18 12:58:51.000000 foldedleastsquares-1.0.39/foldedleastsquares/template_generator/default_transit_template_generator.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1171 2021-04-18 15:50:51.000000 foldedleastsquares-1.0.39/foldedleastsquares/__init__.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     6891 2022-02-20 09:11:20.000000 foldedleastsquares-1.0.39/foldedleastsquares/core.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    12386 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/JAA546A14limb1-4.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     6392 2021-05-13 09:09:02.000000 foldedleastsquares-1.0.39/foldedleastsquares/catalog.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-12 16:01:56.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/
--rwxrwxrwx   0 martin    (1000) martin    (1000)    90800 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC201367065.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3224 2021-05-13 09:02:58.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_transit_depth_min.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      507 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_validation.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     2427 2023-04-12 16:01:05.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_period_grid.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     2051 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_uncertainties.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      352 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/tls_config.cfg
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3450 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_catalog_data.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)       35 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/run_tests.sh
--rwxrwxrwx   0 martin    (1000) martin    (1000)    80075 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC206154641.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)      890 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_duration_grid.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1847 2023-03-31 07:39:45.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_multi_planet.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      326 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/run_tests.bat
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3051 2023-03-31 09:25:29.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_shapes.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4964 2023-03-31 09:41:53.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_stats_gap.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      362 2021-05-13 09:02:58.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_FAP.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)      769 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_cleaned_array.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1372 2021-05-13 09:02:59.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_resample.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     7433 2021-05-13 09:02:57.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/test_synthetic.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    94432 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/tests/EPIC201367065_detrended.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1973 2021-01-23 18:43:31.000000 foldedleastsquares-1.0.39/foldedleastsquares/results.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     8204 2022-12-07 19:16:32.000000 foldedleastsquares-1.0.39/foldedleastsquares/main.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    15976 2022-06-18 12:58:43.000000 foldedleastsquares-1.0.39/foldedleastsquares/stats.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    23488 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/fap.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4206 2021-05-13 09:09:38.000000 foldedleastsquares-1.0.39/foldedleastsquares/command_line.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     8098 2021-05-13 09:08:34.000000 foldedleastsquares-1.0.39/foldedleastsquares/validate.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1052 2021-05-13 09:08:43.000000 foldedleastsquares-1.0.39/foldedleastsquares/grid.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     4800 2021-08-19 15:36:24.000000 foldedleastsquares-1.0.39/foldedleastsquares/tls_constants.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     3844 2021-05-13 09:09:22.000000 foldedleastsquares-1.0.39/foldedleastsquares/helpers.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)    12620 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/ld_claret_tess.csv
--rwxrwxrwx   0 martin    (1000) martin    (1000)       53 2023-04-12 15:52:28.000000 foldedleastsquares-1.0.39/foldedleastsquares/version.py
--rwxrwxrwx   0 martin    (1000) martin    (1000)     1611 2020-07-13 11:13:06.000000 foldedleastsquares-1.0.39/foldedleastsquares/interpolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:38.909865 foldedleastsquares-1.0.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-13 17:51:38.909865 foldedleastsquares-1.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:38.901865 foldedleastsquares-1.0.41/foldedleastsquares/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:38.905865 foldedleastsquares-1.0.41/foldedleastsquares/template_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/template_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/template_generator/default_transit_template_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/template_generator/tailed_transit_template_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/template_generator/transit_template_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:38.909865 foldedleastsquares-1.0.41/foldedleastsquares/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_FAP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_catalog_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_cleaned_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_duration_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_multi_planet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_period_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_stats_gap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_transit_depth_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/tls_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/foldedleastsquares/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:51:38.905865 foldedleastsquares-1.0.41/foldedleastsquares.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-13 17:51:38.000000 foldedleastsquares-1.0.41/foldedleastsquares.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-13 17:51:38.000000 foldedleastsquares-1.0.41/foldedleastsquares.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:51:38.000000 foldedleastsquares-1.0.41/foldedleastsquares.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-13 17:51:38.000000 foldedleastsquares-1.0.41/foldedleastsquares.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-13 17:51:38.000000 foldedleastsquares-1.0.41/foldedleastsquares.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 17:51:38.000000 foldedleastsquares-1.0.41/foldedleastsquares.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:51:38.909865 foldedleastsquares-1.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-13 17:51:27.000000 foldedleastsquares-1.0.41/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares.egg-info/PKG-INFO` & `foldedleastsquares-1.0.41/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: foldedleastsquares
-Version: 1.0.39
-Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
-Home-page: https://github.com/hippke/tls
-Author: Martín Dévora Pajares
-Author-email: martin.devora.pajares@gmail.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
 ### An optimized transit-fitting algorithm to search for periodic transits of small planets
 [![Image](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/hippke/tls/blob/master/LICENSE)
 [![Image](https://img.shields.io/badge/Python-2.7%20%26%203.5%2B-blue.svg)](https://pypi.org/project/transitleastsquares/)
 [![Image](https://img.shields.io/badge/pip%20install-transitleastsquares-blue.svg)](https://pypi.org/project/transitleastsquares/)
 [![Image](https://img.shields.io/badge/documentation-%E2%9C%93-blue.svg)](https://transitleastsquares.readthedocs.io/en/latest/index.html)
 [![Image](https://img.shields.io/badge/tutorials-%E2%9C%93-blue.svg)](https://github.com/hippke/tls/tree/master/tutorials)
@@ -82,9 +70,7 @@
 }
 ```
 
 ## Contributing Code, Bugfixes, or Feedback
 We welcome and encourage contributions. If you have any trouble, [open an issue](https://github.com/hippke/tls/issues).
 
 Copyright 2019 Michael Hippke & René Heller.
-
-
```

### Comparing `foldedleastsquares-1.0.39/PKG-INFO` & `foldedleastsquares-1.0.41/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,87 @@
 Metadata-Version: 2.1
 Name: foldedleastsquares
-Version: 1.0.39
+Version: 1.0.41
 Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
 Home-page: https://github.com/hippke/tls
 Author: Martín Dévora Pajares
 Author-email: martin.devora.pajares@gmail.com
 License: MIT
+Description: ![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
+        ### An optimized transit-fitting algorithm to search for periodic transits of small planets
+        [![Image](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/hippke/tls/blob/master/LICENSE)
+        [![Image](https://img.shields.io/badge/Python-2.7%20%26%203.5%2B-blue.svg)](https://pypi.org/project/transitleastsquares/)
+        [![Image](https://img.shields.io/badge/pip%20install-transitleastsquares-blue.svg)](https://pypi.org/project/transitleastsquares/)
+        [![Image](https://img.shields.io/badge/documentation-%E2%9C%93-blue.svg)](https://transitleastsquares.readthedocs.io/en/latest/index.html)
+        [![Image](https://img.shields.io/badge/tutorials-%E2%9C%93-blue.svg)](https://github.com/hippke/tls/tree/master/tutorials)
+        [![Image](https://img.shields.io/badge/arXiv-1901.02015-blue.svg)](https://arxiv.org/abs/1901.02015)
+        [![Build Status](https://travis-ci.com/hippke/tls.svg?branch=master)](https://travis-ci.com/hippke/tls)
+        
+        
+        ## Motivation
+        We present a new method to detect planetary transits from time-series photometry, the *Transit Least Squares* (TLS) algorithm. While the commonly used Box Least Squares [(BLS, Kovács et al. 2002)](http://adsabs.harvard.edu/abs/2002A%26A...391..369K) algorithm searches for rectangular signals in stellar light curves, *TLS* searches for transit-like features with stellar limb-darkening and including the effects of planetary ingress and egress. Moreover, *TLS* analyses the entire, unbinned data of the phase-folded light curve. These improvements yield a ~10 % higher detection efficiency (and similar false alarm rates) compared to BLS. The higher detection efficiency of our freely available Python implementation comes at the cost of higher computational load, which we partly compensate by applying an optimized period sampling and transit duration sampling, constrained to the physically plausible range. A typical Kepler K2 light curve, worth of 90 d of observations at a cadence of 30 min, can be searched with *TLS* in 10 seconds real time on a standard laptop computer, just as with BLS.
+        
+        ![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/frontpage_rescaled.png)
+        
+        ## Installation
+        
+        TLS can be installed conveniently using: `pip install transitleastsquares`
+        
+        If you have multiple versions of Python and pip on your machine, try: `pip3 install transitleastsquares`
+        
+        The latest version can be pulled from github::
+        ```
+        git clone https://github.com/hippke/tls.git
+        cd tls
+        python setup.py install
+        ```
+        
+        If the command `python` does not point to Python 3 on your machine, you can try to replace the last line with `python3 setup.py install`. If you don't have `git` on your machine, you can find installation instructions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). TLS also runs on Python 2, but without multi-threading.
+        
+        
+        Dependencies:
+        Python 3,
+        [NumPy](http://www.numpy.org/),
+        [numba](http://numba.pydata.org/),
+        [batman-package](https://www.cfa.harvard.edu/~lkreidberg/batman/),
+        [tqdm](https://github.com/tqdm/tqdm),
+        optional:
+        [argparse](https://docs.python.org/3/library/argparse.html) (for the command line version),
+        [astroquery](https://astroquery.readthedocs.io/en/latest/) (for LD and stellar density priors from Kepler K1, K2, and TESS).
+        
+        If you have trouble installing, please [open an issue](https://github.com/hippke/tls/issues).
+        
+        
+        ## Getting started
+        Here is a short animation of a real search for planets in Kepler K2 data. For more examples, have a look at the [tutorials](https://github.com/hippke/tls/tree/master/tutorials) and the [documentation](https://transitleastsquares.readthedocs.io/en/latest/index.html).
+        
+        ![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/animation.gif)
+        
+        ## Attribution
+        Please cite [Hippke & Heller (2019, A&A 623, A39)](https://ui.adsabs.harvard.edu/#abs/2019A&A...623A..39H/abstract) if you find this code useful in your research. The BibTeX entry for the paper is:
+        
+        ```
+        @ARTICLE{2019A&A...623A..39H,
+               author = {{Hippke}, Michael and {Heller}, Ren{\'e}},
+                title = "{Optimized transit detection algorithm to search for periodic transits of small planets}",
+              journal = {\aap},
+                 year = "2019",
+                month = "Mar",
+               volume = {623},
+                  eid = {A39},
+                pages = {A39},
+                  doi = {10.1051/0004-6361/201834672},
+        archivePrefix = {arXiv},
+               eprint = {1901.02015},
+         primaryClass = {astro-ph.EP},
+               adsurl = {https://ui.adsabs.harvard.edu/\#abs/2019A&A...623A..39H},
+              adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+        }
+        ```
+        
+        ## Contributing Code, Bugfixes, or Feedback
+        We welcome and encourage contributions. If you have any trouble, [open an issue](https://github.com/hippke/tls/issues).
+        
+        Copyright 2019 Michael Hippke & René Heller.
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
-### An optimized transit-fitting algorithm to search for periodic transits of small planets
-[![Image](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/hippke/tls/blob/master/LICENSE)
-[![Image](https://img.shields.io/badge/Python-2.7%20%26%203.5%2B-blue.svg)](https://pypi.org/project/transitleastsquares/)
-[![Image](https://img.shields.io/badge/pip%20install-transitleastsquares-blue.svg)](https://pypi.org/project/transitleastsquares/)
-[![Image](https://img.shields.io/badge/documentation-%E2%9C%93-blue.svg)](https://transitleastsquares.readthedocs.io/en/latest/index.html)
-[![Image](https://img.shields.io/badge/tutorials-%E2%9C%93-blue.svg)](https://github.com/hippke/tls/tree/master/tutorials)
-[![Image](https://img.shields.io/badge/arXiv-1901.02015-blue.svg)](https://arxiv.org/abs/1901.02015)
-[![Build Status](https://travis-ci.com/hippke/tls.svg?branch=master)](https://travis-ci.com/hippke/tls)
-
-
-## Motivation
-We present a new method to detect planetary transits from time-series photometry, the *Transit Least Squares* (TLS) algorithm. While the commonly used Box Least Squares [(BLS, Kovács et al. 2002)](http://adsabs.harvard.edu/abs/2002A%26A...391..369K) algorithm searches for rectangular signals in stellar light curves, *TLS* searches for transit-like features with stellar limb-darkening and including the effects of planetary ingress and egress. Moreover, *TLS* analyses the entire, unbinned data of the phase-folded light curve. These improvements yield a ~10 % higher detection efficiency (and similar false alarm rates) compared to BLS. The higher detection efficiency of our freely available Python implementation comes at the cost of higher computational load, which we partly compensate by applying an optimized period sampling and transit duration sampling, constrained to the physically plausible range. A typical Kepler K2 light curve, worth of 90 d of observations at a cadence of 30 min, can be searched with *TLS* in 10 seconds real time on a standard laptop computer, just as with BLS.
-
-![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/frontpage_rescaled.png)
-
-## Installation
-
-TLS can be installed conveniently using: `pip install transitleastsquares`
-
-If you have multiple versions of Python and pip on your machine, try: `pip3 install transitleastsquares`
-
-The latest version can be pulled from github::
-```
-git clone https://github.com/hippke/tls.git
-cd tls
-python setup.py install
-```
-
-If the command `python` does not point to Python 3 on your machine, you can try to replace the last line with `python3 setup.py install`. If you don't have `git` on your machine, you can find installation instructions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). TLS also runs on Python 2, but without multi-threading.
-
-
-Dependencies:
-Python 3,
-[NumPy](http://www.numpy.org/),
-[numba](http://numba.pydata.org/),
-[batman-package](https://www.cfa.harvard.edu/~lkreidberg/batman/),
-[tqdm](https://github.com/tqdm/tqdm),
-optional:
-[argparse](https://docs.python.org/3/library/argparse.html) (for the command line version),
-[astroquery](https://astroquery.readthedocs.io/en/latest/) (for LD and stellar density priors from Kepler K1, K2, and TESS).
-
-If you have trouble installing, please [open an issue](https://github.com/hippke/tls/issues).
-
-
-## Getting started
-Here is a short animation of a real search for planets in Kepler K2 data. For more examples, have a look at the [tutorials](https://github.com/hippke/tls/tree/master/tutorials) and the [documentation](https://transitleastsquares.readthedocs.io/en/latest/index.html).
-
-![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/animation.gif)
-
-## Attribution
-Please cite [Hippke & Heller (2019, A&A 623, A39)](https://ui.adsabs.harvard.edu/#abs/2019A&A...623A..39H/abstract) if you find this code useful in your research. The BibTeX entry for the paper is:
-
-```
-@ARTICLE{2019A&A...623A..39H,
-       author = {{Hippke}, Michael and {Heller}, Ren{\'e}},
-        title = "{Optimized transit detection algorithm to search for periodic transits of small planets}",
-      journal = {\aap},
-         year = "2019",
-        month = "Mar",
-       volume = {623},
-          eid = {A39},
-        pages = {A39},
-          doi = {10.1051/0004-6361/201834672},
-archivePrefix = {arXiv},
-       eprint = {1901.02015},
- primaryClass = {astro-ph.EP},
-       adsurl = {https://ui.adsabs.harvard.edu/\#abs/2019A&A...623A..39H},
-      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-}
-```
-
-## Contributing Code, Bugfixes, or Feedback
-We welcome and encourage contributions. If you have any trouble, [open an issue](https://github.com/hippke/tls/issues).
-
-Copyright 2019 Michael Hippke & René Heller.
-
-
```

### Comparing `foldedleastsquares-1.0.39/LICENSE` & `foldedleastsquares-1.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/README.md` & `foldedleastsquares-1.0.41/foldedleastsquares.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,87 @@
-![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
-### An optimized transit-fitting algorithm to search for periodic transits of small planets
-[![Image](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/hippke/tls/blob/master/LICENSE)
-[![Image](https://img.shields.io/badge/Python-2.7%20%26%203.5%2B-blue.svg)](https://pypi.org/project/transitleastsquares/)
-[![Image](https://img.shields.io/badge/pip%20install-transitleastsquares-blue.svg)](https://pypi.org/project/transitleastsquares/)
-[![Image](https://img.shields.io/badge/documentation-%E2%9C%93-blue.svg)](https://transitleastsquares.readthedocs.io/en/latest/index.html)
-[![Image](https://img.shields.io/badge/tutorials-%E2%9C%93-blue.svg)](https://github.com/hippke/tls/tree/master/tutorials)
-[![Image](https://img.shields.io/badge/arXiv-1901.02015-blue.svg)](https://arxiv.org/abs/1901.02015)
-[![Build Status](https://travis-ci.com/hippke/tls.svg?branch=master)](https://travis-ci.com/hippke/tls)
-
-
-## Motivation
-We present a new method to detect planetary transits from time-series photometry, the *Transit Least Squares* (TLS) algorithm. While the commonly used Box Least Squares [(BLS, Kovács et al. 2002)](http://adsabs.harvard.edu/abs/2002A%26A...391..369K) algorithm searches for rectangular signals in stellar light curves, *TLS* searches for transit-like features with stellar limb-darkening and including the effects of planetary ingress and egress. Moreover, *TLS* analyses the entire, unbinned data of the phase-folded light curve. These improvements yield a ~10 % higher detection efficiency (and similar false alarm rates) compared to BLS. The higher detection efficiency of our freely available Python implementation comes at the cost of higher computational load, which we partly compensate by applying an optimized period sampling and transit duration sampling, constrained to the physically plausible range. A typical Kepler K2 light curve, worth of 90 d of observations at a cadence of 30 min, can be searched with *TLS* in 10 seconds real time on a standard laptop computer, just as with BLS.
-
-![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/frontpage_rescaled.png)
-
-## Installation
-
-TLS can be installed conveniently using: `pip install transitleastsquares`
-
-If you have multiple versions of Python and pip on your machine, try: `pip3 install transitleastsquares`
-
-The latest version can be pulled from github::
-```
-git clone https://github.com/hippke/tls.git
-cd tls
-python setup.py install
-```
-
-If the command `python` does not point to Python 3 on your machine, you can try to replace the last line with `python3 setup.py install`. If you don't have `git` on your machine, you can find installation instructions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). TLS also runs on Python 2, but without multi-threading.
-
-
-Dependencies:
-Python 3,
-[NumPy](http://www.numpy.org/),
-[numba](http://numba.pydata.org/),
-[batman-package](https://www.cfa.harvard.edu/~lkreidberg/batman/),
-[tqdm](https://github.com/tqdm/tqdm),
-optional:
-[argparse](https://docs.python.org/3/library/argparse.html) (for the command line version),
-[astroquery](https://astroquery.readthedocs.io/en/latest/) (for LD and stellar density priors from Kepler K1, K2, and TESS).
-
-If you have trouble installing, please [open an issue](https://github.com/hippke/tls/issues).
-
-
-## Getting started
-Here is a short animation of a real search for planets in Kepler K2 data. For more examples, have a look at the [tutorials](https://github.com/hippke/tls/tree/master/tutorials) and the [documentation](https://transitleastsquares.readthedocs.io/en/latest/index.html).
-
-![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/animation.gif)
-
-## Attribution
-Please cite [Hippke & Heller (2019, A&A 623, A39)](https://ui.adsabs.harvard.edu/#abs/2019A&A...623A..39H/abstract) if you find this code useful in your research. The BibTeX entry for the paper is:
-
-```
-@ARTICLE{2019A&A...623A..39H,
-       author = {{Hippke}, Michael and {Heller}, Ren{\'e}},
-        title = "{Optimized transit detection algorithm to search for periodic transits of small planets}",
-      journal = {\aap},
-         year = "2019",
-        month = "Mar",
-       volume = {623},
-          eid = {A39},
-        pages = {A39},
-          doi = {10.1051/0004-6361/201834672},
-archivePrefix = {arXiv},
-       eprint = {1901.02015},
- primaryClass = {astro-ph.EP},
-       adsurl = {https://ui.adsabs.harvard.edu/\#abs/2019A&A...623A..39H},
-      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-}
-```
-
-## Contributing Code, Bugfixes, or Feedback
-We welcome and encourage contributions. If you have any trouble, [open an issue](https://github.com/hippke/tls/issues).
-
-Copyright 2019 Michael Hippke & René Heller.
+Metadata-Version: 2.1
+Name: foldedleastsquares
+Version: 1.0.41
+Summary: An optimized transit-fitting algorithm to search for periodic features in light curves
+Home-page: https://github.com/hippke/tls
+Author: Martín Dévora Pajares
+Author-email: martin.devora.pajares@gmail.com
+License: MIT
+Description: ![Logo](https://raw.githubusercontent.com/hippke/tls/master/docs/source/logo.png)
+        ### An optimized transit-fitting algorithm to search for periodic transits of small planets
+        [![Image](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/hippke/tls/blob/master/LICENSE)
+        [![Image](https://img.shields.io/badge/Python-2.7%20%26%203.5%2B-blue.svg)](https://pypi.org/project/transitleastsquares/)
+        [![Image](https://img.shields.io/badge/pip%20install-transitleastsquares-blue.svg)](https://pypi.org/project/transitleastsquares/)
+        [![Image](https://img.shields.io/badge/documentation-%E2%9C%93-blue.svg)](https://transitleastsquares.readthedocs.io/en/latest/index.html)
+        [![Image](https://img.shields.io/badge/tutorials-%E2%9C%93-blue.svg)](https://github.com/hippke/tls/tree/master/tutorials)
+        [![Image](https://img.shields.io/badge/arXiv-1901.02015-blue.svg)](https://arxiv.org/abs/1901.02015)
+        [![Build Status](https://travis-ci.com/hippke/tls.svg?branch=master)](https://travis-ci.com/hippke/tls)
+        
+        
+        ## Motivation
+        We present a new method to detect planetary transits from time-series photometry, the *Transit Least Squares* (TLS) algorithm. While the commonly used Box Least Squares [(BLS, Kovács et al. 2002)](http://adsabs.harvard.edu/abs/2002A%26A...391..369K) algorithm searches for rectangular signals in stellar light curves, *TLS* searches for transit-like features with stellar limb-darkening and including the effects of planetary ingress and egress. Moreover, *TLS* analyses the entire, unbinned data of the phase-folded light curve. These improvements yield a ~10 % higher detection efficiency (and similar false alarm rates) compared to BLS. The higher detection efficiency of our freely available Python implementation comes at the cost of higher computational load, which we partly compensate by applying an optimized period sampling and transit duration sampling, constrained to the physically plausible range. A typical Kepler K2 light curve, worth of 90 d of observations at a cadence of 30 min, can be searched with *TLS* in 10 seconds real time on a standard laptop computer, just as with BLS.
+        
+        ![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/frontpage_rescaled.png)
+        
+        ## Installation
+        
+        TLS can be installed conveniently using: `pip install transitleastsquares`
+        
+        If you have multiple versions of Python and pip on your machine, try: `pip3 install transitleastsquares`
+        
+        The latest version can be pulled from github::
+        ```
+        git clone https://github.com/hippke/tls.git
+        cd tls
+        python setup.py install
+        ```
+        
+        If the command `python` does not point to Python 3 on your machine, you can try to replace the last line with `python3 setup.py install`. If you don't have `git` on your machine, you can find installation instructions [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). TLS also runs on Python 2, but without multi-threading.
+        
+        
+        Dependencies:
+        Python 3,
+        [NumPy](http://www.numpy.org/),
+        [numba](http://numba.pydata.org/),
+        [batman-package](https://www.cfa.harvard.edu/~lkreidberg/batman/),
+        [tqdm](https://github.com/tqdm/tqdm),
+        optional:
+        [argparse](https://docs.python.org/3/library/argparse.html) (for the command line version),
+        [astroquery](https://astroquery.readthedocs.io/en/latest/) (for LD and stellar density priors from Kepler K1, K2, and TESS).
+        
+        If you have trouble installing, please [open an issue](https://github.com/hippke/tls/issues).
+        
+        
+        ## Getting started
+        Here is a short animation of a real search for planets in Kepler K2 data. For more examples, have a look at the [tutorials](https://github.com/hippke/tls/tree/master/tutorials) and the [documentation](https://transitleastsquares.readthedocs.io/en/latest/index.html).
+        
+        ![image](https://raw.githubusercontent.com/hippke/tls/master/docs/source/animation.gif)
+        
+        ## Attribution
+        Please cite [Hippke & Heller (2019, A&A 623, A39)](https://ui.adsabs.harvard.edu/#abs/2019A&A...623A..39H/abstract) if you find this code useful in your research. The BibTeX entry for the paper is:
+        
+        ```
+        @ARTICLE{2019A&A...623A..39H,
+               author = {{Hippke}, Michael and {Heller}, Ren{\'e}},
+                title = "{Optimized transit detection algorithm to search for periodic transits of small planets}",
+              journal = {\aap},
+                 year = "2019",
+                month = "Mar",
+               volume = {623},
+                  eid = {A39},
+                pages = {A39},
+                  doi = {10.1051/0004-6361/201834672},
+        archivePrefix = {arXiv},
+               eprint = {1901.02015},
+         primaryClass = {astro-ph.EP},
+               adsurl = {https://ui.adsabs.harvard.edu/\#abs/2019A&A...623A..39H},
+              adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+        }
+        ```
+        
+        ## Contributing Code, Bugfixes, or Feedback
+        We welcome and encourage contributions. If you have any trouble, [open an issue](https://github.com/hippke/tls/issues).
+        
+        Copyright 2019 Michael Hippke & René Heller.
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `foldedleastsquares-1.0.39/setup.py` & `foldedleastsquares-1.0.41/setup.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/template_generator/tailed_transit_template_generator.py` & `foldedleastsquares-1.0.41/foldedleastsquares/template_generator/tailed_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/template_generator/transit_template_generator.py` & `foldedleastsquares-1.0.41/foldedleastsquares/template_generator/transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/template_generator/default_transit_template_generator.py` & `foldedleastsquares-1.0.41/foldedleastsquares/template_generator/default_transit_template_generator.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/__init__.py` & `foldedleastsquares-1.0.41/foldedleastsquares/__init__.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/core.py` & `foldedleastsquares-1.0.41/foldedleastsquares/core.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/catalog.py` & `foldedleastsquares-1.0.41/foldedleastsquares/catalog.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-from __future__ import division, print_function
-import numpy
-from os import path
-from . import tls_constants
-
-
-def catalog_info_KIC(KIC_ID):
-    """Takes KIC_ID, returns stellar information from online catalog using Vizier"""
-
-    if type(KIC_ID) is not int:
-        raise TypeError('KIC_ID ID must be of type "int"')
-    try:
-        from astroquery.vizier import Vizier
-    except:
-        raise ImportError("Package astroquery required but failed to import")
-
-    columns = ["Teff", "log(g)", "Rad", "E_Rad", "e_Rad", "Mass", "E_Mass", "e_Mass"]
-    catalog = "J/ApJS/229/30/catalog"
-    result = (
-        Vizier(columns=columns)
-        .query_constraints(KIC=KIC_ID, catalog=catalog)[0]
-        .as_array()
-    )
-    Teff = result[0][0]
-    logg = result[0][1]
-    radius = result[0][2]
-    radius_max = result[0][3]
-    radius_min = result[0][4]
-    mass = result[0][5]
-    mass_max = result[0][6]
-    mass_min = result[0][7]
-    return Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max
-
-
-def catalog_info_EPIC(EPIC_ID):
-    """Takes EPIC_ID, returns stellar information from online catalog using Vizier"""
-
-    try:
-        from astroquery.vizier import Vizier
-    except:
-        raise ImportError("Package astroquery required but failed to import")
-    if type(EPIC_ID) is not int:
-        raise TypeError('EPIC_ID ID must be of type "int"')
-    if (EPIC_ID < 201000001) or (EPIC_ID > 251813738):
-        raise TypeError("EPIC_ID ID must be in range 201000001 to 251813738")
-    columns = ["Teff", "logg", "Rad", "E_Rad", "e_Rad", "Mass", "E_Mass", "e_Mass"]
-    catalog = "IV/34/epic"
-    result = (
-        Vizier(columns=columns)
-        .query_constraints(ID=EPIC_ID, catalog=catalog)[0]
-        .as_array()
-    )
-    Teff = result[0][0]
-    logg = result[0][1]
-    radius = result[0][2]
-    radius_max = result[0][3]
-    radius_min = result[0][4]
-    mass = result[0][5]
-    mass_max = result[0][6]
-    mass_min = result[0][7]
-    return Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max
-
-
-def catalog_info_TIC(TIC_ID):
-    """Takes TIC_ID, returns stellar information from online catalog using Vizier"""
-    if type(TIC_ID) is not int:
-        raise TypeError('TIC_ID ID must be of type "int"')
-    try:
-        from astroquery.mast import Catalogs
-    except:
-        raise ImportError("Package astroquery required but failed to import")
-
-    result = Catalogs.query_criteria(catalog="Tic", ID=TIC_ID).as_array()
-    Teff = result[0][64]
-    logg = result[0][66]
-    radius = result[0][70]
-    radius_max = result[0][71]
-    radius_min = result[0][71]
-    mass = result[0][72]
-    mass_max = result[0][73]
-    mass_min = result[0][73]
-    return Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max
-
-
-def catalog_info(EPIC_ID=None, TIC_ID=None, KIC_ID=None):
-    """Takes EPIC ID, returns limb darkening parameters u (linear) and
-        a,b (quadratic), and stellar parameters. Values are pulled for minimum
-        absolute deviation between given/catalog Teff and logg. Data are from:
-        - K2 Ecliptic Plane Input Catalog, Huber+ 2016, 2016ApJS..224....2H
-        - New limb-darkening coefficients, Claret+ 2012, 2013,
-          2012A&A...546A..14C, 2013A&A...552A..16C"""
-
-    if (EPIC_ID is None) and (TIC_ID is None) and (KIC_ID is None):
-        raise ValueError("No ID was given")
-    if (EPIC_ID is not None) and (TIC_ID is not None):
-        raise ValueError("Only one ID allowed")
-    if (EPIC_ID is not None) and (KIC_ID is not None):
-        raise ValueError("Only one ID allowed")
-    if (TIC_ID is not None) and (KIC_ID is not None):
-        raise ValueError("Only one ID allowed")
-
-    # KOI CASE (Kepler K1)
-    if KIC_ID is not None:
-        Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max = catalog_info_KIC(
-            KIC_ID
-        )
-
-    # EPIC CASE (Kepler K2)
-    if EPIC_ID is not None:
-        Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max = catalog_info_EPIC(
-            EPIC_ID
-        )
-
-    # TESS CASE
-    if TIC_ID is not None:
-        Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max = catalog_info_TIC(
-            TIC_ID
-        )
-        ld = numpy.genfromtxt(
-            path.join(tls_constants.resources_dir, "ld_claret_tess.csv"),
-            skip_header=1,
-            delimiter=",",
-            dtype="f8, int32, f8, f8",
-            names=["logg", "Teff", "a", "b"],
-        )
-    else:  # Limb darkening is the same for K1 (KIC) and K2 (EPIC)
-        ld = numpy.genfromtxt(
-            path.join(tls_constants.resources_dir, "JAA546A14limb1-4.csv"),
-            skip_header=1,
-            delimiter=",",
-            dtype="f8, int32, f8, f8, f8",
-            names=["logg", "Teff", "u", "a", "b"],
-        )
-
-    if logg is None:
-        logg = 4
-        warnings.warn("No logg in catalog. Proceeding with logg=4")
-
-    if Teff is None:
-        Teff = 6000
-        warnings.warn("No Teff in catalog. Proceeding with Teff=6000")
-
-    """From here on, K2 and TESS catalogs work the same:
-        - Take Teff from star catalog and find nearest entry in LD catalog
-        - Same for logg, but only for the Teff values returned before
-        - Return stellar parameters and best-match LD
-    """
-    nearest_Teff = ld["Teff"][(numpy.abs(ld["Teff"] - Teff)).argmin()]
-    idx_all_Teffs = numpy.where(ld["Teff"] == nearest_Teff)
-    relevant_lds = numpy.copy(ld[idx_all_Teffs])
-    idx_nearest = numpy.abs(relevant_lds["logg"] - logg).argmin()
-    a = relevant_lds["a"][idx_nearest]
-    b = relevant_lds["b"][idx_nearest]
-
-    mass = numpy.array(mass)
-    mass_min = numpy.array(mass_min)
-    mass_max = numpy.array(mass_max)
-    radius = numpy.array(radius)
-    radius_min = numpy.array(radius_min)
-    radius_max = numpy.array(radius_max)
-
-    if mass == 0.0:
-        mass = numpy.nan
-    if mass_min == 0.0:
-        mass_min = numpy.nan
-    if mass_max == 0.0:
-        mass_max = numpy.nan
-    if radius == 0.0:
-        radius = numpy.nan
-    if radius_min == 0.0:
-        radius_min = numpy.nan
-    if radius_max == 0.0:
-        radius_max = numpy.nan
-
-    return ((a, b), mass, mass_min, mass_max, radius, radius_min, radius_max)
+from __future__ import division, print_function
+import numpy
+from os import path
+from . import tls_constants
+
+
+def catalog_info_KIC(KIC_ID):
+    """Takes KIC_ID, returns stellar information from online catalog using Vizier"""
+
+    if type(KIC_ID) is not int:
+        raise TypeError('KIC_ID ID must be of type "int"')
+    try:
+        from astroquery.vizier import Vizier
+    except:
+        raise ImportError("Package astroquery required but failed to import")
+
+    columns = ["Teff", "log(g)", "Rad", "E_Rad", "e_Rad", "Mass", "E_Mass", "e_Mass"]
+    catalog = "J/ApJS/229/30/catalog"
+    result = (
+        Vizier(columns=columns)
+        .query_constraints(KIC=KIC_ID, catalog=catalog)[0]
+        .as_array()
+    )
+    Teff = result[0][0]
+    logg = result[0][1]
+    radius = result[0][2]
+    radius_max = result[0][3]
+    radius_min = result[0][4]
+    mass = result[0][5]
+    mass_max = result[0][6]
+    mass_min = result[0][7]
+    return Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max
+
+
+def catalog_info_EPIC(EPIC_ID):
+    """Takes EPIC_ID, returns stellar information from online catalog using Vizier"""
+
+    try:
+        from astroquery.vizier import Vizier
+    except:
+        raise ImportError("Package astroquery required but failed to import")
+    if type(EPIC_ID) is not int:
+        raise TypeError('EPIC_ID ID must be of type "int"')
+    if (EPIC_ID < 201000001) or (EPIC_ID > 251813738):
+        raise TypeError("EPIC_ID ID must be in range 201000001 to 251813738")
+    columns = ["Teff", "logg", "Rad", "E_Rad", "e_Rad", "Mass", "E_Mass", "e_Mass"]
+    catalog = "IV/34/epic"
+    result = (
+        Vizier(columns=columns)
+        .query_constraints(ID=EPIC_ID, catalog=catalog)[0]
+        .as_array()
+    )
+    Teff = result[0][0]
+    logg = result[0][1]
+    radius = result[0][2]
+    radius_max = result[0][3]
+    radius_min = result[0][4]
+    mass = result[0][5]
+    mass_max = result[0][6]
+    mass_min = result[0][7]
+    return Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max
+
+
+def catalog_info_TIC(TIC_ID):
+    """Takes TIC_ID, returns stellar information from online catalog using Vizier"""
+    if type(TIC_ID) is not int:
+        raise TypeError('TIC_ID ID must be of type "int"')
+    try:
+        from astroquery.mast import Catalogs
+    except:
+        raise ImportError("Package astroquery required but failed to import")
+
+    result = Catalogs.query_criteria(catalog="Tic", ID=TIC_ID).as_array()
+    Teff = result[0][64]
+    logg = result[0][66]
+    radius = result[0][70]
+    radius_max = result[0][71]
+    radius_min = result[0][71]
+    mass = result[0][72]
+    mass_max = result[0][73]
+    mass_min = result[0][73]
+    return Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max
+
+
+def catalog_info(EPIC_ID=None, TIC_ID=None, KIC_ID=None):
+    """Takes EPIC ID, returns limb darkening parameters u (linear) and
+        a,b (quadratic), and stellar parameters. Values are pulled for minimum
+        absolute deviation between given/catalog Teff and logg. Data are from:
+        - K2 Ecliptic Plane Input Catalog, Huber+ 2016, 2016ApJS..224....2H
+        - New limb-darkening coefficients, Claret+ 2012, 2013,
+          2012A&A...546A..14C, 2013A&A...552A..16C"""
+
+    if (EPIC_ID is None) and (TIC_ID is None) and (KIC_ID is None):
+        raise ValueError("No ID was given")
+    if (EPIC_ID is not None) and (TIC_ID is not None):
+        raise ValueError("Only one ID allowed")
+    if (EPIC_ID is not None) and (KIC_ID is not None):
+        raise ValueError("Only one ID allowed")
+    if (TIC_ID is not None) and (KIC_ID is not None):
+        raise ValueError("Only one ID allowed")
+
+    # KOI CASE (Kepler K1)
+    if KIC_ID is not None:
+        Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max = catalog_info_KIC(
+            KIC_ID
+        )
+
+    # EPIC CASE (Kepler K2)
+    if EPIC_ID is not None:
+        Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max = catalog_info_EPIC(
+            EPIC_ID
+        )
+
+    # TESS CASE
+    if TIC_ID is not None:
+        Teff, logg, radius, radius_min, radius_max, mass, mass_min, mass_max = catalog_info_TIC(
+            TIC_ID
+        )
+        ld = numpy.genfromtxt(
+            path.join(tls_constants.resources_dir, "ld_claret_tess.csv"),
+            skip_header=1,
+            delimiter=",",
+            dtype="f8, int32, f8, f8",
+            names=["logg", "Teff", "a", "b"],
+        )
+    else:  # Limb darkening is the same for K1 (KIC) and K2 (EPIC)
+        ld = numpy.genfromtxt(
+            path.join(tls_constants.resources_dir, "JAA546A14limb1-4.csv"),
+            skip_header=1,
+            delimiter=",",
+            dtype="f8, int32, f8, f8, f8",
+            names=["logg", "Teff", "u", "a", "b"],
+        )
+
+    if logg is None:
+        logg = 4
+        warnings.warn("No logg in catalog. Proceeding with logg=4")
+
+    if Teff is None:
+        Teff = 6000
+        warnings.warn("No Teff in catalog. Proceeding with Teff=6000")
+
+    """From here on, K2 and TESS catalogs work the same:
+        - Take Teff from star catalog and find nearest entry in LD catalog
+        - Same for logg, but only for the Teff values returned before
+        - Return stellar parameters and best-match LD
+    """
+    nearest_Teff = ld["Teff"][(numpy.abs(ld["Teff"] - Teff)).argmin()]
+    idx_all_Teffs = numpy.where(ld["Teff"] == nearest_Teff)
+    relevant_lds = numpy.copy(ld[idx_all_Teffs])
+    idx_nearest = numpy.abs(relevant_lds["logg"] - logg).argmin()
+    a = relevant_lds["a"][idx_nearest]
+    b = relevant_lds["b"][idx_nearest]
+
+    mass = numpy.array(mass)
+    mass_min = numpy.array(mass_min)
+    mass_max = numpy.array(mass_max)
+    radius = numpy.array(radius)
+    radius_min = numpy.array(radius_min)
+    radius_max = numpy.array(radius_max)
+
+    if mass == 0.0:
+        mass = numpy.nan
+    if mass_min == 0.0:
+        mass_min = numpy.nan
+    if mass_max == 0.0:
+        mass_max = numpy.nan
+    if radius == 0.0:
+        radius = numpy.nan
+    if radius_min == 0.0:
+        radius_min = numpy.nan
+    if radius_max == 0.0:
+        radius_max = numpy.nan
+
+    return ((a, b), mass, mass_min, mass_max, radius, radius_min, radius_max)
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_transit_depth_min.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_transit_depth_min.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,75 @@
-from __future__ import division, print_function
-import numpy
-import batman
-from foldedleastsquares import transitleastsquares
-
-
-if __name__ == "__main__":
-    print("Starting test: transit_depth_min...", end="")
-    # Test for transit_depth_min=1000*10**-6, where no transit is found
-
-    # Create test data
-    start = 48
-    days = 365.25 * 3
-    samples_per_day = 12  # 48
-    samples = int(days * samples_per_day)  # 48
-    t = numpy.linspace(start, start + days, samples)
-
-    # Use batman to create transits
-    ma = batman.TransitParams()
-    ma.t0 = (
-        start + 20
-    )  # time of inferior conjunction; first transit is X days after start
-    ma.per = 365.25  # orbital period
-    ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
-    ma.a = 217  # semi-major axis (in units of stellar radii)
-    ma.inc = 90  # orbital inclination (in degrees)
-    ma.ecc = 0  # eccentricity
-    ma.w = 90  # longitude of periastron (in degrees)
-    ma.u = [0.5]  # limb darkening coefficients
-    ma.limb_dark = "linear"  # limb darkening model
-    m = batman.TransitModel(ma, t)  # initializes model
-    original_flux = m.light_curve(ma)  # calculates light curve
-
-    # Create noise and merge with flux
-    ppm = 5
-    stdev = 10 ** -6 * ppm
-    noise = numpy.random.normal(0, stdev, int(samples))
-    y = original_flux + noise
-    y[1] = numpy.nan
-    model = transitleastsquares(t, y)
-    results = model.power(
-        transit_depth_min=1000 * 10 ** -6,
-        period_min=360,
-        period_max=370,
-        oversampling_factor=5,
-        duration_grid_step=1.02,
-        T0_fit_margin=0.1,
-    )
-
-    numpy.testing.assert_equal(results.transit_times, numpy.nan)
-    numpy.testing.assert_equal(results.period, numpy.nan)
-    numpy.testing.assert_equal(results.depth, 1)
-    numpy.testing.assert_equal(results.duration, numpy.nan)
-    numpy.testing.assert_equal(results.snr, numpy.nan)
-    numpy.testing.assert_equal(results.snr_pink_per_transit, numpy.nan)
-    numpy.testing.assert_equal(results.odd_even_mismatch, numpy.nan)
-    numpy.testing.assert_equal(results.SDE, 0)
-    numpy.testing.assert_equal(results.SDE_raw, 0)
-    numpy.testing.assert_equal(results.in_transit_count, numpy.nan)
-    numpy.testing.assert_equal(results.after_transit_count, numpy.nan)
-    numpy.testing.assert_equal(results.before_transit_count, numpy.nan)
-    numpy.testing.assert_almost_equal(results.chi2_min, 13148.0)
-    numpy.testing.assert_almost_equal(results.chi2red_min, 1.0003043213633598)
-    numpy.testing.assert_equal(len(results.periods), 278)
-    numpy.testing.assert_almost_equal(max(results.periods), 369.9831654894093)
-    numpy.testing.assert_almost_equal(min(results.periods), 360.0118189140635)
-    numpy.testing.assert_almost_equal(max(results.power), 0)
-    numpy.testing.assert_almost_equal(min(results.periods), 360.0118189140635)
-    numpy.testing.assert_almost_equal(min(results.power), 0)
-    numpy.testing.assert_almost_equal(max(results.chi2), 13148.0)
-    numpy.testing.assert_almost_equal(max(results.chi2red), 1.0003043213633598)
-    print("Test passed: transit_depth_min=1000*10**-6, where no transit is fit")
+from __future__ import division, print_function
+import numpy
+import batman
+from foldedleastsquares import transitleastsquares
+
+
+import unittest
+
+class TestTransitDepthMin(unittest.TestCase):
+    def test(self):
+        print("Starting test: transit_depth_min...", end="")
+        # Test for transit_depth_min=1000*10**-6, where no transit is found
+
+        # Create test data
+        start = 48
+        days = 365.25 * 3
+        samples_per_day = 12  # 48
+        samples = int(days * samples_per_day)  # 48
+        t = numpy.linspace(start, start + days, samples)
+
+        # Use batman to create transits
+        ma = batman.TransitParams()
+        ma.t0 = (
+            start + 20
+        )  # time of inferior conjunction; first transit is X days after start
+        ma.per = 365.25  # orbital period
+        ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
+        ma.a = 217  # semi-major axis (in units of stellar radii)
+        ma.inc = 90  # orbital inclination (in degrees)
+        ma.ecc = 0  # eccentricity
+        ma.w = 90  # longitude of periastron (in degrees)
+        ma.u = [0.5]  # limb darkening coefficients
+        ma.limb_dark = "linear"  # limb darkening model
+        m = batman.TransitModel(ma, t)  # initializes model
+        original_flux = m.light_curve(ma)  # calculates light curve
+
+        # Create noise and merge with flux
+        ppm = 5
+        stdev = 10 ** -6 * ppm
+        noise = numpy.random.normal(0, stdev, int(samples))
+        y = original_flux + noise
+        y[1] = numpy.nan
+        model = transitleastsquares(t, y)
+        results = model.power(
+            transit_depth_min=1000 * 10 ** -6,
+            period_min=360,
+            period_max=370,
+            oversampling_factor=5,
+            duration_grid_step=1.02,
+            T0_fit_margin=0.1,
+        )
+
+        numpy.testing.assert_equal(results.transit_times, numpy.nan)
+        numpy.testing.assert_equal(results.period, numpy.nan)
+        numpy.testing.assert_equal(results.depth, 1)
+        numpy.testing.assert_equal(results.duration, numpy.nan)
+        numpy.testing.assert_equal(results.snr, numpy.nan)
+        numpy.testing.assert_equal(results.snr_pink_per_transit, numpy.nan)
+        numpy.testing.assert_equal(results.odd_even_mismatch, numpy.nan)
+        numpy.testing.assert_equal(results.SDE, 0)
+        numpy.testing.assert_equal(results.SDE_raw, 0)
+        numpy.testing.assert_equal(results.in_transit_count, numpy.nan)
+        numpy.testing.assert_equal(results.after_transit_count, numpy.nan)
+        numpy.testing.assert_equal(results.before_transit_count, numpy.nan)
+        numpy.testing.assert_almost_equal(results.chi2_min, 13148.0)
+        numpy.testing.assert_almost_equal(results.chi2red_min, 1.0003043213633598)
+        numpy.testing.assert_equal(len(results.periods), 278)
+        numpy.testing.assert_almost_equal(max(results.periods), 369.9831654894093)
+        numpy.testing.assert_almost_equal(min(results.periods), 360.0118189140635)
+        numpy.testing.assert_almost_equal(max(results.power), 0)
+        numpy.testing.assert_almost_equal(min(results.periods), 360.0118189140635)
+        numpy.testing.assert_almost_equal(min(results.power), 0)
+        numpy.testing.assert_almost_equal(max(results.chi2), 13148.0)
+        numpy.testing.assert_almost_equal(max(results.chi2red), 1.0003043213633598)
+        print("Test passed: transit_depth_min=1000*10**-6, where no transit is fit")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_period_grid.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_period_grid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,67 @@
-from __future__ import division, print_function
-import numpy
-
-from foldedleastsquares import DefaultTransitTemplateGenerator
-
-if __name__ == "__main__":
-    print("Starting test: period_grid...", end="")
-    default_transit_template_generator = DefaultTransitTemplateGenerator()
-    periods = default_transit_template_generator.period_grid(R_star=1, M_star=1, time_span=0.1)
-    numpy.testing.assert_almost_equal(max(periods), 2.4999999999999987)
-    numpy.testing.assert_almost_equal(min(periods), 0.6002621413799498)
-    numpy.testing.assert_equal(len(periods), 268)
-
-    periods = default_transit_template_generator.period_grid(R_star=1, M_star=1, time_span=20)
-    numpy.testing.assert_almost_equal(max(periods), 10)
-    numpy.testing.assert_almost_equal(min(periods), 0.6015575922909607)
-    numpy.testing.assert_equal(len(periods), 1716)
-
-    periods = default_transit_template_generator.period_grid(
-        R_star=5,  # R_sun
-        M_star=1,  # M_sun
-        time_span=20,  # days
-        period_min=0,
-        period_max=999,
-        oversampling_factor=3,
-    )
-    numpy.testing.assert_almost_equal(max(periods), 10)
-    numpy.testing.assert_almost_equal(min(periods), 0.6015575922909607)
-    numpy.testing.assert_equal(len(periods), 1716)
-
-    periods = default_transit_template_generator.period_grid(
-        R_star=1,  # R_sun
-        M_star=1,  # M_sun
-        time_span=20,  # days
-        period_min=0,
-        period_max=999,
-        oversampling_factor=3,
-    )
-    numpy.testing.assert_almost_equal(max(periods), 10)
-    numpy.testing.assert_almost_equal(min(periods), 0.60155759)
-    numpy.testing.assert_equal(len(periods), 1716)
-
-    periods = default_transit_template_generator.period_grid(
-        R_star=0.1,  # R_sun
-        M_star=1,  # M_sun
-        time_span=1000,  # days
-        period_min=0,
-        period_max=999,
-        oversampling_factor=3,
-    )
-    numpy.testing.assert_equal(len(periods), 4308558)
-
-    periods = default_transit_template_generator.period_grid(
-        R_star=1,  # R_sun
-        M_star=1,  # M_sun
-        time_span=20,  # days
-        period_min=0.5,
-        period_max=999,
-        oversampling_factor=3,
-    )
-    numpy.testing.assert_almost_equal(max(periods), 10)
-    numpy.testing.assert_almost_equal(min(periods), 0.500, 3)
-    numpy.testing.assert_equal(len(periods), 1895)
-    print("passed")
+from __future__ import division, print_function
+import numpy
+
+from foldedleastsquares import DefaultTransitTemplateGenerator
+
+import unittest
+
+class TestPeriodGrid(unittest.TestCase):
+    def test(self):
+        print("Starting test: period_grid...", end="")
+        default_transit_template_generator = DefaultTransitTemplateGenerator()
+        periods = default_transit_template_generator.period_grid(R_star=1, M_star=1, time_span=0.1)
+        numpy.testing.assert_almost_equal(max(periods), 2.4999999999999987)
+        numpy.testing.assert_almost_equal(min(periods), 0.6002621413799498)
+        numpy.testing.assert_equal(len(periods), 268)
+
+        periods = default_transit_template_generator.period_grid(R_star=1, M_star=1, time_span=20)
+        numpy.testing.assert_almost_equal(max(periods), 10)
+        numpy.testing.assert_almost_equal(min(periods), 0.6015575922909607)
+        numpy.testing.assert_equal(len(periods), 1716)
+
+        periods = default_transit_template_generator.period_grid(
+            R_star=5,  # R_sun
+            M_star=1,  # M_sun
+            time_span=20,  # days
+            period_min=0,
+            period_max=999,
+            oversampling_factor=3,
+        )
+        numpy.testing.assert_almost_equal(max(periods), 10)
+        numpy.testing.assert_almost_equal(min(periods), 0.6015575922909607)
+        numpy.testing.assert_equal(len(periods), 1716)
+
+        periods = default_transit_template_generator.period_grid(
+            R_star=1,  # R_sun
+            M_star=1,  # M_sun
+            time_span=20,  # days
+            period_min=0,
+            period_max=999,
+            oversampling_factor=3,
+        )
+        numpy.testing.assert_almost_equal(max(periods), 10)
+        numpy.testing.assert_almost_equal(min(periods), 0.60155759)
+        numpy.testing.assert_equal(len(periods), 1716)
+
+        periods = default_transit_template_generator.period_grid(
+            R_star=0.1,  # R_sun
+            M_star=1,  # M_sun
+            time_span=1000,  # days
+            period_min=0,
+            period_max=999,
+            oversampling_factor=3,
+        )
+        numpy.testing.assert_equal(len(periods), 4308558)
+
+        periods = default_transit_template_generator.period_grid(
+            R_star=1,  # R_sun
+            M_star=1,  # M_sun
+            time_span=20,  # days
+            period_min=0.5,
+            period_max=999,
+            oversampling_factor=3,
+        )
+        numpy.testing.assert_almost_equal(max(periods), 10)
+        numpy.testing.assert_almost_equal(min(periods), 0.500, 3)
+        numpy.testing.assert_equal(len(periods), 1895)
+        print("passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_uncertainties.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_uncertainties.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,61 @@
-from __future__ import division, print_function
-import numpy
-import batman
-from foldedleastsquares import transitleastsquares
-
-
-if __name__ == "__main__":
-    print("Starting test: uncertainties...", end="")
-    numpy.random.seed(seed=0)  # reproducibility
-
-    # Create test data
-    start = 48
-    days = 365.25 * 3
-    samples_per_day = 12  # 48
-    samples = int(days * samples_per_day)  # 48
-    t = numpy.linspace(start, start + days, samples)
-
-    # Use batman to create transits
-    ma = batman.TransitParams()
-    ma.t0 = (
-        start + 20
-    )  # time of inferior conjunction; first transit is X days after start
-    ma.per = 365.25  # orbital period
-    ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
-    ma.a = 217  # semi-major axis (in units of stellar radii)
-    ma.inc = 90  # orbital inclination (in degrees)
-    ma.ecc = 0  # eccentricity
-    ma.w = 90  # longitude of periastron (in degrees)
-    ma.u = [0.5]  # limb darkening coefficients
-    ma.limb_dark = "linear"  # limb darkening model
-    m = batman.TransitModel(ma, t)  # initializes model
-    original_flux = m.light_curve(ma)  # calculates light curve
-
-    # Create noise and merge with flux
-    ppm = 5
-    stdev = 10 ** -6 * ppm
-    noise = numpy.random.normal(0, stdev, int(samples))
-    y = original_flux + noise
-
-    # Inject excess noise near the end of the time series.
-    # When searching without uncertainties, the SDE is 4.827
-    # When searching with uncertainties, the SDE is larger, 5.254. Test passed!
-    noise = numpy.random.normal(0, 10 * stdev, 3149)
-    y[10000:] = y[10000:] + noise
-
-    dy = numpy.full(len(y), stdev)
-    dy[10000:] = 10 * stdev
-
-    model = transitleastsquares(t, y, dy)
-    results = model.power(
-        period_min=360,
-        period_max=370,
-        oversampling_factor=3,
-        duration_grid_step=1.05,
-        T0_fit_margin=0.2,
-    )
-    numpy.testing.assert_almost_equal(results.SDE, 5.292594615900944, decimal=5)
-    print("passed")
+from __future__ import division, print_function
+import numpy
+import batman
+from foldedleastsquares import transitleastsquares
+
+
+import unittest
+
+class TestUncertainties(unittest.TestCase):
+    def test(self):
+        print("Starting test: uncertainties...", end="")
+        numpy.random.seed(seed=0)  # reproducibility
+
+        # Create test data
+        start = 48
+        days = 365.25 * 3
+        samples_per_day = 12  # 48
+        samples = int(days * samples_per_day)  # 48
+        t = numpy.linspace(start, start + days, samples)
+
+        # Use batman to create transits
+        ma = batman.TransitParams()
+        ma.t0 = (
+            start + 20
+        )  # time of inferior conjunction; first transit is X days after start
+        ma.per = 365.25  # orbital period
+        ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
+        ma.a = 217  # semi-major axis (in units of stellar radii)
+        ma.inc = 90  # orbital inclination (in degrees)
+        ma.ecc = 0  # eccentricity
+        ma.w = 90  # longitude of periastron (in degrees)
+        ma.u = [0.5]  # limb darkening coefficients
+        ma.limb_dark = "linear"  # limb darkening model
+        m = batman.TransitModel(ma, t)  # initializes model
+        original_flux = m.light_curve(ma)  # calculates light curve
+
+        # Create noise and merge with flux
+        ppm = 5
+        stdev = 10 ** -6 * ppm
+        noise = numpy.random.normal(0, stdev, int(samples))
+        y = original_flux + noise
+
+        # Inject excess noise near the end of the time series.
+        # When searching without uncertainties, the SDE is 4.827
+        # When searching with uncertainties, the SDE is larger, 5.254. Test passed!
+        noise = numpy.random.normal(0, 10 * stdev, 3149)
+        y[10000:] = y[10000:] + noise
+
+        dy = numpy.full(len(y), stdev)
+        dy[10000:] = 10 * stdev
+
+        model = transitleastsquares(t, y, dy)
+        results = model.power(
+            period_min=360,
+            period_max=370,
+            oversampling_factor=3,
+            duration_grid_step=1.05,
+            T0_fit_margin=0.2,
+        )
+        numpy.testing.assert_almost_equal(results.SDE, 5.292594615900944, decimal=5)
+        print("passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_catalog_data.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_catalog_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,75 @@
-from __future__ import division, print_function
-import numpy
-from foldedleastsquares import catalog_info
-import sys
-
-    
-    
-
-if __name__ == "__main__":
-    if sys.version_info >= (3, 0):
-        print("Starting test: catalog_data...")
-        (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
-            EPIC_ID=204341806
-        )
-        numpy.testing.assert_almost_equal((a, b), (1.1605, -0.1704))
-        numpy.testing.assert_almost_equal(mass, numpy.nan)
-        numpy.testing.assert_almost_equal(mass_min, numpy.nan)
-        numpy.testing.assert_almost_equal(mass_max, numpy.nan)
-        numpy.testing.assert_almost_equal(radius, numpy.nan)
-        numpy.testing.assert_almost_equal(radius_min, numpy.nan)
-        numpy.testing.assert_almost_equal(radius_max, numpy.nan)
-
-        (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
-            EPIC_ID=204099713
-        )
-        numpy.testing.assert_almost_equal((a, b), (0.4804, 0.1867))
-        numpy.testing.assert_almost_equal(mass, 1.046)
-        numpy.testing.assert_almost_equal(mass_min, 0.898)
-        numpy.testing.assert_almost_equal(mass_max, 0.642)
-        numpy.testing.assert_almost_equal(radius, 1.261)
-        numpy.testing.assert_almost_equal(radius_min, 1.044)
-        numpy.testing.assert_almost_equal(radius_max, 0.925)
-        print("Test passed: EPIC catalog pull from Vizier using astroquery")
-
-        (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
-            KIC_ID=757076
-        )
-        numpy.testing.assert_almost_equal((a, b), (0.5819, 0.137))
-        numpy.testing.assert_almost_equal(mass, 1.357)
-        numpy.testing.assert_almost_equal(mass_max, 0.204)
-        numpy.testing.assert_almost_equal(mass_min, 0.475)
-        numpy.testing.assert_almost_equal(radius, 3.128)
-        numpy.testing.assert_almost_equal(radius_max, 0.987)
-        numpy.testing.assert_almost_equal(radius_min, 2.304)
-
-        (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
-            KIC_ID=12557548
-        )
-        numpy.testing.assert_almost_equal((a, b), (0.701, 0.0462))
-        numpy.testing.assert_almost_equal(mass, 0.6666, decimal=3)
-        numpy.testing.assert_almost_equal(mass_max, 0.067, decimal=3)
-        numpy.testing.assert_almost_equal(mass_min, 0.055, decimal=3)
-        numpy.testing.assert_almost_equal(radius, 0.660, decimal=3)
-        numpy.testing.assert_almost_equal(radius_max, 0.054, decimal=3)
-        numpy.testing.assert_almost_equal(radius_min, 0.054, decimal=3)
-        print("Test passed: KIC catalog pull from Vizier using astroquery")
-
-        (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
-            TIC_ID=279741377
-        )
-        numpy.testing.assert_equal((a, b), (0.354, 0.2321))
-        numpy.testing.assert_equal(mass, 1.12)
-        numpy.testing.assert_equal(mass_min, 0.148162)
-        numpy.testing.assert_equal(mass_max, 0.148162)
-        numpy.testing.assert_equal(radius, 3.08104)
-        numpy.testing.assert_equal(radius_min, 0.167789)
-        numpy.testing.assert_equal(radius_max, 0.167789)
-        print("Test passed: TESS Input Catalog (TIC) pull from Vizier using astroquery")
-
-        print("All tests passed")
-    else:
-        print('Skipping test, not working on Python 2')
-
+from __future__ import division, print_function
+
+import unittest
+
+import numpy
+from foldedleastsquares import catalog_info
+import sys
+
+
+class TestCatalog(unittest.TestCase):
+    def test(self):
+        if sys.version_info >= (3, 0):
+            print("Starting test: catalog_data...")
+            (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
+                EPIC_ID=204341806
+            )
+            numpy.testing.assert_almost_equal((a, b), (1.1605, -0.1704))
+            numpy.testing.assert_almost_equal(mass, numpy.nan)
+            numpy.testing.assert_almost_equal(mass_min, numpy.nan)
+            numpy.testing.assert_almost_equal(mass_max, numpy.nan)
+            numpy.testing.assert_almost_equal(radius, numpy.nan)
+            numpy.testing.assert_almost_equal(radius_min, numpy.nan)
+            numpy.testing.assert_almost_equal(radius_max, numpy.nan)
+
+            (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
+                EPIC_ID=204099713
+            )
+            numpy.testing.assert_almost_equal((a, b), (0.4804, 0.1867))
+            numpy.testing.assert_almost_equal(mass, 1.046)
+            numpy.testing.assert_almost_equal(mass_min, 0.898)
+            numpy.testing.assert_almost_equal(mass_max, 0.642)
+            numpy.testing.assert_almost_equal(radius, 1.261)
+            numpy.testing.assert_almost_equal(radius_min, 1.044)
+            numpy.testing.assert_almost_equal(radius_max, 0.925)
+            print("Test passed: EPIC catalog pull from Vizier using astroquery")
+
+            (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
+                KIC_ID=757076
+            )
+            numpy.testing.assert_almost_equal((a, b), (0.5819, 0.137))
+            numpy.testing.assert_almost_equal(mass, 1.357)
+            numpy.testing.assert_almost_equal(mass_max, 0.204)
+            numpy.testing.assert_almost_equal(mass_min, 0.475)
+            numpy.testing.assert_almost_equal(radius, 3.128)
+            numpy.testing.assert_almost_equal(radius_max, 0.987)
+            numpy.testing.assert_almost_equal(radius_min, 2.304)
+
+            (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
+                KIC_ID=12557548
+            )
+            numpy.testing.assert_almost_equal((a, b), (0.701, 0.0462))
+            numpy.testing.assert_almost_equal(mass, 0.6666, decimal=3)
+            numpy.testing.assert_almost_equal(mass_max, 0.067, decimal=3)
+            numpy.testing.assert_almost_equal(mass_min, 0.055, decimal=3)
+            numpy.testing.assert_almost_equal(radius, 0.660, decimal=3)
+            numpy.testing.assert_almost_equal(radius_max, 0.054, decimal=3)
+            numpy.testing.assert_almost_equal(radius_min, 0.054, decimal=3)
+            print("Test passed: KIC catalog pull from Vizier using astroquery")
+
+            (a, b), mass, mass_min, mass_max, radius, radius_min, radius_max = catalog_info(
+                TIC_ID=279741377
+            )
+            numpy.testing.assert_equal((a, b), (0.354, 0.2321))
+            numpy.testing.assert_equal(mass, 1.12)
+            numpy.testing.assert_equal(mass_min, 0.148162)
+            numpy.testing.assert_equal(mass_max, 0.148162)
+            numpy.testing.assert_equal(radius, 3.08104)
+            numpy.testing.assert_equal(radius_min, 0.167789)
+            numpy.testing.assert_equal(radius_max, 0.167789)
+            print("Test passed: TESS Input Catalog (TIC) pull from Vizier using astroquery")
+
+            print("All tests passed")
+        else:
+            print('Skipping test, not working on Python 2')
+
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_duration_grid.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_duration_grid.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from __future__ import division, print_function
-import numpy
-from foldedleastsquares.template_generator.default_transit_template_generator import DefaultTransitTemplateGenerator
-
-if __name__ == "__main__":
-    print("Starting test: duration_grid...", end="")
-    default_transit_template_generator = DefaultTransitTemplateGenerator()
-    periods = default_transit_template_generator.period_grid(
-        R_star=1,  # R_sun
-        M_star=1,  # M_sun
-        time_span=20,  # days
-        period_min=0,
-        period_max=999,
-        oversampling_factor=3,
-    )
-    durations = DefaultTransitTemplateGenerator().duration_grid(periods, log_step=1.05, shortest=2)
-    numpy.testing.assert_almost_equal(max(durations), 0.12)
-    numpy.testing.assert_almost_equal(min(durations), 0.004562690993268325)
-    numpy.testing.assert_equal(len(durations), 69)
-    print("passed")
+from __future__ import division, print_function
+
+import unittest
+
+import numpy
+from foldedleastsquares.template_generator.default_transit_template_generator import DefaultTransitTemplateGenerator
+
+class TestDurationGrid(unittest.TestCase):
+    def test(self):
+        print("Starting test: duration_grid...", end="")
+        default_transit_template_generator = DefaultTransitTemplateGenerator()
+        periods = default_transit_template_generator.period_grid(
+            R_star=1,  # R_sun
+            M_star=1,  # M_sun
+            time_span=20,  # days
+            period_min=0,
+            period_max=999,
+            oversampling_factor=3,
+        )
+        durations = DefaultTransitTemplateGenerator().duration_grid(periods, log_step=1.05, shortest=2)
+        numpy.testing.assert_almost_equal(max(durations), 0.12)
+        numpy.testing.assert_almost_equal(min(durations), 0.004562690993268325)
+        numpy.testing.assert_equal(len(durations), 69)
+        print("passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_multi_planet.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_multi_planet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,63 @@
-from __future__ import division, print_function
-import numpy
-import scipy
-import scipy.signal
-from foldedleastsquares import transitleastsquares, transit_mask, cleaned_array
-
-
-def loadfile(filename):
-    data = numpy.genfromtxt(filename, delimiter=",", dtype="f8, f8", names=["t", "y"])
-    return data["t"], data["y"]
-
-
-if __name__ == "__main__":
-    print("Starting test: Multi-planet...", end="")
-    t, y = loadfile("EPIC201367065.csv")
-    trend = scipy.signal.medfilt(y, 25)
-    y_filt = y / trend
-
-    model = transitleastsquares(t, y_filt)
-    results = model.power()
-
-    numpy.testing.assert_almost_equal(max(results.power), 47.585106066175584, decimal=3)
-    numpy.testing.assert_almost_equal(
-        max(results.power_raw), 42.93056655774114, decimal=3
-    )
-    numpy.testing.assert_almost_equal(min(results.power), -0.6531152137309356, decimal=3)
-    numpy.testing.assert_almost_equal(
-        min(results.power_raw), -0.3043720539933344, decimal=3
-    )
-    print("Detrending of power spectrum from power_raw passed")
-
-    # Mask of the first planet
-    intransit = transit_mask(t, results.period, 2 * results.duration, results.T0)
-    y_second_run = y_filt[~intransit]
-    t_second_run = t[~intransit]
-    t_second_run, y_second_run = cleaned_array(t_second_run, y_second_run)
-
-    # Search for second planet
-    model_second_run = transitleastsquares(t_second_run, y_second_run)
-    results_second_run = model_second_run.power()
-    numpy.testing.assert_almost_equal(
-        results_second_run.duration, 0.14596011421893682, decimal=3
-    )
-    numpy.testing.assert_almost_equal(
-        results_second_run.SDE, 35.031824450265, decimal=3
-    )
-    numpy.testing.assert_almost_equal(
-        results_second_run.rp_rs, 0.025852178872027086, decimal=3
-    )
-
-    print("Passed")
+from __future__ import division, print_function
+import numpy
+import scipy
+import scipy.signal
+from foldedleastsquares import transitleastsquares, transit_mask, cleaned_array
+import pkg_resources
+
+import unittest
+
+class TestMultiPlanet(unittest.TestCase):
+    def loadfile(self, filename):
+        filename = TestMultiPlanet.get_path(filename)
+        data = numpy.genfromtxt(filename, delimiter=",", dtype="f8, f8", names=["t", "y"])
+        return data["t"], data["y"]
+
+    @staticmethod
+    def get_path(path):
+        """
+        Gets right path for tests environment
+        :param path:
+        :return: the real path of the test resource
+        """
+        return pkg_resources.resource_filename(__name__, path)
+
+    def test(self):
+        print("Starting test: Multi-planet...", end="")
+        t, y = self.loadfile("EPIC201367065.csv")
+        trend = scipy.signal.medfilt(y, 25)
+        y_filt = y / trend
+
+        model = transitleastsquares(t, y_filt)
+        results = model.power()
+
+        numpy.testing.assert_almost_equal(max(results.power), 47.585106066175584, decimal=3)
+        numpy.testing.assert_almost_equal(
+            max(results.power_raw), 42.93056655774114, decimal=3
+        )
+        numpy.testing.assert_almost_equal(min(results.power), -0.6531152137309356, decimal=3)
+        numpy.testing.assert_almost_equal(
+            min(results.power_raw), -0.3043720539933344, decimal=3
+        )
+        print("Detrending of power spectrum from power_raw passed")
+
+        # Mask of the first planet
+        intransit = transit_mask(t, results.period, 2 * results.duration, results.T0)
+        y_second_run = y_filt[~intransit]
+        t_second_run = t[~intransit]
+        t_second_run, y_second_run = cleaned_array(t_second_run, y_second_run)
+
+        # Search for second planet
+        model_second_run = transitleastsquares(t_second_run, y_second_run)
+        results_second_run = model_second_run.power()
+        numpy.testing.assert_almost_equal(
+            results_second_run.duration, 0.14596011421893682, decimal=3
+        )
+        numpy.testing.assert_almost_equal(
+            results_second_run.SDE, 35.031824450265, decimal=3
+        )
+        numpy.testing.assert_almost_equal(
+            results_second_run.rp_rs, 0.025852178872027086, decimal=3
+        )
+
+        print("Passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_shapes.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_shapes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,92 @@
 from __future__ import division, print_function
+
+import unittest
+
 import numpy
-import scipy
 import scipy.signal
 from foldedleastsquares import transitleastsquares
 from foldedleastsquares.template_generator.default_transit_template_generator import DefaultTransitTemplateGenerator
+import pkg_resources
 
 
-def loadfile(filename):
-    data = numpy.genfromtxt(filename, delimiter=",", dtype="f8, f8", names=["t", "y"])
-    return data["t"], data["y"]
-
 class TestTransitTemplateGenerator(DefaultTransitTemplateGenerator):
     def __init__(self):
         super().__init__()
 
-if __name__ == "__main__":
-    print("Starting test: transit shapes...", end="")
-
-    # Testing transit shapes
-    t, y = loadfile("EPIC206154641.csv")
-    trend = scipy.signal.medfilt(y, 25)
-    y_filt = y / trend
-
-    # box
-    model_box = transitleastsquares(t, y_filt)
-    results_box = model_box.power(transit_template="box", period_grid=numpy.arange(1, 5, 0.01))
-    numpy.testing.assert_equal(len(model_box.period_grid), 400)
-
-    results_box = model_box.power(transit_template="box")
-    numpy.testing.assert_almost_equal(
-        results_box.duration, 0.06207881501022775, decimal=5)
-    numpy.testing.assert_almost_equal(results_box.rp_rs, 0.08836981203437415, decimal=5)
-    print("Test passed: Box-shaped")
-
-    # grazing
-    model_grazing = transitleastsquares(t, y_filt)
-    results_grazing = model_grazing.power(transit_template="grazing")
-
-    numpy.testing.assert_almost_equal(
-        results_grazing.duration, 0.09079026695245815, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        min(results_grazing.chi2red), 0.06759475703796078, decimal=5)
-    print("Test passed: Grazing-shaped")
-
-    # comet
-    model_comet = transitleastsquares(t, y_filt)
-    results_comet = model_comet.power(transit_template="tailed")
-    numpy.testing.assert_almost_equal(
-        results_comet.duration, 0.23745146741412124, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        min(results_comet.chi2red), 0.0980794344892094, decimal=5)
-    print("Test passed: Comet-shaped")
-
-    model_custom = transitleastsquares(t, y_filt)
-    try:
-        results_custom = model_custom.power(transit_template="custom",
-                                            transit_template_generator="wrongTransitTemplateGenerator")
-        assert False
-    except ValueError as e:
-        if e.args[0] == "The custom transit_template_generator does not implement TransitTemplateGenerator.":
-            print("Test passed: Wrong custom transit template generator.")
-        else:
+class TestShapes(unittest.TestCase):
+    def loadfile(self, filename):
+        filename = TestShapes.get_path(filename)
+        data = numpy.genfromtxt(filename, delimiter=",", dtype="f8, f8", names=["t", "y"])
+        return data["t"], data["y"]
+    @staticmethod
+    def get_path(path):
+        """
+        Gets right path for tests environment
+        :param path:
+        :return: the real path of the test resource
+        """
+        return pkg_resources.resource_filename(__name__, path)
+
+    def test(self):
+        print("Starting test: transit shapes...", end="")
+
+        # Testing transit shapes
+        t, y = self.loadfile("EPIC206154641.csv")
+        trend = scipy.signal.medfilt(y, 25)
+        y_filt = y / trend
+
+        # box
+        model_box = transitleastsquares(t, y_filt)
+        results_box = model_box.power(transit_template="box", period_grid=numpy.arange(1, 5, 0.01))
+        numpy.testing.assert_equal(len(model_box.period_grid), 400)
+
+        results_box = model_box.power(transit_template="box")
+        numpy.testing.assert_almost_equal(
+            results_box.duration, 0.06207881501022775, decimal=5)
+        numpy.testing.assert_almost_equal(results_box.rp_rs, 0.08836981203437415, decimal=5)
+        print("Test passed: Box-shaped")
+
+        # grazing
+        model_grazing = transitleastsquares(t, y_filt)
+        results_grazing = model_grazing.power(transit_template="grazing")
+
+        numpy.testing.assert_almost_equal(
+            results_grazing.duration, 0.09079026695245815, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            min(results_grazing.chi2red), 0.06759475703796078, decimal=5)
+        print("Test passed: Grazing-shaped")
+
+        # comet
+        model_comet = transitleastsquares(t, y_filt)
+        results_comet = model_comet.power(transit_template="tailed")
+        numpy.testing.assert_almost_equal(
+            results_comet.duration, 0.23745146741412124, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            min(results_comet.chi2red), 0.0980794344892094, decimal=5)
+        print("Test passed: Comet-shaped")
+
+        model_custom = transitleastsquares(t, y_filt)
+        try:
+            results_custom = model_custom.power(transit_template="custom",
+                                                transit_template_generator="wrongTransitTemplateGenerator")
             assert False
+        except ValueError as e:
+            if e.args[0] == "The custom transit_template_generator does not implement TransitTemplateGenerator.":
+                print("Test passed: Wrong custom transit template generator.")
+            else:
+                assert False
 
-    # custom
-    model_custom = transitleastsquares(t, y_filt)
-    results_custom = model_custom.power(transit_template="custom",
-                                        transit_template_generator=TestTransitTemplateGenerator())
-    numpy.testing.assert_almost_equal(
-        results_custom.duration, 0.06828669651125058, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        min(results_custom.chi2red), 0.09977336183179186, decimal=5)
-    print("Test passed: Custom-shaped")
+        # custom
+        model_custom = transitleastsquares(t, y_filt)
+        results_custom = model_custom.power(transit_template="custom",
+                                            transit_template_generator=TestTransitTemplateGenerator())
+        numpy.testing.assert_almost_equal(
+            results_custom.duration, 0.06828669651125058, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            min(results_custom.chi2red), 0.09977336183179186, decimal=5)
+        print("Test passed: Custom-shaped")
 
-    print("All tests passed")
+        print("All tests passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_stats_gap.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_stats_gap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,136 @@
-from __future__ import division, print_function
-import numpy
-import batman
-from foldedleastsquares import transitleastsquares
-
-
-# Test case for statistics when data contains gap during a transit
-
-if __name__ == "__main__":
-    print("Starting test: Gap in test statistic...", end="")
-    numpy.random.seed(seed=0)  # reproducibility
-    # Create test data
-    start = 48
-    days = 365.25 * 3
-    samples_per_day = 12  # 48
-    samples = int(days * samples_per_day)  # 48
-    t = numpy.linspace(start, start + days, samples)
-
-    # Use batman to create transits
-    ma = batman.TransitParams()
-    ma.t0 = start + 20
-    ma.per = 365.25  # orbital period
-    ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
-    ma.a = 217  # semi-major axis (in units of stellar radii)
-    ma.inc = 90  # orbital inclination (in degrees)
-    ma.ecc = 0  # eccentricity
-    ma.w = 90  # longitude of periastron (in degrees)
-    ma.u = [0.5]  # limb darkening coefficients
-    ma.limb_dark = "linear"  # limb darkening model
-    m = batman.TransitModel(ma, t)  # initializes model
-    original_flux = m.light_curve(ma)  # calculates light curve
-
-    # Create noise and merge with flux
-    ppm = 5
-    stdev = 10 ** -6 * ppm
-    noise = numpy.random.normal(0, stdev, int(samples))
-    y = original_flux + noise
-    y[1] = numpy.nan
-
-    # print(len(y))
-    y[200:500] = numpy.nan
-    t[200:500] = numpy.nan
-    # import matplotlib.pyplot as plt
-    # plt.plot(t, y)
-    # plt.show()
-
-    model = transitleastsquares(t, y)
-    results = model.power(
-        period_min=360,
-        period_max=370,
-        transit_depth_min=10 * 10 ** -6,
-        oversampling_factor=2,
-        duration_grid_step=1.1,
-        T0_fit_margin=1.2,
-    )
-
-    numpy.testing.assert_almost_equal(
-        results.period_uncertainty, 0.3153203546531813, decimal=5
-    )
-    numpy.testing.assert_equal(results.per_transit_count, [0, 4, 4])
-    numpy.testing.assert_equal(len(results.transit_times), 3)
-    numpy.testing.assert_almost_equal(results.period, 365.22218620040417, decimal=5)
-    numpy.testing.assert_almost_equal(
-        results.transit_times,
-        [68.08637, 433.30855, 798.53074],
-        decimal=5,
-    )
-
-    numpy.testing.assert_almost_equal(results.depth, 0.9998972750356973, decimal=5)
-    numpy.testing.assert_almost_equal(results.duration, 0.3695717615478269, decimal=5)
-    numpy.testing.assert_almost_equal(results.SDE, 4.243572802600693, decimal=3)
-    numpy.testing.assert_almost_equal(
-        results.odd_even_mismatch, 0.4359025761888081, decimal=3
-    )
-    numpy.testing.assert_almost_equal(results.rp_rs, 0.009114758081257387, decimal=3)
-
-    # Full light curve model
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.model_lightcurve_time), 38275494.19583159, decimal=3
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.model_lightcurve_model), 64233.9941755991, decimal=3
-    )
-
-    transit_times_expected = [68.086, 433.309, 798.531]
-    numpy.testing.assert_almost_equal(
-        results.transit_times, transit_times_expected, decimal=3
-    )
-    numpy.testing.assert_almost_equal(results.duration, 0.3695717615478269, decimal=3)
-
-    numpy.testing.assert_almost_equal(
-        max(results.model_folded_phase), 1.0000380285975052, decimal=3
-    )
-    numpy.testing.assert_almost_equal(
-        min(results.model_folded_phase), 3.8028597505324e-05, decimal=3
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.mean(results.model_folded_phase), 0.5000380285975052, decimal=3
-    )
-
-    numpy.testing.assert_almost_equal(
-        results.depth_mean_even, (0.999915, 6.785539e-06), decimal=3
-    )
-    numpy.testing.assert_almost_equal(
-        results.depth_mean_odd, (0.999920, 1.209993e-05), decimal=3
-    )
-    numpy.testing.assert_almost_equal(
-        results.depth_mean, (0.999917, 6.086923e-06), decimal=3
-    )
-
-    numpy.testing.assert_almost_equal(
-        results.transit_depths, [numpy.nan, 0.99991, 0.9999], decimal=3
-    )
-
-    numpy.testing.assert_almost_equal(
-        results.transit_depths_uncertainties,
-        [numpy.nan, 2.92371e-06, 4.48803e-06],
-        decimal=3,
-    )
-    numpy.testing.assert_almost_equal(
-        results.odd_even_mismatch, 0.4359025761888081, decimal=3
-    )
-    numpy.testing.assert_almost_equal(results.transit_count, 3, decimal=3)
-    numpy.testing.assert_almost_equal(results.distinct_transit_count, 2, decimal=3)
-    numpy.testing.assert_almost_equal(results.empty_transit_count, 1, decimal=3)
-    numpy.testing.assert_almost_equal(
-        results.snr_per_transit, [0., 32.666, 33.999], decimal=3
-    )
-    numpy.testing.assert_almost_equal(results.snr, 47.138942974480806, decimal=3)
-    numpy.testing.assert_almost_equal(
-        results.snr_pink_per_transit, [0., 47.049, 48.969], decimal=3
-    )
-    print("passed")
+from __future__ import division, print_function
+import numpy
+import batman
+from foldedleastsquares import transitleastsquares
+
+
+# Test case for statistics when data contains gap during a transit
+
+import unittest
+
+class TestStatsGap(unittest.TestCase):
+    def test(self):
+        print("Starting test: Gap in test statistic...", end="")
+        numpy.random.seed(seed=0)  # reproducibility
+        # Create test data
+        start = 48
+        days = 365.25 * 3
+        samples_per_day = 12  # 48
+        samples = int(days * samples_per_day)  # 48
+        t = numpy.linspace(start, start + days, samples)
+
+        # Use batman to create transits
+        ma = batman.TransitParams()
+        ma.t0 = start + 20
+        ma.per = 365.25  # orbital period
+        ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
+        ma.a = 217  # semi-major axis (in units of stellar radii)
+        ma.inc = 90  # orbital inclination (in degrees)
+        ma.ecc = 0  # eccentricity
+        ma.w = 90  # longitude of periastron (in degrees)
+        ma.u = [0.5]  # limb darkening coefficients
+        ma.limb_dark = "linear"  # limb darkening model
+        m = batman.TransitModel(ma, t)  # initializes model
+        original_flux = m.light_curve(ma)  # calculates light curve
+
+        # Create noise and merge with flux
+        ppm = 5
+        stdev = 10 ** -6 * ppm
+        noise = numpy.random.normal(0, stdev, int(samples))
+        y = original_flux + noise
+        y[1] = numpy.nan
+
+        # print(len(y))
+        y[200:500] = numpy.nan
+        t[200:500] = numpy.nan
+        # import matplotlib.pyplot as plt
+        # plt.plot(t, y)
+        # plt.show()
+
+        model = transitleastsquares(t, y)
+        results = model.power(
+            period_min=360,
+            period_max=370,
+            transit_depth_min=10 * 10 ** -6,
+            oversampling_factor=2,
+            duration_grid_step=1.1,
+            T0_fit_margin=1.2,
+        )
+
+        numpy.testing.assert_almost_equal(
+            results.period_uncertainty, 0.3153203546531813, decimal=5
+        )
+        numpy.testing.assert_equal(results.per_transit_count, [0, 4, 4])
+        numpy.testing.assert_equal(len(results.transit_times), 3)
+        numpy.testing.assert_almost_equal(results.period, 365.22218620040417, decimal=5)
+        numpy.testing.assert_almost_equal(
+            results.transit_times,
+            [68.08637, 433.30855, 798.53074],
+            decimal=5,
+        )
+
+        numpy.testing.assert_almost_equal(results.depth, 0.9998972750356973, decimal=5)
+        numpy.testing.assert_almost_equal(results.duration, 0.3695717615478269, decimal=5)
+        numpy.testing.assert_almost_equal(results.SDE, 4.243572802600693, decimal=3)
+        numpy.testing.assert_almost_equal(
+            results.odd_even_mismatch, 0.4359025761888081, decimal=3
+        )
+        numpy.testing.assert_almost_equal(results.rp_rs, 0.009114758081257387, decimal=3)
+
+        # Full light curve model
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.model_lightcurve_time), 38275494.19583159, decimal=3
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.model_lightcurve_model), 64233.9941755991, decimal=3
+        )
+
+        transit_times_expected = [68.086, 433.309, 798.531]
+        numpy.testing.assert_almost_equal(
+            results.transit_times, transit_times_expected, decimal=3
+        )
+        numpy.testing.assert_almost_equal(results.duration, 0.3695717615478269, decimal=3)
+
+        numpy.testing.assert_almost_equal(
+            max(results.model_folded_phase), 1.0000380285975052, decimal=3
+        )
+        numpy.testing.assert_almost_equal(
+            min(results.model_folded_phase), 3.8028597505324e-05, decimal=3
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.mean(results.model_folded_phase), 0.5000380285975052, decimal=3
+        )
+
+        numpy.testing.assert_almost_equal(
+            results.depth_mean_even, (0.999915, 6.785539e-06), decimal=3
+        )
+        numpy.testing.assert_almost_equal(
+            results.depth_mean_odd, (0.999920, 1.209993e-05), decimal=3
+        )
+        numpy.testing.assert_almost_equal(
+            results.depth_mean, (0.999917, 6.086923e-06), decimal=3
+        )
+
+        numpy.testing.assert_almost_equal(
+            results.transit_depths, [numpy.nan, 0.99991, 0.9999], decimal=3
+        )
+
+        numpy.testing.assert_almost_equal(
+            results.transit_depths_uncertainties,
+            [numpy.nan, 2.92371e-06, 4.48803e-06],
+            decimal=3,
+        )
+        numpy.testing.assert_almost_equal(
+            results.odd_even_mismatch, 0.4359025761888081, decimal=3
+        )
+        numpy.testing.assert_almost_equal(results.transit_count, 3, decimal=3)
+        numpy.testing.assert_almost_equal(results.distinct_transit_count, 2, decimal=3)
+        numpy.testing.assert_almost_equal(results.empty_transit_count, 1, decimal=3)
+        numpy.testing.assert_almost_equal(
+            results.snr_per_transit, [0., 32.666, 33.999], decimal=3
+        )
+        numpy.testing.assert_almost_equal(results.snr, 47.138942974480806, decimal=3)
+        numpy.testing.assert_almost_equal(
+            results.snr_pink_per_transit, [0., 47.049, 48.969], decimal=3
+        )
+        print("passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_cleaned_array.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_cleaned_array.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from __future__ import division, print_function
-import numpy
-from foldedleastsquares import cleaned_array
-
-if __name__ == "__main__":
-    print("Starting test: cleaned_array...", end="")
-
-    dirty_array = numpy.ones(10, dtype=object)
-    time_array = numpy.linspace(1, 10, 10)
-    dy_array = numpy.ones(10, dtype=object)
-    dirty_array[1] = None
-    dirty_array[2] = numpy.inf
-    dirty_array[3] = -numpy.inf
-    dirty_array[4] = numpy.nan
-    dirty_array[5] = -99
-    time_array[8] = numpy.nan
-    dy_array[9] = numpy.inf
-
-    t, y, dy = cleaned_array(time_array, dirty_array, dy_array)
-    numpy.testing.assert_equal(t, [1, 7, 8])
-    numpy.testing.assert_equal(y, [1, 1, 1])
-    numpy.testing.assert_equal(dy, [1, 1, 1])
-    print("passed")
+from __future__ import division, print_function
+
+import unittest
+
+import numpy
+from foldedleastsquares import cleaned_array
+
+class TestCleanedArray(unittest.TestCase):
+    def test(self):
+        print("Starting test: cleaned_array...", end="")
+
+        dirty_array = numpy.ones(10, dtype=object)
+        time_array = numpy.linspace(1, 10, 10)
+        dy_array = numpy.ones(10, dtype=object)
+        dirty_array[1] = None
+        dirty_array[2] = numpy.inf
+        dirty_array[3] = -numpy.inf
+        dirty_array[4] = numpy.nan
+        dirty_array[5] = -99
+        time_array[8] = numpy.nan
+        dy_array[9] = numpy.inf
+
+        t, y, dy = cleaned_array(time_array, dirty_array, dy_array)
+        numpy.testing.assert_equal(t, [1, 7, 8])
+        numpy.testing.assert_equal(y, [1, 1, 1])
+        numpy.testing.assert_equal(dy, [1, 1, 1])
+        print("passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tests/test_synthetic.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tests/test_synthetic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,192 +1,195 @@
-from __future__ import division, print_function
-import os
-import numpy
-import batman
-from foldedleastsquares import transitleastsquares
-
-
-if __name__ == "__main__":
-    print("Starting test: synthetic...", end="")
-    
-    numpy.random.seed(seed=0)  # reproducibility
-    # Create test data
-    start = 48
-    days = 365.25 * 3
-    samples_per_day = 12  # 48
-    samples = int(days * samples_per_day)  # 48
-    t = numpy.linspace(start, start + days, samples)
-
-    # Use batman to create transits
-    ma = batman.TransitParams()
-    ma.t0 = (
-        start + 20
-    )  # time of inferior conjunction; first transit is X days after start
-    ma.per = 365.25  # orbital period
-    ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
-    ma.a = 217  # semi-major axis (in units of stellar radii)
-    ma.inc = 90  # orbital inclination (in degrees)
-    ma.ecc = 0  # eccentricity
-    ma.w = 90  # longitude of periastron (in degrees)
-    ma.u = [0.5]  # limb darkening coefficients
-    ma.limb_dark = "linear"  # limb darkening model
-    m = batman.TransitModel(ma, t)  # initializes model
-    original_flux = m.light_curve(ma)  # calculates light curve
-
-    # Create noise and merge with flux
-    ppm = 5
-    stdev = 10 ** -6 * ppm
-    noise = numpy.random.normal(0, stdev, int(samples))
-    y = original_flux + noise
-    y[1] = numpy.nan
-    model = transitleastsquares(t, y)
-    results = model.power(
-        period_min=360,
-        period_max=370,
-        transit_depth_min=10 * 10 ** -6,
-        oversampling_factor=5,
-        duration_grid_step=1.02,
-    )
-
-    numpy.testing.assert_almost_equal(results.chi2_min, 8831.654060613922, decimal=5)
-    numpy.testing.assert_almost_equal(
-        results.chi2red_min, 0.6719152511118321, decimal=5
-    )
-
-    numpy.testing.assert_almost_equal(
-        results.period_uncertainty, 0.216212529678387, decimal=5
-    )
-    numpy.testing.assert_equal(results.per_transit_count[0], 7)
-    numpy.testing.assert_equal(len(results.transit_times), 3)
-    numpy.testing.assert_almost_equal(results.period, 365.2582192473641, decimal=5)
-    numpy.testing.assert_almost_equal(
-        results.transit_times[0], 68.00349264912924, decimal=5
-    )
-    """
-    numpy.testing.assert_almost_equal(results.depth, 0.999897160189092, decimal=5)
-    numpy.testing.assert_almost_equal(results.duration, 0.5908251624976649, decimal=5)
-    numpy.testing.assert_almost_equal(
-        min(results.chi2red), 0.6719167401148216, decimal=5
-    )
-    numpy.testing.assert_almost_equal(results.SDE, 5.691301613227594, decimal=5)
-    numpy.testing.assert_almost_equal(
-        results.odd_even_mismatch, 0.29083256866622437, decimal=5
-    )
-    numpy.testing.assert_almost_equal(results.rp_rs, 0.009119851811944274, decimal=5)
-
-    # Full light curve model
-    numpy.testing.assert_almost_equal(
-        max(results.model_lightcurve_time), 1143.7472155961277, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        min(results.model_lightcurve_time), 48.0059010663453, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.mean(results.model_lightcurve_time), 595.877471821318, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.model_lightcurve_time), 39166430.34534341, decimal=5
-    )
-
-    numpy.testing.assert_almost_equal(max(results.model_lightcurve_model), 1, decimal=5)
-    numpy.testing.assert_almost_equal(
-        min(results.model_lightcurve_model), 0.999897160189092, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.mean(results.model_lightcurve_model), 0.9999998641488729, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.model_lightcurve_model), 65728.99107064126, decimal=5
-    )
-
-    transit_times_expected = [68.003492, 433.261711, 798.519931]
-    numpy.testing.assert_almost_equal(
-        results.transit_times, transit_times_expected, decimal=5
-    )
-    numpy.testing.assert_almost_equal(results.duration, 0.590825, decimal=5)
-
-    numpy.testing.assert_almost_equal(
-        max(results.model_folded_phase), 1.0000380285975052, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        min(results.model_folded_phase), 3.8028597505324e-05, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.mean(results.model_folded_phase), 0.5000380285975052, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.model_folded_phase), 6574.499999999999, decimal=5
-    )
-
-    numpy.testing.assert_almost_equal(max(results.model_folded_model), 1, decimal=5)
-    numpy.testing.assert_almost_equal(
-        min(results.model_folded_model), 0.999897160189092, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.mean(results.model_folded_model), 0.9999998679702978, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.model_folded_model), 13147.998264073476, decimal=5
-    )
-
-    numpy.testing.assert_almost_equal(
-        max(results.folded_phase), 0.9999608485845858, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        min(results.folded_phase), 1.44015016259047e-05, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.mean(results.folded_phase), 0.500000089528271, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.folded_phase), 6574.001177117707, decimal=5
-    )
-
-    numpy.testing.assert_almost_equal(
-        max(results.folded_y), 1.000019008301075, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        min(results.folded_y), 0.9998860842491378, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.mean(results.folded_y), 0.9999997920032417, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        numpy.sum(results.folded_y), 13147.997265, decimal=5
-    )
-
-    numpy.testing.assert_almost_equal(
-        results.depth_mean_even, (0.999915, 6.785539e-06), decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        results.depth_mean_odd, (0.999920, 1.209993e-05), decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        results.depth_mean, (0.999917, 6.086923e-06), decimal=5
-    )
-
-    numpy.testing.assert_almost_equal(
-        results.transit_depths, [0.99991085, 0.99992095, 0.99992007], decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        results.transit_depths_uncertainties,
-        [4.19177855e-06, 1.20999330e-05, 1.26699399e-05],
-        decimal=5,
-    )
-    numpy.testing.assert_almost_equal(
-        results.odd_even_mismatch, 0.29083256866622437, decimal=5
-    )
-    numpy.testing.assert_almost_equal(
-        results.per_transit_count, [7.0, 7.0, 7.0], decimal=5
-    )
-    numpy.testing.assert_almost_equal(results.transit_count, 3, decimal=5)
-    numpy.testing.assert_almost_equal(results.distinct_transit_count, 3, decimal=5)
-    numpy.testing.assert_almost_equal(results.empty_transit_count, 0, decimal=5)
-    numpy.testing.assert_almost_equal(
-        results.snr_per_transit, [38.92162, 34.51048, 34.89514], decimal=5
-    )
-    numpy.testing.assert_almost_equal(results.snr, 62.542764907612785, decimal=5)
-    numpy.testing.assert_almost_equal(
-        results.snr_pink_per_transit, [52.24377, 46.32278, 46.8391], decimal=5
-    )
-    """
-    print("passed")
+from __future__ import division, print_function
+import os
+import numpy
+import batman
+from foldedleastsquares import transitleastsquares
+
+
+import unittest
+
+class TestSynthetic(unittest.TestCase):
+    def test(self):
+        print("Starting test: synthetic...", end="")
+
+        numpy.random.seed(seed=0)  # reproducibility
+        # Create test data
+        start = 48
+        days = 365.25 * 3
+        samples_per_day = 12  # 48
+        samples = int(days * samples_per_day)  # 48
+        t = numpy.linspace(start, start + days, samples)
+
+        # Use batman to create transits
+        ma = batman.TransitParams()
+        ma.t0 = (
+            start + 20
+        )  # time of inferior conjunction; first transit is X days after start
+        ma.per = 365.25  # orbital period
+        ma.rp = 6371 / 696342  # 6371 planet radius (in units of stellar radii)
+        ma.a = 217  # semi-major axis (in units of stellar radii)
+        ma.inc = 90  # orbital inclination (in degrees)
+        ma.ecc = 0  # eccentricity
+        ma.w = 90  # longitude of periastron (in degrees)
+        ma.u = [0.5]  # limb darkening coefficients
+        ma.limb_dark = "linear"  # limb darkening model
+        m = batman.TransitModel(ma, t)  # initializes model
+        original_flux = m.light_curve(ma)  # calculates light curve
+
+        # Create noise and merge with flux
+        ppm = 5
+        stdev = 10 ** -6 * ppm
+        noise = numpy.random.normal(0, stdev, int(samples))
+        y = original_flux + noise
+        y[1] = numpy.nan
+        model = transitleastsquares(t, y)
+        results = model.power(
+            period_min=360,
+            period_max=370,
+            transit_depth_min=10 * 10 ** -6,
+            oversampling_factor=5,
+            duration_grid_step=1.02,
+        )
+
+        numpy.testing.assert_almost_equal(results.chi2_min, 8831.654060613922, decimal=5)
+        numpy.testing.assert_almost_equal(
+            results.chi2red_min, 0.6719152511118321, decimal=5
+        )
+
+        numpy.testing.assert_almost_equal(
+            results.period_uncertainty, 0.216212529678387, decimal=5
+        )
+        numpy.testing.assert_equal(results.per_transit_count[0], 7)
+        numpy.testing.assert_equal(len(results.transit_times), 3)
+        numpy.testing.assert_almost_equal(results.period, 365.2582192473641, decimal=5)
+        numpy.testing.assert_almost_equal(
+            results.transit_times[0], 68.00349264912924, decimal=5
+        )
+        """
+        numpy.testing.assert_almost_equal(results.depth, 0.999897160189092, decimal=5)
+        numpy.testing.assert_almost_equal(results.duration, 0.5908251624976649, decimal=5)
+        numpy.testing.assert_almost_equal(
+            min(results.chi2red), 0.6719167401148216, decimal=5
+        )
+        numpy.testing.assert_almost_equal(results.SDE, 5.691301613227594, decimal=5)
+        numpy.testing.assert_almost_equal(
+            results.odd_even_mismatch, 0.29083256866622437, decimal=5
+        )
+        numpy.testing.assert_almost_equal(results.rp_rs, 0.009119851811944274, decimal=5)
+    
+        # Full light curve model
+        numpy.testing.assert_almost_equal(
+            max(results.model_lightcurve_time), 1143.7472155961277, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            min(results.model_lightcurve_time), 48.0059010663453, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.mean(results.model_lightcurve_time), 595.877471821318, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.model_lightcurve_time), 39166430.34534341, decimal=5
+        )
+    
+        numpy.testing.assert_almost_equal(max(results.model_lightcurve_model), 1, decimal=5)
+        numpy.testing.assert_almost_equal(
+            min(results.model_lightcurve_model), 0.999897160189092, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.mean(results.model_lightcurve_model), 0.9999998641488729, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.model_lightcurve_model), 65728.99107064126, decimal=5
+        )
+    
+        transit_times_expected = [68.003492, 433.261711, 798.519931]
+        numpy.testing.assert_almost_equal(
+            results.transit_times, transit_times_expected, decimal=5
+        )
+        numpy.testing.assert_almost_equal(results.duration, 0.590825, decimal=5)
+    
+        numpy.testing.assert_almost_equal(
+            max(results.model_folded_phase), 1.0000380285975052, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            min(results.model_folded_phase), 3.8028597505324e-05, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.mean(results.model_folded_phase), 0.5000380285975052, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.model_folded_phase), 6574.499999999999, decimal=5
+        )
+    
+        numpy.testing.assert_almost_equal(max(results.model_folded_model), 1, decimal=5)
+        numpy.testing.assert_almost_equal(
+            min(results.model_folded_model), 0.999897160189092, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.mean(results.model_folded_model), 0.9999998679702978, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.model_folded_model), 13147.998264073476, decimal=5
+        )
+    
+        numpy.testing.assert_almost_equal(
+            max(results.folded_phase), 0.9999608485845858, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            min(results.folded_phase), 1.44015016259047e-05, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.mean(results.folded_phase), 0.500000089528271, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.folded_phase), 6574.001177117707, decimal=5
+        )
+    
+        numpy.testing.assert_almost_equal(
+            max(results.folded_y), 1.000019008301075, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            min(results.folded_y), 0.9998860842491378, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.mean(results.folded_y), 0.9999997920032417, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            numpy.sum(results.folded_y), 13147.997265, decimal=5
+        )
+    
+        numpy.testing.assert_almost_equal(
+            results.depth_mean_even, (0.999915, 6.785539e-06), decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            results.depth_mean_odd, (0.999920, 1.209993e-05), decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            results.depth_mean, (0.999917, 6.086923e-06), decimal=5
+        )
+    
+        numpy.testing.assert_almost_equal(
+            results.transit_depths, [0.99991085, 0.99992095, 0.99992007], decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            results.transit_depths_uncertainties,
+            [4.19177855e-06, 1.20999330e-05, 1.26699399e-05],
+            decimal=5,
+        )
+        numpy.testing.assert_almost_equal(
+            results.odd_even_mismatch, 0.29083256866622437, decimal=5
+        )
+        numpy.testing.assert_almost_equal(
+            results.per_transit_count, [7.0, 7.0, 7.0], decimal=5
+        )
+        numpy.testing.assert_almost_equal(results.transit_count, 3, decimal=5)
+        numpy.testing.assert_almost_equal(results.distinct_transit_count, 3, decimal=5)
+        numpy.testing.assert_almost_equal(results.empty_transit_count, 0, decimal=5)
+        numpy.testing.assert_almost_equal(
+            results.snr_per_transit, [38.92162, 34.51048, 34.89514], decimal=5
+        )
+        numpy.testing.assert_almost_equal(results.snr, 62.542764907612785, decimal=5)
+        numpy.testing.assert_almost_equal(
+            results.snr_pink_per_transit, [52.24377, 46.32278, 46.8391], decimal=5
+        )
+        """
+        print("passed")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/results.py` & `foldedleastsquares-1.0.41/foldedleastsquares/results.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/main.py` & `foldedleastsquares-1.0.41/foldedleastsquares/main.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/stats.py` & `foldedleastsquares-1.0.41/foldedleastsquares/stats.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,416 +1,416 @@
-from __future__ import division, print_function
-import numpy
-from os import path
-from . import tls_constants
-from .helpers import running_median, transit_mask
-
-
-def FAP(SDE):
-    """Returns FAP (False Alarm Probability) for a given SDE"""
-    data = numpy.genfromtxt(
-        path.join(tls_constants.resources_dir, "fap.csv"),
-        dtype="f8, f8",
-        delimiter=",",
-        names=["FAP", "SDE"],
-    )
-    return data["FAP"][numpy.argmax(data["SDE"] > SDE)]
-
-
-def rp_rs_from_depth(depth, law, params):
-    """Takes the maximum transit depth, limb-darkening law and parameters
-    Returns R_P / R_S (ratio of planetary to stellar radius)
-    Source: Heller 2019, https://arxiv.org/abs/1901.01730"""
-
-    # Validations:
-    # - LD law must exist
-    # - All parameters must be floats or ints
-    # - All parameters must be given in the correct quanitity for the law
-
-    if len(params) == 1:
-        params = float(params[0])
-
-    if not isinstance(params, (float, int)) and not all(
-        isinstance(x, (float, int)) for x in params
-    ):
-        raise ValueError("All limb-darkening parameters must be numbers")
-
-    laws = "linear, quadratic, squareroot, logarithmic, nonlinear"
-    if law not in laws:
-        raise ValueError("Please provide a supported limb-darkening law:", laws)
-
-    if law == "linear" and not isinstance(params, float):
-        raise ValueError("Please provide exactly one parameter")
-
-    if law in "quadratic, logarithmic, squareroot" and len(params) != 2:
-        raise ValueError("Please provide exactly two limb-darkening parameters")
-
-    if law == "nonlinear" and len(params) != 4:
-        raise ValueError("Please provide exactly four limb-darkening parameters")
-
-    # Actual calculations of the return value
-    if law == "linear":
-        return (depth * (1 - params / 3)) ** (1 / 2)
-
-    if law == "quadratic":
-        return (depth * (1 - params[0] / 3 - params[1] / 6)) ** (1 / 2)
-
-    if law == "squareroot":
-        return (depth * (1 - params[0] / 3 - params[1] / 5)) ** (1 / 2)
-
-    if law == "logarithmic":
-        return (depth * (1 + 2 * params[1] / 9 - params[0] / 3)) ** (1 / 2)
-
-    if law == "nonlinear":
-        return (
-            depth
-            * (1 - params[0] / 5 - params[1] / 3 - 3 * params[2] / 7 - params[3] / 2)
-        ) ** (1 / 2)
-
-
-def pink_noise(data, width):
-    std = 0
-    datapoints = len(data) - width + 1
-    for i in range(datapoints):
-        std += numpy.std(data[i : i + width]) / width ** 0.5
-    return std / datapoints
-
-
-def period_uncertainty(periods, power):
-    # Determine estimate for uncertainty in period
-    # Method: Full width at half maximum
-    try:
-        # Upper limit
-        index_highest_power = numpy.argmax(power)
-        idx = index_highest_power
-        while True:
-            idx += 1
-            if power[idx] <= 0.5 * power[index_highest_power]:
-                idx_upper = idx
-                break
-        # Lower limit
-        idx = index_highest_power
-        while True:
-            idx -= 1
-            if power[idx] <= 0.5 * power[index_highest_power]:
-                idx_lower = idx
-                break
-        period_uncertainty = 0.5 * (periods[idx_upper] - periods[idx_lower])
-    except:
-        period_uncertainty = float("inf")
-    return period_uncertainty
-
-
-def spectra(chi2, oversampling_factor, chi2_baseline):
-    SR = numpy.min(chi2) / chi2
-    SDE_raw = (1 - numpy.mean(SR)) / numpy.std(SR)
-
-    # Scale SDE_power from 0 to SDE_raw
-    power_raw = SR - numpy.mean(SR)  # shift down to the mean being zero
-    scale = SDE_raw / numpy.max(power_raw)  # scale factor to touch max=SDE_raw
-    power_raw = power_raw * scale
-
-    # Detrended SDE, named "power"
-    kernel = int(oversampling_factor * tls_constants.SDE_MEDIAN_KERNEL_SIZE)
-    if kernel % 2 == 0:
-        kernel = kernel + 1
-    if len(power_raw) > 2 * kernel:
-        my_median = running_median(power_raw, kernel)
-        power = power_raw - my_median
-        # Re-normalize to range between median = 0 and peak = SDE
-        # shift down to the mean being zero
-        power = power - numpy.mean(power)
-        power = power_neighbour_correction(power, kernel, chi2, chi2_baseline)
-        SDE = numpy.max(power / numpy.std(power))
-        # scale factor to touch max=SDE
-        scale = SDE / numpy.max(power)
-        power = power * scale
-    else:
-        power = power_raw
-        SDE = SDE_raw
-
-    return SR, power_raw, power, SDE_raw, SDE
-
-def power_neighbour_correction(sde, kernel, chi2, chi2_baseline):
-    """Returns scaled power spectra taking into account the neighbours used with the given kernel that are below the
-    residuals baseline"""
-    idx = numpy.arange(kernel) + numpy.arange(len(sde) - kernel + 1)[:, None]
-    chi2_idx = chi2[idx]
-    chi2_idx_gtbaseline = [len(numpy.argwhere(chi2_window < chi2_baseline).flatten()) for chi2_window in chi2_idx]
-    # Append the first/last value at the beginning/end to match the length of
-    # data and returned median
-    first_values = chi2_idx_gtbaseline[0]
-    last_values = chi2_idx_gtbaseline[-1]
-    missing_values = len(sde) - len(chi2_idx_gtbaseline)
-    values_front = int(missing_values * 0.5)
-    values_end = missing_values - values_front
-    chi2_idx_gtbaseline = numpy.append(numpy.full(values_front, first_values), chi2_idx_gtbaseline)
-    chi2_idx_gtbaseline = numpy.append(chi2_idx_gtbaseline, numpy.full(values_end, last_values))
-    sde = sde * chi2_idx_gtbaseline / kernel
-    return sde
-
-
-def model_lightcurve(transit_times, period, t, model_transit_single):
-    """Creates the model light curve for the full unfolded dataset"""
-
-    # Append one more transit after and before end of nominal time series
-    # to fully cover beginning and end with out of transit calculations
-    earlier_tt = transit_times[0] - period
-    extended_transit_times = numpy.append(earlier_tt, transit_times)
-    next_tt = transit_times[-1] + period
-    extended_transit_times = numpy.append(extended_transit_times, next_tt)
-    full_x_array = numpy.array([])
-    full_y_array = numpy.array([])
-    rounds = len(extended_transit_times)
-    internal_samples = (
-        int(len(t) / len(transit_times))
-    ) * tls_constants.OVERSAMPLE_MODEL_LIGHT_CURVE
-
-    # Append all periods
-    for i in range(rounds):
-        xmin = extended_transit_times[i] - period / 2
-        xmax = extended_transit_times[i] + period / 2
-        x_array = numpy.linspace(xmin, xmax, internal_samples)
-        full_x_array = numpy.append(full_x_array, x_array)
-        full_y_array = numpy.append(full_y_array, model_transit_single)
-
-    if numpy.all(numpy.isnan(full_x_array)):
-        return None, None
-    else:  # Determine start and end of relevant time series, and crop it
-        start_cadence = numpy.nanargmax(full_x_array > min(t))
-        stop_cadence = numpy.nanargmax(full_x_array > max(t))
-        full_x_array = full_x_array[start_cadence:stop_cadence]
-        full_y_array = full_y_array[start_cadence:stop_cadence]
-        model_lightcurve_model = full_y_array
-        model_lightcurve_time = full_x_array
-        return model_lightcurve_model, model_lightcurve_time
-
-
-def all_transit_times(T0, t, period):
-    """Return all mid-transit times within t"""
-
-    if T0 < min(t):
-        transit_times = [T0 + period]
-    else:
-        transit_times = [T0]
-    previous_transit_time = transit_times[0]
-    transit_number = 0
-    while True:
-        transit_number = transit_number + 1
-        next_transit_time = previous_transit_time + period
-        if next_transit_time < (numpy.min(t) + (numpy.max(t) - numpy.min(t))):
-            transit_times.append(next_transit_time)
-            previous_transit_time = next_transit_time
-        else:
-            break
-    return transit_times
-
-
-def calculate_transit_duration_in_days(t, period, transit_times, duration):
-    """Return estimate for transit duration in days"""
-
-    # Difference between (time series duration / period) and epochs
-    transit_duration_in_days_raw = (
-        duration * calculate_stretch(t, period, transit_times) * period
-    )
-
-    # Correct the duration for gaps in the data
-    transit_duration_in_days = transit_duration_in_days_raw * calculate_fill_factor(t)
-
-    return transit_duration_in_days
-
-
-def calculate_stretch(t, period, transit_times):
-    """Return difference between (time series duration / period) and epochs
-        Example: 
-        - Time series duration = 100 days
-        - Period = 40 days
-        - Epochs = 2 at t0s = [30, 70] days
-        ==> stretch = (100 / 40) / 2 = 1.25"""
-
-    duration_timeseries = (numpy.max(t) - numpy.min(t)) / period
-    epochs = len(transit_times)
-    stretch = duration_timeseries / epochs
-    return stretch
-
-
-def calculate_fill_factor(t):
-    """Return the fraction of existing cadences, assuming constant cadences"""
-
-    average_cadence = numpy.median(numpy.diff(t))
-    span = max(t) - min(t)
-    theoretical_cadences = span / average_cadence
-    fill_factor = (len(t) - 1) / theoretical_cadences
-    return fill_factor
-
-
-def count_stats(t, y, transit_times, transit_duration_in_days):
-    """Return:
-    * in_transit_count:     Number of data points in transit (phase-folded)
-    * after_transit_count:  Number of data points in a bin of transit duration, 
-                            after transit (phase-folded)
-    * before_transit_count: Number of data points in a bin of transit duration, 
-                            before transit (phase-folded)
-    """
-    in_transit_count = 0
-    after_transit_count = 0
-    before_transit_count = 0
-
-    for mid_transit in transit_times:
-        T0 = (
-            mid_transit - 1.5 * transit_duration_in_days
-        )  # start of 1 transit dur before ingress
-        T1 = mid_transit - 0.5 * transit_duration_in_days  # start of ingress
-        T4 = mid_transit + 0.5 * transit_duration_in_days  # end of egress
-        T5 = (
-            mid_transit + 1.5 * transit_duration_in_days
-        )  # end of egress + 1 transit dur
-
-        if T0 > min(t) and T5 < max(t):  # inside time
-            idx_intransit = numpy.where(numpy.logical_and(t > T1, t < T4))
-            idx_before_transit = numpy.where(numpy.logical_and(t > T0, t < T1))
-            idx_after_transit = numpy.where(numpy.logical_and(t > T4, t < T5))
-            points_in_this_in_transit = len(y[idx_intransit])
-            points_in_this_before_transit = len(y[idx_before_transit])
-            points_in_this_after_transit = len(y[idx_after_transit])
-
-            in_transit_count += points_in_this_in_transit
-            before_transit_count += points_in_this_before_transit
-            after_transit_count += points_in_this_after_transit
-
-    return in_transit_count, after_transit_count, before_transit_count
-
-
-def intransit_stats(t, y, transit_times, transit_duration_in_days):
-    """Return all intransit odd and even flux points"""
-
-    all_flux_intransit_odd = numpy.array([])
-    all_flux_intransit_even = numpy.array([])
-    all_flux_intransit = numpy.array([])
-    all_idx_intransit = numpy.array([])
-    per_transit_count = numpy.zeros([len(transit_times)])
-    transit_depths = numpy.zeros([len(transit_times)])
-    transit_depths_uncertainties = numpy.zeros([len(transit_times)])
-
-    for i in range(len(transit_times)):
-
-        depth_mean_odd = numpy.nan
-        depth_mean_even = numpy.nan
-        depth_mean_odd_std = numpy.nan
-        depth_mean_even_std = numpy.nan
-
-        mid_transit = transit_times[i]
-        tmin = mid_transit - 0.5 * transit_duration_in_days
-        tmax = mid_transit + 0.5 * transit_duration_in_days
-        if numpy.isnan(tmin) or numpy.isnan(tmax):
-            idx_intransit = []
-            flux_intransit = []
-            mean_flux = numpy.nan
-        else:
-            idx_intransit = numpy.where(numpy.logical_and(t > tmin, t < tmax))
-            flux_intransit = y[idx_intransit]
-            if len(y[idx_intransit]) > 0:
-                mean_flux = numpy.mean(y[idx_intransit])
-            else:
-                mean_flux = numpy.nan
-        intransit_points = numpy.size(y[idx_intransit])
-        transit_depths[i] = mean_flux
-        if len(y[idx_intransit] > 0):
-            transit_depths_uncertainties[i] = numpy.std(y[idx_intransit]) / numpy.sqrt(
-                intransit_points
-            )
-        else:
-            transit_depths_uncertainties[i] = numpy.nan
-        per_transit_count[i] = intransit_points
-
-        # Check if transit odd/even to collect the flux for the mean calculations
-        if i % 2 == 0:  # even
-            all_flux_intransit_even = numpy.append(
-                all_flux_intransit_even, flux_intransit
-            )
-        else:  # odd
-            all_flux_intransit_odd = numpy.append(
-                all_flux_intransit_odd, flux_intransit
-            )
-        if len(all_flux_intransit_odd) > 0:
-            depth_mean_odd = numpy.mean(all_flux_intransit_odd)
-
-            depth_mean_odd_std = numpy.std(all_flux_intransit_odd) / numpy.sum(
-                len(all_flux_intransit_odd)
-            ) ** (0.5)
-        if len(all_flux_intransit_even) > 0:
-            depth_mean_even = numpy.mean(all_flux_intransit_even)
-            depth_mean_even_std = numpy.std(all_flux_intransit_even) / numpy.sum(
-                len(all_flux_intransit_even)
-            ) ** (0.5)
-
-    return (
-        depth_mean_odd,
-        depth_mean_even,
-        depth_mean_odd_std,
-        depth_mean_even_std,
-        all_flux_intransit_odd,
-        all_flux_intransit_even,
-        per_transit_count,
-        transit_depths,
-        transit_depths_uncertainties,
-    )
-
-
-def snr_stats(
-    t,
-    y,
-    period,
-    duration,
-    T0,
-    transit_times,
-    transit_duration_in_days,
-    per_transit_count,
-    intransit=None
-):
-    """Return snr_per_transit and snr_pink_per_transit"""
-
-    snr_per_transit = numpy.zeros([len(transit_times)])
-    snr_pink_per_transit = numpy.zeros([len(transit_times)])
-    if intransit is None:
-        intransit = transit_mask(t, period, 2 * duration, T0)
-    flux_ootr = y[~intransit]
-
-    try:
-        pinknoise = pink_noise(flux_ootr, int(numpy.mean(per_transit_count)))
-    except:
-        pinknoise = numpy.nan
-
-    # Estimate SNR and pink SNR
-    # Second run because now the out of transit points are known
-    if len(flux_ootr) > 0:
-        std = numpy.std(flux_ootr)
-    else:
-        std = numpy.nan
-    for i in range(len(transit_times)):
-        mid_transit = transit_times[i]
-        tmin = mid_transit - 0.5 * transit_duration_in_days
-        tmax = mid_transit + 0.5 * transit_duration_in_days
-        if numpy.isnan(tmin) or numpy.isnan(tmax):
-            idx_intransit = []
-            mean_flux = numpy.nan
-        else:
-            idx_intransit = numpy.where(numpy.logical_and(t > tmin, t < tmax))
-            if len(y[idx_intransit]) > 0:
-                mean_flux = numpy.mean(y[idx_intransit])
-            else:
-                mean_flux = numpy.nan
-
-        intransit_points = numpy.size(y[idx_intransit])
-        try:
-            snr_pink_per_transit[i] = (1 - mean_flux) / pinknoise if mean_flux < 1 else (mean_flux - 1) / pinknoise
-            if intransit_points > 0 and not numpy.isnan(std):
-                std_binned = std / intransit_points ** 0.5
-                snr_per_transit[i] = (1 - mean_flux) / std_binned if mean_flux < 1 else (mean_flux - 1) / std_binned
-            else:
-                snr_per_transit[i] = 0
-                snr_pink_per_transit[i] = 0
-        except:
-            snr_per_transit[i] = 0
-            snr_pink_per_transit[i] = 0
-
-    return snr_per_transit, snr_pink_per_transit
+from __future__ import division, print_function
+import numpy
+from os import path
+from . import tls_constants
+from .helpers import running_median, transit_mask
+
+
+def FAP(SDE):
+    """Returns FAP (False Alarm Probability) for a given SDE"""
+    data = numpy.genfromtxt(
+        path.join(tls_constants.resources_dir, "fap.csv"),
+        dtype="f8, f8",
+        delimiter=",",
+        names=["FAP", "SDE"],
+    )
+    return data["FAP"][numpy.argmax(data["SDE"] > SDE)]
+
+
+def rp_rs_from_depth(depth, law, params):
+    """Takes the maximum transit depth, limb-darkening law and parameters
+    Returns R_P / R_S (ratio of planetary to stellar radius)
+    Source: Heller 2019, https://arxiv.org/abs/1901.01730"""
+
+    # Validations:
+    # - LD law must exist
+    # - All parameters must be floats or ints
+    # - All parameters must be given in the correct quanitity for the law
+
+    if len(params) == 1:
+        params = float(params[0])
+
+    if not isinstance(params, (float, int)) and not all(
+        isinstance(x, (float, int)) for x in params
+    ):
+        raise ValueError("All limb-darkening parameters must be numbers")
+
+    laws = "linear, quadratic, squareroot, logarithmic, nonlinear"
+    if law not in laws:
+        raise ValueError("Please provide a supported limb-darkening law:", laws)
+
+    if law == "linear" and not isinstance(params, float):
+        raise ValueError("Please provide exactly one parameter")
+
+    if law in "quadratic, logarithmic, squareroot" and len(params) != 2:
+        raise ValueError("Please provide exactly two limb-darkening parameters")
+
+    if law == "nonlinear" and len(params) != 4:
+        raise ValueError("Please provide exactly four limb-darkening parameters")
+
+    # Actual calculations of the return value
+    if law == "linear":
+        return (depth * (1 - params / 3)) ** (1 / 2)
+
+    if law == "quadratic":
+        return (depth * (1 - params[0] / 3 - params[1] / 6)) ** (1 / 2)
+
+    if law == "squareroot":
+        return (depth * (1 - params[0] / 3 - params[1] / 5)) ** (1 / 2)
+
+    if law == "logarithmic":
+        return (depth * (1 + 2 * params[1] / 9 - params[0] / 3)) ** (1 / 2)
+
+    if law == "nonlinear":
+        return (
+            depth
+            * (1 - params[0] / 5 - params[1] / 3 - 3 * params[2] / 7 - params[3] / 2)
+        ) ** (1 / 2)
+
+
+def pink_noise(data, width):
+    std = 0
+    datapoints = len(data) - width + 1
+    for i in range(datapoints):
+        std += numpy.std(data[i : i + width]) / width ** 0.5
+    return std / datapoints
+
+
+def period_uncertainty(periods, power):
+    # Determine estimate for uncertainty in period
+    # Method: Full width at half maximum
+    try:
+        # Upper limit
+        index_highest_power = numpy.argmax(power)
+        idx = index_highest_power
+        while True:
+            idx += 1
+            if power[idx] <= 0.5 * power[index_highest_power]:
+                idx_upper = idx
+                break
+        # Lower limit
+        idx = index_highest_power
+        while True:
+            idx -= 1
+            if power[idx] <= 0.5 * power[index_highest_power]:
+                idx_lower = idx
+                break
+        period_uncertainty = 0.5 * (periods[idx_upper] - periods[idx_lower])
+    except:
+        period_uncertainty = float("inf")
+    return period_uncertainty
+
+
+def spectra(chi2, oversampling_factor, chi2_baseline):
+    SR = numpy.min(chi2) / chi2
+    SDE_raw = (1 - numpy.mean(SR)) / numpy.std(SR)
+
+    # Scale SDE_power from 0 to SDE_raw
+    power_raw = SR - numpy.mean(SR)  # shift down to the mean being zero
+    scale = SDE_raw / numpy.max(power_raw)  # scale factor to touch max=SDE_raw
+    power_raw = power_raw * scale
+
+    # Detrended SDE, named "power"
+    kernel = int(oversampling_factor * tls_constants.SDE_MEDIAN_KERNEL_SIZE)
+    if kernel % 2 == 0:
+        kernel = kernel + 1
+    if len(power_raw) > 2 * kernel:
+        my_median = running_median(power_raw, kernel)
+        power = power_raw - my_median
+        # Re-normalize to range between median = 0 and peak = SDE
+        # shift down to the mean being zero
+        power = power - numpy.mean(power)
+        power = power_neighbour_correction(power, kernel, chi2, chi2_baseline)
+        SDE = numpy.max(power / numpy.std(power))
+        # scale factor to touch max=SDE
+        scale = SDE / numpy.max(power)
+        power = power * scale
+    else:
+        power = power_raw
+        SDE = SDE_raw
+
+    return SR, power_raw, power, SDE_raw, SDE
+
+def power_neighbour_correction(sde, kernel, chi2, chi2_baseline):
+    """Returns scaled power spectra taking into account the neighbours used with the given kernel that are below the
+    residuals baseline"""
+    idx = numpy.arange(kernel) + numpy.arange(len(sde) - kernel + 1)[:, None]
+    chi2_idx = chi2[idx]
+    chi2_idx_gtbaseline = [len(numpy.argwhere(chi2_window < chi2_baseline).flatten()) for chi2_window in chi2_idx]
+    # Append the first/last value at the beginning/end to match the length of
+    # data and returned median
+    first_values = chi2_idx_gtbaseline[0]
+    last_values = chi2_idx_gtbaseline[-1]
+    missing_values = len(sde) - len(chi2_idx_gtbaseline)
+    values_front = int(missing_values * 0.5)
+    values_end = missing_values - values_front
+    chi2_idx_gtbaseline = numpy.append(numpy.full(values_front, first_values), chi2_idx_gtbaseline)
+    chi2_idx_gtbaseline = numpy.append(chi2_idx_gtbaseline, numpy.full(values_end, last_values))
+    sde = sde * chi2_idx_gtbaseline / kernel
+    return sde
+
+
+def model_lightcurve(transit_times, period, t, model_transit_single):
+    """Creates the model light curve for the full unfolded dataset"""
+
+    # Append one more transit after and before end of nominal time series
+    # to fully cover beginning and end with out of transit calculations
+    earlier_tt = transit_times[0] - period
+    extended_transit_times = numpy.append(earlier_tt, transit_times)
+    next_tt = transit_times[-1] + period
+    extended_transit_times = numpy.append(extended_transit_times, next_tt)
+    full_x_array = numpy.array([])
+    full_y_array = numpy.array([])
+    rounds = len(extended_transit_times)
+    internal_samples = (
+        int(len(t) / len(transit_times))
+    ) * tls_constants.OVERSAMPLE_MODEL_LIGHT_CURVE
+
+    # Append all periods
+    for i in range(rounds):
+        xmin = extended_transit_times[i] - period / 2
+        xmax = extended_transit_times[i] + period / 2
+        x_array = numpy.linspace(xmin, xmax, internal_samples)
+        full_x_array = numpy.append(full_x_array, x_array)
+        full_y_array = numpy.append(full_y_array, model_transit_single)
+
+    if numpy.all(numpy.isnan(full_x_array)):
+        return None, None
+    else:  # Determine start and end of relevant time series, and crop it
+        start_cadence = numpy.nanargmax(full_x_array > min(t))
+        stop_cadence = numpy.nanargmax(full_x_array > max(t))
+        full_x_array = full_x_array[start_cadence:stop_cadence]
+        full_y_array = full_y_array[start_cadence:stop_cadence]
+        model_lightcurve_model = full_y_array
+        model_lightcurve_time = full_x_array
+        return model_lightcurve_model, model_lightcurve_time
+
+
+def all_transit_times(T0, t, period):
+    """Return all mid-transit times within t"""
+
+    if T0 < min(t):
+        transit_times = [T0 + period]
+    else:
+        transit_times = [T0]
+    previous_transit_time = transit_times[0]
+    transit_number = 0
+    while True:
+        transit_number = transit_number + 1
+        next_transit_time = previous_transit_time + period
+        if next_transit_time < (numpy.min(t) + (numpy.max(t) - numpy.min(t))):
+            transit_times.append(next_transit_time)
+            previous_transit_time = next_transit_time
+        else:
+            break
+    return transit_times
+
+
+def calculate_transit_duration_in_days(t, period, transit_times, duration):
+    """Return estimate for transit duration in days"""
+
+    # Difference between (time series duration / period) and epochs
+    transit_duration_in_days_raw = (
+        duration * calculate_stretch(t, period, transit_times) * period
+    )
+
+    # Correct the duration for gaps in the data
+    transit_duration_in_days = transit_duration_in_days_raw * calculate_fill_factor(t)
+
+    return transit_duration_in_days
+
+
+def calculate_stretch(t, period, transit_times):
+    """Return difference between (time series duration / period) and epochs
+        Example: 
+        - Time series duration = 100 days
+        - Period = 40 days
+        - Epochs = 2 at t0s = [30, 70] days
+        ==> stretch = (100 / 40) / 2 = 1.25"""
+
+    duration_timeseries = (numpy.max(t) - numpy.min(t)) / period
+    epochs = len(transit_times)
+    stretch = duration_timeseries / epochs
+    return stretch
+
+
+def calculate_fill_factor(t):
+    """Return the fraction of existing cadences, assuming constant cadences"""
+
+    average_cadence = numpy.median(numpy.diff(t))
+    span = max(t) - min(t)
+    theoretical_cadences = span / average_cadence
+    fill_factor = (len(t) - 1) / theoretical_cadences
+    return fill_factor
+
+
+def count_stats(t, y, transit_times, transit_duration_in_days):
+    """Return:
+    * in_transit_count:     Number of data points in transit (phase-folded)
+    * after_transit_count:  Number of data points in a bin of transit duration, 
+                            after transit (phase-folded)
+    * before_transit_count: Number of data points in a bin of transit duration, 
+                            before transit (phase-folded)
+    """
+    in_transit_count = 0
+    after_transit_count = 0
+    before_transit_count = 0
+
+    for mid_transit in transit_times:
+        T0 = (
+            mid_transit - 1.5 * transit_duration_in_days
+        )  # start of 1 transit dur before ingress
+        T1 = mid_transit - 0.5 * transit_duration_in_days  # start of ingress
+        T4 = mid_transit + 0.5 * transit_duration_in_days  # end of egress
+        T5 = (
+            mid_transit + 1.5 * transit_duration_in_days
+        )  # end of egress + 1 transit dur
+
+        if T0 > min(t) and T5 < max(t):  # inside time
+            idx_intransit = numpy.where(numpy.logical_and(t > T1, t < T4))
+            idx_before_transit = numpy.where(numpy.logical_and(t > T0, t < T1))
+            idx_after_transit = numpy.where(numpy.logical_and(t > T4, t < T5))
+            points_in_this_in_transit = len(y[idx_intransit])
+            points_in_this_before_transit = len(y[idx_before_transit])
+            points_in_this_after_transit = len(y[idx_after_transit])
+
+            in_transit_count += points_in_this_in_transit
+            before_transit_count += points_in_this_before_transit
+            after_transit_count += points_in_this_after_transit
+
+    return in_transit_count, after_transit_count, before_transit_count
+
+
+def intransit_stats(t, y, transit_times, transit_duration_in_days):
+    """Return all intransit odd and even flux points"""
+
+    all_flux_intransit_odd = numpy.array([])
+    all_flux_intransit_even = numpy.array([])
+    all_flux_intransit = numpy.array([])
+    all_idx_intransit = numpy.array([])
+    per_transit_count = numpy.zeros([len(transit_times)])
+    transit_depths = numpy.zeros([len(transit_times)])
+    transit_depths_uncertainties = numpy.zeros([len(transit_times)])
+
+    for i in range(len(transit_times)):
+
+        depth_mean_odd = numpy.nan
+        depth_mean_even = numpy.nan
+        depth_mean_odd_std = numpy.nan
+        depth_mean_even_std = numpy.nan
+
+        mid_transit = transit_times[i]
+        tmin = mid_transit - 0.5 * transit_duration_in_days
+        tmax = mid_transit + 0.5 * transit_duration_in_days
+        if numpy.isnan(tmin) or numpy.isnan(tmax):
+            idx_intransit = []
+            flux_intransit = []
+            mean_flux = numpy.nan
+        else:
+            idx_intransit = numpy.where(numpy.logical_and(t > tmin, t < tmax))
+            flux_intransit = y[idx_intransit]
+            if len(y[idx_intransit]) > 0:
+                mean_flux = numpy.mean(y[idx_intransit])
+            else:
+                mean_flux = numpy.nan
+        intransit_points = numpy.size(y[idx_intransit])
+        transit_depths[i] = mean_flux
+        if len(y[idx_intransit] > 0):
+            transit_depths_uncertainties[i] = numpy.std(y[idx_intransit]) / numpy.sqrt(
+                intransit_points
+            )
+        else:
+            transit_depths_uncertainties[i] = numpy.nan
+        per_transit_count[i] = intransit_points
+
+        # Check if transit odd/even to collect the flux for the mean calculations
+        if i % 2 == 0:  # even
+            all_flux_intransit_even = numpy.append(
+                all_flux_intransit_even, flux_intransit
+            )
+        else:  # odd
+            all_flux_intransit_odd = numpy.append(
+                all_flux_intransit_odd, flux_intransit
+            )
+        if len(all_flux_intransit_odd) > 0:
+            depth_mean_odd = numpy.mean(all_flux_intransit_odd)
+
+            depth_mean_odd_std = numpy.std(all_flux_intransit_odd) / numpy.sum(
+                len(all_flux_intransit_odd)
+            ) ** (0.5)
+        if len(all_flux_intransit_even) > 0:
+            depth_mean_even = numpy.mean(all_flux_intransit_even)
+            depth_mean_even_std = numpy.std(all_flux_intransit_even) / numpy.sum(
+                len(all_flux_intransit_even)
+            ) ** (0.5)
+
+    return (
+        depth_mean_odd,
+        depth_mean_even,
+        depth_mean_odd_std,
+        depth_mean_even_std,
+        all_flux_intransit_odd,
+        all_flux_intransit_even,
+        per_transit_count,
+        transit_depths,
+        transit_depths_uncertainties,
+    )
+
+
+def snr_stats(
+    t,
+    y,
+    period,
+    duration,
+    T0,
+    transit_times,
+    transit_duration_in_days,
+    per_transit_count,
+    intransit=None
+):
+    """Return snr_per_transit and snr_pink_per_transit"""
+
+    snr_per_transit = numpy.zeros([len(transit_times)])
+    snr_pink_per_transit = numpy.zeros([len(transit_times)])
+    if intransit is None:
+        intransit = transit_mask(t, period, 2 * duration, T0)
+    flux_ootr = y[~intransit]
+
+    try:
+        pinknoise = pink_noise(flux_ootr, int(numpy.mean(per_transit_count)))
+    except:
+        pinknoise = numpy.nan
+
+    # Estimate SNR and pink SNR
+    # Second run because now the out of transit points are known
+    if len(flux_ootr) > 0:
+        std = numpy.std(flux_ootr)
+    else:
+        std = numpy.nan
+    for i in range(len(transit_times)):
+        mid_transit = transit_times[i]
+        tmin = mid_transit - 0.5 * transit_duration_in_days
+        tmax = mid_transit + 0.5 * transit_duration_in_days
+        if numpy.isnan(tmin) or numpy.isnan(tmax):
+            idx_intransit = []
+            mean_flux = numpy.nan
+        else:
+            idx_intransit = numpy.where(numpy.logical_and(t > tmin, t < tmax))
+            if len(y[idx_intransit]) > 0:
+                mean_flux = numpy.mean(y[idx_intransit])
+            else:
+                mean_flux = numpy.nan
+
+        intransit_points = numpy.size(y[idx_intransit])
+        try:
+            snr_pink_per_transit[i] = (1 - mean_flux) / pinknoise if mean_flux < 1 else (mean_flux - 1) / pinknoise
+            if intransit_points > 0 and not numpy.isnan(std):
+                std_binned = std / intransit_points ** 0.5
+                snr_per_transit[i] = (1 - mean_flux) / std_binned if mean_flux < 1 else (mean_flux - 1) / std_binned
+            else:
+                snr_per_transit[i] = 0
+                snr_pink_per_transit[i] = 0
+        except:
+            snr_per_transit[i] = 0
+            snr_pink_per_transit[i] = 0
+
+    return snr_per_transit, snr_pink_per_transit
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/command_line.py` & `foldedleastsquares-1.0.41/foldedleastsquares/command_line.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from __future__ import division, print_function
-from . import transitleastsquares
-from . import tls_constants as tls_constants
-import numpy
-import os
-import sys
-from configparser import ConfigParser
-
-try:
-    import argparse
-except:
-    raise ImportError("Could not import package argparse")
-
-
-def main():
-    pass
-
-
-print(tls_constants.TLS_VERSION)
-parser = argparse.ArgumentParser()
-parser.add_argument("lightcurve", help="path to lightcurve file")
-parser.add_argument("-o", "--output", help="path to output directory")
-parser.add_argument("-c", "--config", help="path to configuration file")
-args = parser.parse_args()
-
-# Read config file if possible
-use_config_file = False
-if args.config is not None:
-    try:
-        config = ConfigParser()
-        config.read(args.config)
-        R_star = float(config["Grid"]["R_star"])
-        R_star_min = float(config["Grid"]["R_star_min"])
-        R_star_max = float(config["Grid"]["R_star_max"])
-        M_star = float(config["Grid"]["M_star"])
-        M_star_min = float(config["Grid"]["M_star_min"])
-        M_star_max = float(config["Grid"]["M_star_max"])
-        period_min = float(config["Grid"]["period_min"])
-        period_max = float(config["Grid"]["period_max"])
-        n_transits_min = int(config["Grid"]["n_transits_min"])
-        transit_template = config["Template"]["transit_template"]
-        duration_grid_step = float(config["Speed"]["duration_grid_step"])
-        transit_depth_min = float(config["Speed"]["transit_depth_min"])
-        oversampling_factor = int(config["Speed"]["oversampling_factor"])
-        T0_fit_margin = float(config["Speed"]["T0_fit_margin"])
-        use_threads = int(config["Speed"]["use_threads"])
-        delimiter = int(config["File"]["delimiter"])
-        use_config_file = True
-        print("Using TLS configuration from config file", args.config)
-    except:
-        print(
-            "Using default values because of broken or missing configuration file",
-            args.config,
-        )
-else:
-    print("No config file given. Using default values")
-
-# Load data
-if use_config_file:
-    data = numpy.genfromtxt(args.lightcurve, delimiter=args.delimiter)
-else:
-    data = numpy.genfromtxt(args.lightcurve, delimiter=",")
-
-t = data[:, 0]
-y = data[:, 1]
-
-
-# Initiate transitleastsquares model
-try:
-    dy = data[:, 2]
-    model = transitleastsquares(t, y, dy)
-except:
-    model = transitleastsquares(t, y)
-
-if use_config_file:
-    results = model.power(
-        R_star=R_star,
-        R_star_min=R_star_min,
-        R_star_max=R_star_max,
-        M_star=M_star,
-        M_star_min=M_star_min,
-        M_star_max=M_star_max,
-        period_min=period_min,
-        period_max=period_max,
-        n_transits_min=n_transits_min,
-        transit_template=transit_template,
-        duration_grid_step=duration_grid_step,
-        transit_depth_min=transit_depth_min,
-        oversampling_factor=oversampling_factor,
-        T0_fit_margin=T0_fit_margin,
-        use_threads=use_threads,
-    )
-else:
-    results = model.power()
-
-
-# Save results to CSV files
-
-# Determine path and file names of output files
-if args.output is None:
-    file_stats = args.lightcurve + "_statistics.csv"
-    file_power = args.lightcurve + "_power.csv"
-else:
-    file_stats = os.path.join(args.output, args.lightcurve + "_statistics.csv")
-    file_power = os.path.join(args.output, args.lightcurve + "_power.csv")
-
-# Save
-try:
-    numpy.savetxt(
-        file_power,
-        numpy.column_stack(
-            [
-                list(dict(list(results.items())[25:26]).values())[0],
-                list(dict(list(results.items())[26:27]).values())[0],
-            ]
-        ),
-        delimiter=",",
-        fmt="%1.6f",
-    )
-    print("SDE-ogram saved to", file_stats)
-
-    statistics = dict(list(results.items())[0:25])
-    numpy.set_printoptions(precision=8, threshold=10e10)
-    with open(file_stats, "w") as f:
-        for key in statistics.keys():
-            f.write("%s %s\n" % (key, statistics[key]))
-    print("Statistics saved to", file_stats)
-except IOError:
-    print("Error saving result file")
+from __future__ import division, print_function
+from . import transitleastsquares
+from . import tls_constants as tls_constants
+import numpy
+import os
+import sys
+from configparser import ConfigParser
+
+try:
+    import argparse
+except:
+    raise ImportError("Could not import package argparse")
+
+
+def main():
+    pass
+
+
+print(tls_constants.TLS_VERSION)
+parser = argparse.ArgumentParser()
+parser.add_argument("lightcurve", help="path to lightcurve file")
+parser.add_argument("-o", "--output", help="path to output directory")
+parser.add_argument("-c", "--config", help="path to configuration file")
+args = parser.parse_args()
+
+# Read config file if possible
+use_config_file = False
+if args.config is not None:
+    try:
+        config = ConfigParser()
+        config.read(args.config)
+        R_star = float(config["Grid"]["R_star"])
+        R_star_min = float(config["Grid"]["R_star_min"])
+        R_star_max = float(config["Grid"]["R_star_max"])
+        M_star = float(config["Grid"]["M_star"])
+        M_star_min = float(config["Grid"]["M_star_min"])
+        M_star_max = float(config["Grid"]["M_star_max"])
+        period_min = float(config["Grid"]["period_min"])
+        period_max = float(config["Grid"]["period_max"])
+        n_transits_min = int(config["Grid"]["n_transits_min"])
+        transit_template = config["Template"]["transit_template"]
+        duration_grid_step = float(config["Speed"]["duration_grid_step"])
+        transit_depth_min = float(config["Speed"]["transit_depth_min"])
+        oversampling_factor = int(config["Speed"]["oversampling_factor"])
+        T0_fit_margin = float(config["Speed"]["T0_fit_margin"])
+        use_threads = int(config["Speed"]["use_threads"])
+        delimiter = int(config["File"]["delimiter"])
+        use_config_file = True
+        print("Using TLS configuration from config file", args.config)
+    except:
+        print(
+            "Using default values because of broken or missing configuration file",
+            args.config,
+        )
+else:
+    print("No config file given. Using default values")
+
+# Load data
+if use_config_file:
+    data = numpy.genfromtxt(args.lightcurve, delimiter=args.delimiter)
+else:
+    data = numpy.genfromtxt(args.lightcurve, delimiter=",")
+
+t = data[:, 0]
+y = data[:, 1]
+
+
+# Initiate transitleastsquares model
+try:
+    dy = data[:, 2]
+    model = transitleastsquares(t, y, dy)
+except:
+    model = transitleastsquares(t, y)
+
+if use_config_file:
+    results = model.power(
+        R_star=R_star,
+        R_star_min=R_star_min,
+        R_star_max=R_star_max,
+        M_star=M_star,
+        M_star_min=M_star_min,
+        M_star_max=M_star_max,
+        period_min=period_min,
+        period_max=period_max,
+        n_transits_min=n_transits_min,
+        transit_template=transit_template,
+        duration_grid_step=duration_grid_step,
+        transit_depth_min=transit_depth_min,
+        oversampling_factor=oversampling_factor,
+        T0_fit_margin=T0_fit_margin,
+        use_threads=use_threads,
+    )
+else:
+    results = model.power()
+
+
+# Save results to CSV files
+
+# Determine path and file names of output files
+if args.output is None:
+    file_stats = args.lightcurve + "_statistics.csv"
+    file_power = args.lightcurve + "_power.csv"
+else:
+    file_stats = os.path.join(args.output, args.lightcurve + "_statistics.csv")
+    file_power = os.path.join(args.output, args.lightcurve + "_power.csv")
+
+# Save
+try:
+    numpy.savetxt(
+        file_power,
+        numpy.column_stack(
+            [
+                list(dict(list(results.items())[25:26]).values())[0],
+                list(dict(list(results.items())[26:27]).values())[0],
+            ]
+        ),
+        delimiter=",",
+        fmt="%1.6f",
+    )
+    print("SDE-ogram saved to", file_stats)
+
+    statistics = dict(list(results.items())[0:25])
+    numpy.set_printoptions(precision=8, threshold=10e10)
+    with open(file_stats, "w") as f:
+        for key in statistics.keys():
+            f.write("%s %s\n" % (key, statistics[key]))
+    print("Statistics saved to", file_stats)
+except IOError:
+    print("Error saving result file")
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/validate.py` & `foldedleastsquares-1.0.41/foldedleastsquares/validate.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-from __future__ import division, print_function
-import numpy
-import warnings
-import multiprocessing
-
-from .template_generator.transit_template_generator import TransitTemplateGenerator
-from .helpers import cleaned_array, impact_to_inclination
-from . import tls_constants
-
-
-def validate_inputs(t, y, dy):
-    """Check the consistency of the inputs"""
-
-    # Clean array
-    if dy is None:
-        t, y = cleaned_array(t, y)
-    else:
-        t, y, dy = cleaned_array(t, y, dy)
-        # Normalize dy to act as weights in least squares calculatio
-        dy = dy / numpy.mean(dy)
-
-    duration = max(t) - min(t)
-    if duration <= 0:
-        raise ValueError("Time duration must positive")
-    if numpy.size(y) < 3 or numpy.size(t) < 3:
-        raise ValueError("Too few values in data set")
-    if numpy.mean(y) > 1.01 or numpy.mean(y) < 0.99:
-        text = (
-            "Warning: The mean flux should be normalized to 1"
-            + ", but it was found to be "
-            + str(numpy.mean(y))
-        )
-        warnings.warn(text)
-
-    if min(y) < 0:
-        raise ValueError("Flux values must be positive")
-    if max(y) >= float("inf"):
-        raise ValueError("Flux values must be finite")
-
-    # If no dy is given, create it with the standard deviation of the flux
-    if dy is None:
-        dy = numpy.full(len(y), numpy.std(y))
-    if numpy.size(t) != numpy.size(y) or numpy.size(t) != numpy.size(dy):
-        raise ValueError("Arrays (t, y, dy) must be of the same dimensions")
-    if t.ndim != 1:  # Size identity ensures dimensional identity
-        raise ValueError("Inputs (t, y, dy) must be 1-dimensional")
-
-    return t, y, dy
-
-
-def validate_args(self, kwargs):
-
-    # Warn user if unknown parameters
-    for key, value in kwargs.items():
-        if key not in tls_constants.VALID_PARAMETERS:
-            text = "Ignoring unknown parameter: " + str(key)
-            warnings.warn(text)
-
-    """Validate **kwargs and set to defaults where missing"""
-    self.show_progress_bar = kwargs.get("show_progress_bar", True)
-    self.transit_depth_min = kwargs.get(
-        "transit_depth_min", tls_constants.TRANSIT_DEPTH_MIN
-    )
-    self.R_star = kwargs.get("R_star", tls_constants.R_STAR)
-    self.M_star = kwargs.get("M_star", tls_constants.M_STAR)
-    self.oversampling_factor = kwargs.get(
-        "oversampling_factor", tls_constants.OVERSAMPLING_FACTOR
-    )
-    self.period_max = kwargs.get("period_max", float("inf"))
-    self.period_min = kwargs.get("period_min", 0)
-    self.n_transits_min = kwargs.get("n_transits_min", tls_constants.N_TRANSITS_MIN)
-
-    self.R_star_min = kwargs.get("R_star_min", tls_constants.R_STAR_MIN)
-    self.R_star_max = kwargs.get("R_star_max", tls_constants.R_STAR_MAX)
-    self.M_star_min = kwargs.get("M_star_min", tls_constants.M_STAR_MIN)
-    self.M_star_max = kwargs.get("M_star_max", tls_constants.M_STAR_MAX)
-    self.duration_grid_step = kwargs.get(
-        "duration_grid_step", tls_constants.DURATION_GRID_STEP
-    )
-
-    self.use_threads = kwargs.get("use_threads", multiprocessing.cpu_count())
-
-    self.per = kwargs.get("per", tls_constants.DEFAULT_PERIOD)
-    self.rp = kwargs.get("rp", tls_constants.DEFAULT_RP)
-    self.a = kwargs.get("a", tls_constants.DEFAULT_A)
-
-    self.T0_fit_margin = kwargs.get("T0_fit_margin", tls_constants.T0_FIT_MARGIN)
-
-    # If an impact parameter is given, it overrules the supplied inclination
-    if "b" in kwargs:
-        self.b = kwargs.get("b")
-        self.inc = impact_to_inclination(b=self.b, semimajor_axis=self.a)
-    else:
-        self.inc = kwargs.get("inc", tls_constants.DEFAULT_INC)
-
-    self.ecc = kwargs.get("ecc", tls_constants.DEFAULT_ECC)
-    self.w = kwargs.get("w", tls_constants.DEFAULT_W)
-    self.u = kwargs.get("u", tls_constants.DEFAULT_U)
-    self.limb_dark = kwargs.get("limb_dark", tls_constants.DEFAULT_LIMB_DARK)
-
-    self.transit_template = kwargs.get("transit_template", "default")
-    if self.transit_template == "default":
-        self.per = tls_constants.DEFAULT_PERIOD
-        self.rp = tls_constants.DEFAULT_RP
-        self.a = tls_constants.DEFAULT_A
-        self.inc = tls_constants.DEFAULT_INC
-
-    elif self.transit_template == "grazing":
-        self.b = tls_constants.GRAZING_B
-        self.inc = impact_to_inclination(b=self.b, semimajor_axis=self.a)
-
-    elif self.transit_template == "box":
-        self.per = tls_constants.BOX_PERIOD
-        self.rp = tls_constants.BOX_RP
-        self.a = tls_constants.BOX_A
-        self.b = tls_constants.BOX_B
-        self.inc = tls_constants.BOX_INC
-        self.u = tls_constants.BOX_U
-        self.limb_dark = tls_constants.BOX_LIMB_DARK
-
-    elif self.transit_template == "tailed":
-        self.per = tls_constants.DEFAULT_PERIOD
-        self.rp = tls_constants.DEFAULT_RP
-        self.a = tls_constants.DEFAULT_A
-        self.inc = tls_constants.DEFAULT_INC
-
-    elif self.transit_template == "custom":
-        custom_transit_template_generator = kwargs.get("transit_template_generator")
-        if not issubclass(type(custom_transit_template_generator), TransitTemplateGenerator):
-            raise ValueError(
-                'The custom transit_template_generator does not implement TransitTemplateGenerator.'
-            )
-        else:
-            self.transit_template_generators["custom"] = custom_transit_template_generator
-
-    else:
-        raise ValueError(
-            'Unknown transit_template. Known values: \
-            "default", "grazing", "box", "tailed"'
-        )
-
-    self.period_grid = kwargs.get("period_grid", None)
-
-    """Validations to avoid (garbage in ==> garbage out)"""
-
-    # Stellar radius
-    # 0 < R_star < inf
-    if self.R_star <= 0 or self.R_star >= float("inf"):
-        raise ValueError("R_star must be positive")
-
-    # Assert (0 < R_star_min <= R_star)
-    if self.R_star_min > self.R_star:
-        raise ValueError("R_star_min <= R_star is required")
-    if self.R_star_min <= 0 or self.R_star_min >= float("inf"):
-        raise ValueError("R_star_min must be positive")
-
-    # Assert (R_star <= R_star_max < inf)
-    if self.R_star_max < self.R_star:
-        raise ValueError("R_star_max >= R_star is required")
-    if self.R_star_max <= 0 or self.R_star_max >= float("inf"):
-        raise ValueError("R_star_max must be positive")
-
-    # Stellar mass
-    # Assert (0 < M_star < inf)
-    if self.M_star <= 0 or self.M_star >= float("inf"):
-        raise ValueError("M_star must be positive")
-
-    # Assert (0 < M_star_min <= M_star)
-    if self.M_star_min > self.M_star:
-        raise ValueError("M_star_min <= M_star is required")
-    if self.M_star_min <= 0 or self.M_star_min >= float("inf"):
-        raise ValueError("M_star_min must be positive")
-
-    # Assert (M_star <= M_star_max < inf)
-    if self.M_star_max < self.M_star:
-        raise ValueError("M_star_max >= M_star required")
-    if self.M_star_max <= 0 or self.M_star_max >= float("inf"):
-        raise ValueError("M_star_max must be positive")
-
-    # Period grid
-    if self.period_min < 0:
-        raise ValueError("period_min >= 0 required")
-    if self.period_min >= self.period_max:
-        raise ValueError("period_min < period_max required")
-    if not isinstance(self.n_transits_min, int):
-        raise ValueError("n_transits_min must be an integer value")
-    if self.n_transits_min < 1:
-        raise ValueError("n_transits_min must be an integer value >= 1")
-
-    if not isinstance(self.use_threads, int) or self.use_threads < 1:
-        raise ValueError("use_threads must be an integer value >= 1")
-
-    # Assert 0 < T0_fit_margin < 0.1
-    if self.T0_fit_margin < 0:
-        self.T0_fit_margin = 0
-    elif self.T0_fit_margin > 0.1:  # Sensible limit 10% of transit duration
-        self.T0_fit_margin = 0.1
-
-    if self.period_grid is not None and not isinstance(self.period_grid, numpy.ndarray):
-        raise ValueError("period_grid must be a `ndarray`")
-    return self, kwargs
+from __future__ import division, print_function
+import numpy
+import warnings
+import multiprocessing
+
+from .template_generator.transit_template_generator import TransitTemplateGenerator
+from .helpers import cleaned_array, impact_to_inclination
+from . import tls_constants
+
+
+def validate_inputs(t, y, dy):
+    """Check the consistency of the inputs"""
+
+    # Clean array
+    if dy is None:
+        t, y = cleaned_array(t, y)
+    else:
+        t, y, dy = cleaned_array(t, y, dy)
+        # Normalize dy to act as weights in least squares calculatio
+        dy = dy / numpy.mean(dy)
+
+    duration = max(t) - min(t)
+    if duration <= 0:
+        raise ValueError("Time duration must positive")
+    if numpy.size(y) < 3 or numpy.size(t) < 3:
+        raise ValueError("Too few values in data set")
+    if numpy.mean(y) > 1.01 or numpy.mean(y) < 0.99:
+        text = (
+            "Warning: The mean flux should be normalized to 1"
+            + ", but it was found to be "
+            + str(numpy.mean(y))
+        )
+        warnings.warn(text)
+
+    if min(y) < 0:
+        raise ValueError("Flux values must be positive")
+    if max(y) >= float("inf"):
+        raise ValueError("Flux values must be finite")
+
+    # If no dy is given, create it with the standard deviation of the flux
+    if dy is None:
+        dy = numpy.full(len(y), numpy.std(y))
+    if numpy.size(t) != numpy.size(y) or numpy.size(t) != numpy.size(dy):
+        raise ValueError("Arrays (t, y, dy) must be of the same dimensions")
+    if t.ndim != 1:  # Size identity ensures dimensional identity
+        raise ValueError("Inputs (t, y, dy) must be 1-dimensional")
+
+    return t, y, dy
+
+
+def validate_args(self, kwargs):
+
+    # Warn user if unknown parameters
+    for key, value in kwargs.items():
+        if key not in tls_constants.VALID_PARAMETERS:
+            text = "Ignoring unknown parameter: " + str(key)
+            warnings.warn(text)
+
+    """Validate **kwargs and set to defaults where missing"""
+    self.show_progress_bar = kwargs.get("show_progress_bar", True)
+    self.transit_depth_min = kwargs.get(
+        "transit_depth_min", tls_constants.TRANSIT_DEPTH_MIN
+    )
+    self.R_star = kwargs.get("R_star", tls_constants.R_STAR)
+    self.M_star = kwargs.get("M_star", tls_constants.M_STAR)
+    self.oversampling_factor = kwargs.get(
+        "oversampling_factor", tls_constants.OVERSAMPLING_FACTOR
+    )
+    self.period_max = kwargs.get("period_max", float("inf"))
+    self.period_min = kwargs.get("period_min", 0)
+    self.n_transits_min = kwargs.get("n_transits_min", tls_constants.N_TRANSITS_MIN)
+
+    self.R_star_min = kwargs.get("R_star_min", tls_constants.R_STAR_MIN)
+    self.R_star_max = kwargs.get("R_star_max", tls_constants.R_STAR_MAX)
+    self.M_star_min = kwargs.get("M_star_min", tls_constants.M_STAR_MIN)
+    self.M_star_max = kwargs.get("M_star_max", tls_constants.M_STAR_MAX)
+    self.duration_grid_step = kwargs.get(
+        "duration_grid_step", tls_constants.DURATION_GRID_STEP
+    )
+
+    self.use_threads = kwargs.get("use_threads", multiprocessing.cpu_count())
+
+    self.per = kwargs.get("per", tls_constants.DEFAULT_PERIOD)
+    self.rp = kwargs.get("rp", tls_constants.DEFAULT_RP)
+    self.a = kwargs.get("a", tls_constants.DEFAULT_A)
+
+    self.T0_fit_margin = kwargs.get("T0_fit_margin", tls_constants.T0_FIT_MARGIN)
+
+    # If an impact parameter is given, it overrules the supplied inclination
+    if "b" in kwargs:
+        self.b = kwargs.get("b")
+        self.inc = impact_to_inclination(b=self.b, semimajor_axis=self.a)
+    else:
+        self.inc = kwargs.get("inc", tls_constants.DEFAULT_INC)
+
+    self.ecc = kwargs.get("ecc", tls_constants.DEFAULT_ECC)
+    self.w = kwargs.get("w", tls_constants.DEFAULT_W)
+    self.u = kwargs.get("u", tls_constants.DEFAULT_U)
+    self.limb_dark = kwargs.get("limb_dark", tls_constants.DEFAULT_LIMB_DARK)
+
+    self.transit_template = kwargs.get("transit_template", "default")
+    if self.transit_template == "default":
+        self.per = tls_constants.DEFAULT_PERIOD
+        self.rp = tls_constants.DEFAULT_RP
+        self.a = tls_constants.DEFAULT_A
+        self.inc = tls_constants.DEFAULT_INC
+
+    elif self.transit_template == "grazing":
+        self.b = tls_constants.GRAZING_B
+        self.inc = impact_to_inclination(b=self.b, semimajor_axis=self.a)
+
+    elif self.transit_template == "box":
+        self.per = tls_constants.BOX_PERIOD
+        self.rp = tls_constants.BOX_RP
+        self.a = tls_constants.BOX_A
+        self.b = tls_constants.BOX_B
+        self.inc = tls_constants.BOX_INC
+        self.u = tls_constants.BOX_U
+        self.limb_dark = tls_constants.BOX_LIMB_DARK
+
+    elif self.transit_template == "tailed":
+        self.per = tls_constants.DEFAULT_PERIOD
+        self.rp = tls_constants.DEFAULT_RP
+        self.a = tls_constants.DEFAULT_A
+        self.inc = tls_constants.DEFAULT_INC
+
+    elif self.transit_template == "custom":
+        custom_transit_template_generator = kwargs.get("transit_template_generator")
+        if not issubclass(type(custom_transit_template_generator), TransitTemplateGenerator):
+            raise ValueError(
+                'The custom transit_template_generator does not implement TransitTemplateGenerator.'
+            )
+        else:
+            self.transit_template_generators["custom"] = custom_transit_template_generator
+
+    else:
+        raise ValueError(
+            'Unknown transit_template. Known values: \
+            "default", "grazing", "box", "tailed"'
+        )
+
+    self.period_grid = kwargs.get("period_grid", None)
+
+    """Validations to avoid (garbage in ==> garbage out)"""
+
+    # Stellar radius
+    # 0 < R_star < inf
+    if self.R_star <= 0 or self.R_star >= float("inf"):
+        raise ValueError("R_star must be positive")
+
+    # Assert (0 < R_star_min <= R_star)
+    if self.R_star_min > self.R_star:
+        raise ValueError("R_star_min <= R_star is required")
+    if self.R_star_min <= 0 or self.R_star_min >= float("inf"):
+        raise ValueError("R_star_min must be positive")
+
+    # Assert (R_star <= R_star_max < inf)
+    if self.R_star_max < self.R_star:
+        raise ValueError("R_star_max >= R_star is required")
+    if self.R_star_max <= 0 or self.R_star_max >= float("inf"):
+        raise ValueError("R_star_max must be positive")
+
+    # Stellar mass
+    # Assert (0 < M_star < inf)
+    if self.M_star <= 0 or self.M_star >= float("inf"):
+        raise ValueError("M_star must be positive")
+
+    # Assert (0 < M_star_min <= M_star)
+    if self.M_star_min > self.M_star:
+        raise ValueError("M_star_min <= M_star is required")
+    if self.M_star_min <= 0 or self.M_star_min >= float("inf"):
+        raise ValueError("M_star_min must be positive")
+
+    # Assert (M_star <= M_star_max < inf)
+    if self.M_star_max < self.M_star:
+        raise ValueError("M_star_max >= M_star required")
+    if self.M_star_max <= 0 or self.M_star_max >= float("inf"):
+        raise ValueError("M_star_max must be positive")
+
+    # Period grid
+    if self.period_min < 0:
+        raise ValueError("period_min >= 0 required")
+    if self.period_min >= self.period_max:
+        raise ValueError("period_min < period_max required")
+    if not isinstance(self.n_transits_min, int):
+        raise ValueError("n_transits_min must be an integer value")
+    if self.n_transits_min < 1:
+        raise ValueError("n_transits_min must be an integer value >= 1")
+
+    if not isinstance(self.use_threads, int) or self.use_threads < 1:
+        raise ValueError("use_threads must be an integer value >= 1")
+
+    # Assert 0 < T0_fit_margin < 0.1
+    if self.T0_fit_margin < 0:
+        self.T0_fit_margin = 0
+    elif self.T0_fit_margin > 0.1:  # Sensible limit 10% of transit duration
+        self.T0_fit_margin = 0.1
+
+    if self.period_grid is not None and not isinstance(self.period_grid, numpy.ndarray):
+        raise ValueError("period_grid must be a `ndarray`")
+    return self, kwargs
```

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/grid.py` & `foldedleastsquares-1.0.41/foldedleastsquares/grid.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/tls_constants.py` & `foldedleastsquares-1.0.41/foldedleastsquares/tls_constants.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/helpers.py` & `foldedleastsquares-1.0.41/foldedleastsquares/helpers.py`

 * *Files identical despite different names*

### Comparing `foldedleastsquares-1.0.39/foldedleastsquares/interpolation.py` & `foldedleastsquares-1.0.41/foldedleastsquares/interpolation.py`

 * *Files identical despite different names*

