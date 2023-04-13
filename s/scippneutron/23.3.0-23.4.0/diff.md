# Comparing `tmp/scippneutron-23.3.0.tar.gz` & `tmp/scippneutron-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scippneutron-23.3.0.tar", last modified: Wed Mar  8 09:43:13 2023, max compression
+gzip compressed data, was "scippneutron-23.4.0.tar", last modified: Thu Apr 13 14:10:41 2023, max compression
```

## Comparing `scippneutron-23.3.0.tar` & `scippneutron-23.4.0.tar`

### file list

```diff
@@ -1,179 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.983565 scippneutron-23.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.943565 scippneutron-23.3.0/.buildconfig/
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.buildconfig/ci-linux.yml
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.buildconfig/ci-macos.yml
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.buildconfig/ci-windows.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.943565 scippneutron-23.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      593 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.943565 scippneutron-23.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.github/workflows/pr_and_main.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4825 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-03-08 09:42:53.000000 scippneutron-23.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-03-08 09:42:53.000000 scippneutron-23.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-03-08 09:43:13.983565 scippneutron-23.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-03-08 09:42:53.000000 scippneutron-23.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.947565 scippneutron-23.3.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-03-08 09:42:53.000000 scippneutron-23.3.0/benchmarks/load_nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-03-08 09:42:53.000000 scippneutron-23.3.0/benchmarks/transform_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.947565 scippneutron-23.3.0/conda/
--rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-03-08 09:42:53.000000 scippneutron-23.3.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.947565 scippneutron-23.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.947565 scippneutron-23.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    18346 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/_static/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)    19908 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/_static/straight-beamline.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.947565 scippneutron-23.3.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/_templates/scipp-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/_templates/scipp-module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.947565 scippneutron-23.3.0/docs/_templates/sections/
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/_templates/sections/header-article.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.951565 scippneutron-23.3.0/docs/about/
--rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/about/about.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/about/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (122)    12919 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/about/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.951565 scippneutron-23.3.0/docs/buildconfig/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/buildconfig/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     9076 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.951565 scippneutron-23.3.0/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/developer/coding-conventions.rst
--rw-r--r--   0 runner    (1001) docker     (122)    16402 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/developer/data-stream.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.951565 scippneutron-23.3.0/docs/developer/data_stream/
--rw-r--r--   0 runner    (1001) docker     (122)    18688 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/developer/data_stream/data_stream_arch.svg
--rw-r--r--   0 runner    (1001) docker     (122)    19463 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/developer/data_stream/data_stream_arch_testing.svg
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/developer/data_stream/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/developer/file-loading.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/developer/getting-started.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.951565 scippneutron-23.3.0/docs/environments/
--rw-r--r--   0 runner    (1001) docker     (122)      392 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/environments/scippneutron.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.951565 scippneutron-23.3.0/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/getting-started/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.951565 scippneutron-23.3.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/images/question.png
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.955565 scippneutron-23.3.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (122)    18499 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/reference/frame-unwrapping.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.955565 scippneutron-23.3.0/docs/reference/frameunwrapping/
--rw-r--r--   0 runner    (1001) docker     (122)     3598 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/reference/frameunwrapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/reference/free-functions.rst
--rw-r--r--   0 runner    (1001) docker     (122)      195 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.955565 scippneutron-23.3.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (122)    15758 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/tutorials/1_exploring-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     9948 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/tutorials/2_working-with-masks.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    35471 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/tutorials/3_understanding-event-data.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/tutorials/powder-diffraction.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/tutorials/strip-solutions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.959565 scippneutron-23.3.0/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (122)    25490 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/user-guide/coordinate-transformations.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    22020 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/user-guide/from-mantid-to-scipp.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/user-guide/groupby.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     6346 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/user-guide/instrument-view.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      387 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/user-guide/make_PG3_4844_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     4342 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/user-guide/recipes.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-03-08 09:42:53.000000 scippneutron-23.3.0/docs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3281 2023-03-08 09:42:53.000000 scippneutron-23.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.963565 scippneutron-23.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     7574 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (122)      888 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      260 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)     8849 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-03-08 09:42:53.000000 scippneutron-23.3.0/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.963565 scippneutron-23.3.0/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-03-08 09:42:53.000000 scippneutron-23.3.0/resources/logo-2022.svg
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-03-08 09:43:13.983565 scippneutron-23.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.939566 scippneutron-23.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.963565 scippneutron-23.3.0/src/scippneutron/
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.967565 scippneutron-23.3.0/src/scippneutron/_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      796 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4726 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/beamline_components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.967565 scippneutron-23.3.0/src/scippneutron/conversion/
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6157 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/conversion/beamline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.967565 scippneutron-23.3.0/src/scippneutron/conversion/graph/
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/conversion/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/conversion/graph/beamline.py
--rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/conversion/graph/tof.py
--rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/conversion/tof.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.967565 scippneutron-23.3.0/src/scippneutron/core/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5680 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/core/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.967565 scippneutron-23.3.0/src/scippneutron/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.971565 scippneutron-23.3.0/src/scippneutron/data_streaming/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13231 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_consumer_type.py
--rw-r--r--   0 runner    (1001) docker     (122)    20569 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_data_buffer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2746 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_data_consumption_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     2339 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_data_stream_widget.py
--rw-r--r--   0 runner    (1001) docker     (122)     2881 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_serialisation.py
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_stop_time.py
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (122)    12837 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/data_streaming/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)    10498 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/instrument_view.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.971565 scippneutron-23.3.0/src/scippneutron/io/
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.971565 scippneutron-23.3.0/src/scippneutron/io/nexus/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/io/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12651 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/io/nexus/_json_nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/io/nexus/_nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)    15940 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/io/nexus/load_nexus.py
--rw-r--r--   0 runner    (1001) docker     (122)     5474 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/io/xye.py
--rw-r--r--   0 runner    (1001) docker     (122)      673 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    45107 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/mantid.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.975565 scippneutron-23.3.0/src/scippneutron/tof/
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/tof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5465 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/tof/diagram.py
--rw-r--r--   0 runner    (1001) docker     (122)     8424 2023-03-08 09:42:53.000000 scippneutron-23.3.0/src/scippneutron/tof/frames.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.963565 scippneutron-23.3.0/src/scippneutron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-03-08 09:43:13.000000 scippneutron-23.3.0/src/scippneutron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-03-08 09:43:13.000000 scippneutron-23.3.0/src/scippneutron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-08 09:43:13.000000 scippneutron-23.3.0/src/scippneutron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-03-08 09:43:13.000000 scippneutron-23.3.0/src/scippneutron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-08 09:43:13.000000 scippneutron-23.3.0/src/scippneutron.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.979565 scippneutron-23.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/HYS_mask.xml
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/beamline_components_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      767 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.979565 scippneutron-23.3.0/tests/conversion/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4596 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/conversion/beamline_conversions_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.979565 scippneutron-23.3.0/tests/conversion/graph/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/conversion/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1910 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/conversion/graph/beamline_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3866 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/conversion/graph/tof_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    18655 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/conversion/tof_conversions_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    27043 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    47570 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/data_stream_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     4320 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/instrument_view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.979565 scippneutron-23.3.0/tests/io/
--rw-r--r--   0 runner    (1001) docker     (122)     8249 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/io/xye_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/load_nexus_json_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    74908 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/load_nexus_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/load_nxdetector_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/mantid_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.979565 scippneutron-23.3.0/tests/mantid_scipp_comparison/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/mantid_scipp_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/mantid_scipp_comparison/beamline_calculations_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/mantid_scipp_comparison/histogram_events_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5497 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    44649 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/mantid_test.py
--rw-r--r--   0 runner    (1001) docker     (122)    33632 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/nexus_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.979565 scippneutron-23.3.0/tests/tof/
--rw-r--r--   0 runner    (1001) docker     (122)    10330 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tests/tof/frames_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-08 09:43:13.983565 scippneutron-23.3.0/tools/
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tools/make_tutorial_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-03-08 09:42:53.000000 scippneutron-23.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.758372 scippneutron-23.4.0/.buildconfig/
+-rw-r--r--   0 runner    (1001) docker     (122)      865 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.buildconfig/ci-linux.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.buildconfig/ci-macos.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.buildconfig/ci-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.758372 scippneutron-23.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      593 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.758372 scippneutron-23.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.github/workflows/pr_and_main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4825 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1745 2023-04-13 14:10:29.000000 scippneutron-23.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1553 2023-04-13 14:10:29.000000 scippneutron-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-04-13 14:10:41.774372 scippneutron-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-04-13 14:10:29.000000 scippneutron-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.758372 scippneutron-23.4.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-13 14:10:29.000000 scippneutron-23.4.0/benchmarks/load_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-13 14:10:29.000000 scippneutron-23.4.0/benchmarks/transform_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.758372 scippneutron-23.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-04-13 14:10:29.000000 scippneutron-23.4.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.758372 scippneutron-23.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.758372 scippneutron-23.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)   137750 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    18346 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/_static/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    19908 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/_static/straight-beamline.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/_templates/scipp-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1217 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/_templates/scipp-module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/_templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (122)     3900 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/_templates/sections/header-article.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/about/about.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/about/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    14012 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/about/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/bibliography.bib
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/bibliography.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/buildconfig/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/buildconfig/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     9459 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/developer/coding-conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    16402 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/developer/data-stream.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/developer/data_stream/
+-rw-r--r--   0 runner    (1001) docker     (122)    18688 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/developer/data_stream/data_stream_arch.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    19463 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/developer/data_stream/data_stream_arch_testing.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/developer/data_stream/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/developer/file-loading.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1979 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/developer/getting-started.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/environments/
+-rw-r--r--   0 runner    (1001) docker     (122)      392 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/environments/scippneutron.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/getting-started/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/images/question.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (122)    18499 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/reference/frame-unwrapping.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/reference/frameunwrapping/
+-rw-r--r--   0 runner    (1001) docker     (122)     3127 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/reference/frameunwrapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/reference/free-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.762372 scippneutron-23.4.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (122)    15758 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/tutorials/1_exploring-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     9948 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/tutorials/2_working-with-masks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    35590 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/tutorials/3_understanding-event-data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    14963 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/tutorials/powder-diffraction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/tutorials/strip-solutions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.766372 scippneutron-23.4.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (122)    25383 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/user-guide/coordinate-transformations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    22024 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/user-guide/from-mantid-to-scipp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/user-guide/groupby.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     6346 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/user-guide/instrument-view.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      387 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/user-guide/make_PG3_4844_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4342 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/user-guide/recipes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     4162 2023-04-13 14:10:29.000000 scippneutron-23.4.0/docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3449 2023-04-13 14:10:29.000000 scippneutron-23.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.766372 scippneutron-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7574 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (122)      888 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-13 14:10:29.000000 scippneutron-23.4.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.766372 scippneutron-23.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    70398 2023-04-13 14:10:29.000000 scippneutron-23.4.0/resources/logo-2022.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-13 14:10:41.774372 scippneutron-23.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.754372 scippneutron-23.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.766372 scippneutron-23.4.0/src/scippneutron/
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.766372 scippneutron-23.4.0/src/scippneutron/_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      796 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4694 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/beamline_components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.766372 scippneutron-23.4.0/src/scippneutron/conversion/
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6070 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/conversion/beamline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.770372 scippneutron-23.4.0/src/scippneutron/conversion/graph/
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/conversion/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/conversion/graph/beamline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6231 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/conversion/graph/tof.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17383 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/conversion/tof.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.770372 scippneutron-23.4.0/src/scippneutron/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5671 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/core/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.770372 scippneutron-23.4.0/src/scippneutron/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.770372 scippneutron-23.4.0/src/scippneutron/data_streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13258 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_consumer_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_data_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2651 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_data_consumption_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_data_stream_widget.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_stop_time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12624 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/data_streaming/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9542 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/instrument_view.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.770372 scippneutron-23.4.0/src/scippneutron/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.770372 scippneutron-23.4.0/src/scippneutron/io/nexus/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/io/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12723 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/io/nexus/_json_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/io/nexus/_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15756 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/io/nexus/load_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5494 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/io/xye.py
+-rw-r--r--   0 runner    (1001) docker     (122)      673 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43196 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/mantid.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.770372 scippneutron-23.4.0/src/scippneutron/tof/
+-rw-r--r--   0 runner    (1001) docker     (122)      335 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/tof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5252 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/tof/diagram.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8161 2023-04-13 14:10:29.000000 scippneutron-23.4.0/src/scippneutron/tof/frames.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.766372 scippneutron-23.4.0/src/scippneutron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4608 2023-04-13 14:10:41.000000 scippneutron-23.4.0/src/scippneutron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4469 2023-04-13 14:10:41.000000 scippneutron-23.4.0/src/scippneutron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 14:10:41.000000 scippneutron-23.4.0/src/scippneutron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-13 14:10:41.000000 scippneutron-23.4.0/src/scippneutron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-13 14:10:41.000000 scippneutron-23.4.0/src/scippneutron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/HYS_mask.xml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/beamline_components_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/tests/conversion/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4186 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/conversion/beamline_conversions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/tests/conversion/graph/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/conversion/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2027 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/conversion/graph/beamline_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/conversion/graph/tof_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21182 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/conversion/tof_conversions_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25109 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44635 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/data_stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/instrument_view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (122)     7915 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/io/xye_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/load_nexus_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    73865 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/load_nexus_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1114 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/load_nxdetector_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/mantid_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/tests/mantid_scipp_comparison/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/mantid_scipp_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/mantid_scipp_comparison/beamline_calculations_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/mantid_scipp_comparison/histogram_events_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5000 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43036 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/mantid_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32558 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/nexus_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/tests/tof/
+-rw-r--r--   0 runner    (1001) docker     (122)     9554 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tests/tof/frames_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 14:10:41.774372 scippneutron-23.4.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tools/make_tutorial_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-13 14:10:29.000000 scippneutron-23.4.0/tox.ini
```

### Comparing `scippneutron-23.3.0/.github/dependabot.yml` & `scippneutron-23.4.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/.github/workflows/pr_and_main.yml` & `scippneutron-23.4.0/.github/workflows/pr_and_main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -66,12 +66,12 @@
           find html -type f -name "*.ipynb" -not -path "html/_sources/*" -delete
         if: ${{ contains(matrix.variant.os, 'ubuntu') && matrix.python-version == '3.8' }}
 
       - run: python -m sphinx -j4 -v -b linkcheck -d doctrees docs html
         # Linkcheck can be flaky. Avoid randomly breaking PR builds by running only on `main`
         if: ${{ contains(matrix.variant.os, 'ubuntu') && matrix.python-version == '3.8' && github.ref == 'refs/heads/main' }}
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         if: ${{ contains(matrix.variant.os, 'ubuntu') && matrix.python-version == '3.8' }}
         with:
           name: DocumentationHTML
           path: html/
```

### Comparing `scippneutron-23.3.0/.github/workflows/release.yml` & `scippneutron-23.4.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     needs: [build_wheels, build_sdist, build_conda]
     runs-on: ubuntu-20.04
     if: github.event_name == 'release' && github.event.action == 'published'
 
     steps:
       - uses: actions/download-artifact@v3
       - uses: actions/setup-python@v3
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
+      - uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
 
   upload_conda:
     name: Deploy Conda Forge
     needs: [build_wheels, build_sdist, build_conda]
```

### Comparing `scippneutron-23.3.0/.gitignore` & `scippneutron-23.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/.pre-commit-config.yaml` & `scippneutron-23.4.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,18 @@
         args: [ --markdown-linebreak-ext=md ]
         exclude: '\.svg'
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
         name: isort (python)
-  - repo: https://github.com/pre-commit/mirrors-yapf
-    rev: v0.32.0
+  - repo: https://github.com/psf/black
+    rev: 23.1.0
     hooks:
-      - id: yapf
-        args: [ "-i", "-r" ]
-        types: [ "python" ]
-        additional_dependencies: [ "toml" ]
+      - id: black
   - repo: https://github.com/kynan/nbstripout
     rev: 0.6.0
     hooks:
       - id: nbstripout
         types: [ "jupyter" ]
         args: [ "--drop-empty-cells",
                 "--extra-keys 'metadata.language_info.version cell.metadata.jp-MarkdownHeadingCollapsed cell.metadata.pycharm'" ]
```

### Comparing `scippneutron-23.3.0/LICENSE` & `scippneutron-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/PKG-INFO` & `scippneutron-23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippneutron
-Version: 23.3.0
+Version: 23.4.0
 Summary:  Neutron scattering tools for Data Reduction
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `scippneutron-23.3.0/README.md` & `scippneutron-23.4.0/README.md`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/benchmarks/transform_coords.py` & `scippneutron-23.4.0/benchmarks/transform_coords.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import scippneutron as scn
 
 ConfigService.setLogLevel(1)
 
 
 class TransformCoords:
-
     def setup(self):
         da = scn.load(scn.data.get_path('PG3_4844_event.nxs'))
         self.var_tof = da
         self.var_wavelength = scn.convert(self.var_tof, "tof", "wavelength", False)
         self.var_energy = scn.convert(self.var_tof, "tof", "energy", False)
 
     def time_wavelength_to_tof(self):
```

### Comparing `scippneutron-23.3.0/conda/meta.yaml` & `scippneutron-23.4.0/conda/meta.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -23,39 +23,39 @@
   path: ..
 
 requirements:
   build:
     - setuptools
     - setuptools_scm
   run:
-    - h5py<3.2  # see https://github.com/h5py/h5py/issues/1880#issuecomment-823223154
+    - h5py
     - numpy>=1.20.0
     - pooch
     - python
-    - scipp>=23.01.1
+    - scipp>=23.03.2
     - scippnexus>=23.03.0
     - scipy>=1.7.0
 
 test:
   imports:
     - scippneutron
   requires:
-    - hypothesis
-    - ipympl
-    - ipywidgets
+    - hypothesis==6.71.0
+    - ipympl==0.9.3
+    - ipywidgets==8.0.6
     - markupsafe>=1.1.1,<2.1.0  # see https://github.com/pallets/markupsafe/issues/284
-    - matplotlib-base
-    - plopp >= 22.12.1
-    - psutil
-    - pytest
-    - pytest-asyncio
-    - pythreejs
-    - mantid==6.5.* [py==38]
-    - python-confluent-kafka [linux64]
-    - ess-streaming-data-types [linux64]
+    - matplotlib-base==3.7.1
+    - plopp==23.04.0
+    - psutil==5.9.4
+    - pytest==7.3.0
+    - pytest-asyncio==0.21.0
+    - pythreejs==2.4.2
+    - mantid==6.6.0 [py==38]
+    - python-confluent-kafka==1.9.2 [linux64]
+    - ess-streaming-data-types==v0.14.0 [linux64]
   source_files:
     - tests/
   commands:
     - python -m pytest
 
 build:
   ignore_run_exports:
```

### Comparing `scippneutron-23.3.0/docs/_static/favicon.ico` & `scippneutron-23.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/_static/logo-2022.svg` & `scippneutron-23.4.0/docs/_static/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/_static/straight-beamline.svg` & `scippneutron-23.4.0/docs/_static/straight-beamline.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/_templates/scipp-class-template.rst` & `scippneutron-23.4.0/docs/_templates/scipp-class-template.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/_templates/scipp-module-template.rst` & `scippneutron-23.4.0/docs/_templates/scipp-module-template.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/_templates/sections/header-article.html` & `scippneutron-23.4.0/docs/_templates/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/about/about.rst` & `scippneutron-23.4.0/docs/about/about.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/about/contributing.rst` & `scippneutron-23.4.0/docs/about/contributing.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/about/release-notes.rst` & `scippneutron-23.4.0/docs/about/release-notes.rst`

 * *Files 5% similar despite different names*

```diff
@@ -30,36 +30,73 @@
    Contributors
    ~~~~~~~~~~~~
 
    Simon Heybrock :sup:`a`\ ,
    Neil Vaytet :sup:`a`\ ,
    and Jan-Lukas Wynen :sup:`a`
 
-v23.03.0
---------
+v23.04.0 (April 2023)
+---------------------
+
+Features
+~~~~~~~~
+
+* Added :func:`scippneutron.conversion.tof.hkl_vec_from_Q_vec` `#427 <https://github.com/scipp/scippneutron/pull/427>`_.
+* Compatible with Mantid=6.6.0 `#424 <https://github.com/scipp/scippneutron/pull/434>`_.
+
+Breaking changes
+~~~~~~~~~~~~~~~~
+
+* Requires Scipp v23.03.2 `#424 <https://github.com/scipp/scippneutron/pull/434>`_.
+
+Bugfixes
+~~~~~~~~
+
+* Conversion from ``mantid.MaskWorkspace`` now correctly sets ``unit=None`` instead of using dimensionless `#424 <https://github.com/scipp/scippneutron/pull/424>`_.
+
+Documentation
+~~~~~~~~~~~~~
+
+Deprecations
+~~~~~~~~~~~~
+
+Stability, Maintainability, and Testing
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+* Switched to black for Python code formatting `#429 <https://github.com/scipp/scippneutron/pull/429>`_.
+
+Contributors
+~~~~~~~~~~~~
+
+Simon Heybrock :sup:`a`\ ,
+Neil Vaytet :sup:`a`\ ,
+and Jan-Lukas Wynen :sup:`a`
+
+v23.03.0 (March 2023)
+---------------------
 
 Breaking Changes
 ~~~~~~~~~~~~~~~~
 
 * Requires ScippNexus v23.03.0
 
 Features
 ~~~~~~~~
 
-* Coordinate transformation kernel for :math:`\vec{Q}` `412 <https://github.com/scipp/scipp/pull/412>`_.
-* Added :func:`scippneutron.io.xye.save_xye` and :func:`scippneutron.io.xye.load_xye` `417 <https://github.com/scipp/scipp/pull/417>`_.
+* Coordinate transformation kernel for :math:`\vec{Q}` `#412 <https://github.com/scipp/scippneutron/pull/412>`_.
+* Added :func:`scippneutron.io.xye.save_xye` and :func:`scippneutron.io.xye.load_xye` `#417 <https://github.com/scipp/scippneutron/pull/417>`_.
 
 v23.01.0 (January 2023)
 -----------------------
 
 Breaking Changes
 ~~~~~~~~~~~~~~~~
 
 * Requires Scipp v23.1.1 and ScippNexus v23.1.1
-* :func:`scippneutron.load_nexus` may now return ``scipp.DataGroup`` objects if parts of the file cannot be read `401 <https://github.com/scipp/scipp/pull/401>`_.
+* :func:`scippneutron.load_nexus` may now return ``scipp.DataGroup`` objects if parts of the file cannot be read `#401 <https://github.com/scipp/scippneutron/pull/401>`_.
 
 v22.12.4 (December 2022)
 ------------------------
 
 Bugfixes
 ~~~~~~~~
 
@@ -68,50 +105,50 @@
 
 v22.12.0 (December 2022)
 ------------------------
 
 Features
 ~~~~~~~~
 
-* ScippNeutron is now available on PyPI `#384 <https://github.com/scipp/scipp/pull/384>`_.
+* ScippNeutron is now available on PyPI `#384 <https://github.com/scipp/scippneutron/pull/384>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* Removed C++ components and CMake package configuration. This only affects users that linked against the C++ part of ScippNeutron `#384 <https://github.com/scipp/scipp/pull/384>`_.
+* Removed C++ components and CMake package configuration. This only affects users that linked against the C++ part of ScippNeutron `#384 <https://github.com/scipp/scippneutron/pull/384>`_.
 
 Stability, Maintainability, and Testing
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-* ScippNeutron no longer depends on a specific version of Scipp`#384 <https://github.com/scipp/scipp/pull/384>`_.
+* ScippNeutron no longer depends on a specific version of Scipp`#384 <https://github.com/scipp/scippneutron/pull/384>`_.
 
 Contributors
 ~~~~~~~~~~~~
 
 Simon Heybrock :sup:`a`\ ,
 Neil Vaytet :sup:`a`\ ,
 and Jan-Lukas Wynen :sup:`a`
 
 v0.11.0 (November 2022)
 -----------------------
 
 Features
 ~~~~~~~~
 
-* The instrument view will now use ``plopp`` if it is the current default for plotting `#378 <https://github.com/scipp/scipp/pull/378>`_.
+* The instrument view will now use ``plopp`` if it is the current default for plotting `#378 <https://github.com/scipp/scippneutron/pull/378>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* The instrument view no longer accepts a dataset as input, only data arrays are supported `#378 <https://github.com/scipp/scipp/pull/378>`_.
+* The instrument view no longer accepts a dataset as input, only data arrays are supported `#378 <https://github.com/scipp/scippneutron/pull/378>`_.
 
 Bugfixes
 ~~~~~~~~
 
-* :func:`scippneutron.load_nexus` now works with scippnexus 0.4.1 `#380 <https://github.com/scipp/scipp/pull/380>`_.
+* :func:`scippneutron.load_nexus` now works with scippnexus 0.4.1 `#380 <https://github.com/scipp/scippneutron/pull/380>`_.
 
 Contributors
 ~~~~~~~~~~~~
 
 Simon Heybrock :sup:`a`\ ,
 Neil Vaytet :sup:`a`\ ,
 and Jan-Lukas Wynen :sup:`a`
@@ -148,24 +185,24 @@
 
 v0.9.3 (September 2022)
 -----------------------
 
 Features
 ~~~~~~~~
 
-* Update for compatibility with scippnexus v0.3 `#370 <https://github.com/scipp/scipp/pull/370>`_.
+* Update for compatibility with scippnexus v0.3 `#370 <https://github.com/scipp/scippneutron/pull/370>`_.
 
 
 v0.9.2 (August 2022)
 --------------------
 
 Features
 ~~~~~~~~
 
-* Made compatible with scippnexus v0.2 `#369 <https://github.com/scipp/scipp/pull/369>`_.
+* Made compatible with scippnexus v0.2 `#369 <https://github.com/scipp/scippneutron/pull/369>`_.
 
 Contributors
 ~~~~~~~~~~~~
 
 Simon Heybrock :sup:`a`\ ,
 Neil Vaytet :sup:`a`\ ,
 and Jan-Lukas Wynen :sup:`a`
@@ -187,26 +224,26 @@
 
 v0.9.0 (August 2022)
 --------------------
 
 Features
 ~~~~~~~~
 
-* Kernels for coordinate transformations are now public in :mod:`scippneutron.conversion` `#361 <https://github.com/scipp/scipp/pull/361>`_.
+* Kernels for coordinate transformations are now public in :mod:`scippneutron.conversion` `#361 <https://github.com/scipp/scippneutron/pull/361>`_.
 
 Bugfixes
 ~~~~~~~~
 
-* Fixed ``dspacing_from_wavelength``, results used to be wrong by a factor of ``10**10`` `#361 <https://github.com/scipp/scipp/pull/361>`_.
-* ``two_theta`` as used by coordinate transformations now uses a numerically more stable implementation, the old one had an error of up to ``10**-6`` for small angles `#361 <https://github.com/scipp/scipp/pull/361>`_.
+* Fixed ``dspacing_from_wavelength``, results used to be wrong by a factor of ``10**10`` `#361 <https://github.com/scipp/scippneutron/pull/361>`_.
+* ``two_theta`` as used by coordinate transformations now uses a numerically more stable implementation, the old one had an error of up to ``10**-6`` for small angles `#361 <https://github.com/scipp/scippneutron/pull/361>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* ``scippneutron.tof.conversions`` has been split into :mod:`scippneutron.conversion.graph.beamline` and :mod:`scippneutron.conversion.graph.tof` `#361 <https://github.com/scipp/scipp/pull/361>`_.
+* ``scippneutron.tof.conversions`` has been split into :mod:`scippneutron.conversion.graph.beamline` and :mod:`scippneutron.conversion.graph.tof` `#361 <https://github.com/scipp/scippneutron/pull/361>`_.
 * Switched to scipp 0.16.1
 
 Contributors
 ~~~~~~~~~~~~
 
 Simon Heybrock :sup:`a`\ ,
 Neil Vaytet :sup:`a`\ ,
@@ -249,15 +286,15 @@
 
 v0.6.0 (May 2022)
 -----------------
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* Remove accidental dependency on Mantid. Users now have to install Mantid themselves if they need it `#332 <https://github.com/scipp/scipp/pull/332>`_.
+* Remove accidental dependency on Mantid. Users now have to install Mantid themselves if they need it `#332 <https://github.com/scipp/scippneutron/pull/332>`_.
 * Removed module ``scippneutron.nexus`` in favor of `scippnexus <https://scipp.github.io/scippnexus/>`_ to implement :func:`scippneutron.load_nexus`.
 
 Bugfixes
 ~~~~~~~~
 
 * Fixed loading event data for monitors that is stored in a separate NeXus group.
 
@@ -331,20 +368,20 @@
 
 v0.4.0 (October 2021)
 ---------------------
 
 Features
 ~~~~~~~~
 
-* Add ``tof.conversions`` module with building blocks for custom coordinate transformation graphs `#187 <https://github.com/scipp/scipp/pull/187>`_.
+* Add ``tof.conversions`` module with building blocks for custom coordinate transformation graphs `#187 <https://github.com/scipp/scippneutron/pull/187>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
-* Changed behavior of ``convert`` `#162 <https://github.com/scipp/scipp/pull/162>`_.
+* Changed behavior of ``convert`` `#162 <https://github.com/scipp/scippneutron/pull/162>`_.
 
   * It is no longer possible to convert *to* time-of-flight.
   * To compensate, it is now possible to convert between wavelength, energy, and d-spacing directly.
   * Some input coords which used to be preserved are now turned into attributes.
     See `Coordinate transformations <https://scipp.github.io/user-guide/coordinate-transformations.html>`_ in scipp for details.
   * The ``out`` argument is no longer supported.
 
@@ -418,15 +455,15 @@
 Features
 ~~~~~~~~
 
 * Functionality from ``scipp.neutron`` (as previously known as part of the scipp package) is now available in this package.
   This includes in particular the instrument view and "unit conversions" for time-of-flight neutron sources.
 * Convert supports a greatly enhanced way of obtaining required parameters of the beamline.
   Instead of requiring raw component positions it can now work directly with, e.g., ``two_theta``.
-* Add scipp ``datetime64`` support in mantid-scipp converters `#39 <https://github.com/scipp/scipp/pull/39>`_.
+* Add scipp ``datetime64`` support in mantid-scipp converters `#39 <https://github.com/scipp/scippneutron/pull/39>`_.
 
 Breaking changes
 ~~~~~~~~~~~~~~~~
 
 * ``scipp.neutron.diffraction`` is NOT available in ``scippneutron`` since its original content is facility-specific and does not comply with the inclusion guidelines in this librarary.
 * Naming convention for (in particular) coords and attrs used by unit conversion has changed.
   Generally what previously used hyphens ``-`` now uses underscore ``_``.
```

### Comparing `scippneutron-23.3.0/docs/conf.py` & `scippneutron-23.4.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,42 +34,39 @@
     base = "https://scipp.github.io"
     l1 = []
     l1.append({"type": "link", "text": "scipp", "url": f"{base}"})
     l1.append({"type": "link", "text": "scippnexus", "url": f"{base}/scippnexus"})
     l1.append({"type": "link", "text": "scippneutron", "url": f"{base}/scippneutron"})
     l1.append({"type": "link", "text": "ess", "url": f"{base}/ess"})
     header_buttons = context["header_buttons"]
-    header_buttons.append({
-        "type": "group",
-        "buttons": l1,
-        "icon": "fa fa-caret-down",
-        "text": "Related projects"
-    })
+    header_buttons.append(
+        {
+            "type": "group",
+            "buttons": l1,
+            "icon": "fa fa-caret-down",
+            "text": "Related projects",
+        }
+    )
     releases = version_info.minor_releases(first='0.4')
     if outdated:
         current = f"{long_version} (outdated)"
         latest = "latest"
         entries = ['.'.join(long_version.split('.')[:2])]
     else:
         current = f"{long_version} (latest)"
         latest = f"{releases[0]} (latest)"
         entries = releases[1:]
     lines = [{"type": "link", "text": latest, "url": f"{base}/{project}"}]
     for r in entries:
-        lines.append({
-            "type": "link",
-            "text": f"{r}",
-            "url": f"{base}/{project}/release/{r}"
-        })
-    header_buttons.append({
-        "type": "group",
-        "buttons": lines,
-        "icon": "fa fa-caret-down",
-        "text": current
-    })
+        lines.append(
+            {"type": "link", "text": f"{r}", "url": f"{base}/{project}/release/{r}"}
+        )
+    header_buttons.append(
+        {"type": "group", "buttons": lines, "icon": "fa fa-caret-down", "text": current}
+    )
 
 
 sphinx_book_theme.add_launch_buttons = add_buttons
 
 html_show_sourcelink = True
 
 # -- General configuration ------------------------------------------------
@@ -78,19 +75,26 @@
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc', 'sphinx.ext.autosummary', 'sphinx.ext.doctest',
-    'sphinx.ext.intersphinx', 'sphinx.ext.mathjax', 'sphinx.ext.napoleon',
-    'sphinx_autodoc_typehints', 'sphinx_copybutton',
+    'sphinx.ext.autodoc',
+    'sphinx.ext.autosummary',
+    'sphinx.ext.doctest',
+    'sphinx.ext.intersphinx',
+    'sphinx.ext.mathjax',
+    'sphinx.ext.napoleon',
+    'sphinx_autodoc_typehints',
+    'sphinx_copybutton',
+    'sphinxcontrib.bibtex',
     'IPython.sphinxext.ipython_directive',
-    'IPython.sphinxext.ipython_console_highlighting', 'nbsphinx'
+    'IPython.sphinxext.ipython_console_highlighting',
+    'nbsphinx',
 ]
 
 autodoc_type_aliases = {
     'DTypeLike': 'DTypeLike',
     'VariableLike': 'VariableLike',
     'MetaDataMap': 'MetaDataMap',
     'array_like': 'array_like',
@@ -102,15 +106,15 @@
 """  # noqa: E501
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://docs.scipy.org/doc/numpy/', None),
     'scipp': ('https://scipp.github.io/', None),
     'scipy': ('https://docs.scipy.org/doc/scipy/', None),
-    'xarray': ('https://xarray.pydata.org/en/stable/', None)
+    'xarray': ('https://xarray.pydata.org/en/stable/', None),
 }
 
 # autodocs includes everything, even irrelevant API internals. autosummary
 # looks more suitable in the long run when the API grows.
 # For a nice example see how xarray handles its API documentation.
 autosummary_generate = True
 
@@ -189,15 +193,16 @@
 }
 
 if outdated:
     html_theme_options["announcement"] = (
         f"⚠️ You are viewing the documentation for an old version of {project}. "
         f"Switch to <a href='https://scipp.github.io/{project}' "
         "style='color:white;text-decoration:underline;'"
-        ">latest</a> version. ⚠️")
+        ">latest</a> version. ⚠️"
+    )
 
 html_logo = "_static/logo-2022.svg"
 html_favicon = "_static/favicon.ico"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
@@ -212,32 +217,44 @@
 
 latex_elements = {}
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'scippneutron.tex', u'scippneutron Documentation', u'Simon Heybrock',
-     'manual'),
+    (
+        master_doc,
+        'scippneutron.tex',
+        u'scippneutron Documentation',
+        u'Simon Heybrock',
+        'manual',
+    ),
 ]
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [(master_doc, 'scippneutron', u'scippneutron Documentation', [author], 1)]
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'scippneutron', u'scippneutron Documentation', author, 'scippneutron',
-     'One line description of project.', 'Miscellaneous'),
+    (
+        master_doc,
+        'scippneutron',
+        u'scippneutron Documentation',
+        author,
+        'scippneutron',
+        'One line description of project.',
+        'Miscellaneous',
+    ),
 ]
 
 # -- Options for Matplotlib in notebooks ----------------------------------
 
 nbsphinx_execute_arguments = [
     "--Session.metadata=scipp_sphinx_build=True",
 ]
@@ -247,25 +264,34 @@
 doctest_global_setup = '''
 import numpy as np
 import scipp as sc
 '''
 
 # Using normalize whitespace because many __str__ functions in scipp produce
 # extraneous empty lines and it would look strange to include them in the docs.
-doctest_default_flags = doctest.ELLIPSIS | doctest.IGNORE_EXCEPTION_DETAIL | \
-                        doctest.DONT_ACCEPT_TRUE_FOR_1 | \
-                        doctest.NORMALIZE_WHITESPACE
+doctest_default_flags = (
+    doctest.ELLIPSIS
+    | doctest.IGNORE_EXCEPTION_DETAIL
+    | doctest.DONT_ACCEPT_TRUE_FOR_1
+    | doctest.NORMALIZE_WHITESPACE
+)
 
 # -- Options for linkcheck ------------------------------------------------
 
 linkcheck_ignore = [
     # Specific lines in GitHub blobs cannot be found by linkcheck.
     r'https?://github\.com/.*?/blob/[a-f0-9]+/.+?#',
     # Anchors in README's on GitHub cannot be found by linkcheck.
     r'https?://github\.com/[^/]+/[^/]+\#',
     # Many links for PRs from our release notes. Slow and unlikely to cause issues.
     'https://github.com/scipp/scipp/pull/[0-9]+',
+    # This returns '403 Forbidden' but the link works in a browser.
+    'https://opensource.org/licenses/BSD-3-Clause',
 ]
 
 # Set env variable to enable plopp
 docs_dir = pathlib.Path(__file__).parent.absolute()
 os.environ["SCIPPDIR"] = os.path.join(docs_dir, 'buildconfig')
+
+# -- Options for bibtex ---------------------------------------------------
+bibtex_bibfiles = ["bibliography.bib"]
+bibtex_reference_style = "label"
```

### Comparing `scippneutron-23.3.0/docs/developer/data-stream.rst` & `scippneutron-23.4.0/docs/developer/data-stream.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/developer/data_stream/data_stream_arch.svg` & `scippneutron-23.4.0/docs/developer/data_stream/data_stream_arch.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/developer/data_stream/data_stream_arch_testing.svg` & `scippneutron-23.4.0/docs/developer/data_stream/data_stream_arch_testing.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/developer/data_stream/docker-compose.yml` & `scippneutron-23.4.0/docs/developer/data_stream/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/developer/file-loading.rst` & `scippneutron-23.4.0/docs/developer/file-loading.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/developer/getting-started.rst` & `scippneutron-23.4.0/docs/developer/getting-started.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/getting-started/installation.rst` & `scippneutron-23.4.0/docs/getting-started/installation.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/images/question.png` & `scippneutron-23.4.0/docs/images/question.png`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/index.rst` & `scippneutron-23.4.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,7 +73,8 @@
 .. toctree::
    :caption: About
    :maxdepth: 3
 
    about/about
    about/contributing
    about/release-notes
+   bibliography
```

### Comparing `scippneutron-23.3.0/docs/reference/frame-unwrapping.ipynb` & `scippneutron-23.4.0/docs/reference/frame-unwrapping.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/reference/frameunwrapping/__init__.py` & `scippneutron-23.4.0/docs/reference/frameunwrapping/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,92 +5,96 @@
 import scipp as sc
 
 from scippneutron.tof import TimeDistanceDiagram
 
 
 def default_frame_diagram(tmax=None):
     fig, ax = plt.subplots(1, 1)
-    diagram = TimeDistanceDiagram(ax,
-                                  tmax=300 * sc.Unit('ms') if tmax is None else tmax)
+    diagram = TimeDistanceDiagram(
+        ax, tmax=300 * sc.Unit('ms') if tmax is None else tmax
+    )
     det1 = 32.0 * sc.Unit('m')
     det2 = 40.0 * sc.Unit('m')
     lambda_min = 16.0 * sc.units.angstrom
     frame_offset = diagram.to_time(6.0 * sc.Unit('ms'))
     diagram.add_source_pulse(15 * sc.Unit('ms'))
     diagram.add_sample(distance=20.0 * sc.Unit('m'))
     diagram.add_detector(distance=det1, name='detector1')
     diagram.add_detector(distance=det2, name='detector2')
-    diagram.add_neutrons(Lmax=1.05 * det2,
-                         lambda_min=lambda_min,
-                         time_offset=frame_offset)
-    diagram.add_neutron(L=det1,
-                        time_offset=frame_offset,
-                        wavelength=20.0 * sc.units.angstrom,
-                        label=r'$T_0^{i+1}+\Delta t$')
+    diagram.add_neutrons(
+        Lmax=1.05 * det2, lambda_min=lambda_min, time_offset=frame_offset
+    )
+    diagram.add_neutron(
+        L=det1,
+        time_offset=frame_offset,
+        wavelength=20.0 * sc.units.angstrom,
+        label=r'$T_0^{i+1}+\Delta t$',
+    )
 
     props = dict(arrowstyle='-|>')
     x0 = diagram.frame_length
     x1 = diagram.frame_length + frame_offset
     m = sc.Unit('m')
     ms = sc.Unit('ms')
-    diagram.annotate(r'$T_0^i$',
-                     xy=(x0, 0 * m),
-                     xytext=(x0 - 20 * ms, 3 * m),
-                     arrowprops=props)
-    diagram.annotate(r'$T_0^i+\Delta T_0$',
-                     xy=(x1, 0 * m),
-                     xytext=(x1 - 20 * ms, 5 * m),
-                     arrowprops=props)
-    diagram.annotate(r'$T_0^{i+1}+t_{\mathrm{pivot}}(\mathrm{det1})$',
-                     xy=(205 * ms, det1),
-                     xytext=(150 * ms, 10 * m),
-                     arrowprops=props)
-    diagram.annotate(r'$T_0^{i+2}+t_{\mathrm{pivot}}(\mathrm{det2})$',
-                     xy=(235 * ms, det2),
-                     xytext=(220 * ms, 15 * m),
-                     arrowprops=props)
+    diagram.annotate(
+        r'$T_0^i$', xy=(x0, 0 * m), xytext=(x0 - 20 * ms, 3 * m), arrowprops=props
+    )
+    diagram.annotate(
+        r'$T_0^i+\Delta T_0$',
+        xy=(x1, 0 * m),
+        xytext=(x1 - 20 * ms, 5 * m),
+        arrowprops=props,
+    )
+    diagram.annotate(
+        r'$T_0^{i+1}+t_{\mathrm{pivot}}(\mathrm{det1})$',
+        xy=(205 * ms, det1),
+        xytext=(150 * ms, 10 * m),
+        arrowprops=props,
+    )
+    diagram.annotate(
+        r'$T_0^{i+2}+t_{\mathrm{pivot}}(\mathrm{det2})$',
+        xy=(235 * ms, det2),
+        xytext=(220 * ms, 15 * m),
+        arrowprops=props,
+    )
 
     # Pivot line
-    diagram.add_neutron(time_offset=x1,
-                        L=1.1 * det2,
-                        wavelength=lambda_min,
-                        color='black',
-                        ls='dashed')
+    diagram.add_neutron(
+        time_offset=x1, L=1.1 * det2, wavelength=lambda_min, color='black', ls='dashed'
+    )
 
     L = diagram.frame_length.value
     ax.axvspan(2 * L, 3 * L, facecolor='grey', alpha=0.2)
 
     return fig
 
 
 def frame_skipping_diagram(tmax=None):
     fig, ax = plt.subplots(1, 1)
-    diagram = TimeDistanceDiagram(ax,
-                                  tmax=500 * sc.Unit('ms') if tmax is None else tmax)
+    diagram = TimeDistanceDiagram(
+        ax, tmax=500 * sc.Unit('ms') if tmax is None else tmax
+    )
     det1 = 32.0 * sc.Unit('m')
     det2 = 40.0 * sc.Unit('m')
     lambda_min = 16.0 * sc.units.angstrom
     frame_offset = diagram.to_time(1.5 * sc.Unit('ms'))
     diagram.add_source_pulse()
     diagram.add_sample(distance=20.0 * sc.Unit('m'))
     diagram.add_detector(distance=det1, name='detector1')
     diagram.add_detector(distance=det2, name='detector2')
-    diagram.add_neutrons(Lmax=1.05 * det2,
-                         lambda_min=lambda_min,
-                         time_offset=frame_offset,
-                         stride=2)
+    diagram.add_neutrons(
+        Lmax=1.05 * det2, lambda_min=lambda_min, time_offset=frame_offset, stride=2
+    )
 
     props = dict(arrowstyle='-|>')
     x0 = 2 * diagram.frame_length
     x1 = 2 * diagram.frame_length + frame_offset
     m = sc.Unit('m')
     ms = sc.Unit('ms')
-    diagram.annotate(r'$T_0^i$',
-                     xy=(x0, 0 * m),
-                     xytext=(x0 - 20 * ms, 3 * m),
-                     arrowprops=props)
-    diagram.annotate(r'$T_0^i+\Delta T_0$',
-                     xy=(x1, 0 * m),
-                     xytext=(x1, 5 * m),
-                     arrowprops=props)
+    diagram.annotate(
+        r'$T_0^i$', xy=(x0, 0 * m), xytext=(x0 - 20 * ms, 3 * m), arrowprops=props
+    )
+    diagram.annotate(
+        r'$T_0^i+\Delta T_0$', xy=(x1, 0 * m), xytext=(x1, 5 * m), arrowprops=props
+    )
 
     return fig
```

### Comparing `scippneutron-23.3.0/docs/reference/free-functions.rst` & `scippneutron-23.4.0/docs/reference/free-functions.rst`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/tutorials/1_exploring-data.ipynb` & `scippneutron-23.4.0/docs/tutorials/1_exploring-data.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/tutorials/2_working-with-masks.ipynb` & `scippneutron-23.4.0/docs/tutorials/2_working-with-masks.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/tutorials/3_understanding-event-data.ipynb` & `scippneutron-23.4.0/docs/tutorials/3_understanding-event-data.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995958994708994%*

 * *Differences: {"'cells'": '{29: {\'source\': {insert: [(4, \'sc.plot(\\n\'), (5, \'    {\\n\'), (6, "        '*

 * *            '\'original\': da[\'spectrum\', 8050].hist(tof=100),\\n"), (7, "        '*

 * *            '\'prompt_mask\': spec1.hist(tof=100),\\n"), (8, \'    },\\n\'), (9, \'    '*

 * *            "errorbars=False,\\n'), (10, ')')], delete: [6, 5, 4]}}, 56: {'source': {insert: [(4, "*

 * *            '\'pp.slicer(\\n\'), (5, "    binned_da.transpose([\'pulse_time\', \'spectrum\', '*

 * *            '\'tof\']).hist(spectrum=500, tof […]*

```diff
@@ -395,17 +395,21 @@
             },
             "outputs": [],
             "source": [
                 "spec1 = da['spectrum', 8050].copy()  # copy since we do some modifications below\n",
                 "event_tof = spec.bins.coords['tof']\n",
                 "mask = (prompt_start <= event_tof) & (event_tof < prompt_stop)\n",
                 "spec1.bins.masks['prompt_pulse'] = mask\n",
-                "sc.plot({'original': da['spectrum', 8050].hist(tof=100),\n",
-                "         'prompt_mask': spec1.hist(tof=100)},\n",
-                "        errorbars=False)"
+                "sc.plot(\n",
+                "    {\n",
+                "        'original': da['spectrum', 8050].hist(tof=100),\n",
+                "        'prompt_mask': spec1.hist(tof=100),\n",
+                "    },\n",
+                "    errorbars=False,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8b085b0c-2d88-4129-b9c0-62097cdd6ee9",
             "metadata": {},
             "source": [
@@ -805,15 +809,17 @@
             },
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
                 "binned_da = da.bin(tof=prompt_tof_edges, pulse_time=pulse_time_edges)\n",
                 "binned_da.masks['prompt_pulse'] = prompt_mask\n",
                 "binned_da.masks['bad_beam'] = pulse_time_mask\n",
-                "pp.slicer(binned_da.transpose(['pulse_time', 'spectrum', 'tof']).hist(spectrum=500, tof=400))"
+                "pp.slicer(\n",
+                "    binned_da.transpose(['pulse_time', 'spectrum', 'tof']).hist(spectrum=500, tof=400)\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3817845c-75dd-475b-8127-5dd0528b9119",
             "metadata": {},
             "source": [
@@ -846,15 +852,19 @@
             "execution_count": null,
             "id": "d84ee5c8-ee60-48a0-82ba-834060f89dad",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "pp.slicer(da_dspacing.transpose(['pulse_time', 'spectrum', 'dspacing']).hist(spectrum=500, dspacing=400))"
+                "pp.slicer(\n",
+                "    da_dspacing.transpose(['pulse_time', 'spectrum', 'dspacing']).hist(\n",
+                "        spectrum=500, dspacing=400\n",
+                "    )\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "dc5dadaa-0122-420d-867b-8abbb85a5633",
             "metadata": {},
             "source": [
@@ -980,17 +990,17 @@
                 "two_theta_cut = sc.linspace(dim='two_theta', unit='rad', start=0.4, stop=1.0, num=2)\n",
                 "# Do not use many bins, fewer is better for performance\n",
                 "dspacing_cut = sc.linspace(dim='dspacing', unit='Angstrom', start=0.0, stop=2.0, num=2)\n",
                 "pulse_time_cut = tmin + sc.to_unit(\n",
                 "    sc.array(dims=['pulse_time'], unit='s', values=[0, 10 * 60]), 'ns'\n",
                 ")\n",
                 "\n",
-                "cut = da_dspacing.bin(two_theta=two_theta_cut,\n",
-                "                      dspacing=dspacing_cut,\n",
-                "                      pulse_time=pulse_time_cut)\n",
+                "cut = da_dspacing.bin(\n",
+                "    two_theta=two_theta_cut, dspacing=dspacing_cut, pulse_time=pulse_time_cut\n",
+                ")\n",
                 "cut"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4f373177-b23f-497d-8319-933a554ce770",
             "metadata": {},
@@ -1049,15 +1059,17 @@
             "outputs": [],
             "source": [
                 "two_theta_cut = sc.linspace(dim='two_theta', unit='rad', start=0.4, stop=1.0, num=101)\n",
                 "dspacing_cut = sc.linspace(dim='dspacing', unit='Angstrom', start=0.0, stop=2.0, num=2)\n",
                 "pulse_time_cut = tmin + sc.array(dims=['pulse_time'], unit='s', values=[0, 10 * 60]).to(\n",
                 "    unit='ns'\n",
                 ")\n",
-                "cut = da_dspacing.bin(two_theta=two_theta_cut, dspacing=dspacing_cut, pulse_time=pulse_time_cut)\n",
+                "cut = da_dspacing.bin(\n",
+                "    two_theta=two_theta_cut, dspacing=dspacing_cut, pulse_time=pulse_time_cut\n",
+                ")\n",
                 "cut = cut['pulse_time', 0]  # squeeze pulse time (dim of length 1)\n",
                 "dspacing_edges = sc.linspace(\n",
                 "    dim='dspacing', unit='Angstrom', start=0.0, stop=2.0, num=1000\n",
                 ")\n",
                 "cut = cut.hist(dspacing=dspacing_edges)\n",
                 "cut.plot()"
             ]
```

### Comparing `scippneutron-23.3.0/docs/tutorials/powder-diffraction.ipynb` & `scippneutron-23.4.0/docs/tutorials/powder-diffraction.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/tutorials/strip-solutions.py` & `scippneutron-23.4.0/docs/tutorials/strip-solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import argparse
 import os
 
 from nbconvert.exporters import NotebookExporter
 from traitlets.config import Config
 
 c = Config()
-c.TagRemovePreprocessor.remove_cell_tags = ("solution", )
+c.TagRemovePreprocessor.remove_cell_tags = ("solution",)
 c.TagRemovePreprocessor.enabled = True
 c.NotebookExporter.preprocessors = ["nbconvert.preprocessors.TagRemovePreprocessor"]
 
 parser = argparse.ArgumentParser(
-    description='Strip cells tagged with "solution" from notebooks.')
-parser.add_argument('names',
-                    metavar='input_path',
-                    type=str,
-                    nargs='+',
-                    help='Paths of notebooks to convert.')
+    description='Strip cells tagged with "solution" from notebooks.'
+)
+parser.add_argument(
+    'names',
+    metavar='input_path',
+    type=str,
+    nargs='+',
+    help='Paths of notebooks to convert.',
+)
 parser.add_argument('--output-dir', dest='path', help='Output folder')
 
 args = parser.parse_args()
 
 for name in args.names:
     print(f"Stripping solution cells from {name}")
     output = NotebookExporter(config=c).from_filename(name)
```

### Comparing `scippneutron-23.3.0/docs/user-guide/coordinate-transformations.ipynb` & `scippneutron-23.4.0/docs/user-guide/coordinate-transformations.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999426615884449%*

 * *Differences: {"'cells'": "{20: {'source': {insert: [(13, '    drop = g * m_n**2 / (2 * h**2) * wavelength**2 * "*

 * *            "L2**2\\n'), (14, '    return sc.asin(sc.sqrt(x**2 + (y + drop) ** 2) / L2)')], "*

 * *            "delete: [14, 13]}}, 22: {'source': {insert: [(2, 'q_with_gravity = "*

 * *            '{**graph.beamline.beamline(scatter=True), **graph.tof.elastic_Q("tof")}\\n\')], '*

 * *            "delete: [3, 2]}}, 30: {'source': {insert: [(10, 'plane_graph = "*

 * *            '{**graph.beamline.incident_beam(), **graph.tof.kin […]*

```diff
@@ -334,16 +334,16 @@
                 "    g = sc.norm(gravity)\n",
                 "    L2 = sc.norm(scattered_beam)\n",
                 "    y = sc.dot(scattered_beam, gravity) / g\n",
                 "    n = sc.cross(incident_beam, gravity)\n",
                 "    n /= sc.norm(n)\n",
                 "    x = sc.dot(scattered_beam, n)\n",
                 "    wavelength = sc.to_unit(wavelength, \"m\", copy=False)\n",
-                "    drop = g * m_n ** 2 / (2 * h ** 2) * wavelength ** 2 * L2 ** 2\n",
-                "    return sc.asin(sc.sqrt(x ** 2 + (y + drop) ** 2) / L2)"
+                "    drop = g * m_n**2 / (2 * h**2) * wavelength**2 * L2**2\n",
+                "    return sc.asin(sc.sqrt(x**2 + (y + drop) ** 2) / L2)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b30dd7f6-c3a3-443b-a75a-bd163e12ee98",
             "metadata": {},
             "source": [
@@ -355,16 +355,15 @@
             "execution_count": null,
             "id": "89432215-81d0-4316-aa6c-d801a6005f18",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scippneutron.conversion import graph\n",
                 "\n",
-                "q_with_gravity = {**graph.beamline.beamline(scatter=True),\n",
-                "                  **graph.tof.elastic_Q(\"tof\")}\n",
+                "q_with_gravity = {**graph.beamline.beamline(scatter=True), **graph.tof.elastic_Q(\"tof\")}\n",
                 "q_with_gravity[\"two_theta\"] = two_theta"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a1ea05c6-a74c-4bf3-a239-4ff91fcecc8b",
             "metadata": {},
@@ -459,16 +458,15 @@
                 "\n",
                 "def Ltotal(incident_beam, source_position, position):\n",
                 "    n = incident_beam / sc.norm(incident_beam)\n",
                 "    projected = sc.dot(position, n) * n\n",
                 "    return sc.norm(sc.mean(projected) - source_position)\n",
                 "\n",
                 "\n",
-                "plane_graph = {**graph.beamline.incident_beam(),\n",
-                "               **graph.tof.kinematic(\"tof\")}\n",
+                "plane_graph = {**graph.beamline.incident_beam(), **graph.tof.kinematic(\"tof\")}\n",
                 "plane_graph[\"Ltotal\"] = Ltotal\n",
                 "sc.show_graph(plane_graph, simplified=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e813e8c2-1709-49b4-8f77-a002e35cc877",
@@ -586,15 +584,15 @@
             "id": "aed7624e-09fb-47ff-87ab-e3c7a3339bf5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def dspacing_perpendicular(wavelength, two_theta):\n",
                 "    lambda_K = sc.scalar(1.0, unit=\"angstrom\")\n",
                 "    return sc.sqrt(\n",
-                "        wavelength ** 2 - 2 * (lambda_K ** 2) * sc.log(sc.cos(0.5 * two_theta))\n",
+                "        wavelength**2 - 2 * (lambda_K**2) * sc.log(sc.cos(0.5 * two_theta))\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "573c7976-f205-4a15-b356-649701204364",
             "metadata": {},
@@ -607,16 +605,15 @@
             "execution_count": null,
             "id": "aeb8608f-c93a-44ba-ae2a-86d8c8e5ba10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scippneutron.conversion import graph\n",
                 "\n",
-                "graph = {**graph.beamline.beamline(scatter=True),\n",
-                "         **graph.tof.elastic(\"tof\")}\n",
+                "graph = {**graph.beamline.beamline(scatter=True), **graph.tof.elastic(\"tof\")}\n",
                 "graph[\"d\"] = \"dspacing\"  # rename to brief name\n",
                 "graph[\"d_perp\"] = dspacing_perpendicular"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ed5e9435-9c18-409d-a537-81c6099ec710",
@@ -673,16 +670,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "577bec91-b9db-4866-8dfa-fbbdfcb61220",
             "metadata": {},
             "outputs": [],
             "source": [
-                "da_d_d_perp.hist(d_perp=100, d=100) \\\n",
-                "           .plot(norm=\"log\")"
+                "da_d_d_perp.hist(d_perp=100, d=100).plot(norm=\"log\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
```

### Comparing `scippneutron-23.3.0/docs/user-guide/from-mantid-to-scipp.ipynb` & `scippneutron-23.4.0/docs/user-guide/from-mantid-to-scipp.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983010385005067%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'a_mantid = mantid.ExtractSpectra(\\n'), (3, '    "*

 * *            "input_point_data, StartWorkspaceIndex=0, EndWorkspaceIndex=10\\n'), (4, ')\\n'), (5, "*

 * *            "'b_mantid = mantid.ExtractSpectra(\\n'), (6, '    input_point_data, "*

 * *            "StartWorkspaceIndex=10, EndWorkspaceIndex=20\\n'), (7, ')\\n')], delete: [3, 2]}}, "*

 * *            '14: {\'source\': {insert: [(1, "    InputWorkspace=input_point_data, '*

 * *            'OutputWorkspace=\'spec\', WorkspaceIndex […]*

```diff
@@ -93,16 +93,20 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "input_bin_edges = mantid.CreateSampleWorkspace()\n",
                 "input_point_data = mantid.ConvertToPointData(input_bin_edges)\n",
-                "a_mantid = mantid.ExtractSpectra(input_point_data, StartWorkspaceIndex=0, EndWorkspaceIndex=10)\n",
-                "b_mantid = mantid.ExtractSpectra(input_point_data, StartWorkspaceIndex=10, EndWorkspaceIndex=20)\n",
+                "a_mantid = mantid.ExtractSpectra(\n",
+                "    input_point_data, StartWorkspaceIndex=0, EndWorkspaceIndex=10\n",
+                ")\n",
+                "b_mantid = mantid.ExtractSpectra(\n",
+                "    input_point_data, StartWorkspaceIndex=10, EndWorkspaceIndex=20\n",
+                ")\n",
                 "a_scipp = scn.from_mantid(a_mantid)\n",
                 "b_scipp = scn.from_mantid(b_mantid)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -186,17 +190,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "spec = mantid.ExtractSingleSpectrum(\n",
-                "    InputWorkspace=input_point_data,\n",
-                "    OutputWorkspace='spec',\n",
-                "    WorkspaceIndex=7)"
+                "    InputWorkspace=input_point_data, OutputWorkspace='spec', WorkspaceIndex=7\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -240,15 +243,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.ExtractSpectra(\n",
                 "    InputWorkspace=input_point_data,\n",
                 "    OutputWorkspace='spectra',\n",
                 "    StartWorkspaceIndex=1,\n",
-                "    EndWorkspaceIndex=4)"
+                "    EndWorkspaceIndex=4,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -313,16 +317,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.AppendSpectra(\n",
-                "    InputWorkspace1=a_mantid,\n",
-                "    InputWorkspace2=b_mantid, OutputWorkspace='combined')"
+                "    InputWorkspace1=a_mantid, InputWorkspace2=b_mantid, OutputWorkspace='combined'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -346,17 +350,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "mantid.ConjoinXRuns(\n",
-                "    InputWorkspaces=['a_mantid','b_mantid'],\n",
-                "    OutputWorkspace='data')"
+                "mantid.ConjoinXRuns(InputWorkspaces=['a_mantid', 'b_mantid'], OutputWorkspace='data')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -381,17 +383,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.ConjoinSpectra(\n",
-                "    InputWorkspaces='a_mantid, b_mantid',\n",
-                "    OutputWorkspace='out',\n",
-                "    WorkspaceIndex=7)"
+                "    InputWorkspaces='a_mantid, b_mantid', OutputWorkspace='out', WorkspaceIndex=7\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -431,17 +432,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "mantid.GroupWorkspaces(\n",
-                "    InputWorkspaces='a_mantid, b_mantid',\n",
-                "    OutputWorkspace='data')"
+                "mantid.GroupWorkspaces(InputWorkspaces='a_mantid, b_mantid', OutputWorkspace='data')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -449,17 +448,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sc.Dataset(data={\n",
-                "    'data1':a_scipp,\n",
-                "    'data2':a_scipp.copy()})"
+                "sc.Dataset(data={'data1': a_scipp, 'data2': a_scipp.copy()})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This requires aligned dimensions (matching coordinates) in all input arrays. \n",
@@ -479,17 +476,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.Rebin(\n",
-                "    InputWorkspace=input_point_data,\n",
-                "    OutputWorkspace='histo',\n",
-                "    Params='0,100,20000')"
+                "    InputWorkspace=input_point_data, OutputWorkspace='histo', Params='0,100,20000'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -521,15 +517,16 @@
             "source": [
                 "event_workspace = mantid.CreateSampleWorkspace(WorkspaceType='Event')\n",
                 "\n",
                 "mantid.Rebin(\n",
                 "    InputWorkspace=event_workspace,\n",
                 "    OutputWorkspace='rebinned_events',\n",
                 "    Params='0,100,20000',\n",
-                "    PreserveEvents=True)"
+                "    PreserveEvents=True,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -594,16 +591,17 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.Rebin(\n",
                 "    InputWorkspace=event_workspace,\n",
                 "    OutputWorkspace='histo',\n",
-                "    Params=[0,100,20000],\n",
-                "    PreserveEvents=False)"
+                "    Params=[0, 100, 20000],\n",
+                "    PreserveEvents=False,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -629,17 +627,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.Rebin(\n",
-                "    InputWorkspace=event_workspace,\n",
-                "    OutputWorkspace='histo',\n",
-                "    Params='2,-0.035,10')"
+                "    InputWorkspace=event_workspace, OutputWorkspace='histo', Params='2,-0.035,10'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -688,17 +685,18 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.Scale(\n",
                 "    InputWorkspace=input_point_data,\n",
-                "    OutputWorkspace=input_point_data, \n",
+                "    OutputWorkspace=input_point_data,\n",
                 "    Factor=7.5,\n",
-                "    Operation=\"Multiply\")"
+                "    Operation=\"Multiply\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -725,17 +723,18 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.Scale(\n",
                 "    InputWorkspace=input_point_data,\n",
-                "    OutputWorkspace='summed', \n",
+                "    OutputWorkspace='summed',\n",
                 "    Factor=7.5,\n",
-                "    Operation=\"Add\")"
+                "    Operation=\"Add\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -765,15 +764,15 @@
             "outputs": [],
             "source": [
                 "a_scipp.data.unit = sc.units.us\n",
                 "try:\n",
                 "    a_scipp += 7.5\n",
                 "except RuntimeError as err:\n",
                 "    print(str(err))\n",
-                "a_scipp += 7.5 * sc.units.us # This is fine now RHS has units"
+                "a_scipp += 7.5 * sc.units.us  # This is fine now RHS has units"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Mantid does not have this safety net."
@@ -790,17 +789,18 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.ScaleX(\n",
                 "    InputWorkspace=input_point_data,\n",
-                "    OutputWorkspace='output', \n",
+                "    OutputWorkspace='output',\n",
                 "    Factor=7.5,\n",
-                "    Operation=\"Multiply\")"
+                "    Operation=\"Multiply\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -828,15 +828,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "mantid.SumSpectra(\n",
                 "    InputWorkspace=input_point_data,\n",
                 "    OutputWorkspace='summed',\n",
                 "    StartWorkspaceIndex=7,\n",
-                "    EndWorkspaceIndex=88)"
+                "    EndWorkspaceIndex=88,\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
@@ -861,15 +862,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "mantid.ConvertUnits(InputWorkspace=input_point_data, OutputWorkspace='dspacing', Target='dSpacing')"
+                "mantid.ConvertUnits(\n",
+                "    InputWorkspace=input_point_data, OutputWorkspace='dspacing', Target='dSpacing'\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Equivalent in scipp:"
```

### Comparing `scippneutron-23.3.0/docs/user-guide/groupby.ipynb` & `scippneutron-23.4.0/docs/user-guide/groupby.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/user-guide/instrument-view.ipynb` & `scippneutron-23.4.0/docs/user-guide/instrument-view.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/user-guide/recipes.ipynb` & `scippneutron-23.4.0/docs/user-guide/recipes.ipynb`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/docs/version.py` & `scippneutron-23.4.0/docs/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     if r.status_code != 200:
         return []
     data = r.json()
     return sorted([parse(e['tag_name']) for e in data if not e['draft']], reverse=True)
 
 
 class VersionInfo:
-
     def __init__(self, repo: str, organization: str = 'scipp'):
         self._releases = _get_releases(repo=repo, organization=organization)
 
     def _to_version(self, version) -> Version:
         if isinstance(version, str):
             try:
                 return parse(version)
@@ -89,23 +88,24 @@
         print(info.target(version))
     return 0
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Process some integers.')
     parser.add_argument('--repo', dest='repo', required=True, help='Repository name')
-    parser.add_argument('--action',
-                        choices=['is-latest', 'is-new', 'get-replaced', 'get-target'],
-                        required=True,
-                        help='Action to perform: Check whether this major or minor '
-                        'release exists or is new (is-latest), check whether this is a '
-                        'new major or minor release (is-new), get the version this is '
-                        'replacing (get-replaced), get the target folder for '
-                        'publishing the docs (get-target). In all cases the '
-                        'patch/micro version is ignored.')
-    parser.add_argument('--version',
-                        dest='version',
-                        required=True,
-                        help='Version the action refers to')
+    parser.add_argument(
+        '--action',
+        choices=['is-latest', 'is-new', 'get-replaced', 'get-target'],
+        required=True,
+        help='Action to perform: Check whether this major or minor '
+        'release exists or is new (is-latest), check whether this is a '
+        'new major or minor release (is-new), get the version this is '
+        'replacing (get-replaced), get the target folder for '
+        'publishing the docs (get-target). In all cases the '
+        'patch/micro version is ignored.',
+    )
+    parser.add_argument(
+        '--version', dest='version', required=True, help='Version the action refers to'
+    )
 
     args = parser.parse_args()
     sys.exit(main(**vars(args)))
```

### Comparing `scippneutron-23.3.0/pyproject.toml` & `scippneutron-23.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = [
     "h5py",
     "numpy>=1.20",
     "pooch",
-    "scipp>=23.01.1",
+    "scipp>=23.03.0",
     "scippnexus>=23.3.0",
     "scipy>=1.7.0",
 ]
 
 [project.optional-dependencies]
 interactive = ["scipp[interactive]"]
 all = ['scipp[all]']
@@ -48,18 +48,20 @@
 # Excluding tests because bandit doesn't like `assert`.
 exclude_dirs = ["docs/conf.py", "tests", "install", "tools", "setup.py"]
 
 [tool.codespell]
 ignore-words-list = "elemt"
 skip = "./.git,./install,./build,./cmake-build*,./.tox,*/*_cache,*/.virtual_documents,*/.ipynb_checkpoints,*.pdf,*.svg"
 
+[tool.black]
+skip-string-normalization = true
+
 [tool.isort]
 skip_gitignore = true
-line_length = 88
-multi_line_output = 2  # for compatibility with yapf
+profile = "black"
 skip_glob = ["src/scippneutron/__init__.py"]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 testpaths = "tests"
 addopts = """
 --strict-config
@@ -73,14 +75,16 @@
   # Comes from pytest_asyncio and is not our fault.
   "ignore:The 'asyncio_mode' default value will change to 'strict' in future:DeprecationWarning",
   'ignore::scipy.optimize._optimize.OptimizeWarning',
   # From flatbuffers
   'ignore:the imp module is deprecated in favour of importlib:DeprecationWarning',
   # from Mantid
   'ignore:distutils Version classes are deprecated. Use packaging.version instead:DeprecationWarning',
+  # from ipywidgets; they are migrating away from ipykernel, this warning should go away
+  'ignore:The `ipykernel.comm.Comm` class has been deprecated.:DeprecationWarning',
   # Plotting related warnings.
   'ignore:\n            Sentinel is not a public part of the traitlets API:DeprecationWarning',
   'ignore:Keyword `trait` is deprecated in traitlets 5.0, use `value_trait` instead:DeprecationWarning',
   'ignore:Keyword `traits` is deprecated in traitlets 5.0, use `per_key_traits` instead:DeprecationWarning',
   # TODO Plotting warnings that need to be addressed
   'ignore:Support for mapping types has been deprecated and will be dropped in a future release:DeprecationWarning',
   'ignore:The get_cmap function will be deprecated in a future version:PendingDeprecationWarning',
```

### Comparing `scippneutron-23.3.0/requirements/base.txt` & `scippneutron-23.4.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/requirements/ci.txt` & `scippneutron-23.4.0/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/requirements/dev.txt` & `scippneutron-23.4.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/requirements/static.txt` & `scippneutron-23.4.0/requirements/static.txt`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/requirements/test.txt` & `scippneutron-23.4.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/resources/logo-2022.svg` & `scippneutron-23.4.0/resources/logo-2022.svg`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/src/scippneutron/_utils/__init__.py` & `scippneutron-23.4.0/src/scippneutron/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/src/scippneutron/beamline_components.py` & `scippneutron-23.4.0/src/scippneutron/beamline_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Union
 
 import scipp as sc
 
 from .conversion import graph
 
 
-def _derived_coord(da: Union[sc.DataArray, sc.Dataset],
-                   name: str,
-                   scatter: bool = True) -> sc.Variable:
+def _derived_coord(
+    da: Union[sc.DataArray, sc.Dataset], name: str, scatter: bool = True
+) -> sc.Variable:
     tmp = da.transform_coords(
         name,
         graph=graph.beamline.beamline(scatter=scatter),
         rename_dims=False,
         keep_aliases=False,
         keep_inputs=False,
         keep_intermediate=False,
```

### Comparing `scippneutron-23.3.0/src/scippneutron/conversion/__init__.py` & `scippneutron-23.4.0/src/scippneutron/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/src/scippneutron/conversion/beamline.py` & `scippneutron-23.4.0/src/scippneutron/conversion/beamline.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,16 +75,17 @@
     See Also
     --------
     scippneutron.conversions.beamline.straight_scattered_beam:
     """
     return sc.norm(scattered_beam)
 
 
-def straight_incident_beam(*, source_position: VariableLike,
-                           sample_position: VariableLike) -> VariableLike:
+def straight_incident_beam(
+    *, source_position: VariableLike, sample_position: VariableLike
+) -> VariableLike:
     """Compute the length of the beam from source to sample.
 
     Assumes a straight beam.
     The result is
 
     .. math::
 
@@ -102,16 +103,17 @@
     -------
     :
         ``incident_beam``
     """
     return sample_position - source_position
 
 
-def straight_scattered_beam(*, position: VariableLike,
-                            sample_position: VariableLike) -> VariableLike:
+def straight_scattered_beam(
+    *, position: VariableLike, sample_position: VariableLike
+) -> VariableLike:
     """Compute the length of the beam from sample to detector.
 
     Assumes a straight beam.
     The result is
 
     .. math::
 
@@ -152,16 +154,17 @@
     -------
     :
         :math:`L_\\mathsf{total}`
     """
     return L1 + L2
 
 
-def total_straight_beam_length_no_scatter(*, source_position: VariableLike,
-                                          position: VariableLike) -> VariableLike:
+def total_straight_beam_length_no_scatter(
+    *, source_position: VariableLike, position: VariableLike
+) -> VariableLike:
     """Compute the length of the beam from source to given position.
 
     Assumes a straight beam.
     The result is
 
     .. math::
 
@@ -178,16 +181,17 @@
     -------
     :
         :math:`L_\\mathsf{total}`
     """
     return sc.norm(position - source_position)
 
 
-def two_theta(*, incident_beam: VariableLike,
-              scattered_beam: VariableLike) -> VariableLike:
+def two_theta(
+    *, incident_beam: VariableLike, scattered_beam: VariableLike
+) -> VariableLike:
     """Compute the scattering angle between scattered and transmitted beams.
 
     See :mod:`scippneutron.conversions.beamline` for the definition of the angle.
 
     The result is equivalent to
 
     .. math::
```

### Comparing `scippneutron-23.3.0/src/scippneutron/conversion/graph/__init__.py` & `scippneutron-23.4.0/src/scippneutron/conversion/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/src/scippneutron/conversion/graph/beamline.py` & `scippneutron-23.4.0/src/scippneutron/conversion/graph/beamline.py`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/src/scippneutron/conversion/graph/tof.py` & `scippneutron-23.4.0/src/scippneutron/conversion/graph/tof.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,25 +27,33 @@
     'energy': {
         'dspacing': _kernels.dspacing_from_energy,
         'wavelength': _kernels.wavelength_from_energy,
     },
     'tof': {
         'dspacing': _kernels.dspacing_from_tof,
         'energy': _kernels.energy_from_tof,
+        'hkl_vec': _kernels.hkl_vec_from_Q_vec,
+        ('h', 'k', 'l'): _kernels.hkl_elements_from_hkl_vec,
+        'ub_matrix': _kernels.ub_matrix_from_u_and_b,
         'Q': _kernels.Q_from_wavelength,
+        'Q_vec': _kernels.Q_vec_from_Q_elements,
         ('Qx', 'Qy', 'Qz'): _kernels.Q_elements_from_wavelength,
         'wavelength': _kernels.wavelength_from_tof,
     },
     'Q': {
         'wavelength': _kernels.wavelength_from_Q,
     },
     'wavelength': {
         'dspacing': _kernels.dspacing_from_wavelength,
         'energy': _kernels.energy_from_wavelength,
+        'hkl_vec': _kernels.hkl_vec_from_Q_vec,
+        ('h', 'k', 'l'): _kernels.hkl_elements_from_hkl_vec,
+        'ub_matrix': _kernels.ub_matrix_from_u_and_b,
         'Q': _kernels.Q_from_wavelength,
+        'Q_vec': _kernels.Q_vec_from_Q_elements,
         ('Qx', 'Qy', 'Qz'): _kernels.Q_elements_from_wavelength,
     },
 }
 
 
 def _strip_elastic(start: str, keep: list) -> Graph:
     full_graph = elastic(start)
@@ -134,29 +142,56 @@
     -------
     :
         A dict defining a coordinate transformation graph.
     """
     return _strip_elastic(start, keep=['Q', 'wavelength'])
 
 
-def elastic_Q_elements(start: str) -> Graph:
+def elastic_Q_vec(start: str) -> Graph:
     """
     Graph for elastic scattering transformation to Q vector.
 
     Parameters
     ----------
     start:
         Input coordinate. One of 'tof' or 'wavelength'.
 
     Returns
     -------
     :
         A dict defining a coordinate transformation graph.
     """
-    return _strip_elastic(start, keep=['Qx', 'Qy', 'Qz', 'wavelength'])
+    return _strip_elastic(start, keep=[('Qx', 'Qy', 'Qz'), 'Q_vec', 'wavelength'])
+
+
+def elastic_hkl(start: str) -> Graph:
+    """
+    Graph for elastic scattering transformation to Q vector.
+
+    Parameters
+    ----------
+    start:
+        Input coordinate. One of 'tof' or 'wavelength'.
+
+    Returns
+    -------
+    :
+        A dict defining a coordinate transformation graph.
+    """
+    return _strip_elastic(
+        start,
+        keep=[
+            ('Qx', 'Qy', 'Qz'),
+            'Q_vec',
+            ('h', 'k', 'l'),
+            'hkl_vec',
+            'ub_matrix',
+            'wavelength',
+        ],
+    )
 
 
 def elastic_wavelength(start: str) -> Graph:
     """
     Graph for elastic scattering transformation to wavelength.
 
     Parameters
@@ -199,12 +234,10 @@
         Input coordinate. Currently, only 'tof' is supported.
 
     Returns
     -------
     :
         A dict defining a coordinate transformation graph.
     """
-    return {
-        'tof': {
-            'energy_transfer': _kernels.energy_transfer_indirect_from_tof
-        }
-    }[start]
+    return {'tof': {'energy_transfer': _kernels.energy_transfer_indirect_from_tof}}[
+        start
+    ]
```

### Comparing `scippneutron-23.3.0/src/scippneutron/conversion/tof.py` & `scippneutron-23.4.0/src/scippneutron/conversion/tof.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,111 +9,118 @@
 """
 
 from typing import Tuple
 
 import numpy as np
 import scipp as sc
 import scipp.constants as const
-from scipp.typing import VariableLike
+from scipp.typing import Variable
 
 from .._utils import as_float_type, elem_dtype, elem_unit
 
 
 def _common_dtype(a, b):
     """Very limited type promotion.
     Only useful to check if the combination of a and b results in
     single or double precision float.
     """
     if elem_dtype(a) == sc.DType.float32 and elem_dtype(b) == sc.DType.float32:
         return sc.DType.float32
     return sc.DType.float64
 
 
-def wavelength_from_tof(*, tof: VariableLike, Ltotal: VariableLike) -> VariableLike:
-    """Compute the wavelength from time-of-flight.
+def wavelength_from_tof(*, tof: Variable, Ltotal: Variable) -> Variable:
+    r"""Compute the wavelength from time-of-flight.
 
     The result is the de Broglie wavelength
 
     .. math::
 
-        \\lambda = \\frac{h t}{m_n L_\\mathsf{total}}
+        \lambda = \frac{h t}{m_n L_\mathsf{total}}
 
     Where :math:`m_n` is the neutron mass and :math:`h` the Planck constant.
 
     Parameters
     ----------
     tof:
         Time-of-flight :math:`t`.
     Ltotal:
         Total beam length.
 
     Returns
     -------
     :
-        Wavelength :math:`\\lambda`.
+        Wavelength :math:`\lambda`.
         Has unit ångström.
     """
-    c = sc.to_unit(const.h / const.m_n,
-                   sc.units.angstrom * elem_unit(Ltotal) / elem_unit(tof),
-                   copy=False)
+    c = sc.to_unit(
+        const.h / const.m_n,
+        sc.units.angstrom * elem_unit(Ltotal) / elem_unit(tof),
+        copy=False,
+    )
     return as_float_type(c / Ltotal, tof) * tof
 
 
-def dspacing_from_tof(*, tof: VariableLike, Ltotal: VariableLike,
-                      two_theta: VariableLike) -> VariableLike:
-    """Compute the d-spacing from time-of-flight.
+def dspacing_from_tof(
+    *, tof: Variable, Ltotal: Variable, two_theta: Variable
+) -> Variable:
+    r"""Compute the d-spacing from time-of-flight.
 
     The result is the inter-planar lattice spacing
 
     .. math::
 
-        d = \\frac{h t}{m_n L_\\mathsf{total}\\; 2 \\sin \\theta}
+        d = \frac{h t}{m_n L_\mathsf{total}\; 2 \sin \theta}
 
     Where :math:`m_n` is the neutron mass and :math:`h` the Planck constant.
 
     Parameters
     ----------
     tof:
         Time-of-flight :math:`t`.
     Ltotal:
         Total beam length.
     two_theta:
-        Scattering angle :math:`2 \\theta`.
+        Scattering angle :math:`2 \theta`.
 
     Returns
     -------
     :
         Inter-planar lattice spacing :math:`d`.
         Has unit ångström.
 
     See Also
     --------
     scippneutron.conversions.beamline:
         Definitions of ``two_theta`` and ``Ltotal``.
     """
-    c = sc.to_unit(2 * const.m_n / const.h,
-                   elem_unit(tof) / sc.units.angstrom / elem_unit(Ltotal),
-                   copy=False)
+    c = sc.to_unit(
+        2 * const.m_n / const.h,
+        elem_unit(tof) / sc.units.angstrom / elem_unit(Ltotal),
+        copy=False,
+    )
     return 1 / as_float_type(c * Ltotal * sc.sin(two_theta / 2), tof) * tof
 
 
-def _energy_constant(energy_unit: sc.Unit, tof: VariableLike, length: VariableLike):
-    return sc.to_unit(const.m_n / 2,
-                      energy_unit * (elem_unit(tof) / elem_unit(length))**2,
-                      copy=False)
+def _energy_constant(energy_unit: sc.Unit, tof: Variable, length: Variable):
+    return sc.to_unit(
+        const.m_n / 2,
+        energy_unit * (elem_unit(tof) / elem_unit(length)) ** 2,
+        copy=False,
+    )
 
 
-def energy_from_tof(*, tof: VariableLike, Ltotal: VariableLike) -> VariableLike:
-    """Compute the neutron energy from time-of-flight.
+def energy_from_tof(*, tof: Variable, Ltotal: Variable) -> Variable:
+    r"""Compute the neutron energy from time-of-flight.
 
     The result is
 
     .. math::
 
-        E = \\frac{m_n L_\\mathsf{total}^2}{2 t^2}
+        E = \frac{m_n L_\mathsf{total}^2}{2 t^2}
 
     Where :math:`m_n` is the neutron mass.
 
     Parameters
     ----------
     tof:
         Time-of-flight :math:`t`.
@@ -122,39 +129,41 @@
     Returns
     -------
     :
         Neutron energy :math:`E`.
         Has unit meV.
     """
     c = _energy_constant(sc.units.meV, tof, Ltotal)
-    return as_float_type(c * Ltotal**2, tof) / tof**sc.scalar(2, dtype=elem_dtype(tof))
+    return as_float_type(c * Ltotal**2, tof) / tof ** sc.scalar(
+        2, dtype=elem_dtype(tof)
+    )
 
 
 def _energy_transfer_t0(energy, tof, length):
     dtype = _common_dtype(energy, tof)
     c = as_float_type(_energy_constant(elem_unit(energy), tof, length), energy)
     return length.astype(dtype, copy=False) * sc.sqrt(c / energy)
 
 
-def energy_transfer_direct_from_tof(*, tof: VariableLike, L1: VariableLike,
-                                    L2: VariableLike,
-                                    incident_energy: VariableLike) -> VariableLike:
-    """Compute the energy transfer in direct inelastic scattering.
+def energy_transfer_direct_from_tof(
+    *, tof: Variable, L1: Variable, L2: Variable, incident_energy: Variable
+) -> Variable:
+    r"""Compute the energy transfer in direct inelastic scattering.
 
     The result is
 
     .. math::
 
-        \\Delta E = E_i - \\frac{m_n L_2^2}{2 {(t - t_0)}^2}
+        \Delta E = E_i - \frac{m_n L_2^2}{2 {(t - t_0)}^2}
 
     With
 
     .. math::
 
-        t_0 = \\sqrt{m_n L_1^2 / (2 E_i)}
+        t_0 = \sqrt{m_n L_1^2 / (2 E_i)}
 
     and :math:`m_n` the neutron mass.
 
     The result is ``NaN`` for unphysical points, that is, where :math:`t < t_0`.
 
     Parameters
     ----------
@@ -166,47 +175,49 @@
         Secondary beam length.
     incident_energy:
         Energy before scattering :math:`E_i`.
 
     Returns
     -------
     :
-        Energy transfer :math:`\\Delta E`.
+        Energy transfer :math:`\Delta E`.
         Has the same unit as incident_energy.
 
     See Also
     --------
     scippneutron.conversions.tof.energy_transfer_indirect_from_tof
     """
     t0 = _energy_transfer_t0(incident_energy, tof, L1)
     c = _energy_constant(elem_unit(incident_energy), tof, L2)
     dtype = _common_dtype(incident_energy, tof)
     scale = (c * L2**2).astype(dtype, copy=False)
     delta_tof = tof - t0
-    return sc.where(delta_tof <= sc.scalar(0, unit=elem_unit(delta_tof)),
-                    sc.scalar(np.nan, dtype=dtype, unit=elem_unit(incident_energy)),
-                    incident_energy - scale / delta_tof**2)
+    return sc.where(
+        delta_tof <= sc.scalar(0, unit=elem_unit(delta_tof)),
+        sc.scalar(np.nan, dtype=dtype, unit=elem_unit(incident_energy)),
+        incident_energy - scale / delta_tof**2,
+    )
 
 
-def energy_transfer_indirect_from_tof(*, tof: VariableLike, L1: VariableLike,
-                                      L2: VariableLike,
-                                      final_energy: VariableLike) -> VariableLike:
-    """Compute the energy transfer in indirect inelastic scattering.
+def energy_transfer_indirect_from_tof(
+    *, tof: Variable, L1: Variable, L2: Variable, final_energy: Variable
+) -> Variable:
+    r"""Compute the energy transfer in indirect inelastic scattering.
 
     The result is
 
     .. math::
 
-        \\Delta E = \\frac{m_n L_1^2}{2 {(t - t_0)}^2} - E_f
+        \Delta E = \frac{m_n L_1^2}{2 {(t - t_0)}^2} - E_f
 
     With
 
     .. math::
 
-        t_0 = \\sqrt{m_n L_2^2 / (2 E_f)}
+        t_0 = \sqrt{m_n L_2^2 / (2 E_f)}
 
     and :math:`m_n` the neutron mass.
 
     The result is ``NaN`` for unphysical points, that is, where :math:`t < t_0`.
 
     Parameters
     ----------
@@ -218,265 +229,432 @@
         Secondary beam length.
     final_energy:
         Energy after scattering :math:`E_f`.
 
     Returns
     -------
     :
-        Energy transfer :math:`\\Delta E`.
+        Energy transfer :math:`\Delta E`.
         Has the same unit as final_energy.
 
     See Also
     --------
     scippneutron.conversions.tof.energy_transfer_direct_from_tof
     """
     t0 = _energy_transfer_t0(final_energy, tof, L2)
     c = _energy_constant(elem_unit(final_energy), tof, L1)
     dtype = _common_dtype(final_energy, tof)
     scale = (c * L1**2).astype(dtype, copy=False)
     delta_tof = -t0 + tof  # Order chosen such that output.dims = ['spectrum', 'tof']
-    return sc.where(delta_tof <= sc.scalar(0, unit=elem_unit(delta_tof)),
-                    sc.scalar(np.nan, dtype=dtype, unit=elem_unit(final_energy)),
-                    scale / delta_tof**2 - final_energy)
+    return sc.where(
+        delta_tof <= sc.scalar(0, unit=elem_unit(delta_tof)),
+        sc.scalar(np.nan, dtype=dtype, unit=elem_unit(final_energy)),
+        scale / delta_tof**2 - final_energy,
+    )
 
 
-def energy_from_wavelength(*, wavelength: VariableLike) -> VariableLike:
-    """Compute the neutron energy from wavelength.
+def energy_from_wavelength(*, wavelength: Variable) -> Variable:
+    r"""Compute the neutron energy from wavelength.
 
     The result is
 
     .. math::
 
-        E = \\frac{h^2}{2 m_n \\lambda^2}
+        E = \frac{h^2}{2 m_n \lambda^2}
 
     Where :math:`m_n` is the neutron mass and :math:`h` the Planck constant.
 
     Parameters
     ----------
     wavelength:
-        De Broglie wavelength :math:`\\lambda`.
+        De Broglie wavelength :math:`\lambda`.
         Has unit meV.
 
     Returns
     -------
     :
         Neutron energy :math:`E`.
     """
     c = as_float_type(
-        sc.to_unit(const.h**2 / 2 / const.m_n,
-                   sc.units.meV * elem_unit(wavelength)**2), wavelength)
+        sc.to_unit(
+            const.h**2 / 2 / const.m_n, sc.units.meV * elem_unit(wavelength) ** 2
+        ),
+        wavelength,
+    )
     return c / wavelength**2
 
 
-def wavelength_from_energy(*, energy: VariableLike) -> VariableLike:
-    """Compute the wavelength from the neutron energy.
+def wavelength_from_energy(*, energy: Variable) -> Variable:
+    r"""Compute the wavelength from the neutron energy.
 
     The result is the de Broglie wavelength
 
     .. math::
 
-        \\lambda = \\frac{h}{\\sqrt{2 m_n E}}
+        \lambda = \frac{h}{\sqrt{2 m_n E}}
 
     Where :math:`m_n` is the neutron mass and :math:`h` the Planck constant.
 
     Parameters
     ----------
     energy:
         Neutron energy :math:`E`.
 
     Returns
     -------
     :
-        Wavelength :math:`\\lambda`.
+        Wavelength :math:`\lambda`.
         Has unit ångström.
     """
     c = as_float_type(
-        sc.to_unit(const.h**2 / 2 / const.m_n,
-                   sc.units.angstrom**2 * elem_unit(energy)), energy)
+        sc.to_unit(
+            const.h**2 / 2 / const.m_n, sc.units.angstrom**2 * elem_unit(energy)
+        ),
+        energy,
+    )
     return sc.sqrt(c / energy)
 
 
-def _wavelength_Q_conversions(x: VariableLike, two_theta: VariableLike) -> VariableLike:
+def _wavelength_Q_conversions(x: Variable, two_theta: Variable) -> Variable:
     """Convert either from Q to wavelength or vice-versa."""
     c = as_float_type(4 * const.pi, x)
     return c * sc.sin(as_float_type(two_theta, x) / 2) / x
 
 
-def Q_from_wavelength(*, wavelength: VariableLike,
-                      two_theta: VariableLike) -> VariableLike:
-    """Compute the absolute value of the momentum transfer from wavelength.
+def Q_from_wavelength(*, wavelength: Variable, two_theta: Variable) -> Variable:
+    r"""Compute the absolute value of the momentum transfer from wavelength.
 
     The result is
 
     .. math::
 
-        Q = \\frac{4 \\pi \\sin \\theta}{\\lambda}
+        Q = \frac{4 \pi \sin \theta}{\lambda}
 
     Parameters
     ----------
     wavelength:
-        De Broglie wavelength :math:`\\lambda`.
+        De Broglie wavelength :math:`\lambda`.
     two_theta:
-        Scattering angle :math:`2 \\theta`.
+        Scattering angle :math:`2 \theta`.
 
     Returns
     -------
     :
         Momentum transfer :math:`Q`.
 
     See Also
     --------
     scippneutron.conversions.beamline:
         Definition of ``two_theta``.
     """
     return _wavelength_Q_conversions(wavelength, two_theta)
 
 
-def wavelength_from_Q(*, Q: VariableLike, two_theta: VariableLike) -> VariableLike:
-    """Compute the wavelength from momentum transfer.
+def wavelength_from_Q(*, Q: Variable, two_theta: Variable) -> Variable:
+    r"""Compute the wavelength from momentum transfer.
 
     The result is the de Broglie wavelength
 
     .. math::
 
-        \\lambda = \\frac{4 \\pi \\sin \\theta}{Q}
+        \lambda = \frac{4 \pi \sin \theta}{Q}
 
     Parameters
     ----------
     Q:
         Momentum transfer.
     two_theta:
-        Scattering angle :math:`2 \\theta`.
+        Scattering angle :math:`2 \theta`.
 
     Returns
     -------
     :
-        Wavelength :math:`\\lambda`
+        Wavelength :math:`\lambda`
         Has unit ångström.
 
     See Also
     --------
     scippneutron.conversions.beamline:
         Definition of ``two_theta``.
     """
-    return sc.to_unit(_wavelength_Q_conversions(Q, two_theta),
-                      unit='angstrom',
-                      copy=False)
+    return sc.to_unit(
+        _wavelength_Q_conversions(Q, two_theta), unit='angstrom', copy=False
+    )
 
 
 def Q_elements_from_wavelength(
-        *, wavelength: VariableLike, incident_beam: VariableLike,
-        scattered_beam: VariableLike
-) -> Tuple[VariableLike, VariableLike, VariableLike]:
-    """Compute them momentum transfer vector from wavelength.
+    *, wavelength: Variable, incident_beam: Variable, scattered_beam: Variable
+) -> Tuple[Variable, Variable, Variable]:
+    r"""Compute them momentum transfer vector from wavelength.
 
-    Computes the three components of the Q-vector  :math:`Q_x, Q_y, Q_z`
+    Computes the three components of the Q-vector :math:`Q_x, Q_y, Q_z`
     separately using
 
     .. math::
 
-        \\vec{Q} &= (Q_x, Q_y, Q_z) \\\\
-        \\vec{Q} &= \\vec{k}_i - \\vec{k}_f
-                 = \\frac{2\\pi}{\\lambda} \\left(\\hat{e}_i - \\hat{e}_f\\right),
+        \vec{Q} &= (Q_x, Q_y, Q_z) \\
+        \vec{Q} &= \vec{k}_i - \vec{k}_f
+                 = \frac{2\pi}{\lambda} \left(\hat{e}_i - \hat{e}_f\right),
 
     where the unit vectors for incident momentum and final momentum
 
     .. math::
 
-        \\hat{e}_i &= \\vec{k_i} / | \\vec{k_i} | \\\\
-        \\hat{e}_f &= \\vec{k_f} / | \\vec{k_f} |
+        \hat{e}_i &= \vec{k_i} / | \vec{k_i} | \\
+        \hat{e}_f &= \vec{k_f} / | \vec{k_f} |
 
     are defined as the directions of ``incident_beam`` and ``scattered_beam``,
     respectively.
 
     Parameters
     ----------
     wavelength:
-        De Broglie wavelength :math:`\\lambda`.
+        De Broglie wavelength :math:`\lambda`.
     incident_beam:
         Beam from source to sample. Expects ``dtype=vector3``.
     scattered_beam:
         Beam from sample to detector. Expects ``dtype=vector3``.
 
     Returns
     -------
-    Qx: scipp.VariableLike
-        x-component of the momentum transfer :math:`\\vec{Q}`.
-    Qy: scipp.VariableLike
-        y-component of the momentum transfer :math:`\\vec{Q}`.
-    Qz: scipp.VariableLike
-        z-component of the momentum transfer :math:`\\vec{Q}`.
+    Qx: scipp.Variable
+        x-component of the momentum transfer :math:`\vec{Q}`.
+    Qy: scipp.Variable
+        y-component of the momentum transfer :math:`\vec{Q}`.
+    Qz: scipp.Variable
+        z-component of the momentum transfer :math:`\vec{Q}`.
     """
     e_i = incident_beam / sc.norm(incident_beam)
     e_f = scattered_beam / sc.norm(scattered_beam)
     e = e_i - e_f
     k = 2 * np.pi / wavelength
     return k * e.fields.x, k * e.fields.y, k * e.fields.z
 
 
-def dspacing_from_wavelength(*, wavelength: VariableLike,
-                             two_theta: VariableLike) -> VariableLike:
-    """Compute the d-spacing from wavelength.
+def dspacing_from_wavelength(*, wavelength: Variable, two_theta: Variable) -> Variable:
+    r"""Compute the d-spacing from wavelength.
 
     The result is the inter-planar lattice spacing
 
     .. math::
 
-        d = \\frac{\\lambda}{2 \\sin \\theta}
+        d = \frac{\lambda}{2 \sin \theta}
 
     Parameters
     ----------
     wavelength:
-        De Broglie wavelength :math:`\\lambda`.
+        De Broglie wavelength :math:`\lambda`.
     two_theta:
-        Scattering angle :math:`2 \\theta`.
+        Scattering angle :math:`2 \theta`.
 
     Returns
     -------
     :
         Inter-planar lattice spacing :math:`d`.
         Has unit ångström.
 
     See Also
     --------
     scippneutron.conversions.beamline:
         Definition of ``two_theta``.
     """
     c = as_float_type(
-        sc.scalar(0.5).to(unit=sc.units.angstrom / elem_unit(wavelength)), wavelength)
+        sc.scalar(0.5).to(unit=sc.units.angstrom / elem_unit(wavelength)), wavelength
+    )
     return c * wavelength / sc.sin(as_float_type(two_theta, wavelength) / 2)
 
 
-def dspacing_from_energy(*, energy: VariableLike,
-                         two_theta: VariableLike) -> VariableLike:
-    """Compute the d-spacing from the neutron energy.
+def dspacing_from_energy(*, energy: Variable, two_theta: Variable) -> Variable:
+    r"""Compute the d-spacing from the neutron energy.
 
     The result is the inter-planar lattice spacing
 
     .. math::
 
-        d = \\frac{h}{\\sqrt{8 m_n E} \\sin \\theta}
+        d = \frac{h}{\sqrt{8 m_n E} \sin \theta}
 
     Where :math:`m_n` is the neutron mass and :math:`h` the Planck constant.
 
     Parameters
     ----------
     energy:
         Neutron energy :math:`E`.
     two_theta:
-        Scattering angle :math:`2 \\theta`.
+        Scattering angle :math:`2 \theta`.
 
     Returns
     -------
     :
         Inter-planar lattice spacing :math:`d`.
         Has unit ångström.
 
     See Also
     --------
     scippneutron.conversions.beamline:
         Definition of ``two_theta``.
     """
     c = as_float_type(
-        sc.to_unit(const.h**2 / 8 / const.m_n,
-                   sc.units.angstrom**2 * elem_unit(energy)), energy)
+        sc.to_unit(
+            const.h**2 / 8 / const.m_n, sc.units.angstrom**2 * elem_unit(energy)
+        ),
+        energy,
+    )
     return sc.sqrt(c / energy) / sc.sin(as_float_type(two_theta, energy) / 2)
+
+
+def Q_vec_from_Q_elements(*, Qx: Variable, Qy: Variable, Qz: Variable) -> Variable:
+    """Combine elements of Q into a single vector variable.
+
+    Parameters
+    ----------
+    Qx:
+        x-elements of the momentum transfer.
+    Qy:
+        y-elements of the momentum transfer.
+    Qz:
+        z-elements of the momentum transfer.
+
+    Returns
+    -------
+    :
+        ``Qx``, ``Qy``, ``Qz`` combined into a single variable of dtype ``vector3``.
+    """
+    if Qx.sizes != Qy.sizes or Qx.sizes != Qz.sizes:
+        raise sc.DimensionError(
+            "Qx, Qy, Qz must have the same sizes. "
+            f"Got {Qx.sizes=}, {Qy.sizes=}, {Qz.sizes=}."
+        )
+    return sc.spatial.as_vectors(Qx, Qy, Qz)
+
+
+def ub_matrix_from_u_and_b(*, u_matrix: Variable, b_matrix: Variable) -> Variable:
+    r"""Compute the UB matrix from U and B matrices.
+
+    .. math::
+
+        \mathsf{UB} = U \cdot B
+
+    where :math:`U` and :math:`B` are defined as in
+    :cite:`busing:1967,mantid-lattice:2023`.
+
+    Parameters
+    ----------
+    u_matrix:
+        :math:`U`.
+    b_matrix:
+        :math:`B`.
+
+    Returns
+    -------
+    :
+        :math:`\mathsf{UB}`.
+    """
+    return u_matrix * b_matrix
+
+
+def hkl_vec_from_Q_vec(
+    *, Q_vec: Variable, ub_matrix: Variable, sample_rotation: Variable
+) -> Variable:
+    r"""Compute hkl indices from momentum transfer.
+
+    The hkl indices define the components of the momentum transfer in the
+    sample coordinate system
+
+    .. math::
+
+        \vec{Q} = \begin{pmatrix} h \\ k \\ l \end{pmatrix}.
+
+    In the lab frame, the momentum transfer as computed by
+    :func:`scippneutron.conversion.tof.Q_elements_from_wavelength`
+    is defined as
+
+    .. math::
+
+        \vec{Q}_l = \vec{k}_i - \vec{k}_f .
+
+    This quantity is called :math:`Q` elsewhere in ScippNeutron.
+
+    Those two :math:`Q`'s are related by via
+
+    .. math::
+
+        \vec{Q}_l = 2 \pi R U B \vec{Q},
+
+    where :math:`U` and :math:`B` transform from sample space to the lab frame.
+    :math:`R` encodes the sample rotation, e.g., as given by a goniometer.
+    See, e.g., Refs. :cite:`busing:1967,mantid-lattice:2023,savici:2011`
+    for a definition.
+
+    This function computes the elements of :math:`\vec{Q}`, :math:`h, k, l` by inverting
+    the above equation.
+
+    Parameters
+    ----------
+    Q_vec:
+        Momentum transfer :math:`\vec{Q}_l` as a vector variable.
+    ub_matrix:
+        Matrix :math:`\mathsf{UB}`.
+    sample_rotation:
+        Sample rotation matrix :math:`R`.
+
+    Returns
+    -------
+    :
+        :math:`h, k, l` as a vector variable.
+
+    See also
+    --------
+    scippneutron.conversion.tof.Q_elements_from_wavelength:
+        Computes ``Q_l``.
+    scippneutron.conversion.tof.Q_vec_from_Q_elements:
+        Packs elements ``Qx``, ``Qy``, ``Qz`` into a single vector.
+    scippneutron.conversion.tof.ub_matrix_from_u_and_b:
+        Compute :math:`\mathsf{UB}` from :math:`B` and :math:`B` matrices.
+    scippneutron.conversion.tof.hkl_elements_from_hkl_vec:
+        Unpack the returned hkl vector.
+    """
+    # There are different ways to implement this with different performance and
+    # accuracy characteristics.
+    # Matrix-matrix products typically have worse accuracy than matrix-vector
+    # products due to repeated floating point cutoffs.
+    # Matrix inversions are often unstable; however, all matrices used here are small.
+    # Potential implementations are
+    #
+    # (sc.spatial.inv(B) * (sc.spatial.inv(U) * (sc.spatial.inv(R) * Q))) / (2*np.pi)
+    #
+    # (((sc.spatial.inv(B) * sc.spatial.inv(U)) * sc.spatial.inv(R)) * Q) / (2*np.pi)
+    #
+    # (sc.spatial.inv((R * U) * B) * Q) / (2*np.pi)
+    #
+    # All 3 were tested with random matrices and vectors and the first was found
+    # to have the best overall accuracy, being an order of magnitude better than the
+    # others in particularly bad cases and equal in the majority of cases.
+    #
+    # Concerning performance, R, U, B are scalar variables or short array variables
+    # in typical use cases while Q is typically a long, potentially multi-dim array.
+    # So implementation 3 will likely perform the best.
+    #
+    # This function uses implementation 3 as the performance gain
+    # is expected to be significant over 1 and 2.
+    return (sc.spatial.inv(sample_rotation * ub_matrix) * Q_vec) / (2 * np.pi)
+
+
+def hkl_elements_from_hkl_vec(
+    *, hkl_vec: Variable
+) -> Tuple[Variable, Variable, Variable]:
+    """Unpack vector of hkl indices into separate variables.
+
+    Parameters
+    ----------
+    hkl_vec:
+        Vector of hkl indices.
+
+    Returns
+    -------
+    h: scipp.Variable
+        1st component of the hkl vector.
+    k: scipp.Variable
+        2nd component of the hkl vector.
+    l: scipp.Variable
+        3rd component of the hkl vector.
+    """
+    return hkl_vec.fields.x, hkl_vec.fields.y, hkl_vec.fields.z
```

### Comparing `scippneutron-23.3.0/src/scippneutron/core/conversions.py` & `scippneutron-23.4.0/src/scippneutron/core/conversions.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,38 +12,44 @@
 def _inelastic_scatter_graph(energy_mode):
     inelastic_graph_factory = {
         'direct_inelastic': _graphs.tof.direct_inelastic,
         'indirect_inelastic': _graphs.tof.indirect_inelastic,
     }
     return {
         **_graphs.beamline.beamline(scatter=True),
-        **inelastic_graph_factory[energy_mode](start='tof')
+        **inelastic_graph_factory[energy_mode](start='tof'),
     }
 
 
 def _reachable_by(target, graph):
-    return any(target == targets if isinstance(targets, str) else target in targets
-               for targets in graph.keys())
+    return any(
+        target == targets if isinstance(targets, str) else target in targets
+        for targets in graph.keys()
+    )
 
 
 def _elastic_scatter_graph(origin, target):
     scatter_graph_kinematics = _graphs.beamline.beamline(scatter=True)
     if _reachable_by(target, scatter_graph_kinematics):
         return dict(scatter_graph_kinematics)
     return {**scatter_graph_kinematics, **_graphs.tof.elastic(origin)}
 
 
 def _scatter_graph(origin, target, energy_mode):
-    graph = (_elastic_scatter_graph(origin, target)
-             if energy_mode == 'elastic' else _inelastic_scatter_graph(energy_mode))
+    graph = (
+        _elastic_scatter_graph(origin, target)
+        if energy_mode == 'elastic'
+        else _inelastic_scatter_graph(energy_mode)
+    )
     return graph
 
 
-def conversion_graph(origin: str, target: str, scatter: bool,
-                     energy_mode: str) -> Dict[Union[str, Tuple[str]], Callable]:
+def conversion_graph(
+    origin: str, target: str, scatter: bool, energy_mode: str
+) -> Dict[Union[str, Tuple[str]], Callable]:
     """
     Get a conversion graph for given parameters.
 
     The graph can be used with `scipp.transform_coords`.
 
     :param origin: Name of the input coordinate.
     :param target: Name of the output coordinate.
@@ -57,68 +63,73 @@
 
     # Results are copied to ensure users do not modify the global dictionaries.
     if scatter:
         return dict(_scatter_graph(origin, target, energy_mode))
     else:
         return {
             **_graphs.beamline.beamline(scatter=False),
-            **_graphs.tof.kinematic(start='tof')
+            **_graphs.tof.kinematic(start='tof'),
         }
 
 
 def _find_inelastic_inputs(data):
     return [name for name in ('incident_energy', 'final_energy') if name in data.coords]
 
 
 def _deduce_energy_mode(data, origin, target):
     inelastic_inputs = _find_inelastic_inputs(data)
     if target == 'energy_transfer':
         if len(inelastic_inputs) > 1:
             raise RuntimeError(
                 "Data contains coords for incident *and* final energy, cannot have "
-                "both for inelastic scattering.")
+                "both for inelastic scattering."
+            )
         if len(inelastic_inputs) == 0:
             raise RuntimeError(
                 "Data contains neither coords for incident nor for final energy, this "
                 "does not appear to be inelastic-scattering data, cannot convert to "
-                "energy transfer.")
+                "energy transfer."
+            )
         return {
             'incident_energy': 'direct_inelastic',
-            'final_energy': 'indirect_inelastic'
+            'final_energy': 'indirect_inelastic',
         }[inelastic_inputs[0]]
 
     if 'energy' in (origin, target):
         if inelastic_inputs:
             raise RuntimeError(
                 f"Data contains coords for inelastic scattering "
                 f"({inelastic_inputs}) but conversion with elastic energy requested. "
-                f"This is not implemented.")
+                f"This is not implemented."
+            )
     return 'elastic'
 
 
-def deduce_conversion_graph(data: Union[sc.DataArray,
-                                        sc.Dataset], origin: str, target: str,
-                            scatter: bool) -> Dict[Union[str, Tuple[str]], Callable]:
+def deduce_conversion_graph(
+    data: Union[sc.DataArray, sc.Dataset], origin: str, target: str, scatter: bool
+) -> Dict[Union[str, Tuple[str]], Callable]:
     """
     Get the conversion graph used by :py:func:`scippneutron.convert`
     when called with identical arguments.
 
     :param data: Input data.
     :param origin: Name of the input coordinate.
     :param target: Name of the output coordinate.
     :param scatter: Choose whether to use scattering or non-scattering conversions.
     :return: Conversion graph.
     :seealso: :py:func:`scippneutron.convert`, :py:func:`scippneutron.conversion_graph`.
     """
-    return conversion_graph(origin, target, scatter,
-                            _deduce_energy_mode(data, origin, target))
+    return conversion_graph(
+        origin, target, scatter, _deduce_energy_mode(data, origin, target)
+    )
 
 
-def convert(data: Union[sc.DataArray, sc.Dataset], origin: str, target: str,
-            scatter: bool) -> Union[sc.DataArray, sc.Dataset]:
+def convert(
+    data: Union[sc.DataArray, sc.Dataset], origin: str, target: str, scatter: bool
+) -> Union[sc.DataArray, sc.Dataset]:
     """
     Perform a unit conversion from the given origin unit to target.
     See the documentation page on "Coordinate Transformations"
     (https://scipp.github.io/scippneutron/user-guide/coordinate-transformations.html)
     for more details.
 
     :param data: Input data.
@@ -133,13 +144,17 @@
 
     graph = deduce_conversion_graph(data, origin, target, scatter)
 
     try:
         converted = data.transform_coords(target, graph=graph)
     except KeyError as err:
         if err.args[0] == target:
-            raise RuntimeError(f"No viable conversion from '{origin}' to '{target}' "
-                               f"with scatter={scatter}.")
-        raise RuntimeError(f"Missing coordinate '{err.args[0]}' for conversion "
-                           f"from '{origin}' to '{target}'") from None
+            raise RuntimeError(
+                f"No viable conversion from '{origin}' to '{target}' "
+                f"with scatter={scatter}."
+            )
+        raise RuntimeError(
+            f"Missing coordinate '{err.args[0]}' for conversion "
+            f"from '{origin}' to '{target}'"
+        ) from None
 
     return converted
```

### Comparing `scippneutron-23.3.0/src/scippneutron/data/__init__.py` & `scippneutron-23.4.0/src/scippneutron/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 _version = '5'
 
 __all__ = ['tutorial_dense_data', 'tutorial_event_data', 'get_path']
 
 
 def _make_pooch():
     import pooch
+
     return pooch.create(
         path=pooch.os_cache('scippneutron'),
         env='SCIPPNEUTRON_DATA_DIR',
         retry_if_failed=3,
         base_url='https://public.esss.dk/groups/scipp/scippneutron/{version}/',
         version=_version,
         registry={
@@ -27,15 +28,16 @@
             'CNCS_51936_event.nxs': 'md5:5ba401e489260a44374b5be12b780911',
             'GEM40979.raw': 'md5:6df0f1c2fc472af200eec43762e9a874',
             'PG3_4844_calibration.h5': 'md5:39005d7b4befcafa173f00645549e2b4',
             'PG3_4844_event.nxs': 'md5:d5ae38871d0a09a28ae01f85d969de1e',
             'PG3_4866_event.nxs': 'md5:3d543bc6a646e622b3f4542bc3435e7e',
             'PG3_4871_event.nxs': 'md5:a3d0edcb36ab8e9e3342cd8a4440b779',
             'WISH00016748.raw': 'md5:37ecc6f99662b57e405ed967bdc068af',
-        })
+        },
+    )
 
 
 _pooch = _make_pooch()
 
 
 def bigfake():
     return get_path('bigfake.nxs')
```

### Comparing `scippneutron-23.3.0/src/scippneutron/data_streaming/_consumer.py` & `scippneutron-23.4.0/src/scippneutron/data_streaming/_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,18 @@
     """
     Use in place of confluent_kafka.Consumer
     to avoid network io in unit tests
     """
 
     def __init__(self, input_queue: Optional[mp.Queue]):
         if input_queue is None:
-            raise RuntimeError("A multiprocessing queue for test messages "
-                               "must be provided when using FakeConsumer")
+            raise RuntimeError(
+                "A multiprocessing queue for test messages "
+                "must be provided when using FakeConsumer"
+            )
         # This queue is used to provide the consumer with
         # messages in unit tests, instead of it getting messages
         # from the Kafka broker
         self._input_queue = input_queue
 
     def assign(self, topic_partitions: List[TopicPartition]):
         pass
@@ -63,20 +65,21 @@
             pass
 
     def close(self):
         pass
 
 
 class KafkaConsumer:
-
-    def __init__(self,
-                 topic_partition: TopicPartition,
-                 consumer: Union[Consumer, FakeConsumer],
-                 callback: Callable,
-                 stop_time_ms: Optional[int] = None):
+    def __init__(
+        self,
+        topic_partition: TopicPartition,
+        consumer: Union[Consumer, FakeConsumer],
+        callback: Callable,
+        stop_time_ms: Optional[int] = None,
+    ):
         self._consumer = consumer
         # To consume messages the consumer must "subscribe" to one
         # or more topics or "assign" specific topic partitions, the
         # latter allows us to start consuming at an offset specified
         # in the TopicPartition. Each KafkaConsumer consumes from only
         # a single partition, this simplifies the logic around run stop
         # behaviour.
@@ -97,15 +100,14 @@
     def start(self):
         self.stopped = False
         self.cancelled = False
         self._consume_data = threading.Thread(target=self._consume_loop)
         self._consume_data.start()
 
     def _consume_loop(self):
-
         def time_now_ms() -> int:
             return time_ns() // 1_000_000
 
         reached_message_after_stop_time = False
         reached_stop_time = False
         at_end_of_partition = False
 
@@ -155,15 +157,15 @@
                         break
                     continue
             self._callback(msg.value())
 
     def stop(self):
         self.cancelled = True
         if self._consume_data is not None and self._consume_data.is_alive():
-            self._consume_data.join(5.)
+            self._consume_data.join(5.0)
         self._consumer.close()
         self.stopped = True
 
     def update_stop_time(self, new_stop_time_ms: int):
         with self._stop_time_mutex:
             self._stop_time = new_stop_time_ms
 
@@ -187,15 +189,15 @@
         # multiple messages in the forward direction each time we step
         # backwards by 1 offset
         conf = {
             "bootstrap.servers": broker,
             "group.id": "consumer_group_name",
             "auto.offset.reset": "latest",
             "enable.auto.commit": False,
-            "queued.min.messages": 1
+            "queued.min.messages": 1,
         }
         self._consumer = Consumer(**conf)
 
     def get_topic_partitions(self, topic: str, offset: int = -1):
         metadata = self._consumer.list_topics(topic)
         return [
             TopicPartition(topic, partition[1].id, offset=offset)
@@ -204,15 +206,15 @@
 
     def seek(self, partition: TopicPartition):
         """
         Set offset in partition, the consumer will seek to that offset
         """
         self._consumer.seek(partition)
 
-    def poll(self, timeout=2.):
+    def poll(self, timeout=2.0):
         """
         Poll for a message from Kafka
         """
         return self._consumer.poll(timeout=timeout)
 
     def get_watermark_offsets(self, partition: TopicPartition) -> Tuple[int, int]:
         """
@@ -225,35 +227,37 @@
         self._consumer.assign(partitions)
 
     def offsets_for_times(self, partitions: List[TopicPartition]):
         return self._consumer.offsets_for_times(partitions)
 
 
 def create_consumers(
-        start_time_ms: int,
-        stop_time_ms: Optional[int],
-        topics: List[str],
-        kafka_broker: str,
-        consumer_type_enum: ConsumerType,  # so we can inject fake consumer
-        callback: Callable,
-        test_message_queue: Optional[mp.Queue]) -> List[KafkaConsumer]:
+    start_time_ms: int,
+    stop_time_ms: Optional[int],
+    topics: List[str],
+    kafka_broker: str,
+    consumer_type_enum: ConsumerType,  # so we can inject fake consumer
+    callback: Callable,
+    test_message_queue: Optional[mp.Queue],
+) -> List[KafkaConsumer]:
     """
     Creates one consumer per TopicPartition that start consuming
     at specified timestamp in the data stream
 
     Having each consumer only be responsible for one partition
     greatly simplifies the logic around stopping at the end of
     the stream (making use of "end of partition" event)
     """
     topic_partitions = []
     if consumer_type_enum == ConsumerType.REAL:
         query_consumer = KafkaQueryConsumer(kafka_broker)
         for topic in topics:
             topic_partitions.extend(
-                query_consumer.get_topic_partitions(topic, offset=start_time_ms))
+                query_consumer.get_topic_partitions(topic, offset=start_time_ms)
+            )
         topic_partitions = query_consumer.offsets_for_times(topic_partitions)
 
     # Run start messages are typically much larger than the
     # default maximum message size of 1MB. There are
     # corresponding settings on the broker.
     # Note: the "message.max.bytes" does not necessarily have to agree with the
     # size set in the broker. The lower of the two will set the limit.
@@ -272,16 +276,20 @@
     if consumer_type_enum == ConsumerType.REAL:
         consumers = [
             KafkaConsumer(topic_partition, Consumer(config), callback, stop_time_ms)
             for topic_partition in topic_partitions
         ]
     else:
         consumers = [
-            KafkaConsumer(TopicPartition(""), FakeConsumer(test_message_queue),
-                          callback, stop_time_ms)
+            KafkaConsumer(
+                TopicPartition(""),
+                FakeConsumer(test_message_queue),
+                callback,
+                stop_time_ms,
+            )
         ]
 
     return consumers
 
 
 def start_consumers(consumers: List[KafkaConsumer]):
     for consumer in consumers:
@@ -301,48 +309,52 @@
             if consumer.cancelled:
                 consumer.stop()
                 continue
             return False
     return True
 
 
-def get_run_start_message(topic: str,
-                          query_consumer: KafkaQueryConsumer) -> RunStartInfo:
+def get_run_start_message(
+    topic: str, query_consumer: KafkaQueryConsumer
+) -> RunStartInfo:
     """
     Get the last run start message on the given topic.
 
     TODO: we may need to carry out some filtering on instrument name,
     since it is possible that start messages from other instruments end up on
     the same Kafka topic (unless there is a separate topic for each instrument)
     """
     topic_partitions = query_consumer.get_topic_partitions(topic)
     n_partitions = len(topic_partitions)
     if n_partitions != 1:
         raise RuntimeError(
             f"Expected run start topic to contain exactly one partition, "
-            f"the specified topic '{topic}' has {n_partitions} partitions.")
+            f"the specified topic '{topic}' has {n_partitions} partitions."
+        )
     partition = topic_partitions[0]
-    low_watermark_offset, current_offset = \
-        query_consumer.get_watermark_offsets(partition)
+    low_watermark_offset, current_offset = query_consumer.get_watermark_offsets(
+        partition
+    )
     partition.offset = current_offset
     query_consumer.assign([partition])
 
     # Consume backwards from the end of the partition
     # until we find a run start message or reach the
     # start of the partition
     while current_offset > low_watermark_offset:
         current_offset -= 1
         partition.offset = current_offset
         query_consumer.seek(partition)
-        message = query_consumer.poll(timeout=2.)
+        message = query_consumer.poll(timeout=2.0)
         if message is None:
             raise RunStartError("Timed out when trying to retrieve run start message")
         elif message.error():
-            raise RunStartError(f"Error encountered consuming run start "
-                                f"message: {message.error()}")
+            raise RunStartError(
+                f"Error encountered consuming run start " f"message: {message.error()}"
+            )
         try:
             return deserialise_pl72(message.value())
         except WrongSchemaException:
             # Not a run start message, keep trying
             pass
 
     raise RunStartError(f"Run start message not found in topic '{topic}'")
```

### Comparing `scippneutron-23.3.0/src/scippneutron/data_streaming/_data_buffer.py` & `scippneutron-23.4.0/src/scippneutron/data_streaming/_data_buffer.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,25 +39,25 @@
 SLOW_FB_ID = "f142"
 FAST_FB_ID = "senv"
 CHOPPER_FB_ID = "tdct"
 EVENT_FB_ID = "ev42"
 
 
 def _create_metadata_buffer_array(name: str, unit: str, dtype: Any, buffer_size: int):
-    return sc.DataArray(sc.zeros(dims=[name],
-                                 shape=(buffer_size, ),
-                                 unit=unit,
-                                 dtype=dtype),
-                        coords={
-                            "time":
-                            sc.zeros(dims=[name],
-                                     shape=(buffer_size, ),
-                                     unit=sc.Unit("nanoseconds"),
-                                     dtype=np.dtype('datetime64[ns]'))
-                        })
+    return sc.DataArray(
+        sc.zeros(dims=[name], shape=(buffer_size,), unit=unit, dtype=dtype),
+        coords={
+            "time": sc.zeros(
+                dims=[name],
+                shape=(buffer_size,),
+                unit=sc.Unit("nanoseconds"),
+                dtype=np.dtype('datetime64[ns]'),
+            )
+        },
+    )
 
 
 class _SlowMetadataBuffer:
     """
     Buffer for "slowly" changing metadata from Kafka messages serialised
     according to the flatbuffer schema with id SLOW_FB_ID.
     Typically, the data sources are EPICS PVs with updates published to
@@ -65,36 +65,38 @@
     """
 
     def __init__(self, stream_info: StreamInfo, buffer_size: int):
         self._buffer_mutex = threading.Lock()
         self._buffer_size = buffer_size
         self._name = stream_info.source_name
         self._buffer_filled_size = 0
-        self._data_array = _create_metadata_buffer_array(self._name, stream_info.unit,
-                                                         stream_info.dtype, buffer_size)
+        self._data_array = _create_metadata_buffer_array(
+            self._name, stream_info.unit, stream_info.dtype, buffer_size
+        )
 
     def append_data(self, log_event: LogDataInfo, emit_data: Callable):
         if self._buffer_filled_size == self._buffer_size:
             emit_data()
 
         # Each LogDataInfo contains a single value-timestamp pair
         with self._buffer_mutex:
             self._data_array[self._name, self._buffer_filled_size] = log_event.value
             self._data_array.coords["time"][
-                self._name, self._buffer_filled_size].value = np.datetime64(
-                    log_event.timestamp_unix_ns, 'ns')
+                self._name, self._buffer_filled_size
+            ].value = np.datetime64(log_event.timestamp_unix_ns, 'ns')
             self._buffer_filled_size += 1
 
     def get_metadata_array(self) -> Tuple[bool, sc.Variable]:
         """
         Copy collected data from the buffer
         """
         with self._buffer_mutex:
             return_array = self._data_array[
-                self._name, :self._buffer_filled_size].copy()
+                self._name, : self._buffer_filled_size
+            ].copy()
             new_data_exists = self._buffer_filled_size != 0
             self._buffer_filled_size = 0
         return new_data_exists, sc.scalar(return_array)
 
 
 class _FastMetadataBuffer:
     """
@@ -107,82 +109,91 @@
 
     def __init__(self, stream_info: StreamInfo, buffer_size: int, data_queue: mp.Queue):
         self._buffer_mutex = threading.Lock()
         self._buffer_size = buffer_size
         self._name = stream_info.source_name
         self._data_queue = data_queue
         self._buffer_filled_size = 0
-        self._data_array = _create_metadata_buffer_array(self._name, stream_info.unit,
-                                                         stream_info.dtype, buffer_size)
+        self._data_array = _create_metadata_buffer_array(
+            self._name, stream_info.unit, stream_info.dtype, buffer_size
+        )
 
     def append_data(self, log_events: FastSampleEnvData, emit_data: Callable):
         # Each FastSampleEnvData contains an array of values and either:
         #  - an array of corresponding timestamps, or
         #  - the timedelta for linearly spaced timestamps
         message_size = log_events.values.size
         if message_size > self._buffer_size:
             self._data_queue.put(
                 BufferSizeWarning(
                     "Single message would overflow the fast metadata buffer, "
                     "please restart with a larger buffer size:\n"
                     f"message_size: {message_size}, fast_metadata_buffer_size:"
                     f" {self._buffer_size}. These data have been "
-                    f"skipped!"))
+                    f"skipped!"
+                )
+            )
             return
 
         if self._buffer_filled_size + message_size > self._buffer_size:
             emit_data()
 
         def _datetime_to_epoch_ns(input_timestamp: datetime) -> int:
             return int(input_timestamp.timestamp() * 1_000_000_000)
 
         with self._buffer_mutex:
-            self._data_array[self._name,
-                             self._buffer_filled_size:self._buffer_filled_size +
-                             message_size].values = log_events.values
+            self._data_array[
+                self._name,
+                self._buffer_filled_size : self._buffer_filled_size + message_size,
+            ].values = log_events.values
             if log_events.value_ts is not None:
                 timestamps = log_events.value_ts
             else:
                 # Generate linearly spaced sample timestamps assuming that
                 # the message timestamp falls at the start of the sample range
                 timestamps = np.arange(0, message_size, dtype=np.int64) * int(
-                    log_events.sample_ts_delta) + _datetime_to_epoch_ns(
-                        log_events.timestamp)
+                    log_events.sample_ts_delta
+                ) + _datetime_to_epoch_ns(log_events.timestamp)
                 if log_events.ts_location == TimestampLocation.Middle:
                     # Shift timestamps so that the message timestamp falls
                     # in the middle of the sample range
-                    timestamps = timestamps - int(0.5 *
-                                                  (timestamps[-1] - timestamps[0]))
+                    timestamps = timestamps - int(
+                        0.5 * (timestamps[-1] - timestamps[0])
+                    )
                 elif log_events.ts_location == TimestampLocation.End:
                     # Shift timestamps so that the message timestamp falls at
                     # the end of the sample range
                     timestamps = timestamps - (timestamps[-1] - timestamps[0])
                 elif log_events.ts_location == TimestampLocation.Start:
                     pass  # timestamps are already correct
                 else:
                     # We have accounted for all enum values so this can only
                     # happen if someone really messed up when serialising the
                     # message or a breaking change was made to the schema
                     # without a new schema id being assigned (which is
                     # against ECDC policy)
-                    raise RuntimeError("Unrecognised timestamp location in fast sample "
-                                       "environment data message (flatbuffer id: "
-                                       f"'{FAST_FB_ID}')")
-            self._data_array[self._name,
-                             self._buffer_filled_size:self._buffer_filled_size +
-                             message_size].coords["time"].values = timestamps
+                    raise RuntimeError(
+                        "Unrecognised timestamp location in fast sample "
+                        "environment data message (flatbuffer id: "
+                        f"'{FAST_FB_ID}')"
+                    )
+            self._data_array[
+                self._name,
+                self._buffer_filled_size : self._buffer_filled_size + message_size,
+            ].coords["time"].values = timestamps
             self._buffer_filled_size += message_size
 
     def get_metadata_array(self) -> Tuple[bool, sc.Variable]:
         """
         Copy collected data from the buffer
         """
         with self._buffer_mutex:
             return_array = self._data_array[
-                self._name, :self._buffer_filled_size].copy()
+                self._name, : self._buffer_filled_size
+            ].copy()
             new_data_exists = self._buffer_filled_size != 0
             self._buffer_filled_size = 0
         return new_data_exists, sc.scalar(return_array)
 
 
 class _ChopperMetadataBuffer:
     """
@@ -192,167 +203,196 @@
 
     def __init__(self, stream_info: StreamInfo, buffer_size: int, data_queue: mp.Queue):
         self._buffer_mutex = threading.Lock()
         self._buffer_size = buffer_size
         self._name = stream_info.source_name
         self._data_queue = data_queue
         self._buffer_filled_size = 0
-        self._data_array = sc.zeros(dims=[self._name],
-                                    shape=(buffer_size, ),
-                                    unit=sc.Unit("nanoseconds"),
-                                    dtype=np.int64)
+        self._data_array = sc.zeros(
+            dims=[self._name],
+            shape=(buffer_size,),
+            unit=sc.Unit("nanoseconds"),
+            dtype=np.int64,
+        )
 
     def append_data(self, chopper_timestamps: Timestamps, emit_data: Callable):
         # Each Timestamps contains an array of top-dead-centre timestamps
         message_size = chopper_timestamps.timestamps.size
         if message_size > self._buffer_size:
             self._data_queue.put(
                 BufferSizeWarning(
                     "Single message would overflow the chopper data buffer, "
                     "please restart with a larger buffer size:\n"
                     f"message_size: {message_size}, chopper_buffer_size:"
                     f" {self._buffer_size}. These data have been "
-                    f"skipped!"))
+                    f"skipped!"
+                )
+            )
             return
 
         if self._buffer_filled_size + message_size > self._buffer_size:
             emit_data()
 
         with self._buffer_mutex:
-            self._data_array[self._name,
-                             self._buffer_filled_size:self._buffer_filled_size +
-                             message_size].values = chopper_timestamps.timestamps
+            self._data_array[
+                self._name,
+                self._buffer_filled_size : self._buffer_filled_size + message_size,
+            ].values = chopper_timestamps.timestamps
             self._buffer_filled_size += message_size
 
     def get_metadata_array(self) -> Tuple[bool, sc.Variable]:
         """
         Copy collected data from the buffer
         """
         with self._buffer_mutex:
             return_array = self._data_array[
-                self._name, :self._buffer_filled_size].copy()
+                self._name, : self._buffer_filled_size
+            ].copy()
             new_data_exists = self._buffer_filled_size != 0
             self._buffer_filled_size = 0
         return new_data_exists, sc.scalar(return_array)
 
 
 metadata_ids = (SLOW_FB_ID, FAST_FB_ID, CHOPPER_FB_ID)
-_MetadataBuffer = Union[_FastMetadataBuffer, _SlowMetadataBuffer,
-                        _ChopperMetadataBuffer]
+_MetadataBuffer = Union[
+    _FastMetadataBuffer, _SlowMetadataBuffer, _ChopperMetadataBuffer
+]
 
 
 class StreamedDataBuffer:
     """
     This owns the buffers for data consumed from Kafka.
     It periodically emits accumulated data to a queue
     and resets the buffer. If a buffer fills up within the emit time
     interval then data are emitted early.
 
     TODO: This also owns the metadata buffers. Maybe this should be moved to a
     separate place in the future?
     """
 
-    def __init__(self, queue: mp.Queue, event_buffer_size: int,
-                 slow_metadata_buffer_size: int, fast_metadata_buffer_size: int,
-                 chopper_buffer_size: int, interval_s: float, run_id: str):
+    def __init__(
+        self,
+        queue: mp.Queue,
+        event_buffer_size: int,
+        slow_metadata_buffer_size: int,
+        fast_metadata_buffer_size: int,
+        chopper_buffer_size: int,
+        interval_s: float,
+        run_id: str,
+    ):
         self._buffer_mutex = threading.Lock()
         self._interval_s = interval_s
         self._event_buffer_size = event_buffer_size
         self._slow_metadata_buffer_size = slow_metadata_buffer_size
         self._fast_metadata_buffer_size = fast_metadata_buffer_size
         self._chopper_buffer_size = chopper_buffer_size
         self._current_run_id = run_id
-        tof_buffer = sc.zeros(dims=['event'],
-                              shape=[event_buffer_size],
-                              unit=sc.units.ns,
-                              dtype=sc.DType.int32)
-        id_buffer = sc.zeros(dims=['event'],
-                             shape=[event_buffer_size],
-                             unit=sc.units.one,
-                             dtype=sc.DType.int32)
-        pulse_times = sc.zeros(dims=['event'],
-                               shape=[event_buffer_size],
-                               unit=sc.units.ns,
-                               dtype=sc.DType.int64)
-        weights = sc.ones(dims=['event'],
-                          shape=[event_buffer_size],
-                          with_variances=True)
-        self._events_buffer = sc.DataArray(weights,
-                                           coords={
-                                               'tof': tof_buffer,
-                                               'detector_id': id_buffer,
-                                               'pulse_time': pulse_times
-                                           })
+        tof_buffer = sc.zeros(
+            dims=['event'],
+            shape=[event_buffer_size],
+            unit=sc.units.ns,
+            dtype=sc.DType.int32,
+        )
+        id_buffer = sc.zeros(
+            dims=['event'],
+            shape=[event_buffer_size],
+            unit=sc.units.one,
+            dtype=sc.DType.int32,
+        )
+        pulse_times = sc.zeros(
+            dims=['event'],
+            shape=[event_buffer_size],
+            unit=sc.units.ns,
+            dtype=sc.DType.int64,
+        )
+        weights = sc.ones(
+            dims=['event'], shape=[event_buffer_size], with_variances=True
+        )
+        self._events_buffer = sc.DataArray(
+            weights,
+            coords={
+                'tof': tof_buffer,
+                'detector_id': id_buffer,
+                'pulse_time': pulse_times,
+            },
+        )
         self._current_event = 0
         self._cancelled = False
         self._notify_cancelled = threading.Condition()
         self._unrecognised_fb_id_count = 0
         self._periodic_emit: Optional[threading.Thread] = None
         self._emit_queue = queue
         # Access metadata buffer by
         # self._metadata_buffers[flatbuffer_id][source_name]
         self._metadata_buffers: Dict[str, Dict[str, _MetadataBuffer]] = {
-            flatbuffer_id: {}
-            for flatbuffer_id in metadata_ids
+            flatbuffer_id: {} for flatbuffer_id in metadata_ids
         }
 
     def init_metadata_buffers(self, stream_info: List[StreamInfo]):
         """
         Create a buffer for each of the metadata sources.
         This is not in the constructor which allows the StreamedDataBuffer
         to be constructed before metadata sources are extracted from the
         run start message, this means the StreamedDataBuffer can be passed
         into data_stream to facilitate unit testing.
         """
         for stream in stream_info:
             if stream.flatbuffer_id == SLOW_FB_ID:
                 self._metadata_buffers[stream.flatbuffer_id][
-                    stream.source_name] = _SlowMetadataBuffer(
-                        stream, self._slow_metadata_buffer_size)
+                    stream.source_name
+                ] = _SlowMetadataBuffer(stream, self._slow_metadata_buffer_size)
             elif stream.flatbuffer_id == FAST_FB_ID:
                 self._metadata_buffers[stream.flatbuffer_id][
-                    stream.source_name] = _FastMetadataBuffer(
-                        stream, self._fast_metadata_buffer_size, self._emit_queue)
+                    stream.source_name
+                ] = _FastMetadataBuffer(
+                    stream, self._fast_metadata_buffer_size, self._emit_queue
+                )
             elif stream.flatbuffer_id == CHOPPER_FB_ID:
                 self._metadata_buffers[stream.flatbuffer_id][
-                    stream.source_name] = _ChopperMetadataBuffer(
-                        stream, self._chopper_buffer_size, self._emit_queue)
+                    stream.source_name
+                ] = _ChopperMetadataBuffer(
+                    stream, self._chopper_buffer_size, self._emit_queue
+                )
             elif stream.flatbuffer_id == EVENT_FB_ID:
                 pass  # detection events, not metadata
             else:
                 self._emit_queue.put(
                     UnknownFlatbufferIdWarning(
                         f"Stream in run start message specified flatbuffer id "
                         f"'{stream.flatbuffer_id}' which scippneutron does "
-                        f"not know how to deserialise."))
+                        f"not know how to deserialise."
+                    )
+                )
 
     def start(self):
         self._cancelled = False
         self._unrecognised_fb_id_count = 0
         self._periodic_emit = threading.Thread(target=self._emit_loop)
         self._periodic_emit.start()
 
     def stop(self):
         self._cancelled = True
         with self._notify_cancelled:
             self._notify_cancelled.notifyAll()
-        if (self._periodic_emit is not None and self._periodic_emit.is_alive()):
-            self._periodic_emit.join(5.)
+        if self._periodic_emit is not None and self._periodic_emit.is_alive():
+            self._periodic_emit.join(5.0)
         self._emit_data()  # flush the buffer
 
     def _emit_data(self):
         with self._buffer_mutex:
             if self._unrecognised_fb_id_count:
                 self._emit_queue.put(
                     UnknownFlatbufferIdWarning(
                         f"Received {self._unrecognised_fb_id_count}"
-                        " messages with unrecognised FlatBuffer ids"))
+                        " messages with unrecognised FlatBuffer ids"
+                    )
+                )
                 self._unrecognised_fb_id_count = 0
-            new_data = self._events_buffer['event', :self._current_event].copy()
-            new_data_exists = (self._current_event != 0)
+            new_data = self._events_buffer['event', : self._current_event].copy()
+            new_data_exists = self._current_event != 0
             for _, buffers in self._metadata_buffers.items():
                 for name, buffer in buffers.items():
                     (new_metadata_exists, metadata_array) = buffer.get_metadata_array()
                     new_data.attrs[name] = metadata_array
                     if new_metadata_exists:
                         new_data_exists = True
             self._current_event = 0
@@ -372,43 +412,47 @@
             if message_size > self._event_buffer_size:
                 self._emit_queue.put(
                     BufferSizeWarning(
                         "Single message would overflow the event data buffer, "
                         "please restart with a larger buffer size:\n"
                         f"message_size: {message_size}, event_buffer_size:"
                         f" {self._event_buffer_size}. These data have been "
-                        f"skipped!"))
+                        f"skipped!"
+                    )
+                )
                 return True
             # If new data would overfill buffer then emit data
             # currently in buffer first
             if self._current_event + message_size > self._event_buffer_size:
                 self._emit_data()
             with self._buffer_mutex:
-                frame = self._events_buffer['event',
-                                            self._current_event:self._current_event +
-                                            message_size]
+                frame = self._events_buffer[
+                    'event', self._current_event : self._current_event + message_size
+                ]
                 frame.coords['detector_id'].values = deserialised_data.detector_id
                 frame.coords['tof'].values = deserialised_data.time_of_flight
-                frame.coords['pulse_time'].values = \
-                    deserialised_data.pulse_time * \
-                    np.ones_like(deserialised_data.time_of_flight)
+                frame.coords[
+                    'pulse_time'
+                ].values = deserialised_data.pulse_time * np.ones_like(
+                    deserialised_data.time_of_flight
+                )
                 self._current_event += message_size
         except WrongSchemaException:
             return False
         return True
 
-    def _handled_metadata(self, new_data: bytes, source_field_name: str,
-                          deserialise: Callable, fb_id: str) -> bool:
+    def _handled_metadata(
+        self, new_data: bytes, source_field_name: str, deserialise: Callable, fb_id: str
+    ) -> bool:
         try:
             deserialised_data = deserialise(new_data)
             try:
-                self._metadata_buffers[fb_id][getattr(deserialised_data,
-                                                      source_field_name)].append_data(
-                                                          deserialised_data,
-                                                          self._emit_data)
+                self._metadata_buffers[fb_id][
+                    getattr(deserialised_data, source_field_name)
+                ].append_data(deserialised_data, self._emit_data)
                 return True
             except KeyError:
                 # Ignore data from unknown source name
                 pass
         except WrongSchemaException:
             return False
         return False
@@ -424,16 +468,17 @@
 
     def new_data(self, new_data: bytes):
         """
         This is the callback which is given to the consumers.
         """
         if self._handled_event_data(new_data):
             return
-        if self._handled_metadata(new_data, "source_name", deserialise_f142,
-                                  SLOW_FB_ID):
+        if self._handled_metadata(
+            new_data, "source_name", deserialise_f142, SLOW_FB_ID
+        ):
             return
         if self._handled_metadata(new_data, "name", deserialise_senv, FAST_FB_ID):
             return
         if self._handled_metadata(new_data, "name", deserialise_tdct, CHOPPER_FB_ID):
             return
         if self._handled_stop_run(new_data):
             return
```

### Comparing `scippneutron-23.3.0/src/scippneutron/data_streaming/_data_consumption_manager.py` & `scippneutron-23.4.0/src/scippneutron/data_streaming/_data_consumption_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 import multiprocessing as mp
 from dataclasses import dataclass
 from enum import Enum
 from queue import Empty as QueueEmpty
 from typing import List, Optional
 
 from ..io.nexus.load_nexus import StreamInfo
-from ._consumer import all_consumers_stopped, create_consumers, start_consumers, \
-    stop_consumers
+from ._consumer import (
+    all_consumers_stopped,
+    create_consumers,
+    start_consumers,
+    stop_consumers,
+)
 from ._consumer_type import ConsumerType
 from ._data_buffer import StreamedDataBuffer
 
 
 class InstructionType(Enum):
     STOP_NOW = 1
     UPDATE_STOP_TIME = 2
@@ -20,45 +24,67 @@
 
 @dataclass(frozen=True)
 class ManagerInstruction:
     type: InstructionType
     stop_time_ms: Optional[int] = None  # milliseconds from unix epoch
 
 
-def data_consumption_manager(start_time_ms: int, stop_time_ms: Optional[int],
-                             run_id: str, topics: List[str], kafka_broker: str,
-                             consumer_type: ConsumerType,
-                             stream_info: Optional[List[StreamInfo]], interval_s: float,
-                             event_buffer_size: int, slow_metadata_buffer_size: int,
-                             fast_metadata_buffer_size: int, chopper_buffer_size: int,
-                             worker_instruction_queue: mp.Queue, data_queue: mp.Queue,
-                             test_message_queue: Optional[mp.Queue]):
+def data_consumption_manager(
+    start_time_ms: int,
+    stop_time_ms: Optional[int],
+    run_id: str,
+    topics: List[str],
+    kafka_broker: str,
+    consumer_type: ConsumerType,
+    stream_info: Optional[List[StreamInfo]],
+    interval_s: float,
+    event_buffer_size: int,
+    slow_metadata_buffer_size: int,
+    fast_metadata_buffer_size: int,
+    chopper_buffer_size: int,
+    worker_instruction_queue: mp.Queue,
+    data_queue: mp.Queue,
+    test_message_queue: Optional[mp.Queue],
+):
     """
     Starts and stops buffers and data consumers which collect data and
     send them back to the main process via a queue.
 
     All input args must be mp.Queue or pickleable as this function is launched
     as a multiprocessing.Process.
     """
-    buffer = StreamedDataBuffer(data_queue, event_buffer_size,
-                                slow_metadata_buffer_size, fast_metadata_buffer_size,
-                                chopper_buffer_size, interval_s, run_id)
+    buffer = StreamedDataBuffer(
+        data_queue,
+        event_buffer_size,
+        slow_metadata_buffer_size,
+        fast_metadata_buffer_size,
+        chopper_buffer_size,
+        interval_s,
+        run_id,
+    )
 
     if stream_info is not None:
         buffer.init_metadata_buffers(stream_info)
 
-    consumers = create_consumers(start_time_ms, stop_time_ms, set(topics), kafka_broker,
-                                 consumer_type, buffer.new_data, test_message_queue)
+    consumers = create_consumers(
+        start_time_ms,
+        stop_time_ms,
+        set(topics),
+        kafka_broker,
+        consumer_type,
+        buffer.new_data,
+        test_message_queue,
+    )
 
     start_consumers(consumers)
     buffer.start()
 
     while not all_consumers_stopped(consumers):
         try:
-            instruction = worker_instruction_queue.get(timeout=.5)
+            instruction = worker_instruction_queue.get(timeout=0.5)
             if instruction.type == InstructionType.STOP_NOW:
                 stop_consumers(consumers)
             elif instruction.type == InstructionType.UPDATE_STOP_TIME:
                 for consumer in consumers:
                     consumer.update_stop_time(instruction.stop_time_ms)
         except QueueEmpty:
             pass
```

### Comparing `scippneutron-23.3.0/src/scippneutron/data_streaming/_data_stream_widget.py` & `scippneutron-23.4.0/src/scippneutron/data_streaming/_data_stream_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 from datetime import datetime
 from typing import Optional
 
 
 def _unix_ms_to_datetime(unix_ms: int) -> datetime:
-    return datetime.fromtimestamp(unix_ms / 1000.)
+    return datetime.fromtimestamp(unix_ms / 1000.0)
 
 
 class DataStreamWidget:
-
-    def __init__(self,
-                 start_time_ms: Optional[int] = None,
-                 stop_time_ms: Optional[int] = None,
-                 run_title: Optional[str] = None):
+    def __init__(
+        self,
+        start_time_ms: Optional[int] = None,
+        stop_time_ms: Optional[int] = None,
+        run_title: Optional[str] = None,
+    ):
         import ipywidgets as widgets
         from IPython.display import display
+
         self._stop_button = widgets.ToggleButton(description="Stop stream")
         self._stop_button.observe(self._on_button_clicked, "value")
         self._title = widgets.Label("-")
         self._start_time = widgets.Label("-")
         self._stop_time = widgets.Label("-")
         self._time_format = "%m/%d/%Y %H:%M:%S"
 
@@ -29,33 +31,38 @@
             self.set_start_time(start_time_ms)
         if stop_time_ms is not None and stop_time_ms != 0:
             # 0 is the default in the run start message flatbuffer
             # if stop time field is not populated
             self.set_stop_time(stop_time_ms)
 
         display(
-            widgets.HBox([
-                self._stop_button,
-                widgets.HBox([widgets.Label('Run title:'), self._title]),
-                widgets.HBox([widgets.Label('Start time:'), self._start_time]),
-                widgets.HBox([widgets.Label('Stop time:'), self._stop_time])
-            ]))
+            widgets.HBox(
+                [
+                    self._stop_button,
+                    widgets.HBox([widgets.Label('Run title:'), self._title]),
+                    widgets.HBox([widgets.Label('Start time:'), self._start_time]),
+                    widgets.HBox([widgets.Label('Stop time:'), self._stop_time]),
+                ]
+            )
+        )
 
     @staticmethod
     def _on_button_clicked(b):
         b["owner"].description = "Stopping..."
         b["owner"].disabled = True
 
     def set_start_time(self, start_time_ms: int):
         self._start_time.value = _unix_ms_to_datetime(start_time_ms).strftime(
-            self._time_format)
+            self._time_format
+        )
 
     def set_stop_time(self, stop_time_ms: int):
         self._stop_time.value = _unix_ms_to_datetime(stop_time_ms).strftime(
-            self._time_format)
+            self._time_format
+        )
 
     def set_title(self, new_run_title: str):
         self._title.value = new_run_title
 
     @property
     def stop_requested(self) -> bool:
         return self._stop_button.value
```

### Comparing `scippneutron-23.3.0/src/scippneutron/data_streaming/_serialisation.py` & `scippneutron-23.4.0/src/scippneutron/data_streaming/_serialisation.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,56 +20,61 @@
         for k, v in d.items():
             if isinstance(v, dict):
                 _unit_and_dtype_to_str(v)
             elif k == "unit":
                 d[k] = str(v)
             elif k == "dtype":
                 d[k] = str(v)
-                if any(scipp_container_type == d[k]
-                       for scipp_container_type in _scipp_containers):
+                if any(
+                    scipp_container_type == d[k]
+                    for scipp_container_type in _scipp_containers
+                ):
                     d["values"] = sc.to_dict(d["values"])
                     _unit_and_dtype_to_str(d["values"])
 
     _unit_and_dtype_to_str(data_dict)
     return data_dict
 
 
 def convert_from_pickleable_dict(data_dict: Dict) -> sc.DataArray:
-
     def convert_from_str_unit_and_dtype(d):
         delete_dtype = False
         for k, v in d.items():
             if isinstance(v, dict):
                 convert_from_str_unit_and_dtype(v)
                 if k not in ("attrs", "masks", "coords"):
                     if {"coords", "data"}.issubset(set(v.keys())):
                         # from_dict does not work with nested DataArrays,
                         # so we have to manually construct DataArrays here.
-                        d[k] = sc.DataArray(coords=v["coords"],
-                                            data=v["data"],
-                                            attrs=v["attrs"])
+                        d[k] = sc.DataArray(
+                            coords=v["coords"], data=v["data"], attrs=v["attrs"]
+                        )
                     else:
                         try:
-                            if any(scipp_container_type in str(v["dtype"])
-                                   for scipp_container_type in _scipp_containers):
+                            if any(
+                                scipp_container_type in str(v["dtype"])
+                                for scipp_container_type in _scipp_containers
+                            ):
                                 del v["dtype"]
                         except KeyError:
                             pass
                         d[k] = sc.from_dict(v)
             else:
                 if k == "dtype":
                     try:
                         d[k] = np.dtype(v)
                     except TypeError:
                         if v == "string":
                             d[k] = sc.DType.string
-                        elif any(scipp_container_type in k
-                                 for scipp_container_type in _scipp_containers):
+                        elif any(
+                            scipp_container_type in k
+                            for scipp_container_type in _scipp_containers
+                        ):
                             delete_dtype = True
         # Delete now, not while looping through dictionary
         if delete_dtype:
             del d["dtype"]
 
     convert_from_str_unit_and_dtype(data_dict)
-    return sc.DataArray(data=data_dict["data"],
-                        coords=data_dict["coords"],
-                        attrs=data_dict["attrs"])
+    return sc.DataArray(
+        data=data_dict["data"], coords=data_dict["coords"], attrs=data_dict["attrs"]
+    )
```

### Comparing `scippneutron-23.3.0/src/scippneutron/data_streaming/data_stream.py` & `scippneutron-23.4.0/src/scippneutron/data_streaming/data_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 
 
 _missing_dependency_message = (
     "Confluent Kafka Python library and/or serialisation library"
     "not found, please install confluent-kafka and "
     "ess-streaming-data-types as detailed in the "
     "installation instructions (https://scipp.github.io/"
-    "scippneutron/getting-started/installation.html)")
+    "scippneutron/getting-started/installation.html)"
+)
 
 
 async def data_stream(
     kafka_broker: str,
     topics: Optional[List[str]] = None,
     event_buffer_size: int = 1_048_576,
     slow_metadata_buffer_size: int = 1000,
     fast_metadata_buffer_size: int = 100_000,
     chopper_buffer_size: int = 10_000,
-    interval: sc.Variable = 2. * sc.units.s,
+    interval: sc.Variable = 2.0 * sc.units.s,
     run_info_topic: Optional[str] = None,
     start_time: StartTime = StartTime.NOW,
     stop_time: StopTime = StopTime.NEVER,
 ) -> Generator[sc.DataArray, None, None]:
     """
     Periodically yields accumulated data from stream.
     If the buffer fills up more frequently than the set interval
@@ -83,87 +84,107 @@
       in the future.
     - `start_time`: it is possible to go back to the start of the run, even if
       `data_stream()` is started after or during the run. It simply finds the
       start time in the last run_start message. The data can persist on Kafka
       for a significant duration (hours? days?), making this lookup possible.
     """
 
-    validate_buffer_size_args(chopper_buffer_size, event_buffer_size,
-                              fast_metadata_buffer_size, slow_metadata_buffer_size)
+    validate_buffer_size_args(
+        chopper_buffer_size,
+        event_buffer_size,
+        fast_metadata_buffer_size,
+        slow_metadata_buffer_size,
+    )
 
     ctx = mp.get_context("spawn")
     data_queue = ctx.Queue()
     instruction_queue = ctx.Queue()
 
     # Use "async for" as "yield from" cannot be used in an async function, see
     # https://www.python.org/dev/peps/pep-0525/#asynchronous-yield-from
-    async for data_chunk in _data_stream(data_queue, instruction_queue, kafka_broker,
-                                         topics, interval, event_buffer_size,
-                                         slow_metadata_buffer_size,
-                                         fast_metadata_buffer_size, chopper_buffer_size,
-                                         run_info_topic, start_time,
-                                         stop_time):  # noqa: E125
+    async for data_chunk in _data_stream(
+        data_queue,
+        instruction_queue,
+        kafka_broker,
+        topics,
+        interval,
+        event_buffer_size,
+        slow_metadata_buffer_size,
+        fast_metadata_buffer_size,
+        chopper_buffer_size,
+        run_info_topic,
+        start_time,
+        stop_time,
+    ):  # noqa: E125
         yield data_chunk
 
 
-def validate_buffer_size_args(chopper_buffer_size, event_buffer_size,
-                              fast_metadata_buffer_size, slow_metadata_buffer_size):
-    for buffer_name, buffer_size in (("event_buffer_size",
-                                      event_buffer_size), ("slow_metadata_buffer_size",
-                                                           slow_metadata_buffer_size),
-                                     ("fast_metadata_buffer_size",
-                                      fast_metadata_buffer_size),
-                                     ("chopper_buffer_size", chopper_buffer_size)):
+def validate_buffer_size_args(
+    chopper_buffer_size,
+    event_buffer_size,
+    fast_metadata_buffer_size,
+    slow_metadata_buffer_size,
+):
+    for buffer_name, buffer_size in (
+        ("event_buffer_size", event_buffer_size),
+        ("slow_metadata_buffer_size", slow_metadata_buffer_size),
+        ("fast_metadata_buffer_size", fast_metadata_buffer_size),
+        ("chopper_buffer_size", chopper_buffer_size),
+    ):
         if buffer_size < 1:
             raise ValueError(f"{buffer_name} must be greater than zero")
 
 
 def _cleanup_queue(queue: Optional[mp.Queue]):
     if queue is not None:
         queue.cancel_join_thread()
         queue.close()
         queue.join_thread()
 
 
 async def _data_stream(
-        data_queue: mp.Queue,
-        worker_instruction_queue: mp.Queue,
-        kafka_broker: str,
-        topics: Optional[List[str]],
-        interval: sc.Variable,
-        event_buffer_size: int,
-        slow_metadata_buffer_size: int,
-        fast_metadata_buffer_size: int,
-        chopper_buffer_size: int,
-        run_info_topic: Optional[str] = None,
-        start_at: StartTime = StartTime.NOW,
-        end_at: StopTime = StopTime.NEVER,
-        query_consumer: Optional["KafkaQueryConsumer"] = None,  # noqa: F821
-        consumer_type: ConsumerType = ConsumerType.REAL,
-        halt_after_n_data_chunks: int = np.iinfo(np.int32).max,  # noqa: B008
-        halt_after_n_warnings: int = np.iinfo(np.int32).max,  # noqa: B008
-        test_message_queue: Optional[mp.Queue] = None,  # for tests
-        timeout: Optional[sc.Variable] = None,  # for tests
+    data_queue: mp.Queue,
+    worker_instruction_queue: mp.Queue,
+    kafka_broker: str,
+    topics: Optional[List[str]],
+    interval: sc.Variable,
+    event_buffer_size: int,
+    slow_metadata_buffer_size: int,
+    fast_metadata_buffer_size: int,
+    chopper_buffer_size: int,
+    run_info_topic: Optional[str] = None,
+    start_at: StartTime = StartTime.NOW,
+    end_at: StopTime = StopTime.NEVER,
+    query_consumer: Optional["KafkaQueryConsumer"] = None,  # noqa: F821
+    consumer_type: ConsumerType = ConsumerType.REAL,
+    halt_after_n_data_chunks: int = np.iinfo(np.int32).max,  # noqa: B008
+    halt_after_n_warnings: int = np.iinfo(np.int32).max,  # noqa: B008
+    test_message_queue: Optional[mp.Queue] = None,  # for tests
+    timeout: Optional[sc.Variable] = None,  # for tests
 ) -> Generator[sc.DataArray, None, None]:
     """
     Main implementation of data stream is extracted to this function so that
     fake consumers can be injected for unit tests
     """
 
     # Search backwards to find the last run_start message
     try:
         from ._consumer import KafkaQueryConsumer, get_run_start_message
-        from ._data_consumption_manager import InstructionType, ManagerInstruction, \
-            data_consumption_manager
+        from ._data_consumption_manager import (
+            InstructionType,
+            ManagerInstruction,
+            data_consumption_manager,
+        )
     except ImportError:
         raise ImportError(_missing_dependency_message)
 
     if topics is None and run_info_topic is None:
-        raise ValueError("At least one of 'topics' and 'run_info_topic'"
-                         " must be specified")
+        raise ValueError(
+            "At least one of 'topics' and 'run_info_topic'" " must be specified"
+        )
 
     # This is defaulted to None in the function signature
     # to avoid it having to be imported earlier
     if query_consumer is None:
         query_consumer = KafkaQueryConsumer(kafka_broker)
 
     # stream_info contains information on where to look for data and metadata.
@@ -190,20 +211,22 @@
         run_id = run_start_info.job_id
         run_title = run_start_info.run_name
         # default value for stop_time in message flatbuffer is 0,
         # it means that field has not been populated
         if end_at == StopTime.END_OF_RUN and run_start_info.stop_time != 0:
             stop_time_ms = run_start_info.stop_time
         if topics is None:
-            loaded_data, stream_info = _load_nexus_json(run_start_info.nexus_structure,
-                                                        get_start_info=True)
+            loaded_data, stream_info = _load_nexus_json(
+                run_start_info.nexus_structure, get_start_info=True
+            )
             topics = [stream.topic for stream in stream_info]
         else:
-            loaded_data, _ = _load_nexus_json(run_start_info.nexus_structure,
-                                              get_start_info=False)
+            loaded_data, _ = _load_nexus_json(
+                run_start_info.nexus_structure, get_start_info=False
+            )
         topics.append(run_info_topic)  # listen for stop run message
         yield loaded_data
         n_data_chunks += 1
 
     if start_at == StartTime.START_OF_RUN:
         start_time = run_start_info.start_time * sc.Unit("milliseconds")
     else:
@@ -224,35 +247,51 @@
     # https://pytorch.org/docs/stable/notes/multiprocessing.html
     #
     # Note also that daemonising this Process is important so that resources are
     # properly freed when restarting the notebook kernel (or shutting down the
     # notebook entirely).
     data_collect_process = mp.get_context("spawn").Process(
         target=data_consumption_manager,
-        args=(start_time_ms, stop_time_ms, run_id, topics, kafka_broker, consumer_type,
-              stream_info, interval_s, event_buffer_size, slow_metadata_buffer_size,
-              fast_metadata_buffer_size, chopper_buffer_size, worker_instruction_queue,
-              data_queue, test_message_queue),
-        daemon=True)
+        args=(
+            start_time_ms,
+            stop_time_ms,
+            run_id,
+            topics,
+            kafka_broker,
+            consumer_type,
+            stream_info,
+            interval_s,
+            event_buffer_size,
+            slow_metadata_buffer_size,
+            fast_metadata_buffer_size,
+            chopper_buffer_size,
+            worker_instruction_queue,
+            data_queue,
+            test_message_queue,
+        ),
+        daemon=True,
+    )
     try:
-        data_stream_widget = DataStreamWidget(start_time_ms=start_time_ms,
-                                              stop_time_ms=stop_time_ms,
-                                              run_title=run_title)
+        data_stream_widget = DataStreamWidget(
+            start_time_ms=start_time_ms, stop_time_ms=stop_time_ms, run_title=run_title
+        )
         data_collect_process.start()
 
         # When testing, if something goes wrong, the while loop below can
         # become infinite. So we introduce a timeout.
         if timeout is not None:
             start_timeout = time.time()
             timeout_s = float(sc.to_unit(timeout, 's').value)
         n_warnings = 0
-        while data_collect_process.is_alive(
-        ) and n_data_chunks < halt_after_n_data_chunks and \
-                n_warnings < halt_after_n_warnings and \
-                not data_stream_widget.stop_requested:
+        while (
+            data_collect_process.is_alive()
+            and n_data_chunks < halt_after_n_data_chunks
+            and n_warnings < halt_after_n_warnings
+            and not data_stream_widget.stop_requested
+        ):
             if timeout is not None and (time.time() - start_timeout) > timeout_s:
                 raise TimeoutError("data_stream timed out in test")
             try:
                 new_data = data_queue.get_nowait()
 
                 if isinstance(new_data, Warning):
                     # Raise warnings in this process so that they
@@ -260,25 +299,27 @@
                     warn(new_data)
                     n_warnings += 1
                     continue
                 elif isinstance(new_data, StopTimeUpdate):
                     data_stream_widget.set_stop_time(new_data.stop_time_ms)
                     if end_at == StopTime.END_OF_RUN:
                         worker_instruction_queue.put(
-                            ManagerInstruction(InstructionType.UPDATE_STOP_TIME,
-                                               new_data.stop_time_ms))
+                            ManagerInstruction(
+                                InstructionType.UPDATE_STOP_TIME, new_data.stop_time_ms
+                            )
+                        )
                     continue
                 n_data_chunks += 1
                 yield convert_from_pickleable_dict(new_data)
             except QueueEmpty:
                 await asyncio.sleep(0.5 * interval_s)
     finally:
         # Ensure cleanup happens however the loop exits
         worker_instruction_queue.put(ManagerInstruction(InstructionType.STOP_NOW))
         if data_collect_process.is_alive():
-            process_halt_timeout_s = 4.
+            process_halt_timeout_s = 4.0
             data_collect_process.join(process_halt_timeout_s)
         if data_collect_process.is_alive():
             data_collect_process.terminate()
         for queue in (data_queue, worker_instruction_queue, test_message_queue):
             _cleanup_queue(queue)
         data_stream_widget.set_stopped()
```

### Comparing `scippneutron-23.3.0/src/scippneutron/instrument_view.py` & `scippneutron-23.4.0/src/scippneutron/instrument_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,47 +15,49 @@
 
 def _create_text_sprite(position, bounding_box, display_text):
     # Position offset in y
     text_position = tuple(position.value + np.array([0, 0.8 * bounding_box[1], 0]))
     text = p3.TextTexture(string=display_text, color='black', size=300)
     text_material = p3.SpriteMaterial(map=text, transparent=True)
     size = 1.0
-    return p3.Sprite(material=text_material,
-                     position=text_position,
-                     scale=[size, size, size])
+    return p3.Sprite(
+        material=text_material, position=text_position, scale=[size, size, size]
+    )
 
 
 def _create_mesh(geometry, color, wireframe, position):
     if wireframe:
         edges = p3.EdgesGeometry(geometry)
-        mesh = p3.LineSegments(geometry=edges,
-                               material=p3.LineBasicMaterial(color=color))
+        mesh = p3.LineSegments(
+            geometry=edges, material=p3.LineBasicMaterial(color=color)
+        )
 
     else:
         material = p3.MeshBasicMaterial(color=color)
         mesh = p3.Mesh(geometry=geometry, material=material)
     mesh.position = tuple(position.value)
     return mesh
 
 
 def _box(position, display_text, bounding_box, color, wireframe, **kwargs):
-    geometry = p3.BoxGeometry(width=bounding_box[0],
-                              height=bounding_box[1],
-                              depth=bounding_box[2],
-                              widthSegments=2,
-                              heightSegments=2,
-                              depthSegments=2)
-
-    mesh = _create_mesh(geometry=geometry,
-                        color=color,
-                        wireframe=wireframe,
-                        position=position)
-    text_mesh = _create_text_sprite(position=position,
-                                    bounding_box=bounding_box,
-                                    display_text=display_text)
+    geometry = p3.BoxGeometry(
+        width=bounding_box[0],
+        height=bounding_box[1],
+        depth=bounding_box[2],
+        widthSegments=2,
+        heightSegments=2,
+        depthSegments=2,
+    )
+
+    mesh = _create_mesh(
+        geometry=geometry, color=color, wireframe=wireframe, position=position
+    )
+    text_mesh = _create_text_sprite(
+        position=position, bounding_box=bounding_box, display_text=display_text
+    )
     return mesh, text_mesh
 
 
 def _find_beam(det_com, pos):
     # Assume beam is axis aligned and follows largest axis
     # delta between component and detector COM
     beam_dir = np.argmax(np.abs(det_com.value - pos.value))
@@ -68,75 +70,81 @@
     rot_axis = np.cross(to_align, target)
     magnitude = np.linalg.norm(to_align) * np.linalg.norm(target)
     axis_angle = np.arcsin(rot_axis / magnitude)
     return Rot.from_rotvec(axis_angle).as_matrix()
 
 
 def _disk_chopper(position, display_text, bounding_box, color, wireframe, **kwargs):
-    geometry = p3.CylinderGeometry(radiusTop=bounding_box[0] / 2,
-                                   radiusBottom=bounding_box[0] / 2,
-                                   height=bounding_box[0] / 100,
-                                   radialSegments=24,
-                                   heightSegments=12,
-                                   openEnded=False,
-                                   thetaStart=np.pi / 8,
-                                   thetaLength=2 * np.pi - (np.pi / 8))
-
-    mesh = _create_mesh(geometry=geometry,
-                        color=color,
-                        wireframe=wireframe,
-                        position=position)
+    geometry = p3.CylinderGeometry(
+        radiusTop=bounding_box[0] / 2,
+        radiusBottom=bounding_box[0] / 2,
+        height=bounding_box[0] / 100,
+        radialSegments=24,
+        heightSegments=12,
+        openEnded=False,
+        thetaStart=np.pi / 8,
+        thetaLength=2 * np.pi - (np.pi / 8),
+    )
+
+    mesh = _create_mesh(
+        geometry=geometry, color=color, wireframe=wireframe, position=position
+    )
     beam = _find_beam(det_com=kwargs['det_center'], pos=position)
     disk_axis = np.array([0, 1, 0])  # Disk created with this axis
     rotation = _alignment_matrix(to_align=disk_axis, target=beam)
     mesh.setRotationFromMatrix(rotation.flatten())
-    text_mesh = _create_text_sprite(position=position,
-                                    bounding_box=bounding_box,
-                                    display_text=display_text)
+    text_mesh = _create_text_sprite(
+        position=position, bounding_box=bounding_box, display_text=display_text
+    )
     return mesh, text_mesh
 
 
 def _cylinder(position, display_text, bounding_box, color, wireframe, **kwargs):
-    geometry = p3.CylinderGeometry(radiusTop=bounding_box[0] / 2,
-                                   radiusBottom=bounding_box[0] / 2,
-                                   height=bounding_box[1],
-                                   radialSegments=12,
-                                   heightSegments=12,
-                                   openEnded=False,
-                                   thetaStart=0,
-                                   thetaLength=2.0 * np.pi)
-    mesh = _create_mesh(geometry=geometry,
-                        color=color,
-                        wireframe=wireframe,
-                        position=position)
+    geometry = p3.CylinderGeometry(
+        radiusTop=bounding_box[0] / 2,
+        radiusBottom=bounding_box[0] / 2,
+        height=bounding_box[1],
+        radialSegments=12,
+        heightSegments=12,
+        openEnded=False,
+        thetaStart=0,
+        thetaLength=2.0 * np.pi,
+    )
+    mesh = _create_mesh(
+        geometry=geometry, color=color, wireframe=wireframe, position=position
+    )
     # Position label above cylinder
-    text_mesh = _create_text_sprite(position=position,
-                                    bounding_box=bounding_box,
-                                    display_text=display_text)
+    text_mesh = _create_text_sprite(
+        position=position, bounding_box=bounding_box, display_text=display_text
+    )
     return mesh, text_mesh
 
 
 def _unpack_to_scene(scene, items):
     if hasattr(items, "__iter__"):
         for item in items:
             scene.add(item)
     else:
         scene.add(items)
 
 
-def _add_to_scene(position, scene, shape, display_text, bounding_box, color, wireframe,
-                  **kwargs):
+def _add_to_scene(
+    position, scene, shape, display_text, bounding_box, color, wireframe, **kwargs
+):
     _unpack_to_scene(
         scene,
-        shape(position,
-              display_text=display_text,
-              bounding_box=bounding_box,
-              color=color,
-              wireframe=wireframe,
-              **kwargs))
+        shape(
+            position,
+            display_text=display_text,
+            bounding_box=bounding_box,
+            color=color,
+            wireframe=wireframe,
+            **kwargs,
+        ),
+    )
 
 
 def _furthest_component(det_center, scipp_obj, additional):
     distances = [
         sc.norm(settings["center"] - det_center).value
         for settings in list(additional.values())
     ]
@@ -148,60 +156,62 @@
     return {"box": _box, "cylinder": _cylinder, "disk": _disk_chopper}
 
 
 def _as_vector(var):
     if var.dtype == sc.DType.vector3:
         return var
     else:
-        return sc.geometry.position(x=var, y=var, z=var)
+        return sc.spatial.as_vectors(x=var, y=var, z=var)
 
 
 def _plot_components(scipp_obj, components, positions_var, scene):
     det_center = sc.mean(positions_var)
     # Some scaling to set width according to distance from detector center
     shapes = _instrument_view_shape_types()
     for name, settings in components.items():
         type = settings["type"]
         size = _as_vector(settings["size"])
         component_position = settings["center"]
         color = settings.get("color", "#808080")
         wireframe = settings.get("wireframe", False)
         if type not in shapes:
             supported_shapes = ", ".join(shapes.keys())
-            raise ValueError(f"Unknown shape: {type} requested for {name}. "
-                             f"Allowed values are: {supported_shapes}")
+            raise ValueError(
+                f"Unknown shape: {type} requested for {name}. "
+                f"Allowed values are: {supported_shapes}"
+            )
         component_position = sc.to_unit(component_position, positions_var.unit)
         size = sc.to_unit(size, positions_var.unit)
-        _add_to_scene(position=component_position,
-                      scene=scene,
-                      shape=shapes[type],
-                      display_text=name,
-                      bounding_box=tuple(size.values),
-                      color=color,
-                      wireframe=wireframe,
-                      det_center=det_center)
+        _add_to_scene(
+            position=component_position,
+            scene=scene,
+            shape=shapes[type],
+            display_text=name,
+            bounding_box=tuple(size.values),
+            color=color,
+            wireframe=wireframe,
+            det_center=det_center,
+        )
     # Reset camera
     camera = _get_camera(scene)
     if camera:
         furthest_distance = _furthest_component(det_center, scipp_obj, components)
         camera.far = max(camera.far, furthest_distance * 5.0)
 
 
 def _get_camera(scene):
     for child in scene.children:
         if isinstance(child, p3.PerspectiveCamera):
             return child
     return None
 
 
-def instrument_view(scipp_obj,
-                    positions="position",
-                    pixel_size=None,
-                    components=None,
-                    **kwargs):
+def instrument_view(
+    scipp_obj, positions="position", pixel_size=None, components=None, **kwargs
+):
     """
     :param scipp_obj: scipp object holding geometries
     :param positions: Key for coord/attr holding positions to use for pixels
     :param pixel_size: Custom pixel size to use for detector pixels
     :param components: Dictionary containing display names and corresponding
     settings (also a Dictionary) for additional components to display
      items with known positions to be shown
@@ -250,24 +260,27 @@
 
     positions_var = scipp_obj.meta[positions]
     if pixel_size is None:
         pos_array = positions_var.values
         if len(pos_array) > 1:
             pixel_size = np.linalg.norm(pos_array[1] - pos_array[0])
 
-    if (pp is not None) and ((sc.plot is pp.plot)
-                             or sc.config['plot'].get('use_plopp')):
+    if (pp is not None) and (
+        (sc.plot is pp.plot) or sc.config['plot'].get('use_plopp')
+    ):
         fig = pp.scatter3d(scipp_obj, pos=positions, pixel_size=pixel_size, **kwargs)
         scene = fig.children[0].canvas.scene
     else:
-        fig = sc.plot(scipp_obj,
-                      projection="3d",
-                      positions=positions,
-                      pixel_size=pixel_size,
-                      **kwargs)
+        fig = sc.plot(
+            scipp_obj,
+            projection="3d",
+            positions=positions,
+            pixel_size=pixel_size,
+            **kwargs,
+        )
         scene = fig.view.figure.scene
 
     # Add additional components from the beamline
     if components:
         _plot_components(scipp_obj, components, positions_var, scene)
 
     return fig
```

### Comparing `scippneutron-23.3.0/src/scippneutron/io/nexus/_json_nexus.py` & `scippneutron-23.4.0/src/scippneutron/io/nexus/_json_nexus.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,30 +29,30 @@
     "int16": np.int32,
     "int32": np.int32,
     "int64": np.int64,
     "uint8": np.int32,
     "uint16": np.int32,
     "uint32": np.int32,
     "uint64": np.int64,
-    "string": np.str_
+    "string": np.str_,
 }
 
 numpy_to_filewriter_type = {
     np.float32: "float32",
     np.float64: "float64",
     np.int8: "int8",
     np.int16: "int16",
     np.int32: "int32",
     np.int64: "int64",
     np.uint8: "uint8",
     np.uint16: "uint16",
     np.uint32: "uint32",
     np.uint64: "uint64",
     np.str_: "string",
-    np.object_: "string"
+    np.object_: "string",
 }
 
 
 class MissingAttribute(Exception):
     pass
 
 
@@ -64,15 +64,15 @@
     elif isinstance(value, int):
         attr_info = {"size": 1, "type": "int64"}
     elif isinstance(value, list):
         attr_info = {"size": len(value), "type": "string"}
     else:
         attr_info = {
             "size": value.shape,
-            "type": numpy_to_filewriter_type[value.dtype.type]
+            "type": numpy_to_filewriter_type[value.dtype.type],
         }
     name_and_value = {"name": name, "values": value}
     return {**attr_info, **name_and_value}
 
 
 def make_json_dataset(name: str, data) -> dict:
     if isinstance(data, (str, bytes)):
@@ -80,28 +80,29 @@
     elif isinstance(data, float):
         dataset_info = {"size": 1, "type": "float64"}
     elif isinstance(data, int):
         dataset_info = {"size": 1, "type": "int32"}
     else:
         dataset_info = {
             "size": data.shape,
-            "type": numpy_to_filewriter_type[data.dtype.type]
+            "type": numpy_to_filewriter_type[data.dtype.type],
         }
 
     return {
         "type": "dataset",
         "name": name,
         "values": data,
         "dataset": dataset_info,
-        "attributes": []
+        "attributes": [],
     }
 
 
-def _get_attribute_value(element: Dict,
-                         attribute_name: str) -> Union[str, float, int, List]:
+def _get_attribute_value(
+    element: Dict, attribute_name: str
+) -> Union[str, float, int, List]:
     """
     attributes can be a dictionary of key-value pairs, or an array
     of dictionaries with key, value, type, etc
     """
     try:
         attributes = element["attributes"]
         try:
@@ -112,47 +113,51 @@
                     return attribute[_nexus_values]
     except KeyError:
         pass
     raise MissingAttribute
 
 
 class _Node(dict):
-
     def __init__(self, parent: dict, name: str, file: dict, group: dict):
         super().__init__(**group)
         self.parent = parent
         self.name = name
         self.file = file
 
 
-def _visit_nodes(root: Dict, group: Dict, nx_class_names: Tuple[str, ...],
-                 groups_with_requested_nx_class: Dict[str,
-                                                      List[H5Group]], path: List[str]):
+def _visit_nodes(
+    root: Dict,
+    group: Dict,
+    nx_class_names: Tuple[str, ...],
+    groups_with_requested_nx_class: Dict[str, List[H5Group]],
+    path: List[str],
+):
     try:
         for child in group[_nexus_children]:
             try:
                 path.append(child[_nexus_name])
             except KeyError:
                 # If the object doesn't have a name it can't be a NeXus
                 # class we are looking for, nor can it be a group
                 # containing a NeXus class we are looking for, so skip to
                 # next object
                 continue
             try:
                 nx_class = _get_attribute_value(child, _nexus_class)
                 if nx_class in nx_class_names:
                     groups_with_requested_nx_class[nx_class].append(
-                        _Node(group=child, parent=group, name="/".join(path),
-                              file=root))
+                        _Node(group=child, parent=group, name="/".join(path), file=root)
+                    )
             except MissingAttribute:
                 # It may be a group but not an NX_class,
                 # that's fine, continue to its children
                 pass
-            _visit_nodes(root, child, nx_class_names, groups_with_requested_nx_class,
-                         path)
+            _visit_nodes(
+                root, child, nx_class_names, groups_with_requested_nx_class, path
+            )
             path.pop(-1)
     except KeyError:
         pass
 
 
 def contains_stream(group: Dict) -> bool:
     """
@@ -178,53 +183,55 @@
 
 def _find_by_type(type_name: str, root: Dict) -> List[H5Group]:
     """
     Finds objects with the requested "type" value
     Returns a list of objects with requested type
     """
 
-    def _visit_nodes_for_type(obj: Dict, requested_type: str,
-                              objects_found: List[H5Group]):
+    def _visit_nodes_for_type(
+        obj: Dict, requested_type: str, objects_found: List[H5Group]
+    ):
         try:
             for child in obj[_nexus_children]:
                 if child["type"] == requested_type:
                     objects_found.append(
-                        _Node(group=child,
-                              parent=obj,
-                              name="",
-                              file={_nexus_children: [obj]}))
+                        _Node(
+                            group=child,
+                            parent=obj,
+                            name="",
+                            file={_nexus_children: [obj]},
+                        )
+                    )
                 _visit_nodes_for_type(child, requested_type, objects_found)
         except KeyError:
             # If this object does not have "children" array then go to next
             pass
 
     objects_with_requested_type: List[H5Group] = []
     _visit_nodes_for_type(root, type_name, objects_with_requested_type)
 
     return objects_with_requested_type
 
 
-class JSONTypeStringID():
-
+class JSONTypeStringID:
     def get_cset(self):
         import h5py
+
         return h5py.h5t.CSET_UTF8
 
 
 class JSONAttrID:
-
     def __init__(self):
         pass
 
     def get_type(self):
         return JSONTypeStringID()
 
 
 class JSONAttributeManager:
-
     def __init__(self, node: dict):
         self._node = node
 
     def __contains__(self, name):
         try:
             self[name]
         except MissingAttribute:
@@ -255,15 +262,14 @@
     def get_id(self, name) -> JSONAttrID:
         # TODO This is a hack that only works since this is used only for a single
         # purpose by scippnexus.NXobject
         return JSONAttrID()
 
 
 class JSONNode:
-
     def __init__(self, node: dict, *, parent=None):
         self._file = parent.file if parent is not None else self
         self._parent = self if parent is None else parent
         self._node = node
         if parent is None or parent.name == '/':
             self._name = f'/{self._node.get(_nexus_name, "")}'
         else:
@@ -283,15 +289,14 @@
 
     @property
     def parent(self):
         return self._parent
 
 
 class JSONDataset(JSONNode):
-
     @property
     def dtype(self) -> str:
         try:
             dtype = self._node[_nexus_dataset]["type"]
         except KeyError:
             dtype = self._node[_nexus_dataset]["dtype"]
         if dtype == 'string':
@@ -313,15 +318,14 @@
         buf[...] = self[source_sel]
 
     def asstr(self, **ignored):
         return self
 
 
 class JSONGroup(JSONNode):
-
     def __contains__(self, name: str) -> bool:
         try:
             self[name]
             return True
         except KeyError:
             return False
 
@@ -358,20 +362,20 @@
 
         raise KeyError(f"Unable to open object (object '{name}' doesn't exist)")
 
     def __iter__(self):
         yield from self.keys()
 
     def visititems(self, callable):
-
         def skip(node):
             return node['type'] == _nexus_link or contains_stream(self)
 
         children = [
-            child[_nexus_name] for child in self._node[_nexus_children]
+            child[_nexus_name]
+            for child in self._node[_nexus_children]
             if not skip(child)
         ]
         for key in children:
             item = self[key]
             callable(key, item)
             if isinstance(item, JSONGroup):
                 item.visititems(callable)
@@ -415,10 +419,16 @@
         units = "dimensionless"
         try:
             units = _get_attribute_value(stream.parent, _nexus_units)
         except MissingAttribute:
             pass
 
         streams.append(
-            StreamInfo(stream["stream"]["topic"], stream["stream"]["writer_module"],
-                       stream["stream"]["source"], dtype, units))
+            StreamInfo(
+                stream["stream"]["topic"],
+                stream["stream"]["writer_module"],
+                stream["stream"]["source"],
+                dtype,
+                units,
+            )
+        )
     return streams
```

### Comparing `scippneutron-23.3.0/src/scippneutron/io/nexus/load_nexus.py` & `scippneutron-23.4.0/src/scippneutron/io/nexus/load_nexus.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,30 +21,35 @@
 
 
 class BadSource(Exception):
     """
     Raise if something is wrong with data source which
     prevents it being used. Warn the user.
     """
+
     pass
 
 
 class SkipSource(Exception):
     """
     Raise to abort using the data source, do not
     warn the user.
     """
+
     pass
 
 
-def add_position_and_transforms_to_data(data: Union[sc.DataArray,
-                                                    sc.Dataset], transform_name: str,
-                                        position_name: str, base_position_name: str,
-                                        transforms: sc.Variable,
-                                        positions: sc.Variable):
+def add_position_and_transforms_to_data(
+    data: Union[sc.DataArray, sc.Dataset],
+    transform_name: str,
+    position_name: str,
+    base_position_name: str,
+    transforms: sc.Variable,
+    positions: sc.Variable,
+):
     if isinstance(data, sc.DataArray):
         coords = data.coords
         attrs = data.attrs
     else:
         coords = data
         attrs = data
 
@@ -73,16 +78,18 @@
     else:
         yield file_in
 
 
 def _load_instrument_name(instruments: Dict[str, NXobject]) -> Dict:
     instrument = next(iter(instruments.values()))
     if len(instruments) > 1:
-        warn(f"More than one NXinstrument found in file, "
-             f"loading name from {instrument.name} only")
+        warn(
+            f"More than one NXinstrument found in file, "
+            f"loading name from {instrument.name} only"
+        )
     if (name := instrument.get("name")) is not None:
         return {"instrument_name": sc.scalar(name[()])}
     return {}
 
 
 def _load_title(entry: NXobject) -> Dict:
     if (title := entry.get('title')) is not None:
@@ -94,17 +101,17 @@
     times = {}
     for time in ["start_time", "end_time"]:
         if (dataset := entry.get(time)) is not None:
             times[time] = sc.scalar(dataset[()])
     return times
 
 
-def load_nexus(data_file: Union[str, Path, h5py.File],
-               root: str = "/",
-               quiet=True) -> Optional[ScippData]:
+def load_nexus(
+    data_file: Union[str, Path, h5py.File], root: str = "/", quiet=True
+) -> Optional[ScippData]:
     """
     Load a NeXus file and return required information.
 
     :param data_file: path of NeXus file containing data to load
     :param root: path of group in file, only load data from the subtree of
       this group
     :param quiet: if False prints some details of what is being loaded
@@ -124,16 +131,18 @@
 
 def _origin(unit) -> sc.Variable:
     return sc.vector(value=[0, 0, 0], unit=unit)
 
 
 def _depends_on_to_position(obj) -> Union[None, sc.Variable]:
     if (transform := obj.get('depends_on')) is not None:
-        if isinstance(transform,
-                      (str, sc.DataArray)) or transform.dtype == sc.DType.DataArray:
+        if (
+            isinstance(transform, (str, sc.DataArray))
+            or transform.dtype == sc.DType.DataArray
+        ):
             return None  # cannot compute position if bad transform or time-dependent
         else:
             if transform.dtype == sc.DType.rotation3:
                 return transform * _origin('m')
             else:
                 return transform.to(unit='m') * _origin('m')
 
@@ -141,17 +150,19 @@
 def _monitor_to_canonical(monitor):
     if isinstance(monitor, sc.DataGroup):
         return monitor
     if monitor.bins is not None:
         monitor.bins.coords['tof'] = monitor.bins.coords.pop('event_time_offset')
         monitor.bins.coords['detector_id'] = monitor.bins.coords.pop('event_id')
         monitor.bins.coords['pulse_time'] = sc.bins_like(
-            monitor, fill_value=monitor.coords.pop('event_time_zero'))
+            monitor, fill_value=monitor.coords.pop('event_time_zero')
+        )
         da = sc.DataArray(
-            sc.broadcast(monitor.data.bins.concat('pulse'), dims=['tof'], shape=[1]))
+            sc.broadcast(monitor.data.bins.concat('pulse'), dims=['tof'], shape=[1])
+        )
     else:
         da = monitor.copy(deep=False)
     if (position := _depends_on_to_position(monitor.coords)) is not None:
         da.coords['position'] = position
     return da
 
 
@@ -171,14 +182,15 @@
         offset.fields.z = z.to(dtype='float64', unit=x.unit, copy=False)
     da.coords['pixel_offset'] = offset.rename_dims(dict(zip(offset.dims, da.dims)))
     return da
 
 
 def _by_nx_class(group) -> Dict[str, Dict[str, 'NXobject']]:
     from scippnexus.nxobject import _nx_class_registry
+
     classes = {name: [] for name in _nx_class_registry()}
 
     def _match_nx_class(_, node):
         if not hasattr(node, 'shape'):
             if (nx_class := node.attrs.get('NX_class')) is not None:
                 if not isinstance(nx_class, str):
                     nx_class = nx_class.decode('UTF-8')
@@ -192,30 +204,33 @@
         names = [group.name.split('/')[-1] for group in groups]
         if len(names) != len(set(names)):  # fall back to full path if duplicate
             names = [group.name for group in groups]
         out[nx_class] = {n: group._make(g) for n, g in zip(names, groups)}
     return out
 
 
-def _load_data(nexus_file: Union[h5py.File, Dict], root: Optional[str],
-               quiet: bool) -> Optional[ScippData]:
+def _load_data(
+    nexus_file: Union[h5py.File, Dict], root: Optional[str], quiet: bool
+) -> Optional[ScippData]:
     """
     Main implementation for loading data is extracted to this function so that
     in-memory data can be used for unit tests.
     """
     root = NXroot(nexus_file if root is None else nexus_file[root])
     classes = _by_nx_class(root)
 
     if len(classes['NXentry']) > 1:
         # We can't sensibly load from multiple NXentry, for example each
         # could could contain a description of the same detector bank
         # and lead to problems with clashing detector ids etc
-        raise RuntimeError(f"More than one NXentry group in file, use 'root' argument "
-                           "to specify which to load data from, for example"
-                           f"{__name__}('my_file.nxs', '/entry_2')")
+        raise RuntimeError(
+            f"More than one NXentry group in file, use 'root' argument "
+            "to specify which to load data from, for example"
+            f"{__name__}('my_file.nxs', '/entry_2')"
+        )
 
     # In the following, we map the file structure onto a partially flattened in-memory
     # structure. This behavior is quite error prone and cumbersome and will probably
     # disappear in this form. We therefore keep this length code directly in this
     # function to provide an overview and facility future refactoring steps.
     detectors = classes.get('NXdetector', {})
     loaded_detectors = []
@@ -232,26 +247,35 @@
                 det.coords['detector_id'] = det.coords.pop('detector_number')
             elif 'pixel_id' in det.coords:
                 det.coords['detector_id'] = det.coords.pop('pixel_id')
             elif 'spectrum_index' in det.coords:
                 det.coords['detector_id'] = det.coords.pop('spectrum_index')
             else:
                 raise KeyError(
-                    "Found neither of detector_number, pixel_id, or spectrum_index.")
+                    "Found neither of detector_number, pixel_id, or spectrum_index."
+                )
             if 'pixel_offset' in det.coords:
                 add_position_and_transforms_to_data(
                     data=det,
                     transform_name="position_transformations",
                     position_name="position",
                     base_position_name="base_position",
                     positions=det.coords.pop('pixel_offset'),
-                    transforms=det.coords.pop('depends_on', None))
+                    transforms=det.coords.pop('depends_on', None),
+                )
             loaded_detectors.append(det)
-        except (BadSource, SkipSource, NexusStructureError, KeyError, sc.DTypeError,
-                ValueError, IndexError) as e:
+        except (
+            BadSource,
+            SkipSource,
+            NexusStructureError,
+            KeyError,
+            sc.DTypeError,
+            ValueError,
+            IndexError,
+        ) as e:
             if not contains_stream(group._group):
                 warn(f"Skipped loading {group.name} due to:\n{e}")
 
     no_event_data = True
     loaded_data = sc.Dataset()
 
     # If no event data are found, make a Dataset and add the metadata as
@@ -271,86 +295,97 @@
                 events.bins.coords['tof'] = events.bins.coords.pop('event_time_offset')
                 events.bins.coords['detector_id'] = events.bins.coords.pop('event_id')
                 det_min = events.bins.coords['detector_id'].min().value
                 det_max = events.bins.coords['detector_id'].max().value
                 if len(events.bins.constituents['data']) != 0:
                     # See scipp/scipp#2490
                     det_id = sc.arange('detector_id', det_min, det_max + 1, unit=None)
-                    events = make_binned(events,
-                                         groups=[det_id],
-                                         erase=['pulse', 'bank'])
+                    events = make_binned(
+                        events, groups=[det_id], erase=['pulse', 'bank']
+                    )
                 loaded_events.append(events)
             except (BadSource, SkipSource, NexusStructureError, IndexError) as e:
                 if not contains_stream(group._group):
                     warn(f"Skipped loading {group.name} due to:\n{e}")
         if len(loaded_events):
             no_event_data = False
             loaded_data = sc.concat(loaded_events, 'detector_id')
 
     if not no_event_data:
         # Add single tof bin
-        loaded_data = sc.DataArray(loaded_data.data.fold(dim='detector_id',
-                                                         sizes={
-                                                             'detector_id': -1,
-                                                             'tof': 1
-                                                         }),
-                                   coords=dict(loaded_data.coords.items()),
-                                   attrs=dict(loaded_data.attrs.items()))
+        loaded_data = sc.DataArray(
+            loaded_data.data.fold(
+                dim='detector_id', sizes={'detector_id': -1, 'tof': 1}
+            ),
+            coords=dict(loaded_data.coords.items()),
+            attrs=dict(loaded_data.attrs.items()),
+        )
         tof_min = loaded_data.bins.coords['tof'].min().to(dtype='float64')
         tof_max = loaded_data.bins.coords['tof'].max().to(dtype='float64')
         tof_max.value = np.nextafter(tof_max.value, float("inf"))
         loaded_data.coords['tof'] = sc.concat([tof_min, tof_max], 'tof')
 
     def add_metadata(metadata: Dict[str, sc.Variable]):
         for key, value in metadata.items():
             if isinstance(loaded_data, sc.DataArray):
                 loaded_data.attrs[key] = value
             else:
                 loaded_data[key] = value
 
-    if (entries := classes['NXentry']):
+    if entries := classes['NXentry']:
         entry = next(iter(entries.values()))
         add_metadata(_load_title(entry))
         add_metadata(_load_start_and_end_time(entry))
-    if (instruments := classes['NXinstrument']):
+    if instruments := classes['NXinstrument']:
         add_metadata(_load_instrument_name(instruments))
 
     def load_and_add_metadata(groups, process=lambda x: x):
         items = {}
         loaded_groups = []
         for name, group in groups.items():
             try:
                 items[name] = sc.scalar(process(group[()]))
                 loaded_groups.append(name)
-            except (BadSource, SkipSource, TransformationError, sc.DimensionError,
-                    sc.UnitError, NexusStructureError, KeyError, ValueError) as e:
+            except (
+                BadSource,
+                SkipSource,
+                TransformationError,
+                sc.DimensionError,
+                sc.UnitError,
+                NexusStructureError,
+                KeyError,
+                ValueError,
+            ) as e:
                 if not contains_stream(group._group):
                     warn(f"Skipped loading {group.name} due to:\n{e}")
         add_metadata(items)
         return loaded_groups
 
     load_and_add_metadata(classes.get('NXdisk_chopper', {}))
     load_and_add_metadata(classes.get('NXlog', {}))
     load_and_add_metadata(classes.get('NXmonitor', {}), _monitor_to_canonical)
     for name, tag in {'sample': 'NXsample', 'source': 'NXsource'}.items():
         comps = classes.get(tag, {})
         comps = load_and_add_metadata(comps)
-        attrs = loaded_data if isinstance(loaded_data,
-                                          sc.Dataset) else loaded_data.attrs
-        coords = loaded_data if isinstance(loaded_data,
-                                           sc.Dataset) else loaded_data.coords
+        attrs = (
+            loaded_data if isinstance(loaded_data, sc.Dataset) else loaded_data.attrs
+        )
+        coords = (
+            loaded_data if isinstance(loaded_data, sc.Dataset) else loaded_data.coords
+        )
         for comp_name in comps:
             comp = attrs[comp_name].value
             if (position := _depends_on_to_position(comp)) is not None:
                 coords[f'{comp_name}_position'] = position
             elif (distance := comp.get('distance')) is not None:
                 if not isinstance(distance, sc.Variable):
                     distance = sc.scalar(distance, unit=None)
                 coords[f'{comp_name}_position'] = sc.vector(
-                    value=[0, 0, distance.value], unit=distance.unit)
+                    value=[0, 0, distance.value], unit=distance.unit
+                )
             elif name == 'sample':
                 coords[f'{comp_name}_position'] = _origin('m')
 
     # Return None if we have an empty dataset at this point
     if no_event_data and not loaded_data.keys():
         loaded_data = None
     return loaded_data
```

### Comparing `scippneutron-23.3.0/src/scippneutron/io/xye.py` & `scippneutron-23.4.0/src/scippneutron/io/xye.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 import numpy as np
 import scipp as sc
 
 from ..logging import get_logger
 
 
 class GenerateHeaderType:
-
     def __repr__(self) -> str:
         return 'GenerateHeader'
 
 
 GenerateHeader = GenerateHeaderType()
 
 
-def save_xye(fname: Union[str, Path, io.TextIOBase],
-             da: sc.DataArray,
-             *,
-             coord: Optional[str] = None,
-             header: Union[str, GenerateHeaderType] = GenerateHeader) -> None:
+def save_xye(
+    fname: Union[str, Path, io.TextIOBase],
+    da: sc.DataArray,
+    *,
+    coord: Optional[str] = None,
+    header: Union[str, GenerateHeaderType] = GenerateHeader,
+) -> None:
     """Write a data array to an XYE file.
 
     The input must be 1-dimensional, have variances, and at least one coordinate.
     It is possible to select which coordinate gets written with the ``coord`` argument.
 
     The data are written as an ASCII table with columns X, Y, E, where
 
@@ -63,35 +64,45 @@
     See Also
     --------
     scippneutron.io.xye.load_xye:
         Function to load XYE files.
     """
     if da.variances is None:
         raise sc.VariancesError(
-            'Cannot save data to XYE file because it has no variances.')
+            'Cannot save data to XYE file because it has no variances.'
+        )
     if da.ndim != 1:
         raise sc.DimensionError(
             'Cannot save data to XYE file because it is not one-dimensional. '
-            f'It has dimensions {da.dims}')
+            f'It has dimensions {da.dims}'
+        )
     if da.masks:
-        raise ValueError('Cannot save data to XYE file because it has masks: '
-                         f'{list(da.masks.keys())}')
+        raise ValueError(
+            'Cannot save data to XYE file because it has masks: '
+            f'{list(da.masks.keys())}'
+        )
     if len(da.coords) == 0:
         raise ValueError('Cannot save data to XYE file because it has no coordinates.')
     coord = _deduce_coord(da) if coord is None else coord
     if da.coords.is_edges(coord):
-        raise sc.CoordError('Cannot save data with bin-edges to XYE file. '
-                            'Compute bin-centers before calling save_xye. '
-                            'Use, e.g., scipp.midpoints for linearly spaced bins.')
+        raise sc.CoordError(
+            'Cannot save data with bin-edges to XYE file. '
+            'Compute bin-centers before calling save_xye. '
+            'Use, e.g., scipp.midpoints for linearly spaced bins.'
+        )
     to_save = np.c_[da.coords[coord].values, da.values, np.sqrt(da.variances)]
     if header is GenerateHeader:
         header = _generate_xye_header(da, coord)
 
-    get_logger().info("Saving data with unit %s and coordinate '%s' to XYE file %s",
-                      da.unit, coord, fname)
+    get_logger().info(
+        "Saving data with unit %s and coordinate '%s' to XYE file %s",
+        da.unit,
+        coord,
+        fname,
+    )
     np.savetxt(fname, to_save, delimiter=' ', header=header)
 
 
 def load_xye(
     fname: Union[str, Path, io.TextIOBase],
     *,
     dim: str,
@@ -131,20 +142,20 @@
         Function to write XYE files.
     """
     coord = dim if coord is None else coord
     loaded = np.loadtxt(fname, delimiter=' ', unpack=True)
     if loaded.ndim == 1:
         loaded = loaded[:, np.newaxis]
     return sc.DataArray(
-        sc.array(dims=[dim], values=loaded[1], variances=loaded[2]**2, unit=unit),
-        coords={coord: sc.array(dims=[dim], values=loaded[0], unit=coord_unit)})
+        sc.array(dims=[dim], values=loaded[1], variances=loaded[2] ** 2, unit=unit),
+        coords={coord: sc.array(dims=[dim], values=loaded[0], unit=coord_unit)},
+    )
 
 
 def _generate_xye_header(da: sc.DataArray, coord: str) -> str:
-
     def format_unit(unit):
         return f'[{unit}]' if unit is not None else ''
 
     c = f'{coord} {format_unit(da.coords[coord].unit)}'
     y = f'Y {format_unit(da.unit)}'
     e = f'E {format_unit(da.unit)}'
     # Widths are for the default format of `0.0`
@@ -154,9 +165,10 @@
 def _deduce_coord(da: sc.DataArray) -> str:
     if len(da.coords) == 1:
         return next(iter(da.coords))
     if len(da.coords) > 1 and da.dim not in da.coords:
         raise ValueError(
             'Cannot deduce which coordinate to save because the data has more '
             f'than one and no dimension-coordinate (dim={da.dim}): '
-            f'{list(da.coords.keys())}')
+            f'{list(da.coords.keys())}'
+        )
     return da.dim
```

### Comparing `scippneutron-23.3.0/src/scippneutron/logging.py` & `scippneutron-23.4.0/src/scippneutron/logging.py`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/src/scippneutron/mantid.py` & `scippneutron-23.4.0/src/scippneutron/mantid.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         from mantid import simpleapi as mantid
         from mantid.api import AnalysisDataService
     except ImportError:
         raise ImportError(
             "Mantid Python API was not found, please install Mantid framework "
             "as detailed in the installation instructions ("
             "https://scipp.github.io/scippneutron/getting-started/"
-            "installation.html)")
+            "installation.html)"
+        )
     # Deal with multiple calls to this function, which may have conflicting
     # names in the global AnalysisDataService by using uuid.
     ws_name = f'scipp.run_mantid_alg.{uuid.uuid4()}'
     # Deal with non-standard ways to define the prefix of output workspaces
     if alg == 'Fit':
         kwargs['Output'] = ws_name
     elif alg == 'LoadDiffCal':
@@ -42,16 +43,19 @@
     finally:
         for name in AnalysisDataService.Instance().getObjectNames():
             if name.startswith(ws_name):
                 mantid.DeleteWorkspace(name)
 
 
 def get_pos(pos):
-    return None if pos is None else sc.vector(
-        value=[pos.X(), pos.Y(), pos.Z()], unit=sc.units.m)
+    return (
+        None
+        if pos is None
+        else sc.vector(value=[pos.X(), pos.Y(), pos.Z()], unit=sc.units.m)
+    )
 
 
 def make_run(ws):
     return sc.scalar(deepcopy(ws.run()))
 
 
 additional_unit_mapping = {
@@ -68,16 +72,18 @@
         except RuntimeError:  # TODO catch UnitError once exposed from C++
             # Parsing unit string failed
             unit = None
 
         values = deepcopy(ws.run()[property_name].value)
 
         if units_string and unit is None:
-            warnings.warn(f"Workspace run log '{property_name}' "
-                          f"has unrecognised units: '{units_string}'")
+            warnings.warn(
+                f"Workspace run log '{property_name}' "
+                f"has unrecognised units: '{units_string}'"
+            )
         if unit is None:
             unit = sc.units.one
 
         try:
             times = deepcopy(ws.run()[property_name].times)
             is_time_series = True
             dimension_label = "time"
@@ -85,26 +91,26 @@
             times = None
             is_time_series = False
             dimension_label = property_name
 
         if np.isscalar(values):
             property_data = sc.scalar(values, unit=unit)
         else:
-            property_data = sc.Variable(values=values,
-                                        unit=unit,
-                                        dims=[dimension_label])
+            property_data = sc.Variable(
+                values=values, unit=unit, dims=[dimension_label]
+            )
 
         if is_time_series:
             # If property has timestamps, create a DataArray
-            data_array = sc.DataArray(data=property_data,
-                                      coords={
-                                          dimension_label:
-                                          sc.Variable(dims=[dimension_label],
-                                                      values=times)
-                                      })
+            data_array = sc.DataArray(
+                data=property_data,
+                coords={
+                    dimension_label: sc.Variable(dims=[dimension_label], values=times)
+                },
+            )
             yield property_name, sc.scalar(data_array)
         elif not np.isscalar(values):
             # If property is multi-valued, create a wrapper single
             # value variable. This prevents interference with
             # global dimensions for for output Dataset.
             yield property_name, sc.scalar(property_data)
         else:
@@ -114,16 +120,17 @@
 def make_mantid_sample(ws):
     return sc.scalar(deepcopy(ws.sample()))
 
 
 def make_sample_ub(ws):
     # B matrix transforms the h,k,l triplet into a Cartesian system
     # https://docs.mantidproject.org/nightly/concepts/Lattice.html
-    return sc.spatial.linear_transform(value=ws.sample().getOrientedLattice().getUB(),
-                                       unit=sc.units.angstrom**-1)
+    return sc.spatial.linear_transform(
+        value=ws.sample().getOrientedLattice().getUB(), unit=sc.units.angstrom**-1
+    )
 
 
 def make_sample_u(ws):
     # U matrix rotation for sample alignment
     # https://docs.mantidproject.org/nightly/concepts/Lattice.html
     return sc.spatial.linear_transform(value=ws.sample().getOrientedLattice().getU())
 
@@ -144,35 +151,36 @@
     return get_pos(sourcePos), get_pos(samplePos)
 
 
 def make_detector_info(ws, spectrum_dim):
     det_info = ws.detectorInfo()
     # det -> spec mapping
     nDet = det_info.size()
-    spectrum = np.empty(shape=(nDet, ), dtype=np.int32)
-    has_spectrum = np.full((nDet, ), False)
+    spectrum = np.empty(shape=(nDet,), dtype=np.int32)
+    has_spectrum = np.full((nDet,), False)
     spec_info = ws.spectrumInfo()
     for i, spec in enumerate(spec_info):
         spec_def = spec.spectrumDefinition
         for j in range(len(spec_def)):
             det, time = spec_def[j]
             if time != 0:
                 raise RuntimeError(
                     "Conversion of Mantid Workspace with scanning instrument "
-                    "not supported yet.")
+                    "not supported yet."
+                )
             spectrum[det] = i
             has_spectrum[det] = True
 
     # Store only information about detectors with data (a spectrum). The rest
     # mostly just gets in the way and including it in the default converter
     # is probably not required.
     spectrum = sc.array(dims=['detector'], values=spectrum[has_spectrum], unit=None)
-    detector = sc.array(dims=['detector'],
-                        values=det_info.detectorIDs()[has_spectrum],
-                        unit=None)
+    detector = sc.array(
+        dims=['detector'], values=det_info.detectorIDs()[has_spectrum], unit=None
+    )
 
     # May want to include more information here, such as detector positions,
     # but for now this is not necessary.
 
     return sc.scalar(sc.Dataset(coords={'detector': detector, spectrum_dim: spectrum}))
 
 
@@ -200,23 +208,25 @@
     pattern_result = zip(patterns, dims)
     for pattern, result in pattern_result:
         if re.search(pattern, mantid_dim.name, re.IGNORECASE):
             return result
 
     raise ValueError(
         "Cannot infer scipp dimension from input mantid dimension {}".format(
-            mantid_dim.name()))
+            mantid_dim.name()
+        )
+    )
 
 
 def md_unit(frame):
     known_md_units = {
         "Angstrom^-1": sc.units.dimensionless / sc.units.angstrom,
         "r.l.u": sc.units.dimensionless,
         "T": sc.units.K,
-        "DeltaE": sc.units.meV
+        "DeltaE": sc.units.meV,
     }
     if frame.getUnitLabel().ascii() in known_md_units:
         return known_md_units[frame.getUnitLabel().ascii()]
     else:
         return sc.units.dimensionless
 
 
@@ -229,46 +239,49 @@
     known_units = {
         "DeltaE": ['energy_transfer', sc.units.meV],
         "TOF": ['tof', sc.units.us],
         "Wavelength": ['wavelength', sc.units.angstrom],
         "Energy": ['energy', sc.units.meV],
         "dSpacing": ['dspacing', sc.units.angstrom],
         "MomentumTransfer": ['Q', sc.units.dimensionless / sc.units.angstrom],
-        "QSquared":
-        ['Q^2', sc.units.dimensionless / (sc.units.angstrom * sc.units.angstrom)],
+        "QSquared": [
+            'Q^2',
+            sc.units.dimensionless / (sc.units.angstrom * sc.units.angstrom),
+        ],
         "Spectrum": ['spectrum', None],
         "Empty": ['empty', sc.units.dimensionless],
-        "Counts": ['counts', sc.units.counts]
+        "Counts": ['counts', sc.units.counts],
     }
 
     if unit not in known_units.keys():
         return [str(unit), sc.units.dimensionless]
     else:
         return known_units[unit]
 
 
 def _to_spherical(pos, output):
     output["r"] = sc.sqrt(sc.dot(pos, pos))
     output["t"] = sc.acos(pos.fields.z / output["r"].data)
     signed_phi = sc.atan2(y=pos.fields.y, x=pos.fields.x)
     abs_phi = sc.abs(signed_phi)
-    output["p-delta"] = (np.pi *
-                         sc.units.rad) - abs_phi  # angular delta (magnitude) from pole
+    output["p-delta"] = (
+        np.pi * sc.units.rad
+    ) - abs_phi  # angular delta (magnitude) from pole
     output['p-sign'] = signed_phi  # weighted sign of phi
     return output
 
 
 def _rot_from_vectors(vec1, vec2):
     a = sc.vector(value=vec1.value / np.linalg.norm(vec1.value))
     b = sc.vector(value=vec2.value / np.linalg.norm(vec2.value))
     c = sc.vector(value=np.cross(a.value, b.value))
     angle = sc.acos(sc.dot(a, b)).value
-    return sc.spatial.linear_transform(
-        value=sc.geometry.rotation_matrix_from_quaternion_coeffs(
-            list(c.value * np.sin(angle / 2)) + [np.cos(angle / 2)]))
+    return sc.spatial.rotation(
+        value=list(c.value * np.sin(angle / 2)) + [np.cos(angle / 2)]
+    )
 
 
 def get_detector_pos(ws, spectrum_dim):
     nHist = ws.getNumberHistograms()
     pos = np.zeros([nHist, 3])
 
     spec_info = ws.spectrumInfo()
@@ -279,43 +292,42 @@
             pos[i, 1] = p.Y()
             pos[i, 2] = p.Z()
         else:
             pos[i, :] = [np.nan, np.nan, np.nan]
     return sc.vectors(dims=[spectrum_dim], values=pos, unit=sc.units.m)
 
 
-def get_detector_properties(ws,
-                            source_pos,
-                            sample_pos,
-                            spectrum_dim,
-                            advanced_geometry=False):
+def get_detector_properties(
+    ws, source_pos, sample_pos, spectrum_dim, advanced_geometry=False
+):
     if not advanced_geometry:
         return (get_detector_pos(ws, spectrum_dim), None, None)
     spec_info = ws.spectrumInfo()
     det_info = ws.detectorInfo()
     comp_info = ws.componentInfo()
     nspec = len(spec_info)
-    det_rot = np.zeros([nspec, 3, 3])
+    det_rot_quaternions = np.zeros([nspec, 4])
     det_bbox = np.zeros([nspec, 3])
 
     if sample_pos is not None and source_pos is not None:
         total_detectors = spec_info.detectorCount()
-        act_beam = (sample_pos - source_pos)
+        act_beam = sample_pos - source_pos
         rot = _rot_from_vectors(act_beam, sc.vector(value=[0, 0, 1]))
         inv_rot = _rot_from_vectors(sc.vector(value=[0, 0, 1]), act_beam)
 
         pos_d = sc.Dataset()
         # Create empty to hold position info for all spectra detectors
-        pos_d["x"] = sc.zeros(dims=["detector"],
-                              shape=[total_detectors],
-                              unit=sc.units.m)
+        pos_d["x"] = sc.zeros(
+            dims=["detector"], shape=[total_detectors], unit=sc.units.m
+        )
         pos_d["y"] = sc.zeros_like(pos_d["x"])
         pos_d["z"] = sc.zeros_like(pos_d["x"])
-        pos_d.coords[spectrum_dim] = sc.array(dims=["detector"],
-                                              values=np.empty(total_detectors))
+        pos_d.coords[spectrum_dim] = sc.array(
+            dims=["detector"], values=np.empty(total_detectors)
+        )
 
         spectrum_values = pos_d.coords[spectrum_dim].values
 
         x_values = pos_d["x"].values
         y_values = pos_d["y"].values
         z_values = pos_d["z"].values
 
@@ -335,45 +347,50 @@
                     y_values[idx] = p.Y()
                     z_values[idx] = p.Z()
                     idx += 1
                     quats.append(np.array([r.imagI(), r.imagJ(), r.imagK(), r.real()]))
                     if comp_info.hasValidShape(det_idx):
                         s = comp_info.shape(det_idx)
                         bboxes.append(s.getBoundingBox().width())
-                det_rot[i, :] = sc.geometry.rotation_matrix_from_quaternion_coeffs(
-                    np.mean(quats, axis=0))
+                det_rot_quaternions[i] = np.mean(quats, axis=0)
                 det_bbox[i, :] = np.sum(bboxes, axis=0)
 
-        rot_pos = rot * sc.geometry.position(pos_d["x"].data, pos_d["y"].data,
-                                             pos_d["z"].data)
+        rot_pos = rot * sc.spatial.as_vectors(
+            pos_d["x"].data, pos_d["y"].data, pos_d["z"].data
+        )
 
         _to_spherical(rot_pos, pos_d)
 
-        averaged = sc.groupby(pos_d,
-                              spectrum_dim,
-                              bins=sc.Variable(dims=[spectrum_dim],
-                                               values=np.arange(
-                                                   -0.5,
-                                                   len(spec_info) + 0.5,
-                                                   1.0))).mean("detector")
+        averaged = sc.groupby(
+            pos_d,
+            spectrum_dim,
+            bins=sc.Variable(
+                dims=[spectrum_dim], values=np.arange(-0.5, len(spec_info) + 0.5, 1.0)
+            ),
+        ).mean("detector")
 
         sign = averaged["p-sign"].data / sc.abs(averaged["p-sign"].data)
         averaged["p"] = sign * ((np.pi * sc.units.rad) - averaged["p-delta"].data)
-        averaged["x"] = averaged["r"].data * sc.sin(averaged["t"].data) * sc.cos(
-            averaged["p"].data)
-        averaged["y"] = averaged["r"].data * sc.sin(averaged["t"].data) * sc.sin(
-            averaged["p"].data)
+        averaged["x"] = (
+            averaged["r"].data * sc.sin(averaged["t"].data) * sc.cos(averaged["p"].data)
+        )
+        averaged["y"] = (
+            averaged["r"].data * sc.sin(averaged["t"].data) * sc.sin(averaged["p"].data)
+        )
         averaged["z"] = averaged["r"].data * sc.cos(averaged["t"].data)
 
-        pos = sc.geometry.position(averaged["x"].data, averaged["y"].data,
-                                   averaged["z"].data)
-
-        return (inv_rot * pos,
-                sc.spatial.linear_transforms(dims=[spectrum_dim], values=det_rot),
-                sc.vectors(dims=[spectrum_dim], values=det_bbox, unit=sc.units.m))
+        pos = sc.spatial.as_vectors(
+            averaged["x"].data, averaged["y"].data, averaged["z"].data
+        )
+
+        return (
+            inv_rot * pos,
+            sc.spatial.rotations(dims=[spectrum_dim], values=det_rot_quaternions),
+            sc.vectors(dims=[spectrum_dim], values=det_bbox, unit=sc.units.m),
+        )
     else:
         pos = np.zeros([nspec, 3])
 
         for i, spec in enumerate(spec_info):
             if spec.hasDetectors:
                 definition = spec_info.getSpectrumDefinition(i)
                 n_dets = len(definition)
@@ -386,28 +403,29 @@
                     r = det_info.rotation(det_idx)
                     vec3s.append([p.X(), p.Y(), p.Z()])
                     quats.append(np.array([r.imagI(), r.imagJ(), r.imagK(), r.real()]))
                     if comp_info.hasValidShape(det_idx):
                         s = comp_info.shape(det_idx)
                         bboxes.append(s.getBoundingBox().width())
                 pos[i, :] = np.mean(vec3s, axis=0)
-                det_rot[i, :] = sc.geometry.rotation_matrix_from_quaternion_coeffs(
-                    np.mean(quats, axis=0))
+                det_rot_quaternions[i] = np.mean(quats, axis=0)
                 det_bbox[i, :] = np.sum(bboxes, axis=0)
             else:
                 pos[i, :] = [np.nan, np.nan, np.nan]
-                det_rot[i, :] = [np.nan, np.nan, np.nan, np.nan]
+                det_rot_quaternions[i] = [np.nan, np.nan, np.nan, np.nan]
                 det_bbox[i, :] = [np.nan, np.nan, np.nan]
-        return (sc.vectors(dims=[spectrum_dim], values=pos, unit=sc.units.m),
-                sc.spatial.linear_transforms(dims=[spectrum_dim], values=det_rot),
-                sc.vectors(
-                    dims=[spectrum_dim],
-                    values=det_bbox,
-                    unit=sc.units.m,
-                ))
+        return (
+            sc.vectors(dims=[spectrum_dim], values=pos, unit=sc.units.m),
+            sc.spatial.rotations(dims=[spectrum_dim], values=det_rot_quaternions),
+            sc.vectors(
+                dims=[spectrum_dim],
+                values=det_bbox,
+                unit=sc.units.m,
+            ),
+        )
 
 
 def _get_dtype_from_values(values, coerce_floats_to_ints):
     if coerce_floats_to_ints and np.all(np.mod(values, 1.0) == 0.0):
         dtype = sc.DType.int32
     elif hasattr(values, 'dtype'):
         dtype = values.dtype
@@ -417,19 +435,21 @@
             if dtype is str:
                 dtype = sc.DType.string
             elif dtype is int:
                 dtype = sc.DType.int64
             elif dtype is float:
                 dtype = sc.DType.float64
             else:
-                raise RuntimeError("Cannot handle the dtype that this "
-                                   "workspace has on Axis 1.")
+                raise RuntimeError(
+                    "Cannot handle the dtype that this " "workspace has on Axis 1."
+                )
         else:
-            raise RuntimeError("Axis 1 of this workspace has no values. "
-                               "Cannot determine dtype.")
+            raise RuntimeError(
+                "Axis 1 of this workspace has no values. " "Cannot determine dtype."
+            )
     return dtype
 
 
 def init_spec_axis(ws):
     axis = ws.getAxis(1)
     dim, unit = validate_and_get_unit(axis.getUnit())
     values = axis.extractValues()
@@ -440,41 +460,41 @@
 def set_bin_masks(bin_masks, dim, index, masked_bins):
     for masked_bin in masked_bins:
         bin_masks['spectrum', index][dim, masked_bin].value = True
 
 
 def _convert_MatrixWorkspace_info(ws, advanced_geometry=False, load_run_logs=True):
     from mantid.kernel import DeltaEModeType
+
     common_bins = ws.isCommonBins()
     dim, unit = validate_and_get_unit(ws.getAxis(0).getUnit())
     source_pos, sample_pos = make_component_info(ws)
     spec_dim, spec_coord = init_spec_axis(ws)
-    pos, rot, shp = get_detector_properties(ws,
-                                            source_pos,
-                                            sample_pos,
-                                            spec_dim,
-                                            advanced_geometry=advanced_geometry)
+    pos, rot, shp = get_detector_properties(
+        ws, source_pos, sample_pos, spec_dim, advanced_geometry=advanced_geometry
+    )
 
     coords = {spec_dim: spec_coord}
     # possible x - coord
     if not ws.id() == 'MaskWorkspace':
         if common_bins:
             coords[dim] = sc.Variable(dims=[dim], values=ws.readX(0), unit=unit)
         else:
-            coords[dim] = sc.Variable(dims=[spec_dim, dim],
-                                      values=ws.extractX(),
-                                      unit=unit)
+            coords[dim] = sc.Variable(
+                dims=[spec_dim, dim], values=ws.extractX(), unit=unit
+            )
 
     info = {
         "coords": coords,
         "masks": {},
         "attrs": {
             "sample": make_mantid_sample(ws),
-            "instrument_name":
-            sc.scalar(ws.componentInfo().name(ws.componentInfo().root()))
+            "instrument_name": sc.scalar(
+                ws.componentInfo().name(ws.componentInfo().root())
+            ),
         },
     }
 
     if load_run_logs:
         for run_log_name, run_log_variable in make_variables_from_run_logs(ws):
             info["attrs"][run_log_name] = run_log_variable
 
@@ -492,92 +512,97 @@
 
     if sample_pos is not None:
         info["coords"]["sample_position"] = sample_pos
 
     if ws.detectorInfo().hasMaskedDetectors():
         spectrum_info = ws.spectrumInfo()
         mask = np.array(
-            [spectrum_info.isMasked(i) for i in range(ws.getNumberHistograms())])
+            [spectrum_info.isMasked(i) for i in range(ws.getNumberHistograms())]
+        )
         info["masks"][spec_dim] = sc.Variable(dims=[spec_dim], values=mask)
 
     if ws.getEMode() == DeltaEModeType.Direct:
         info["coords"]["incident_energy"] = _extract_einitial(ws)
     elif ws.getEMode() == DeltaEModeType.Indirect:
         info["coords"]["final_energy"] = _extract_efinal(ws, spec_dim)
 
     if ws.sample().hasOrientedLattice():
-        info["attrs"].update({
-            "sample_ub": make_sample_ub(ws),
-            "sample_u": make_sample_u(ws)
-        })
+        info["attrs"].update(
+            {"sample_ub": make_sample_ub(ws), "sample_u": make_sample_u(ws)}
+        )
     return info
 
 
 def convert_monitors_ws(ws, converter, **ignored):
     spec_dim, spec_coord = init_spec_axis(ws)
     spec_info = ws.spectrumInfo()
     comp_info = ws.componentInfo()
     monitors = []
-    spec_indices = ((ws.getIndexFromSpectrumNumber(int(i)), i)
-                    for i in spec_coord.values)
+    spec_indices = (
+        (ws.getIndexFromSpectrumNumber(int(i)), i) for i in spec_coord.values
+    )
     for index, number in spec_indices:
         definition = spec_info.getSpectrumDefinition(index)
         if not definition.size() == 1:
             raise RuntimeError("Cannot deal with grouped monitor detectors")
         det_index = definition[0][0]  # Ignore time index
         # We only ExtractSpectra for compatibility with
         # existing convert_Workspace2D_to_dataarray. This could instead be
         # refactored if found to be slow
-        with run_mantid_alg('ExtractSpectra',
-                            InputWorkspace=ws,
-                            WorkspaceIndexList=[index]) as monitor_ws:
+        with run_mantid_alg(
+            'ExtractSpectra', InputWorkspace=ws, WorkspaceIndexList=[index]
+        ) as monitor_ws:
             # Run logs are already loaded in the data workspace
             single_monitor = converter(monitor_ws, load_run_logs=False)
         # Storing sample_position as a coord of monitors means that monitor
         # data cannot be combined with scattered data even after conversion
         # to wavelength, d-spacing, etc. because conversions of monitors do
         # not use the sample position.
         # But keep it as an attr in case a user needs it.
         single_monitor.attrs['sample_position'] = single_monitor.coords.pop(
-            'sample_position')
+            'sample_position'
+        )
         # Remove redundant information that is duplicated from workspace
         # We get this extra information from the generic converter reuse
         if 'detector_info' in single_monitor.coords:
             del single_monitor.coords['detector_info']
         del single_monitor.attrs['sample']
         name = comp_info.name(det_index)
         if not comp_info.uniqueName(name):
             name = f'{name}_{number}'
         monitors.append((name, single_monitor))
     return monitors
 
 
-def convert_Workspace2D_to_data_array(ws,
-                                      load_run_logs=True,
-                                      advanced_geometry=False,
-                                      **ignored):
-
+def convert_Workspace2D_to_data_array(
+    ws, load_run_logs=True, advanced_geometry=False, **ignored
+):
     dim, unit = validate_and_get_unit(ws.getAxis(0).getUnit())
     spec_dim, spec_coord = init_spec_axis(ws)
 
     coords_labs_data = _convert_MatrixWorkspace_info(
-        ws, advanced_geometry=advanced_geometry, load_run_logs=load_run_logs)
+        ws, advanced_geometry=advanced_geometry, load_run_logs=load_run_logs
+    )
     _, data_unit = validate_and_get_unit(ws.YUnit(), allow_empty=True)
     if ws.id() == 'MaskWorkspace':
-        coords_labs_data["data"] = sc.Variable(dims=[spec_dim],
-                                               unit=data_unit,
-                                               values=ws.extractY().flatten(),
-                                               dtype=sc.DType.bool)
+        coords_labs_data["data"] = sc.Variable(
+            dims=[spec_dim],
+            unit=None,
+            values=ws.extractY().flatten(),
+            dtype=sc.DType.bool,
+        )
     else:
         stddev2 = ws.extractE()
         np.multiply(stddev2, stddev2, out=stddev2)  # much faster than np.power
-        coords_labs_data["data"] = sc.Variable(dims=[spec_dim, dim],
-                                               unit=data_unit,
-                                               values=ws.extractY(),
-                                               variances=stddev2)
+        coords_labs_data["data"] = sc.Variable(
+            dims=[spec_dim, dim],
+            unit=data_unit,
+            values=ws.extractY(),
+            variances=stddev2,
+        )
     array = sc.DataArray(**coords_labs_data)
 
     if ws.hasAnyMaskedBins():
         bin_mask = sc.zeros(dims=array.dims, shape=array.shape, dtype=sc.DType.bool)
         for i in range(ws.getNumberHistograms()):
             # maskedBinsIndices throws instead of returning empty list
             if ws.hasMaskedBins(i):
@@ -596,69 +621,76 @@
             array.coords['position'] = array.coords['position'][spec_dim, 0]
         array = array[spec_dim, 0].copy()
     return array
 
 
 def _contains_weighted_events(spectrum) -> bool:
     from mantid.api import EventType
+
     return spectrum.getEventType() in (EventType.WEIGHTED, EventType.WEIGHTED_NOTIME)
 
 
-def convert_EventWorkspace_to_data_array(ws,
-                                         load_pulse_times=True,
-                                         advanced_geometry=False,
-                                         load_run_logs=True,
-                                         **ignored):
+def convert_EventWorkspace_to_data_array(
+    ws, load_pulse_times=True, advanced_geometry=False, load_run_logs=True, **ignored
+):
     dim, unit = validate_and_get_unit(ws.getAxis(0).getUnit())
     spec_dim, spec_coord = init_spec_axis(ws)
     nHist = ws.getNumberHistograms()
     _, data_unit = validate_and_get_unit(ws.YUnit(), allow_empty=True)
 
     n_event = ws.getNumberEvents()
     coord = sc.empty(dims=['event'], shape=[n_event], unit=unit, dtype=sc.DType.float64)
-    weights = sc.ones(dims=['event'],
-                      shape=[n_event],
-                      unit=data_unit,
-                      dtype=sc.DType.float32,
-                      with_variances=True)
-    pulse_times = sc.empty(
-        dims=['event'], shape=[n_event], dtype=sc.DType.datetime64,
-        unit=sc.units.ns) if load_pulse_times else None
-
-    begins = sc.zeros(dims=[spec_dim, dim],
-                      shape=[nHist, 1],
-                      dtype=sc.DType.int64,
-                      unit=None)
+    weights = sc.ones(
+        dims=['event'],
+        shape=[n_event],
+        unit=data_unit,
+        dtype=sc.DType.float32,
+        with_variances=True,
+    )
+    pulse_times = (
+        sc.empty(
+            dims=['event'], shape=[n_event], dtype=sc.DType.datetime64, unit=sc.units.ns
+        )
+        if load_pulse_times
+        else None
+    )
+
+    begins = sc.zeros(
+        dims=[spec_dim, dim], shape=[nHist, 1], dtype=sc.DType.int64, unit=None
+    )
     ends = begins.copy()
     if n_event > 0:  # Skip expensive loop if there are no events
         current = 0
         for i in range(nHist):
             sp = ws.getSpectrum(i)
             size = sp.getNumberEvents()
             begins.values[i] = current
             ends.values[i] = current + size
             if size == 0:  # Skip expensive getters
                 continue
-            coord['event', current:current + size].values = sp.getTofs()
+            coord['event', current : current + size].values = sp.getTofs()
             if load_pulse_times:
-                pulse_times['event',
-                            current:current + size].values = sp.getPulseTimesAsNumpy()
+                pulse_times[
+                    'event', current : current + size
+                ].values = sp.getPulseTimesAsNumpy()
             if _contains_weighted_events(sp):
-                weights['event', current:current + size].values = sp.getWeights()
-                weights['event',
-                        current:current + size].variances = sp.getWeightErrors()
+                weights['event', current : current + size].values = sp.getWeights()
+                weights[
+                    'event', current : current + size
+                ].variances = sp.getWeightErrors()
             current += size
 
     proto_events = {'data': weights, 'coords': {dim: coord}}
     if load_pulse_times:
         proto_events["coords"]["pulse_time"] = pulse_times
     events = sc.DataArray(**proto_events)
 
     coords_labs_data = _convert_MatrixWorkspace_info(
-        ws, advanced_geometry=advanced_geometry, load_run_logs=load_run_logs)
+        ws, advanced_geometry=advanced_geometry, load_run_logs=load_run_logs
+    )
     # For now we ignore potential finer bin edges to avoid creating too many
     # bins. Use just a single bin along dim and use extents given by workspace
     # edges.
     # TODO If there are events outside edges this might create bins with
     # events that are not within bin bounds. Consider using `bin` instead
     # of `bins`?
     edges = coords_labs_data['coords'][dim]
@@ -673,24 +705,26 @@
     ndims = md_histo.getNumDims()
     coords = dict()
     dims_used = []
     for i in range(ndims):
         dim = md_histo.getDimension(i)
         frame = dim.getMDFrame()
         sc_dim = md_dimension(dim, i)
-        coords[sc_dim] = sc.Variable(dims=[sc_dim],
-                                     values=np.linspace(dim.getMinimum(),
-                                                        dim.getMaximum(),
-                                                        dim.getNBins()),
-                                     unit=md_unit(frame))
+        coords[sc_dim] = sc.Variable(
+            dims=[sc_dim],
+            values=np.linspace(dim.getMinimum(), dim.getMaximum(), dim.getNBins()),
+            unit=md_unit(frame),
+        )
         dims_used.append(sc_dim)
-    data = sc.Variable(dims=dims_used,
-                       values=md_histo.getSignalArray(),
-                       variances=md_histo.getErrorSquaredArray(),
-                       unit=sc.units.counts)
+    data = sc.Variable(
+        dims=dims_used,
+        values=md_histo.getSignalArray(),
+        variances=md_histo.getErrorSquaredArray(),
+        unit=sc.units.counts,
+    )
     nevents = sc.Variable(dims=dims_used, values=md_histo.getNumEventsArray())
     return sc.DataArray(coords=coords, data=data, attrs={'nevents': nevents})
 
 
 def convert_TableWorkspace_to_dataset(ws, error_connection=None, **ignored):
     """
     Converts from a Mantid TableWorkspace to a scipp dataset.
@@ -729,57 +763,65 @@
         elif data_name in error_connection:
             # This data has error available
             error_name = error_connection[data_name]
             error_index = columnNames.index(error_name)
 
             if columnTypes[error_index] in blacklist_variance_types:
                 # Raise error to avoid numpy square error for strings
-                raise RuntimeError("Variance can not have type string. \n" +
-                                   "Data:     " + str(data_name) + "\n" + "Variance: " +
-                                   str(error_name) + "\n")
-
-            variance = np.array(ws.column(error_name))**2
-            dataset[data_name] = sc.Variable(dims=['row'],
-                                             values=np.array(ws.column(i)),
-                                             variances=variance)
+                raise RuntimeError(
+                    "Variance can not have type string. \n"
+                    + "Data:     "
+                    + str(data_name)
+                    + "\n"
+                    + "Variance: "
+                    + str(error_name)
+                    + "\n"
+                )
+
+            variance = np.array(ws.column(error_name)) ** 2
+            dataset[data_name] = sc.Variable(
+                dims=['row'], values=np.array(ws.column(i)), variances=variance
+            )
         elif data_name not in error_connection.values():
             # This data is not an error for another dataset, and has no error
             dataset[data_name] = sc.Variable(dims=['row'], values=ws.column(i))
 
     return dataset
 
 
 def convert_WorkspaceGroup_to_dataarray_dict(group_workspace, **kwargs):
     workspace_dict = {}
     for i in range(group_workspace.getNumberOfEntries()):
         workspace = group_workspace.getItem(i)
-        workspace_name = workspace.name().replace(f'{group_workspace.name()}',
-                                                  '').strip('_')
+        workspace_name = (
+            workspace.name().replace(f'{group_workspace.name()}', '').strip('_')
+        )
         workspace_dict[workspace_name] = from_mantid(workspace, **kwargs)
 
     return workspace_dict
 
 
 def from_mantid(workspace, **kwargs):
     """Convert Mantid workspace to a scipp data array or dataset.
     :param workspace: Mantid workspace to convert.
     """
     scipp_obj = None  # This is either a Dataset or DataArray
     monitor_ws = None
     workspaces_to_delete = []
     w_id = workspace.id()
-    if (w_id == 'Workspace2D' or w_id == 'RebinnedOutput' or w_id == 'MaskWorkspace'):
+    if w_id == 'Workspace2D' or w_id == 'RebinnedOutput' or w_id == 'MaskWorkspace':
         n_monitor = 0
         spec_info = workspace.spectrumInfo()
         for i in range(len(spec_info)):
             if spec_info.hasDetectors(i) and spec_info.isMonitor(i):
                 n_monitor += 1
         # If there are *only* monitors we do not move them to an attribute
         if n_monitor > 0 and n_monitor < len(spec_info):
             import mantid.simpleapi as mantid
+
             workspace, monitor_ws = mantid.ExtractMonitors(workspace)
             workspaces_to_delete.append(workspace)
             workspaces_to_delete.append(monitor_ws)
         scipp_obj = convert_Workspace2D_to_data_array(workspace, **kwargs)
     elif w_id == 'EventWorkspace':
         scipp_obj = convert_EventWorkspace_to_data_array(workspace, **kwargs)
     elif w_id == 'TableWorkspace':
@@ -813,21 +855,23 @@
             scipp_obj.attrs[name] = sc.scalar(monitor)
     for ws in workspaces_to_delete:
         mantid.DeleteWorkspace(ws)
 
     return scipp_obj
 
 
-def load(filename: Union[str, Path] = "",
-         load_pulse_times=True,
-         instrument_filename=None,
-         error_connection=None,
-         mantid_alg='Load',
-         mantid_args=None,
-         advanced_geometry=False) -> sc.Dataset:
+def load(
+    filename: Union[str, Path] = "",
+    load_pulse_times=True,
+    instrument_filename=None,
+    error_connection=None,
+    mantid_alg='Load',
+    mantid_args=None,
+    advanced_geometry=False,
+) -> sc.Dataset:
     """Load a file using Mantid.
 
     Wraps Mantid's loaders and converts the result to a scipp dataset.
 
     See also the neutron-data tutorial.
 
     Note that this function requires mantid to be installed and available in
@@ -882,47 +926,53 @@
         mantid_args = {}
 
     _check_file_path(str(filename), mantid_alg)
 
     with run_mantid_alg(mantid_alg, str(filename), **mantid_args) as loaded:
         # Determine what Load has provided us
         from mantid.api import Workspace
+
         if isinstance(loaded, Workspace):
             # A single workspace
             data_ws = loaded
         else:
             # Separate data and monitor workspaces
             data_ws = loaded.OutputWorkspace
 
         if instrument_filename is not None:
             import mantid.simpleapi as mantid
-            mantid.LoadInstrument(data_ws,
-                                  FileName=instrument_filename,
-                                  RewriteSpectraMap=True)
-        return from_mantid(data_ws,
-                           load_pulse_times=load_pulse_times,
-                           error_connection=error_connection,
-                           advanced_geometry=advanced_geometry)
+
+            mantid.LoadInstrument(
+                data_ws, FileName=instrument_filename, RewriteSpectraMap=True
+            )
+        return from_mantid(
+            data_ws,
+            load_pulse_times=load_pulse_times,
+            error_connection=error_connection,
+            advanced_geometry=advanced_geometry,
+        )
 
 
 def _is_mantid_loadable(filename):
     from mantid.api import FileFinder
+
     if FileFinder.getFullPath(filename):
         return True
     else:
         try:
             # findRuns throws rather than return empty so need try-catch
             FileFinder.findRuns(filename)
             return True
         except Exception:
             return False
 
 
 def _check_file_path(filename, mantid_alg):
     from mantid.api import AlgorithmManager, FileProperty, FrameworkManager
+
     FrameworkManager.Instance()
     alg = AlgorithmManager.createUnmanaged(mantid_alg)
     filename_property = [
         prop for prop in alg.getProperties() if isinstance(prop, FileProperty)
     ]
     # Only with FileProperty can Mantid take fuzzy matches to filenames and run numbers
     # If the top level Load algorithm is requested (has no properties of its own)
@@ -933,15 +983,16 @@
         if not _is_mantid_loadable(filename):
             raise ValueError(
                 f"Mantid cannot find {filename} and therefore will not load it."
             ) from None
     else:
         if not os.path.isfile(filename):
             raise ValueError(
-                f"Cannot find file {filename} and therefore will not load it.")
+                f"Cannot find file {filename} and therefore will not load it."
+            )
 
 
 def validate_dim_and_get_mantid_string(unit_dim):
     known_units = {
         'energy_transfer': "DeltaE",
         'tof': "TOF",
         'wavelength': "Wavelength",
@@ -951,18 +1002,19 @@
         'Q^2': "QSquared",
     }
 
     user_k = str(unit_dim).casefold()
     known_units = {k.casefold(): v for k, v in known_units.items()}
 
     if user_k not in known_units:
-        raise RuntimeError("Axis unit not currently supported."
-                           "Possible values are: {}, "
-                           "got '{}'. ".format([k for k in known_units.keys()],
-                                               unit_dim))
+        raise RuntimeError(
+            "Axis unit not currently supported."
+            "Possible values are: {}, "
+            "got '{}'. ".format([k for k in known_units.keys()], unit_dim)
+        )
     else:
         return known_units[user_k]
 
 
 def to_mantid(data, dim, instrument_file=None):
     """
     Convert data to a Mantid workspace.
@@ -977,22 +1029,24 @@
     :param instrument_file: Instrument file that will be
                             loaded into the workspace
     :returns: Workspace containing converted data. The concrete workspace type
               may differ depending on the content of `data`.
     """
     if not isinstance(data, sc.DataArray):
         raise RuntimeError(
-            "Currently only data arrays can be converted to a Mantid workspace")
+            "Currently only data arrays can be converted to a Mantid workspace"
+        )
     try:
         import mantid.simpleapi as mantid
     except ImportError:
         raise ImportError(
             "Mantid Python API was not found, please install Mantid framework "
             "as detailed in the installation instructions (https://scipp."
-            "github.io/getting-started/installation.html)")
+            "github.io/getting-started/installation.html)"
+        )
     x = data.coords[dim].values
     y = data.values
     e = data.variances
 
     if len(y.shape) not in (1, 2):
         raise ValueError("Currently can only handle 2D data.")
 
@@ -1012,18 +1066,17 @@
         # SCIPP is using a  1:n spectra coord mapping, Mantid needs
         # a 1:1 mapping so expand this out
         x = np.broadcast_to(x, shape=(nspec, len(x)))
 
     nbins = x.shape[1]
     nitems = y.shape[1]
 
-    ws = mantid.WorkspaceFactory.create("Workspace2D",
-                                        NVectors=nspec,
-                                        XLength=nbins,
-                                        YLength=nitems)
+    ws = mantid.WorkspaceFactory.create(
+        "Workspace2D", NVectors=nspec, XLength=nbins, YLength=nitems
+    )
     if data.unit != sc.units.counts:
         ws.setDistribution(True)
 
     for i in range(nspec):
         ws.setX(i, x[i])
         ws.setY(i, y[i])
         ws.setE(i, e[i])
@@ -1037,53 +1090,57 @@
     return ws
 
 
 def _table_to_data_array(table, key, value, stddev):
     stddevs = table[stddev].values
     dim = 'parameter'
     coord = table[key].data.copy().rename_dims({'row': dim})
-    return sc.DataArray(data=sc.Variable(dims=[dim],
-                                         values=table[value].values,
-                                         variances=stddevs * stddevs),
-                        coords={dim: coord})
+    return sc.DataArray(
+        data=sc.Variable(
+            dims=[dim], values=table[value].values, variances=stddevs * stddevs
+        ),
+        coords={dim: coord},
+    )
 
 
 def _fit_workspace(ws, mantid_args):
     """
     Performs a fit on the workspace.
 
     :param ws: The workspace on which the fit will be performed
     :returns: Dataset containing all of Fit's outputs
     """
-    with run_mantid_alg('Fit', InputWorkspace=ws, **mantid_args,
-                        CreateOutput=True) as fit:
+    with run_mantid_alg(
+        'Fit', InputWorkspace=ws, **mantid_args, CreateOutput=True
+    ) as fit:
         # This is assuming that all parameters are dimensionless. If this is
         # not the case we should use a dataset with a scalar variable per
         # parameter instead. Or better, a dict of scalar variables?
         parameters = convert_TableWorkspace_to_dataset(fit.OutputParameters)
-        parameters = _table_to_data_array(parameters,
-                                          key='Name',
-                                          value='Value',
-                                          stddev='Error')
+        parameters = _table_to_data_array(
+            parameters, key='Name', value='Value', stddev='Error'
+        )
         out = convert_Workspace2D_to_data_array(fit.OutputWorkspace)
         data = sc.Dataset()
         data['data'] = out['empty', 0]
         data['calculated'] = out['empty', 1]
         data['diff'] = out['empty', 2]
         parameters.coords['status'] = sc.scalar(fit.OutputStatus)
         parameters.coords['chi^2/d.o.f.'] = sc.scalar(fit.OutputChi2overDoF)
         parameters.coords['function'] = sc.scalar(str(fit.Function))
         parameters.coords['cost_function'] = sc.scalar(fit.CostFunction)
         return parameters, data
 
 
 def fit(data, mantid_args):
     if len(data.dims) != 1 or 'WorkspaceIndex' in mantid_args:
-        raise RuntimeError("Only 1D fitting is supported. Use scipp slicing and do not"
-                           "provide a WorkspaceIndex.")
+        raise RuntimeError(
+            "Only 1D fitting is supported. Use scipp slicing and do not"
+            "provide a WorkspaceIndex."
+        )
     dim = data.dims[0]
     ws = to_mantid(data, dim)
     mantid_args['workspace_index'] = 0
     return _fit_workspace(ws, mantid_args)
 
 
 def _try_except(op, possible_except, failure, **kwargs):
@@ -1117,27 +1174,29 @@
         ei = 0
     return sc.scalar(ei, unit=sc.Unit("meV"))
 
 
 def _extract_efinal(ws, spec_dim):
     detInfo = ws.detectorInfo()
     specInfo = ws.spectrumInfo()
-    ef = np.empty(shape=(specInfo.size(), ), dtype=float)
+    ef = np.empty(shape=(specInfo.size(),), dtype=float)
     ef[:] = np.nan
     analyser_ef = _get_instrument_efixed(workspace=ws)
     ids = detInfo.detectorIDs()
     for spec_index in range(len(specInfo)):
         detector_ef = None
         if specInfo.hasDetectors(spec_index):
             # Just like mantid, we only take the first entry of the group.
             det_index = specInfo.getSpectrumDefinition(spec_index)[0][0]
-            detector_ef = _try_except(op=ws.getEFixed,
-                                      possible_except=RuntimeError,
-                                      failure=None,
-                                      detId=int(ids[det_index]))
+            detector_ef = _try_except(
+                op=ws.getEFixed,
+                possible_except=RuntimeError,
+                failure=None,
+                detId=int(ids[det_index]),
+            )
         detector_ef = detector_ef if detector_ef is not None else analyser_ef
         if not detector_ef:
             continue  # Cannot assign an Ef. May or may not be an error
             # - i.e. a diffraction detector, monitor etc.
         ef[spec_index] = detector_ef
 
     return sc.Variable(dims=[spec_dim], values=ef, unit=sc.Unit("meV"))
```

### Comparing `scippneutron-23.3.0/src/scippneutron/tof/diagram.py` & `scippneutron-23.4.0/src/scippneutron/tof/diagram.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import scipp as sc
 from matplotlib.patches import Rectangle
 
 from scippneutron.tof.frames import _tof_from_wavelength
 
 
 class TimeDistanceDiagram:
-
     def __init__(self, ax, *, tmax, frame_rate=None):
         self._ax = ax
         self._time_unit = sc.Unit('ms')
         self._distance_unit = sc.Unit('m')
         frame_rate = 14.0 * sc.Unit('Hz') if frame_rate is None else frame_rate
         self._frame_length = (1.0 / frame_rate).to(unit=self._time_unit)
         self._tmax = tmax.to(unit=self._time_unit)
@@ -26,65 +25,68 @@
     def to_time(self, time):
         return time.to(unit=self._time_unit)
 
     def to_distance(self, distance):
         return distance.to(unit=self._distance_unit)
 
     def annotate(self, text, *, xy, xytext, **kwargs):
-
         def to_mpl(point):
             x, y = point
             return self.to_time(x).value, self.to_distance(y).value
 
         self._ax.annotate(text, xy=to_mpl(xy), xytext=to_mpl(xytext), **kwargs)
 
     def add_source_pulse(self, pulse_length=None, ls='dotted'):
         pulse_length = 3.0 * sc.Unit('ms') if pulse_length is None else pulse_length
         t0 = 0.0
         t1 = self.to_time(pulse_length).value
-        self._ax.text(t0,
-                      -2,
-                      f"Source pulse ({pulse_length.value} {pulse_length.unit})",
-                      ha="left",
-                      va="top",
-                      fontsize=6)
+        self._ax.text(
+            t0,
+            -2,
+            f"Source pulse ({pulse_length.value} {pulse_length.unit})",
+            ha="left",
+            va="top",
+            fontsize=6,
+        )
         while t0 < self._tmax.value:
             rect = Rectangle((t0, 0), t1, -1, lw=1, fc='orange', ec='k')
             self._ax.add_patch(rect)
             self._ax.axvline(x=t0, ls=ls)
             t0 += self._frame_length.value
 
-    def add_neutron(self,
-                    *,
-                    time_offset: sc.Variable,
-                    wavelength: sc.Variable,
-                    L: sc.Variable,
-                    label=None,
-                    color='black',
-                    ls='solid',
-                    lw=0.7):
+    def add_neutron(
+        self,
+        *,
+        time_offset: sc.Variable,
+        wavelength: sc.Variable,
+        L: sc.Variable,
+        label=None,
+        color='black',
+        ls='solid',
+        lw=0.7,
+    ):
         tof = self.to_time(_tof_from_wavelength(wavelength=wavelength, Ltotal=L))
         t0 = self.to_time(time_offset).value
-        self._ax.plot([t0, t0 + tof.value], [0, L.value],
-                      marker='',
-                      color=color,
-                      ls=ls,
-                      lw=lw)
+        self._ax.plot(
+            [t0, t0 + tof.value], [0, L.value], marker='', color=color, ls=ls, lw=lw
+        )
         if label is not None:
             self._ax.text(tof.value, L.value, label, ha="center", va="bottom")
 
-    def add_neutrons(self,
-                     *,
-                     lambda_min: sc.Variable,
-                     lambda_max: sc.Variable = None,
-                     Lmin: sc.Variable = 0.0 * sc.units.m,
-                     Lmax: sc.Variable,
-                     time_offset: sc.Variable,
-                     stride=1,
-                     frames=2):
+    def add_neutrons(
+        self,
+        *,
+        lambda_min: sc.Variable,
+        lambda_max: sc.Variable = None,
+        Lmin: sc.Variable = 0.0 * sc.units.m,
+        Lmax: sc.Variable,
+        time_offset: sc.Variable,
+        stride=1,
+        frames=2,
+    ):
         """
         Draw a wavelength band to depict propagation of neutrons. Neutrons are assumed
         to be emitted from a single point, i.e., no resolution effects are taken into
         account.
 
         Parameters
         ----------
@@ -102,36 +104,44 @@
             is None (the default) it is set such that there is no frame overlap at Lmax.
         time_offset:
             Offset time at which neutrons are emitted.
         frames:
             The number of frames that should be drawn.
         """
         tof_min = self.to_time(
-            _tof_from_wavelength(wavelength=lambda_min, Ltotal=Lmax - Lmin))
+            _tof_from_wavelength(wavelength=lambda_min, Ltotal=Lmax - Lmin)
+        )
         if lambda_max is None:
             tof_max = tof_min + (stride - 1 + 0.95) * self._frame_length  # small 5% gap
         else:
             tof_max = self.to_time(
-                _tof_from_wavelength(wavelength=lambda_max, Ltotal=Lmax - Lmin))
+                _tof_from_wavelength(wavelength=lambda_max, Ltotal=Lmax - Lmin)
+            )
         time_offset = self.to_time(time_offset)
         t0 = time_offset
         tmin = t0 + tof_min
         tmax = t0 + tof_max
         t = sc.concat([t0, t0, tmax, tmin], 't')
         L = sc.concat([Lmin, Lmin, Lmax, Lmax], 'L')
         for _ in range(frames):
             self._ax.fill(t.values, L.values, alpha=0.3)
             t += stride * self._frame_length
 
     def add_detector(self, *, distance, name='detector'):
         # TODO This could accept a list of positions and plot a rectangle from min to
         # max detector distance
-        self._ax.plot([0, self._tmax.max().value], [distance.value, distance.value],
-                      lw=3,
-                      color='grey')
+        self._ax.plot(
+            [0, self._tmax.max().value],
+            [distance.value, distance.value],
+            lw=3,
+            color='grey',
+        )
         self._ax.text(0.0, distance.value, name, va="bottom", ha="left")
 
     def add_sample(self, *, distance):
-        self._ax.plot([0, self._tmax.max().value], [distance.value, distance.value],
-                      lw=3,
-                      color='green')
+        self._ax.plot(
+            [0, self._tmax.max().value],
+            [distance.value, distance.value],
+            lw=3,
+            color='green',
+        )
         self._ax.text(0.0, distance.value, 'sample', va="bottom", ha="left")
```

### Comparing `scippneutron-23.3.0/src/scippneutron/tof/frames.py` & `scippneutron-23.4.0/src/scippneutron/tof/frames.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,44 +9,54 @@
 import scipp as sc
 from scipp.constants import h, m_n
 
 from .._utils import as_float_type, elem_unit
 from ..conversion.graph.beamline import Ltotal
 
 
-def _tof_from_wavelength(*, wavelength: sc.Variable,
-                         Ltotal: sc.Variable) -> sc.Variable:
+def _tof_from_wavelength(
+    *, wavelength: sc.Variable, Ltotal: sc.Variable
+) -> sc.Variable:
     scale = (m_n / h).to(unit=sc.units.us / elem_unit(Ltotal) / elem_unit(wavelength))
     return as_float_type(Ltotal * scale, wavelength) * wavelength
 
 
-def _time_offset_from_tof(*, tof: sc.Variable, frame_period: sc.Variable,
-                          frame_offset: sc.Variable) -> sc.Variable:
+def _time_offset_from_tof(
+    *, tof: sc.Variable, frame_period: sc.Variable, frame_offset: sc.Variable
+) -> sc.Variable:
     unit = elem_unit(tof)
     frame_period = frame_period.to(unit=unit)
     arrival_time_offset = frame_offset.to(unit=unit) + tof
     time_offset = arrival_time_offset % frame_period
     return time_offset
 
 
-def _tof_from_time_offset(*, time_offset: sc.Variable, time_offset_pivot: sc.Variable,
-                          tof_min: sc.Variable,
-                          frame_period: sc.Variable) -> sc.Variable:
+def _tof_from_time_offset(
+    *,
+    time_offset: sc.Variable,
+    time_offset_pivot: sc.Variable,
+    tof_min: sc.Variable,
+    frame_period: sc.Variable,
+) -> sc.Variable:
     frame_period = frame_period.to(unit=elem_unit(time_offset))
     time_offset_pivot = time_offset_pivot.to(unit=elem_unit(time_offset))
     tof_min = tof_min.to(unit=elem_unit(time_offset))
     shift = tof_min - time_offset_pivot
     tof = sc.where(time_offset >= time_offset_pivot, shift, shift + frame_period)
     tof += time_offset
     return tof
 
 
-def pulse_offset_from_time_zero(*, pulse_period: sc.Variable, pulse_stride: sc.Variable,
-                                event_time_zero: sc.Variable,
-                                first_pulse_time: sc.Variable) -> sc.Variable:
+def pulse_offset_from_time_zero(
+    *,
+    pulse_period: sc.Variable,
+    pulse_stride: sc.Variable,
+    event_time_zero: sc.Variable,
+    first_pulse_time: sc.Variable,
+) -> sc.Variable:
     """
     Return 0-based source frame index of detection frame.
 
     The source frames containing the time marked by tof_min receive index 0.
     The frame after that index 1, and so on, until frame_stride-1.
 
     Example
@@ -56,26 +66,29 @@
         event_time_zero = 12:05:00
         first_pulse_time = 12:00:00  # time of first (or any) pulse
                                        that passes through choppers
     """
     # This is roughly equivalent to
     #   (event_time_zero - first_pulse_time) % frame_period
     # but should avoid some issues with precision and drift
-    pulse_index = (event_time_zero -
-                   first_pulse_time) // pulse_period.to(unit=elem_unit(event_time_zero))
+    pulse_index = (event_time_zero - first_pulse_time) // pulse_period.to(
+        unit=elem_unit(event_time_zero)
+    )
     return pulse_period * (pulse_index % pulse_stride)
 
 
-def update_time_offset_for_pulse_skipping(*, event_time_offset: sc.Variable,
-                                          pulse_offset: sc.Variable) -> sc.Variable:
+def update_time_offset_for_pulse_skipping(
+    *, event_time_offset: sc.Variable, pulse_offset: sc.Variable
+) -> sc.Variable:
     return event_time_offset + pulse_offset.to(unit=elem_unit(event_time_offset))
 
 
-def frame_period_from_pulse_period(*, pulse_period: sc.Variable,
-                                   pulse_stride: sc.Variable) -> sc.Variable:
+def frame_period_from_pulse_period(
+    *, pulse_period: sc.Variable, pulse_stride: sc.Variable
+) -> sc.Variable:
     return pulse_period * pulse_stride
 
 
 def to_tof(*, pulse_skipping: Optional[bool] = False) -> dict:
     """
     Return a graph suitable for :py:func:`scipp.transform_coords` to convert frames
     to time-of-flight.
@@ -92,17 +105,17 @@
     applicable.
     """
 
     def _tof_min(*, Ltotal, lambda_min):
         return _tof_from_wavelength(Ltotal=Ltotal, wavelength=lambda_min)
 
     def _time_offset_pivot(*, tof_min, frame_period, frame_offset):
-        return _time_offset_from_tof(tof=tof_min,
-                                     frame_period=frame_period,
-                                     frame_offset=frame_offset)
+        return _time_offset_from_tof(
+            tof=tof_min, frame_period=frame_period, frame_offset=frame_offset
+        )
 
     graph = {}
     if pulse_skipping:
         graph['frame_period'] = frame_period_from_pulse_period
         graph['time_offset'] = update_time_offset_for_pulse_skipping
         graph['pulse_offset'] = pulse_offset_from_time_zero
     else:
@@ -111,22 +124,24 @@
 
     graph['tof_min'] = _tof_min
     graph['time_offset_pivot'] = _time_offset_pivot
     graph['tof'] = _tof_from_time_offset
     return graph
 
 
-def unwrap_frames(da: sc.DataArray,
-                  *,
-                  scatter: Optional[bool] = None,
-                  pulse_period: sc.Variable,
-                  pulse_stride: int = 1,
-                  frame_offset: sc.Variable,
-                  lambda_min: sc.Variable,
-                  first_pulse_time: Optional[sc.Variable] = None) -> sc.DataArray:
+def unwrap_frames(
+    da: sc.DataArray,
+    *,
+    scatter: Optional[bool] = None,
+    pulse_period: sc.Variable,
+    pulse_stride: int = 1,
+    frame_offset: sc.Variable,
+    lambda_min: sc.Variable,
+    first_pulse_time: Optional[sc.Variable] = None,
+) -> sc.DataArray:
     """
     Unwrap raw timestamps from ``NXevent_data`` into time-of-flight.
 
     The input data must provide the following coordinates:
 
     - ``event_time_offset``, as read from ``NXevent_data``
     - ``event_time_zero``, as read from ``NXevent_data``
@@ -172,24 +187,32 @@
 
     Returns
     -------
     :
         Data with 'tof' coordinate.
     """
     if 'tof' in da.meta or (da.bins is not None and 'tof' in da.bins.meta):
-        raise ValueError("Coordinate 'tof' already defined in input data array. "
-                         "Expected input with 'event_time_offset' coordinate.")
+        raise ValueError(
+            "Coordinate 'tof' already defined in input data array. "
+            "Expected input with 'event_time_offset' coordinate."
+        )
     da = da.copy(deep=False)
     coords = [
-        'pulse_period', 'pulse_stride', 'first_pulse_time', 'frame_offset', 'lambda_min'
+        'pulse_period',
+        'pulse_stride',
+        'first_pulse_time',
+        'frame_offset',
+        'lambda_min',
     ]
     for x in coords:
         if x in da.meta:
-            raise ValueError(f"Input data has '{x}' coord or attr, but values should "
-                             "be given only as a function parameter.")
+            raise ValueError(
+                f"Input data has '{x}' coord or attr, but values should "
+                "be given only as a function parameter."
+            )
     da.attrs['pulse_period'] = pulse_period
     da.attrs['frame_offset'] = frame_offset
     da.attrs['lambda_min'] = lambda_min
     if pulse_stride != 1:
         da.attrs['pulse_stride'] = sc.scalar(pulse_stride)
         da.attrs['first_pulse_time'] = first_pulse_time
     graph = {} if scatter is None else Ltotal(scatter=scatter)
```

### Comparing `scippneutron-23.3.0/src/scippneutron.egg-info/PKG-INFO` & `scippneutron-23.4.0/src/scippneutron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scippneutron
-Version: 23.3.0
+Version: 23.4.0
 Summary:  Neutron scattering tools for Data Reduction
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Scipp contributors (https://github.com/scipp)
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `scippneutron-23.3.0/src/scippneutron.egg-info/SOURCES.txt` & `scippneutron-23.4.0/src/scippneutron.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.git-blame-ignore-revs
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 tox.ini
@@ -11,14 +12,16 @@
 .github/dependabot.yml
 .github/workflows/pr_and_main.yml
 .github/workflows/release.yml
 benchmarks/__init__.py
 benchmarks/load_nexus.py
 benchmarks/transform_coords.py
 conda/meta.yaml
+docs/bibliography.bib
+docs/bibliography.rst
 docs/conf.py
 docs/index.rst
 docs/version.py
 docs/_static/favicon.ico
 docs/_static/logo-2022.svg
 docs/_static/straight-beamline.svg
 docs/_templates/scipp-class-template.rst
@@ -55,16 +58,14 @@
 docs/user-guide/recipes.ipynb
 requirements/base.in
 requirements/base.txt
 requirements/ci.in
 requirements/ci.txt
 requirements/dev.in
 requirements/dev.txt
-requirements/docs.in
-requirements/docs.txt
 requirements/static.in
 requirements/static.txt
 requirements/test.in
 requirements/test.txt
 requirements/wheels.in
 requirements/wheels.txt
 resources/logo-2022.svg
@@ -108,14 +109,15 @@
 src/scippneutron/tof/__init__.py
 src/scippneutron/tof/diagram.py
 src/scippneutron/tof/frames.py
 tests/HYS_mask.xml
 tests/__init__.py
 tests/beamline_components_test.py
 tests/common.py
+tests/conftest.py
 tests/convert_test.py
 tests/data_stream_test.py
 tests/instrument_view_test.py
 tests/load_nexus_json_test.py
 tests/load_nexus_test.py
 tests/load_nxdetector_test.py
 tests/mantid_helper.py
```

### Comparing `scippneutron-23.3.0/tests/beamline_components_test.py` & `scippneutron-23.4.0/tests/beamline_components_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,59 +7,63 @@
 
 import scippneutron as scn
 
 
 @pytest.fixture
 def data_array():
     positions = [[-1, 0, 0], [0, 1, 0], [0, 0, 1]]
-    return sc.DataArray(sc.Variable(dims=['position', 'tof'],
-                                    values=np.random.rand(3, 9)),
-                        coords={
-                            'position':
-                            sc.vectors(dims=['position'], values=positions, unit='m'),
-                            'source_position':
-                            sc.vector(value=np.array([0, 0, -10]), unit='m'),
-                            'sample_position':
-                            sc.vector(value=np.array([0, 1, 0]), unit='m')
-                        })
+    return sc.DataArray(
+        sc.Variable(dims=['position', 'tof'], values=np.random.rand(3, 9)),
+        coords={
+            'position': sc.vectors(dims=['position'], values=positions, unit='m'),
+            'source_position': sc.vector(value=np.array([0, 0, -10]), unit='m'),
+            'sample_position': sc.vector(value=np.array([0, 1, 0]), unit='m'),
+        },
+    )
 
 
 def test_position(data_array):
     assert sc.identical(scn.position(data_array), data_array.coords['position'])
 
 
 def test_source_position(data_array):
-    assert sc.identical(scn.source_position(data_array),
-                        sc.vector(value=np.array([0, 0, -10]), unit='m'))
+    assert sc.identical(
+        scn.source_position(data_array),
+        sc.vector(value=np.array([0, 0, -10]), unit='m'),
+    )
 
 
 def test_sample_position(data_array):
-    assert sc.identical(scn.sample_position(data_array),
-                        sc.vector(value=np.array([0, 1, 0]), unit='m'))
+    assert sc.identical(
+        scn.sample_position(data_array), sc.vector(value=np.array([0, 1, 0]), unit='m')
+    )
 
 
 def test_L1(data_array):
     assert sc.identical(scn.L1(data_array), sc.scalar(np.sqrt(1 + 100), unit='m'))
 
 
 def test_L2(data_array):
     assert sc.identical(
         scn.L2(data_array),
-        sc.array(dims=['position'], values=np.sqrt([1 + 1, 0, 1 + 1]), unit='m'))
+        sc.array(dims=['position'], values=np.sqrt([1 + 1, 0, 1 + 1]), unit='m'),
+    )
 
 
 def test_Ltotal_scatter(data_array):
-    assert sc.identical(scn.Ltotal(data_array, scatter=True),
-                        scn.L1(data_array) + scn.L2(data_array))
+    assert sc.identical(
+        scn.Ltotal(data_array, scatter=True), scn.L1(data_array) + scn.L2(data_array)
+    )
 
 
 def test_Ltotal_no_scatter(data_array):
     assert sc.identical(
         scn.Ltotal(data_array, scatter=False),
-        sc.array(dims=['position'], values=np.sqrt([1 + 100, 1 + 100, 121]), unit='m'))
+        sc.array(dims=['position'], values=np.sqrt([1 + 100, 1 + 100, 121]), unit='m'),
+    )
 
 
 def test_two_theta(data_array):
     # Bare-bones test because computation of 2theta is complicated,
     # and it is tested separately elsewhere.
     two_theta = scn.two_theta(data_array)
     assert two_theta.unit == 'rad'
```

### Comparing `scippneutron-23.3.0/tests/conversion/beamline_conversions_test.py` & `scippneutron-23.4.0/tests/conversion/beamline_conversions_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,104 +5,119 @@
 import numpy as np
 import scipp as sc
 
 from scippneutron.conversion import beamline
 
 
 def test_straight_incident_beam():
-    source_position = sc.vectors(dims=['siti'],
-                                 values=[[40, 80, 20], [30, 10, 50]],
-                                 unit='mm')
+    source_position = sc.vectors(
+        dims=['siti'], values=[[40, 80, 20], [30, 10, 50]], unit='mm'
+    )
     sample_position = sc.vector([7, 5, 3], unit='mm')
-    incident_beam = beamline.straight_incident_beam(source_position=source_position,
-                                                    sample_position=sample_position)
+    incident_beam = beamline.straight_incident_beam(
+        source_position=source_position, sample_position=sample_position
+    )
     assert sc.allclose(
         incident_beam,
-        sc.vectors(dims=['siti'], values=[[-33, -75, -17], [-23, -5, -47]], unit='mm'))
+        sc.vectors(dims=['siti'], values=[[-33, -75, -17], [-23, -5, -47]], unit='mm'),
+    )
 
 
 def test_straight_scattered_beam():
     position = sc.vectors(dims=['on'], values=[[6, 3, 9], [8, 3, 1]], unit='km')
     sample_position = sc.vector([0.4, 0.6, 0.2], unit='km')
-    scattered_beam = beamline.straight_scattered_beam(position=position,
-                                                      sample_position=sample_position)
+    scattered_beam = beamline.straight_scattered_beam(
+        position=position, sample_position=sample_position
+    )
     assert sc.allclose(
         scattered_beam,
-        sc.vectors(dims=['on'], values=[[5.6, 2.4, 8.8], [7.6, 2.4, 0.8]], unit='km'))
+        sc.vectors(dims=['on'], values=[[5.6, 2.4, 8.8], [7.6, 2.4, 0.8]], unit='km'),
+    )
 
 
 def test_L1():
-    incident_beam = sc.vectors(dims=['inc'],
-                               values=[[0.5, 1.0, 1.5], [-0.3, 0.6, -0.9]],
-                               unit='um')
+    incident_beam = sc.vectors(
+        dims=['inc'], values=[[0.5, 1.0, 1.5], [-0.3, 0.6, -0.9]], unit='um'
+    )
     L1 = beamline.L1(incident_beam=incident_beam)
     assert sc.allclose(
-        L1, sc.array(dims=['inc'], values=[1.870828693386, 1.122497216032], unit='um'))
+        L1, sc.array(dims=['inc'], values=[1.870828693386, 1.122497216032], unit='um')
+    )
 
 
 def test_L2():
-    scattered_beam = sc.vectors(dims=['scat'],
-                                values=[[11, 22, 33], [95, 84, 73]],
-                                unit='am')
+    scattered_beam = sc.vectors(
+        dims=['scat'], values=[[11, 22, 33], [95, 84, 73]], unit='am'
+    )
     L2 = beamline.L2(scattered_beam=scattered_beam)
     assert sc.allclose(
         L2,
-        sc.array(dims=['scat'], values=[41.158231254513, 146.321563687653], unit='am'))
+        sc.array(dims=['scat'], values=[41.158231254513, 146.321563687653], unit='am'),
+    )
 
 
 def test_total_beam_length():
     L1 = sc.scalar(5.134, unit='cm')
     L2 = sc.array(dims=['secondary'], values=[3.14159, 42.0, 999.0], unit='cm')
     Ltotal = beamline.total_beam_length(L1=L1, L2=L2)
     assert sc.allclose(
         Ltotal,
-        sc.array(dims=['secondary'], values=[8.27559, 47.134, 1004.134], unit='cm'))
+        sc.array(dims=['secondary'], values=[8.27559, 47.134, 1004.134], unit='cm'),
+    )
 
 
 def test_total_straight_beam_length_no_scatter():
     position = sc.vectors(dims=['po'], values=[[1, 2, 3], [4, 5, 6]], unit='m')
     source_position = sc.vector([0.1, 0.2, 0.3], unit='m')
     Ltotal = beamline.total_straight_beam_length_no_scatter(
-        source_position=source_position, position=position)
+        source_position=source_position, position=position
+    )
     assert sc.allclose(
-        Ltotal, sc.array(dims=['po'], values=[3.367491648096, 8.410707461325],
-                         unit='m'))
+        Ltotal, sc.array(dims=['po'], values=[3.367491648096, 8.410707461325], unit='m')
+    )
 
 
 def test_two_theta_arbitrary_values():
     incident_beam = sc.vector([0.564, 1.2, -10.4], unit='m')
-    scattered_beam = sc.vectors(dims=['beam'],
-                                values=[[13, 24, 35], [51, -42, 33]],
-                                unit='m')
-    two_theta = beamline.two_theta(incident_beam=incident_beam,
-                                   scattered_beam=scattered_beam)
+    scattered_beam = sc.vectors(
+        dims=['beam'], values=[[13, 24, 35], [51, -42, 33]], unit='m'
+    )
+    two_theta = beamline.two_theta(
+        incident_beam=incident_beam, scattered_beam=scattered_beam
+    )
     assert sc.allclose(
         two_theta,
-        sc.array(dims=['beam'], values=[2.352629742382, 2.061447408052], unit='rad'))
+        sc.array(dims=['beam'], values=[2.352629742382, 2.061447408052], unit='rad'),
+    )
 
 
 def test_two_theta_parallel_beams():
     incident_beam = sc.vector([1.0, 0.2, 0.0], unit='mm')
     scattered_beam = sc.array(dims=['beam'], values=[1.0, 2.0, 0.1]) * incident_beam
-    two_theta = beamline.two_theta(incident_beam=incident_beam,
-                                   scattered_beam=scattered_beam)
+    two_theta = beamline.two_theta(
+        incident_beam=incident_beam, scattered_beam=scattered_beam
+    )
     assert sc.allclose(two_theta, sc.zeros(dims=['beam'], shape=[3], unit='rad'))
 
 
 def test_two_theta_anti_parallel_beams():
     incident_beam = sc.vector([10.2, -0.8, 4.1], unit='mm')
     scattered_beam = sc.array(dims=['beam'], values=[-2.1, -31.0, -1.0]) * incident_beam
-    two_theta = beamline.two_theta(incident_beam=incident_beam,
-                                   scattered_beam=scattered_beam)
-    assert sc.allclose(two_theta,
-                       sc.full(value=np.pi, dims=['beam'], shape=[3], unit='rad'))
+    two_theta = beamline.two_theta(
+        incident_beam=incident_beam, scattered_beam=scattered_beam
+    )
+    assert sc.allclose(
+        two_theta, sc.full(value=np.pi, dims=['beam'], shape=[3], unit='rad')
+    )
 
 
 def test_two_theta_orthogonal_beams():
     incident_beam = sc.vector([0.1, 0.0, 10.0], unit='m')
-    scattered_beam = sc.vectors(dims=['beam'],
-                                values=[[0.0, -2.1, 0.0], [10.0, 123.0, -0.1]],
-                                unit='m')
-    two_theta = beamline.two_theta(incident_beam=incident_beam,
-                                   scattered_beam=scattered_beam)
-    assert sc.allclose(two_theta,
-                       sc.full(value=np.pi / 2, dims=['beam'], shape=[2], unit='rad'))
+    scattered_beam = sc.vectors(
+        dims=['beam'], values=[[0.0, -2.1, 0.0], [10.0, 123.0, -0.1]], unit='m'
+    )
+    two_theta = beamline.two_theta(
+        incident_beam=incident_beam, scattered_beam=scattered_beam
+    )
+    assert sc.allclose(
+        two_theta, sc.full(value=np.pi / 2, dims=['beam'], shape=[2], unit='rad')
+    )
```

### Comparing `scippneutron-23.3.0/tests/conversion/graph/tof_graph_test.py` & `scippneutron-23.4.0/tests/conversion/graph/tof_graph_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,23 +6,38 @@
 
 from scippneutron.conversion.graph import tof
 
 
 def test_elastic():
     assert set(tof.elastic('energy').keys()) == {'dspacing', 'wavelength'}
     assert set(tof.elastic('tof').keys()) == {
-        'dspacing', 'energy', 'Q', 'wavelength', ('Qx', 'Qy', 'Qz')
+        'dspacing',
+        'energy',
+        'Q',
+        'wavelength',
+        ('Qx', 'Qy', 'Qz'),
+        'Q_vec',
+        'hkl_vec',
+        ('h', 'k', 'l'),
+        'ub_matrix',
     }
     assert set(tof.elastic('Q').keys()) == {'wavelength'}
     assert set(tof.elastic('wavelength').keys()) == {
-        'dspacing', 'energy', 'Q', ('Qx', 'Qy', 'Qz')
+        'dspacing',
+        'energy',
+        'Q',
+        ('Qx', 'Qy', 'Qz'),
+        'Q_vec',
+        'hkl_vec',
+        ('h', 'k', 'l'),
+        'ub_matrix',
     }
 
 
-@pytest.mark.parametrize('start', ('dspacing', ))
+@pytest.mark.parametrize('start', ('dspacing',))
 def test_elastic_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic(start)
 
 
 def test_kinematic():
     assert set(tof.kinematic('tof').keys()) == {'energy', 'wavelength'}
@@ -38,15 +53,15 @@
 
 def test_elastic_dspacing():
     assert set(tof.elastic_dspacing('energy').keys()) == {'dspacing'}
     assert set(tof.elastic_dspacing('tof').keys()) == {'dspacing'}
     assert set(tof.elastic_dspacing('wavelength').keys()) == {'dspacing'}
 
 
-@pytest.mark.parametrize('start', ('Q', ))
+@pytest.mark.parametrize('start', ('Q',))
 def test_elastic_dspacing_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic_dspacing(start)
 
 
 def test_elastic_energy():
     assert set(tof.elastic_energy('tof').keys()) == {'energy'}
@@ -72,15 +87,15 @@
 
 def test_elastic_wavelength():
     assert set(tof.elastic_wavelength('energy').keys()) == {'wavelength'}
     assert set(tof.elastic_wavelength('tof').keys()) == {'wavelength'}
     assert set(tof.elastic_wavelength('Q').keys()) == {'wavelength'}
 
 
-@pytest.mark.parametrize('start', ('dspacing', ))
+@pytest.mark.parametrize('start', ('dspacing',))
 def test_elastic_wavelength_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.elastic_wavelength(start)
 
 
 def test_direct_inelastic():
     assert set(tof.direct_inelastic('tof').keys()) == {'energy_transfer'}
@@ -98,23 +113,26 @@
 
 @pytest.mark.parametrize('start', ('wavelength', 'Q', 'dspacing'))
 def test_indirect_inelastic_unsupported_starts(start):
     with pytest.raises(KeyError):
         tof.indirect_inelastic(start)
 
 
-@pytest.mark.parametrize('arg', (
-    (tof.elastic, ('energy', 'tof', 'Q', 'wavelength')),
-    (tof.kinematic, ('tof', 'wavelength', 'energy')),
-    (tof.elastic_dspacing, ('tof', 'wavelength', 'energy')),
-    (tof.elastic_energy, ('tof', 'wavelength')),
-    (tof.elastic_Q, ('tof', 'wavelength')),
-    (tof.elastic_wavelength, ('tof', 'energy', 'Q')),
-    (tof.direct_inelastic, ('tof', )),
-    (tof.indirect_inelastic, ('tof', )),
-))
+@pytest.mark.parametrize(
+    'arg',
+    (
+        (tof.elastic, ('energy', 'tof', 'Q', 'wavelength')),
+        (tof.kinematic, ('tof', 'wavelength', 'energy')),
+        (tof.elastic_dspacing, ('tof', 'wavelength', 'energy')),
+        (tof.elastic_energy, ('tof', 'wavelength')),
+        (tof.elastic_Q, ('tof', 'wavelength')),
+        (tof.elastic_wavelength, ('tof', 'energy', 'Q')),
+        (tof.direct_inelastic, ('tof',)),
+        (tof.indirect_inelastic, ('tof',)),
+    ),
+)
 def test_returns_new_graph(arg):
     fn, starts = arg
     for start in starts:
         g = fn(start)
         g['a_new_node'] = lambda position: 2 * position
         assert 'a_new_node' not in fn(start)
```

### Comparing `scippneutron-23.3.0/tests/conversion/tof_conversions_test.py` & `scippneutron-23.4.0/tests/conversion/tof_conversions_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,105 +13,126 @@
 
 from scippneutron.conversion import beamline as beamline_conv
 from scippneutron.conversion import tof as tof_conv
 
 global_settings = {
     'max_examples': 20,
     # Generating variables needs a lot of memory. Nothing we can fix in scippneutron.
-    'suppress_health_check': [HealthCheck.data_too_large]
+    'suppress_health_check': [HealthCheck.data_too_large],
 }
 
 
 def element_args():
     return {
         'allow_nan': False,
         'allow_infinity': False,
         'allow_subnormal': False,
         'min_value': 1e-2,
-        'max_value': 1e6
+        'max_value': 1e6,
     }
 
 
 def simple_variables(dims, unit):
-    return scst.variables(sizes=st.dictionaries(keys=dims,
-                                                values=st.integers(min_value=1,
-                                                                   max_value=4),
-                                                min_size=1,
-                                                max_size=1),
-                          unit=unit,
-                          with_variances=False,
-                          dtype='float',
-                          elements=element_args())
+    return scst.variables(
+        sizes=st.dictionaries(
+            keys=dims,
+            values=st.integers(min_value=1, max_value=4),
+            min_size=1,
+            max_size=1,
+        ),
+        unit=unit,
+        with_variances=False,
+        dtype='float',
+        elements=element_args(),
+    )
 
 
 def n_simple_variables(n, dims, unit):
-    return scst.n_variables(n,
-                            sizes=st.dictionaries(keys=dims,
-                                                  values=st.integers(min_value=1,
-                                                                     max_value=4),
-                                                  min_size=1,
-                                                  max_size=1),
-                            unit=unit,
-                            with_variances=False,
-                            dtype='float',
-                            elements=element_args())
+    return scst.n_variables(
+        n,
+        sizes=st.dictionaries(
+            keys=dims,
+            values=st.integers(min_value=1, max_value=4),
+            min_size=1,
+            max_size=1,
+        ),
+        unit=unit,
+        with_variances=False,
+        dtype='float',
+        elements=element_args(),
+    )
 
 
 def time_variables():
-    return simple_variables(dims=st.sampled_from(('time', 't', 'tof')),
-                            unit=st.sampled_from(('s', 'ms', 'us')))
+    return simple_variables(
+        dims=st.sampled_from(('time', 't', 'tof')),
+        unit=st.sampled_from(('s', 'ms', 'us')),
+    )
 
 
 def space_variables():
-    return simple_variables(dims=st.sampled_from(('position', 'spectrum', 'x')),
-                            unit=st.sampled_from(('m', 'cm', 'angstrom')))
+    return simple_variables(
+        dims=st.sampled_from(('position', 'spectrum', 'x')),
+        unit=st.sampled_from(('m', 'cm', 'angstrom')),
+    )
 
 
 def n_space_variables(n):
-    return n_simple_variables(n,
-                              dims=st.sampled_from(('position', 'spectrum', 'x')),
-                              unit=st.sampled_from(('m', 'cm', 'angstrom')))
+    return n_simple_variables(
+        n,
+        dims=st.sampled_from(('position', 'spectrum', 'x')),
+        unit=st.sampled_from(('m', 'cm', 'angstrom')),
+    )
 
 
 def angle_variables():
-    return simple_variables(dims=st.sampled_from(('angle', 'two_theta', 'alpha')),
-                            unit=st.sampled_from(('deg', 'rad')))
+    return simple_variables(
+        dims=st.sampled_from(('angle', 'two_theta', 'alpha')),
+        unit=st.sampled_from(('deg', 'rad')),
+    )
 
 
 def energy_variables():
-    return simple_variables(dims=st.sampled_from(('energy', 'E', 'energy_transfer')),
-                            unit=st.sampled_from(('meV', 'J')))
+    return simple_variables(
+        dims=st.sampled_from(('energy', 'E', 'energy_transfer')),
+        unit=st.sampled_from(('meV', 'J')),
+    )
 
 
 def vectors_variables():
-    return st.fixed_dictionaries({
-        'size':
-        st.integers(min_value=1, max_value=4),
-        'dim':
-        st.sampled_from(('position', 'detector', 'pixel')),
-        'unit':
-        st.sampled_from(('m', 'cm'))
-    }).flatmap(
+    return st.fixed_dictionaries(
+        {
+            'size': st.integers(min_value=1, max_value=4),
+            'dim': st.sampled_from(('position', 'detector', 'pixel')),
+            'unit': st.sampled_from(('m', 'cm')),
+        }
+    ).flatmap(
         lambda args: npst.arrays(float, (args['size'], 3), elements=element_args()).map(
             lambda values: sc.vectors(
-                dims=[args['dim']], values=values, unit=args['unit'])))
+                dims=[args['dim']], values=values, unit=args['unit']
+            )
+        )
+    )
 
 
 def vector_variables():
-    return st.sampled_from(
-        ('m', 'cm')).flatmap(lambda unit: npst.arrays(float, 3, elements=element_args())
-                             .map(lambda values: sc.vector(values, unit=unit)))
+    return st.sampled_from(('m', 'cm')).flatmap(
+        lambda unit: npst.arrays(float, 3, elements=element_args()).map(
+            lambda values: sc.vector(values, unit=unit)
+        )
+    )
 
 
 @given(tof=time_variables(), Ltotal=space_variables())
 @settings(**global_settings)
 def test_wavelength_from_tof(tof, Ltotal):
     wavelength = tof_conv.wavelength_from_tof(tof=tof, Ltotal=Ltotal)
-    assert sc.allclose(wavelength,
-                       sc.to_unit(const.h * tof / const.m_n / Ltotal, unit='angstrom'))
+    assert sc.allclose(
+        wavelength, sc.to_unit(const.h * tof / const.m_n / Ltotal, unit='angstrom')
+    )
 
 
 @pytest.mark.parametrize('tof_dtype', ('float64', 'int64', 'int32'))
 @pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
 def test_wavelength_from_tof_double_precision(tof_dtype, Ltotal_dtype):
     tof = sc.scalar(1.2, unit='s', dtype=tof_dtype)
     Ltotal = sc.scalar(10.1, unit='m', dtype=Ltotal_dtype)
@@ -121,55 +142,65 @@
 @pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
 def test_wavelength_from_tof_single_precision(Ltotal_dtype):
     tof = sc.scalar(1.2, unit='s', dtype='float32')
     Ltotal = sc.scalar(10.1, unit='m', dtype=Ltotal_dtype)
     assert tof_conv.wavelength_from_tof(tof=tof, Ltotal=Ltotal).dtype == 'float32'
 
 
-@given(tof=time_variables(),
-       Ltotal_and_two_theta=n_space_variables(2),
-       two_theta_unit=st.sampled_from(('deg', 'rad')))
+@given(
+    tof=time_variables(),
+    Ltotal_and_two_theta=n_space_variables(2),
+    two_theta_unit=st.sampled_from(('deg', 'rad')),
+)
 @settings(**global_settings)
 def test_dspacing_from_tof(tof, Ltotal_and_two_theta, two_theta_unit):
     Ltotal, two_theta = Ltotal_and_two_theta
     two_theta.unit = two_theta_unit
     dspacing = tof_conv.dspacing_from_tof(tof=tof, Ltotal=Ltotal, two_theta=two_theta)
     assert sc.allclose(
         dspacing,
-        sc.to_unit(const.h * tof / const.m_n / Ltotal / 2 / sc.sin(two_theta / 2),
-                   unit='angstrom'))
+        sc.to_unit(
+            const.h * tof / const.m_n / Ltotal / 2 / sc.sin(two_theta / 2),
+            unit='angstrom',
+        ),
+    )
 
 
 @pytest.mark.parametrize('tof_dtype', ('float64', 'int64', 'int32'))
 @pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64', 'int32'))
 def test_dspacing_from_tof_double_precision(tof_dtype, Ltotal_dtype, two_theta_dtype):
     tof = sc.scalar(52.0, unit='s', dtype=tof_dtype)
     Ltotal = sc.scalar(0.341, unit='m', dtype=Ltotal_dtype)
     two_theta = sc.scalar(1.68, unit='rad', dtype=two_theta_dtype)
-    assert tof_conv.dspacing_from_tof(tof=tof, Ltotal=Ltotal,
-                                      two_theta=two_theta).dtype == 'float64'
+    assert (
+        tof_conv.dspacing_from_tof(tof=tof, Ltotal=Ltotal, two_theta=two_theta).dtype
+        == 'float64'
+    )
 
 
 @pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64', 'int32'))
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64', 'int32'))
 def test_dspacing_from_tof_single_precision(Ltotal_dtype, two_theta_dtype):
     tof = sc.scalar(52.0, unit='s', dtype='float32')
     Ltotal = sc.scalar(0.341, unit='m', dtype=Ltotal_dtype)
     two_theta = sc.scalar(1.68, unit='rad', dtype=two_theta_dtype)
-    assert tof_conv.dspacing_from_tof(tof=tof, Ltotal=Ltotal,
-                                      two_theta=two_theta).dtype == 'float32'
+    assert (
+        tof_conv.dspacing_from_tof(tof=tof, Ltotal=Ltotal, two_theta=two_theta).dtype
+        == 'float32'
+    )
 
 
 @given(tof=time_variables(), Ltotal=space_variables())
 @settings(**global_settings)
 def test_energy_from_tof(tof, Ltotal):
     energy = tof_conv.energy_from_tof(tof=tof, Ltotal=Ltotal)
-    assert sc.allclose(energy, sc.to_unit(const.m_n * Ltotal**2 / 2 / tof**2,
-                                          unit='meV'))
+    assert sc.allclose(
+        energy, sc.to_unit(const.m_n * Ltotal**2 / 2 / tof**2, unit='meV')
+    )
 
 
 @pytest.mark.parametrize('tof_dtype', ('float64', 'int64'))
 @pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64'))
 def test_energy_from_tof_double_precision(tof_dtype, Ltotal_dtype):
     tof = sc.scalar(478.9, unit='s', dtype=tof_dtype)
     Ltotal = sc.scalar(1.256, unit='m', dtype=Ltotal_dtype)
@@ -179,63 +210,74 @@
 @pytest.mark.parametrize('Ltotal_dtype', ('float64', 'float32', 'int64'))
 def test_energy_from_tof_single_precision(Ltotal_dtype):
     tof = sc.scalar(478.9, unit='s', dtype='float32')
     Ltotal = sc.scalar(1.256, unit='m', dtype=Ltotal_dtype)
     assert tof_conv.energy_from_tof(tof=tof, Ltotal=Ltotal).dtype == 'float32'
 
 
-@given(tof=time_variables(),
-       L1_and_L2=n_space_variables(2),
-       L2_unit=st.sampled_from(('m', 'mm', 'cm')),
-       incident_energy=energy_variables())
+@given(
+    tof=time_variables(),
+    L1_and_L2=n_space_variables(2),
+    L2_unit=st.sampled_from(('m', 'mm', 'cm')),
+    incident_energy=energy_variables(),
+)
 @settings(**global_settings)
 def test_energy_transfer_direct_from_tof(tof, L1_and_L2, L2_unit, incident_energy):
     L1, L2 = L1_and_L2
     L2.unit = L2_unit
     # Energies are always > 0. This matters for detection of invalid tof values.
     incident_energy = abs(incident_energy) * 1.0001
 
     energy_transfer = tof_conv.energy_transfer_direct_from_tof(
-        tof=tof, L1=L1, L2=L2, incident_energy=incident_energy)
+        tof=tof, L1=L1, L2=L2, incident_energy=incident_energy
+    )
 
     t0 = sc.to_unit(sc.sqrt(const.m_n * L1**2 / 2 / incident_energy), tof.unit)
-    expected = incident_energy - sc.to_unit(const.m_n * L2**2 / 2 /
-                                            (tof - t0)**2, incident_energy.unit)
-    expected = sc.where(tof >= t0, expected, sc.scalar(np.nan,
-                                                       unit=incident_energy.unit))
+    expected = incident_energy - sc.to_unit(
+        const.m_n * L2**2 / 2 / (tof - t0) ** 2, incident_energy.unit
+    )
+    expected = sc.where(
+        tof >= t0, expected, sc.scalar(np.nan, unit=incident_energy.unit)
+    )
     assert sc.allclose(energy_transfer, expected, equal_nan=True)
 
 
-@given(tof=time_variables(),
-       L1_and_L2=n_space_variables(2),
-       L2_unit=st.sampled_from(('m', 'mm', 'cm')),
-       final_energy=energy_variables())
+@given(
+    tof=time_variables(),
+    L1_and_L2=n_space_variables(2),
+    L2_unit=st.sampled_from(('m', 'mm', 'cm')),
+    final_energy=energy_variables(),
+)
 @settings(**global_settings)
 def test_energy_transfer_indirect_from_tof(tof, L1_and_L2, L2_unit, final_energy):
     L1, L2 = L1_and_L2
     L2.unit = L2_unit
     # Energies are always > 0. This matters for detection of invalid tof values.
     final_energy = abs(final_energy) * 1.0001
 
     energy_transfer = tof_conv.energy_transfer_indirect_from_tof(
-        tof=tof, L1=L1, L2=L2, final_energy=final_energy)
+        tof=tof, L1=L1, L2=L2, final_energy=final_energy
+    )
 
     t0 = sc.to_unit(sc.sqrt(const.m_n * L2**2 / 2 / final_energy), tof.unit)
-    expected = sc.to_unit(const.m_n * L1**2 / 2 /
-                          (tof - t0)**2, final_energy.unit) - final_energy
+    expected = (
+        sc.to_unit(const.m_n * L1**2 / 2 / (tof - t0) ** 2, final_energy.unit)
+        - final_energy
+    )
     expected = sc.where(tof >= t0, expected, sc.scalar(np.nan, unit=final_energy.unit))
     assert sc.allclose(energy_transfer, expected, equal_nan=True)
 
 
 @given(wavelength=space_variables())
 @settings(**global_settings)
 def test_energy_from_wavelength(wavelength):
     energy = tof_conv.energy_from_wavelength(wavelength=wavelength)
     assert sc.allclose(
-        energy, sc.to_unit(const.h**2 / 2 / const.m_n / wavelength**2, unit='meV'))
+        energy, sc.to_unit(const.h**2 / 2 / const.m_n / wavelength**2, unit='meV')
+    )
 
 
 @pytest.mark.parametrize('wavelength_dtype', ('float64', 'int64'))
 def test_energy_from_wavelength_double_precision(wavelength_dtype):
     wavelength = sc.scalar(60.5, unit='m', dtype=wavelength_dtype)
     assert tof_conv.energy_from_wavelength(wavelength=wavelength).dtype == 'float64'
 
@@ -247,15 +289,16 @@
 
 @given(energy=energy_variables())
 @settings(**global_settings)
 def test_wavelength_from_energy(energy):
     wavelength = tof_conv.wavelength_from_energy(energy=energy)
     assert sc.allclose(
         wavelength,
-        sc.to_unit(const.h / sc.sqrt(2 * const.m_n * energy), unit='angstrom'))
+        sc.to_unit(const.h / sc.sqrt(2 * const.m_n * energy), unit='angstrom'),
+    )
 
 
 @pytest.mark.parametrize('energy_dtype', ('float64', 'int64'))
 def test_wavelength_from_energy_double_precision(energy_dtype):
     energy = sc.scalar(61.0, unit='meV', dtype=energy_dtype)
     assert tof_conv.wavelength_from_energy(energy=energy).dtype == 'float64'
 
@@ -273,33 +316,38 @@
 
 
 @pytest.mark.parametrize('wavelength_dtype', ('float64', 'int64'))
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
 def test_Q_from_wavelength_double_precision(wavelength_dtype, two_theta_dtype):
     wavelength = sc.scalar(3.51, unit='s', dtype=wavelength_dtype)
     two_theta = sc.scalar(0.041, unit='deg', dtype=two_theta_dtype)
-    assert tof_conv.Q_from_wavelength(wavelength=wavelength,
-                                      two_theta=two_theta).dtype == 'float64'
+    assert (
+        tof_conv.Q_from_wavelength(wavelength=wavelength, two_theta=two_theta).dtype
+        == 'float64'
+    )
 
 
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
 def test_Q_from_wavelength_single_precision(two_theta_dtype):
     wavelength = sc.scalar(3.51, unit='s', dtype='float32')
     two_theta = sc.scalar(0.041, unit='deg', dtype=two_theta_dtype)
-    assert tof_conv.Q_from_wavelength(wavelength=wavelength,
-                                      two_theta=two_theta).dtype == 'float32'
+    assert (
+        tof_conv.Q_from_wavelength(wavelength=wavelength, two_theta=two_theta).dtype
+        == 'float32'
+    )
 
 
 @given(Q=space_variables(), two_theta=angle_variables())
 @settings(**global_settings)
 def test_wavelength_from_Q(Q, two_theta):
     Q.unit = f'1/{Q.unit}'
     wavelength = tof_conv.wavelength_from_Q(Q=Q, two_theta=two_theta)
     assert sc.allclose(
-        wavelength, sc.to_unit(4 * np.pi * sc.sin(two_theta / 2) / Q, unit='angstrom'))
+        wavelength, sc.to_unit(4 * np.pi * sc.sin(two_theta / 2) / Q, unit='angstrom')
+    )
 
 
 @pytest.mark.parametrize('Q_dtype', ('float64', 'int64'))
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
 def test_wavelength_from_Q_double_precision(Q_dtype, two_theta_dtype):
     Q = sc.scalar(4.151, unit='1/nm', dtype=Q_dtype)
     two_theta = sc.scalar(5.71, unit='deg', dtype=two_theta_dtype)
@@ -313,104 +361,251 @@
     assert tof_conv.wavelength_from_Q(Q=Q, two_theta=two_theta).dtype == 'float32'
 
 
 @given(incident_beam=vector_variables(), wavelength=space_variables())
 @settings(**global_settings)
 def test_Q_elements_from_wavelength_equal_beams(incident_beam, wavelength):
     scattered_beam = incident_beam.copy()
-    (Qx, Qy, Qz) = tof_conv.Q_elements_from_wavelength(wavelength=wavelength,
-                                                       incident_beam=incident_beam,
-                                                       scattered_beam=scattered_beam)
+    (Qx, Qy, Qz) = tof_conv.Q_elements_from_wavelength(
+        wavelength=wavelength,
+        incident_beam=incident_beam,
+        scattered_beam=scattered_beam,
+    )
     assert sc.allclose(Qx, 0.0 / wavelength.unit)
     assert sc.allclose(Qy, 0.0 / wavelength.unit)
     assert sc.allclose(Qz, 0.0 / wavelength.unit)
 
 
-@given(incident_beam=vector_variables(),
-       scattered_beam=vectors_variables(),
-       wavelength=space_variables())
-@settings(**global_settings)
-def test_Q_elements_from_wavelength_consistent_with_Q(incident_beam, scattered_beam,
-                                                      wavelength):
+@given(
+    incident_beam=vector_variables(),
+    scattered_beam=vectors_variables(),
+    wavelength=space_variables(),
+)
+@settings(**global_settings)
+def test_Q_elements_from_wavelength_consistent_with_Q(
+    incident_beam, scattered_beam, wavelength
+):
     wavelength = wavelength.rename({wavelength.dim: 'wavelength'})
-    (Qx, Qy, Qz) = tof_conv.Q_elements_from_wavelength(wavelength=wavelength,
-                                                       incident_beam=incident_beam,
-                                                       scattered_beam=scattered_beam)
-    Q_vec = sc.geometry.position(Qx, Qy, Qz)
-    Q = tof_conv.Q_from_wavelength(wavelength=wavelength,
-                                   two_theta=beamline_conv.two_theta(
-                                       incident_beam=incident_beam,
-                                       scattered_beam=scattered_beam))
+    (Qx, Qy, Qz) = tof_conv.Q_elements_from_wavelength(
+        wavelength=wavelength,
+        incident_beam=incident_beam,
+        scattered_beam=scattered_beam,
+    )
+    Q_vec = sc.spatial.as_vectors(Qx, Qy, Qz)
+    Q = tof_conv.Q_from_wavelength(
+        wavelength=wavelength,
+        two_theta=beamline_conv.two_theta(
+            incident_beam=incident_beam, scattered_beam=scattered_beam
+        ),
+    )
     assert sc.allclose(sc.norm(Q_vec), Q)
 
 
 def test_Q_elements_from_wavelength():
     incident_beam = sc.vector([0.0, 0.0, 10.0], unit='m')
-    scattered_beam = sc.vectors(dims=['pos'],
-                                values=[[1.0, 0.0, 0.0], [0.0, 1.0, 0.0],
-                                        [0.0, 1.0, 2.0]],
-                                unit='cm')
+    scattered_beam = sc.vectors(
+        dims=['pos'],
+        values=[[1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 1.0, 2.0]],
+        unit='cm',
+    )
     wavelength = sc.array(dims=['wavelength'], values=[0.3, 2.0], unit='angstrom')
-    (Qx, Qy, Qz) = tof_conv.Q_elements_from_wavelength(wavelength=wavelength,
-                                                       incident_beam=incident_beam,
-                                                       scattered_beam=scattered_beam)
-    Q_vec = sc.geometry.position(Qx, Qy, Qz)
-    assert sc.identical(Q_vec['pos', 0],
-                        2 * np.pi / wavelength * sc.vector([-1.0, 0.0, 1.0]))
-    assert sc.identical(Q_vec['pos', 1],
-                        2 * np.pi / wavelength * sc.vector([0.0, -1.0, 1.0]))
+    (Qx, Qy, Qz) = tof_conv.Q_elements_from_wavelength(
+        wavelength=wavelength,
+        incident_beam=incident_beam,
+        scattered_beam=scattered_beam,
+    )
+    Q_vec = sc.spatial.as_vectors(Qx, Qy, Qz)
+    assert sc.identical(
+        Q_vec['pos', 0], 2 * np.pi / wavelength * sc.vector([-1.0, 0.0, 1.0])
+    )
+    assert sc.identical(
+        Q_vec['pos', 1], 2 * np.pi / wavelength * sc.vector([0.0, -1.0, 1.0])
+    )
     assert sc.allclose(
-        Q_vec['pos', 2], 2 * np.pi / wavelength *
-        sc.vector([0.0, -0.4472135954999579, 0.1055728090000841]))
+        Q_vec['pos', 2],
+        2
+        * np.pi
+        / wavelength
+        * sc.vector([0.0, -0.4472135954999579, 0.1055728090000841]),
+    )
 
 
 @given(wavelength=space_variables(), two_theta=angle_variables())
 @settings(**global_settings)
 def test_dspacing_from_wavelength(wavelength, two_theta):
-    dspacing = tof_conv.dspacing_from_wavelength(wavelength=wavelength,
-                                                 two_theta=two_theta)
+    dspacing = tof_conv.dspacing_from_wavelength(
+        wavelength=wavelength, two_theta=two_theta
+    )
     assert sc.allclose(
-        dspacing, sc.to_unit(wavelength / 2 / sc.sin(two_theta / 2), unit='angstrom'))
+        dspacing, sc.to_unit(wavelength / 2 / sc.sin(two_theta / 2), unit='angstrom')
+    )
 
 
 @pytest.mark.parametrize('wavelength_dtype', ('float64', 'int64'))
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
 def test_dspacing_from_wavelength_double_precision(wavelength_dtype, two_theta_dtype):
     wavelength = sc.scalar(41.4, unit='m', dtype=wavelength_dtype)
     two_theta = sc.scalar(8.4, unit='rad', dtype=two_theta_dtype)
-    assert tof_conv.dspacing_from_wavelength(wavelength=wavelength,
-                                             two_theta=two_theta).dtype == 'float64'
+    assert (
+        tof_conv.dspacing_from_wavelength(
+            wavelength=wavelength, two_theta=two_theta
+        ).dtype
+        == 'float64'
+    )
 
 
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
 def test_dspacing_from_wavelength_single_precision(two_theta_dtype):
     wavelength = sc.scalar(41.4, unit='m', dtype='float32')
     two_theta = sc.scalar(8.4, unit='rad', dtype=two_theta_dtype)
-    assert tof_conv.dspacing_from_wavelength(wavelength=wavelength,
-                                             two_theta=two_theta).dtype == 'float32'
+    assert (
+        tof_conv.dspacing_from_wavelength(
+            wavelength=wavelength, two_theta=two_theta
+        ).dtype
+        == 'float32'
+    )
 
 
 @given(energy=energy_variables(), two_theta=angle_variables())
 @settings(**global_settings)
 def test_dspacing_from_energy(energy, two_theta):
     dspacing = tof_conv.dspacing_from_energy(energy=energy, two_theta=two_theta)
     assert sc.allclose(
         dspacing,
-        sc.to_unit(const.h / sc.sqrt(8 * const.m_n * energy) / sc.sin(two_theta / 2),
-                   unit='angstrom'))
+        sc.to_unit(
+            const.h / sc.sqrt(8 * const.m_n * energy) / sc.sin(two_theta / 2),
+            unit='angstrom',
+        ),
+    )
 
 
 @pytest.mark.parametrize('energy_dtype', ('float64', 'int64'))
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
 def test_dspacing_from_energy_double_precision(energy_dtype, two_theta_dtype):
     energy = sc.scalar(26.90, unit='J', dtype=energy_dtype)
     two_theta = sc.scalar(1.985, unit='rad', dtype=two_theta_dtype)
-    assert tof_conv.dspacing_from_energy(energy=energy,
-                                         two_theta=two_theta).dtype == 'float64'
+    assert (
+        tof_conv.dspacing_from_energy(energy=energy, two_theta=two_theta).dtype
+        == 'float64'
+    )
 
 
 @pytest.mark.parametrize('two_theta_dtype', ('float64', 'float32', 'int64'))
 def test_dspacing_from_energy_single_precision(two_theta_dtype):
     energy = sc.scalar(26.90, unit='J', dtype='float32')
     two_theta = sc.scalar(1.985, unit='rad', dtype=two_theta_dtype)
-    assert tof_conv.dspacing_from_energy(energy=energy,
-                                         two_theta=two_theta).dtype == 'float32'
+    assert (
+        tof_conv.dspacing_from_energy(energy=energy, two_theta=two_theta).dtype
+        == 'float32'
+    )
+
+
+def test_q_vec_from_q_elements():
+    Qx, Qy, Qz = (
+        sc.array(dims=['Q'], values=[2.1 * i, i / 3], unit='1/angstrom')
+        for i in range(3)
+    )
+    q_vec = tof_conv.Q_vec_from_Q_elements(Qx=Qx, Qy=Qy, Qz=Qz)
+    sc.testing.assert_identical(q_vec.fields.x, Qx)
+    sc.testing.assert_identical(q_vec.fields.y, Qy)
+    sc.testing.assert_identical(q_vec.fields.z, Qz)
+
+
+def test_q_vec_from_q_elements_raises_for_shape_mismatch():
+    Qx = sc.array(dims=['q'], values=[2.0, 3.0])
+    Qy = Qx.copy()
+    Qz = sc.array(dims=['q'], values=[2.0, 3.0, 4.0])
+    with pytest.raises(sc.DimensionError):
+        tof_conv.Q_vec_from_Q_elements(Qx=Qx, Qy=Qy, Qz=Qz)
+
+
+def test_q_vec_from_q_elements_raises_for_dim_mismatch():
+    Qx = sc.array(dims=['q'], values=[2.0, 3.0])
+    Qy = Qx.copy()
+    Qz = sc.array(dims=['Q'], values=[2.0, 3.0])
+    with pytest.raises(sc.DimensionError):
+        tof_conv.Q_vec_from_Q_elements(Qx=Qx, Qy=Qy, Qz=Qz)
+
+
+def test_q_vec_from_q_elements_raises_for_unit_mismatch():
+    Qx, Qy, Qz = (
+        sc.array(dims=['Q'], values=[2.1 * i, i / 3], unit='1/angstrom')
+        for i in range(3)
+    )
+    Qy.unit = '1/m'
+    with pytest.raises(sc.UnitError):
+        tof_conv.Q_vec_from_Q_elements(Qx=Qx, Qy=Qy, Qz=Qz)
+
+
+def make_b_matrix() -> sc.Variable:
+    """Return a B matrix.
+
+    Uses and Levi convention
+      W. R. Busing and H. A. Levy
+      Angle calculations for 3- and 4-circle X-ray and neutron diffractometers
+      Acta Cryst. (1967). 22, 457-464)
+    """
+    a = 3.1
+    b = 0.3
+    c = 1.1
+    alpha = 0.7
+    beta = 4.6
+    gamma = 1.4
+
+    return sc.spatial.linear_transform(
+        value=[
+            [a, b * np.cos(gamma), c * np.cos(beta)],
+            [0, b * np.sin(gamma), -c * np.sin(beta) * np.cos(alpha)],
+            [0, 0, 1 / c],
+        ],
+        unit='1/angstrom',
+    )
+
+
+def test_ub_matrix_from_u_and_b():
+    b_matrix = make_b_matrix()
+    u_coeffs = np.array([0.5, 0.1, -0.4, 0.9])
+    u_matrix = sc.spatial.rotation(value=u_coeffs / np.linalg.norm(u_coeffs))
+    expected = u_matrix * b_matrix
+
+    assert sc.allclose(
+        tof_conv.ub_matrix_from_u_and_b(u_matrix=u_matrix, b_matrix=b_matrix), expected
+    )
+
+
+@given(inv_q=n_space_variables(3))
+def test_hkl_vec_from_Q_vec(inv_q):
+    Qx, Qy, Qz = (sc.reciprocal(x.to(dtype='float64')) for x in inv_q)
+    Q_vec = tof_conv.Q_vec_from_Q_elements(Qx=Qx, Qy=Qy, Qz=Qz)
+
+    b_matrix = make_b_matrix()
+    u_coeffs = np.array([0.5, 0.1, -0.4, 0.9])
+    u_matrix = sc.spatial.rotation(value=u_coeffs / np.linalg.norm(u_coeffs))
+    ub_matrix = u_matrix * b_matrix
+
+    sample_rotation_coeffs = np.array([1.2, 0.8, -1.2, -0.1])
+    sample_rotation_matrix = sc.spatial.rotation(
+        value=sample_rotation_coeffs / np.linalg.norm(sample_rotation_coeffs)
+    )
+
+    hkl_vec = tof_conv.hkl_vec_from_Q_vec(
+        Q_vec=Q_vec, ub_matrix=ub_matrix, sample_rotation=sample_rotation_matrix
+    )
+
+    # hkl is dimensionless but may have a multiplier.
+    assert 'powers' not in hkl_vec.unit.to_dict()
+
+    assert hkl_vec.sizes == Q_vec.sizes
+    assert hkl_vec.dtype == sc.DType.vector3
+
+    reconstructed_Q = (
+        2 * np.pi * (sample_rotation_matrix * u_matrix * b_matrix * hkl_vec)
+    )
+    assert sc.allclose(reconstructed_Q, Q_vec)
+
+
+def test_hkl_elements_from_hkl_vec():
+    hkl_vec = sc.vector([3.1, 4.5, 6.9])
+    h, k, l = tof_conv.hkl_elements_from_hkl_vec(hkl_vec=hkl_vec)
+    sc.testing.assert_identical(h, hkl_vec.fields.x)
+    sc.testing.assert_identical(k, hkl_vec.fields.y)
+    sc.testing.assert_identical(l, hkl_vec.fields.z)
```

### Comparing `scippneutron-23.3.0/tests/convert_test.py` & `scippneutron-23.4.0/tests/convert_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 
 def make_sample_position():
     # Test assume that the sample is in the origin.
     return sc.vector(value=[0.0, 0.0, 0.0], unit='m')
 
 
 def make_position():
-    return sc.vectors(dims=['spectrum'],
-                      values=[[1.0, 0.0, 0.0], [0.1, 0.0, 1.0]],
-                      unit='m')
+    return sc.vectors(
+        dims=['spectrum'], values=[[1.0, 0.0, 0.0], [0.1, 0.0, 1.0]], unit='m'
+    )
 
 
 def make_incident_beam():
     return sc.vector(value=[0.0, 0.0, 10.0], unit='m')
 
 
 def make_scattered_beam():
-    return sc.vectors(dims=['spectrum'],
-                      values=[[1.0, 0.0, 0.0], [0.1, 0.0, 1.0]],
-                      unit='m')
+    return sc.vectors(
+        dims=['spectrum'], values=[[1.0, 0.0, 0.0], [0.1, 0.0, 1.0]], unit='m'
+    )
 
 
 def make_L1():
     return sc.norm(make_incident_beam())
 
 
 def make_L2():
@@ -47,15 +47,16 @@
 
 def make_Ltotal():
     return make_L1() + make_L2()
 
 
 def make_two_theta():
     return sc.acos(
-        sc.array(dims=['spectrum'], values=[0, 10], unit='m^2') / make_L1() / make_L2())
+        sc.array(dims=['spectrum'], values=[0, 10], unit='m^2') / make_L1() / make_L2()
+    )
 
 
 def make_tof():
     return sc.array(dims=['tof'], values=[5300.0, 6000.0, 6100.0, 7300.0], unit='us')
 
 
 _COORD_MAKERS = {
@@ -64,60 +65,54 @@
     'position': make_position,
     'incident_beam': make_incident_beam,
     'scattered_beam': make_scattered_beam,
     'L1': make_L1,
     'L2': make_L2,
     'Ltotal': make_Ltotal,
     'two_theta': make_two_theta,
-    'tof': make_tof
+    'tof': make_tof,
 }
 
 
 def make_test_data(coords=(), dataset=False):
     da = sc.DataArray(
-        sc.arange('x', 1, 7, unit='counts').fold('x', {
-            'spectrum': 2,
-            'tof': 3
-        }))
+        sc.arange('x', 1, 7, unit='counts').fold('x', {'spectrum': 2, 'tof': 3})
+    )
     for name, maker in _COORD_MAKERS.items():
         if name in coords:
             da.coords[name] = maker()
 
     if dataset:
         return sc.Dataset(data={'counts': da})
     return da
 
 
 def make_tof_binned_events():
     buffer = sc.DataArray(
         sc.zeros(dims=['event'], shape=[7], dtype=float),
         coords={
-            'tof':
-            sc.array(dims=['event'],
-                     values=[1000.0, 3000.0, 2000.0, 4000.0, 5000.0, 6000.0, 3000.0],
-                     unit='us')
-        })
-    return sc.bins(data=buffer,
-                   dim='event',
-                   begin=sc.array(dims=['spectrum'],
-                                  values=[0, 4],
-                                  dtype='int64',
-                                  unit=None),
-                   end=sc.array(dims=['spectrum'],
-                                values=[4, 7],
-                                dtype='int64',
-                                unit=None))
+            'tof': sc.array(
+                dims=['event'],
+                values=[1000.0, 3000.0, 2000.0, 4000.0, 5000.0, 6000.0, 3000.0],
+                unit='us',
+            )
+        },
+    )
+    return sc.bins(
+        data=buffer,
+        dim='event',
+        begin=sc.array(dims=['spectrum'], values=[0, 4], dtype='int64', unit=None),
+        end=sc.array(dims=['spectrum'], values=[4, 7], dtype='int64', unit=None),
+    )
 
 
 def make_count_density_variable(unit):
-    return sc.arange('x', 1.0, 7.0,
-                     unit=sc.units.counts / unit).fold('x', {
-                         'spectrum': 2,
-                         'tof': 3
-                     })
+    return sc.arange('x', 1.0, 7.0, unit=sc.units.counts / unit).fold(
+        'x', {'spectrum': 2, 'tof': 3}
+    )
 
 
 def check_tof_conversion_metadata(converted, target, coord_unit):
     assert 'tof' not in converted.coords
     assert target in converted.coords
     assert 'counts' in converted
     assert converted['counts'].sizes == {'spectrum': 2, target: 3}
@@ -135,23 +130,25 @@
 def make_dataset_in(dim):
     tof_dset = make_test_data(coords=('tof', 'Ltotal', 'two_theta'), dataset=True)
     return scn.convert(tof_dset, origin='tof', target=dim, scatter=True)
 
 
 @pytest.mark.parametrize(
     ('origin', 'target'),
-    (('tof', 'dspacing'), ('tof', 'wavelength'), ('tof', 'energy')))
+    (('tof', 'dspacing'), ('tof', 'wavelength'), ('tof', 'energy')),
+)
 def test_convert_dataset_vs_dataarray(origin, target):
     inputs = make_dataset_in(origin)
     expected = scn.convert(inputs, origin=origin, target=target, scatter=True)
     result = sc.Dataset(
         data={
             name: scn.convert(data.copy(), origin=origin, target=target, scatter=True)
             for name, data in inputs.items()
-        })
+        }
+    )
     for name, data in result.items():
         assert sc.identical(data, expected[name])
 
 
 def test_convert_input_unchanged():
     inputs = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
     original = inputs.copy(deep=True)
@@ -161,34 +158,41 @@
 
 
 TOF_TARGET_DIMS = ('dspacing', 'wavelength', 'energy')
 
 
 @pytest.mark.parametrize('target', TOF_TARGET_DIMS)
 def test_convert_slice(target):
-    tof = make_test_data(coords=('tof', 'position', 'sample_position',
-                                 'source_position'),
-                         dataset=True)
-    expected = scn.convert(tof['counts'], origin='tof', target=target,
-                           scatter=True)['spectrum', 0].copy()
+    tof = make_test_data(
+        coords=('tof', 'position', 'sample_position', 'source_position'), dataset=True
+    )
+    expected = scn.convert(tof['counts'], origin='tof', target=target, scatter=True)[
+        'spectrum', 0
+    ].copy()
     assert sc.identical(
-        scn.convert(tof['counts']['spectrum', 0].copy(),
-                    origin='tof',
-                    target=target,
-                    scatter=True), expected)
+        scn.convert(
+            tof['counts']['spectrum', 0].copy(),
+            origin='tof',
+            target=target,
+            scatter=True,
+        ),
+        expected,
+    )
     # Converting slice of item is same as item of converted slice
     assert sc.identical(
-        scn.convert(tof['counts']['spectrum', 0].copy(),
-                    origin='tof',
-                    target=target,
-                    scatter=True).data,
-        scn.convert(tof['spectrum', 0].copy(),
-                    origin='tof',
-                    target=target,
-                    scatter=True)['counts'].data)
+        scn.convert(
+            tof['counts']['spectrum', 0].copy(),
+            origin='tof',
+            target=target,
+            scatter=True,
+        ).data,
+        scn.convert(
+            tof['spectrum', 0].copy(), origin='tof', target=target, scatter=True
+        )['counts'].data,
+    )
 
 
 def test_convert_scattering_conversion_fails_with_noscatter_mode():
     tof = make_test_data(coords=('tof', 'Ltotal', 'two_theta'), dataset=True)
     scn.convert(tof, origin='tof', target='dspacing', scatter=True)  # no exception
     with pytest.raises(RuntimeError):
         scn.convert(tof, origin='tof', target='dspacing', scatter=False)
@@ -200,67 +204,77 @@
 
 
 def test_convert_coords_vs_attributes():
     with_coords = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
     with_attrs = with_coords.copy()
     with_attrs['counts'].attrs['Ltotal'] = with_attrs.coords.pop('Ltotal')
 
-    from_coords = scn.convert(with_coords,
-                              origin='tof',
-                              target='wavelength',
-                              scatter=True)
-    from_attrs = scn.convert(with_attrs,
-                             origin='tof',
-                             target='wavelength',
-                             scatter=True)
+    from_coords = scn.convert(
+        with_coords, origin='tof', target='wavelength', scatter=True
+    )
+    from_attrs = scn.convert(
+        with_attrs, origin='tof', target='wavelength', scatter=True
+    )
     assert sc.identical(from_coords, from_attrs)
 
 
 @pytest.mark.parametrize('target', ('incident_beam', 'scattered_beam'))
 def test_convert_beams(target):
-
     def check_positions(data):
         assert 'sample_position' not in data.coords
         assert ('source_position' in data.coords) == (target == 'scattered_beam')
         assert ('position' in data.coords) == (target == 'incident_beam')
 
     # A single sample position.
     original = make_test_data(coords=('position', 'sample_position', 'source_position'))
     converted = scn.convert(original, origin='position', target=target, scatter=True)
     check_positions(converted)
     assert sc.identical(
         converted.coords[target],
-        make_incident_beam() if target == 'incident_beam' else make_scattered_beam())
+        make_incident_beam() if target == 'incident_beam' else make_scattered_beam(),
+    )
 
     # Two sample positions.
     original = make_test_data(coords=('position', 'source_position'))
-    original.coords['sample_position'] = sc.vectors(dims=['spectrum'],
-                                                    values=[[1.0, 0.0, 0.2],
-                                                            [2.1, -0.3, 1.4]],
-                                                    unit='m')
+    original.coords['sample_position'] = sc.vectors(
+        dims=['spectrum'], values=[[1.0, 0.0, 0.2], [2.1, -0.3, 1.4]], unit='m'
+    )
     converted = scn.convert(original, origin='position', target=target, scatter=True)
     check_positions(converted)
     if target == 'incident_beam':
-        assert sc.allclose(converted.coords['incident_beam'],
-                           sc.vectors(dims=['spectrum'],
-                                      values=[[1.0, 0.0, 10.2], [2.1, -0.3, 11.4]],
-                                      unit='m'),
-                           rtol=1e-14 * sc.units.one)
+        assert sc.allclose(
+            converted.coords['incident_beam'],
+            sc.vectors(
+                dims=['spectrum'],
+                values=[[1.0, 0.0, 10.2], [2.1, -0.3, 11.4]],
+                unit='m',
+            ),
+            rtol=1e-14 * sc.units.one,
+        )
     if target == 'scattered_beam':
-        assert sc.allclose(converted.coords['scattered_beam'],
-                           sc.vectors(dims=['spectrum'],
-                                      values=[[0.0, 0.0, -0.2], [-2.0, 0.3, -0.4]],
-                                      unit='m'),
-                           rtol=1e-14 * sc.units.one)
+        assert sc.allclose(
+            converted.coords['scattered_beam'],
+            sc.vectors(
+                dims=['spectrum'],
+                values=[[0.0, 0.0, -0.2], [-2.0, 0.3, -0.4]],
+                unit='m',
+            ),
+            rtol=1e-14 * sc.units.one,
+        )
 
 
 @pytest.mark.parametrize(
     ('target', 'make_ref'),
-    (('L1', make_L1), ('L2', make_L2), ('two_theta', make_two_theta),
-     ('Ltotal', lambda: make_L1() + make_L2())))
+    (
+        ('L1', make_L1),
+        ('L2', make_L2),
+        ('two_theta', make_two_theta),
+        ('Ltotal', lambda: make_L1() + make_L2()),
+    ),
+)
 def test_convert_beam_length_and_angle(target, make_ref):
     original = make_test_data(coords=('incident_beam', 'scattered_beam'))
     converted = scn.convert(original, origin='position', target=target, scatter=True)
     assert sc.allclose(converted.meta[target], make_ref(), rtol=sc.scalar(1e-12))
 
 
 def test_convert_beam_length_no_scatter():
@@ -278,45 +292,50 @@
     # Rule of thumb (https://www.psi.ch/niag/neutron-physics):
     # v [m/s] = 3956 / \lambda [ Angstrom ]
     tof_in_seconds = tof.coords['tof'] * 1e-6
 
     # Spectrum 0 is 11 m from source
     # 2d sin(theta) = n \lambda
     # theta = 45 deg => d = lambda / (2 * 1 / sqrt(2))
-    for val, t in zip(dspacing.coords['dspacing']['spectrum', 0].values,
-                      tof_in_seconds.values):
-        np.testing.assert_almost_equal(val, 3956.0 / (11.0 / t) / math.sqrt(2.0),
-                                       val * 1e-3)
+    for val, t in zip(
+        dspacing.coords['dspacing']['spectrum', 0].values, tof_in_seconds.values
+    ):
+        np.testing.assert_almost_equal(
+            val, 3956.0 / (11.0 / t) / math.sqrt(2.0), val * 1e-3
+        )
 
     # Spectrum 1
     # sin(2 theta) = 0.1/(L-10)
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
     lambda_to_d = 1.0 / (2.0 * math.sin(0.5 * math.asin(0.1 / (L - 10.0))))
-    for val, t in zip(dspacing.coords['dspacing']['spectrum', 1].values,
-                      tof_in_seconds.values):
+    for val, t in zip(
+        dspacing.coords['dspacing']['spectrum', 1].values, tof_in_seconds.values
+    ):
         np.testing.assert_almost_equal(val, 3956.0 / (L / t) * lambda_to_d, val * 1e-3)
 
 
 def test_convert_tof_to_wavelength():
     tof = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
     wavelength = scn.convert(tof, origin='tof', target='wavelength', scatter=True)
     check_tof_conversion_metadata(wavelength, 'wavelength', sc.units.angstrom)
 
     # Rule of thumb (https://www.psi.ch/niag/neutron-physics):
     # v [m/s] = 3956 / \lambda [ Angstrom ]
     tof_in_seconds = tof.coords['tof'] * 1e-6
 
     # Spectrum 0 is 11 m from source
-    for val, t in zip(wavelength.coords['wavelength']['spectrum', 0].values,
-                      tof_in_seconds.values):
+    for val, t in zip(
+        wavelength.coords['wavelength']['spectrum', 0].values, tof_in_seconds.values
+    ):
         np.testing.assert_almost_equal(val, 3956.0 / (11.0 / t), val * 1e-3)
     # Spectrum 1
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
-    for val, t in zip(wavelength.coords['wavelength']['spectrum', 1].values,
-                      tof_in_seconds.values):
+    for val, t in zip(
+        wavelength.coords['wavelength']['spectrum', 1].values, tof_in_seconds.values
+    ):
         np.testing.assert_almost_equal(val, 3956.0 / (L / t), val * 1e-3)
 
 
 def test_convert_tof_to_wavelength_no_scatter():
     # scatter=True and scatter=False only differ in how Ltotal is computed.
     tof = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
     no_scatter = scn.convert(tof, origin='tof', target='wavelength', scatter=False)
@@ -324,83 +343,90 @@
     assert sc.identical(no_scatter, scatter)
 
 
 def test_convert_tof_to_Q():
     tof = make_test_data(coords=('tof', 'Ltotal', 'two_theta'), dataset=True)
     wavelength = scn.convert(tof, origin='tof', target='wavelength', scatter=True)
     Q_from_tof = scn.convert(tof, origin='tof', target='Q', scatter=True)
-    Q_from_wavelength = scn.convert(wavelength,
-                                    origin='wavelength',
-                                    target='Q',
-                                    scatter=True)
+    Q_from_wavelength = scn.convert(
+        wavelength, origin='wavelength', target='Q', scatter=True
+    )
     check_tof_conversion_metadata(Q_from_tof, 'Q', sc.units.one / sc.units.angstrom)
-    check_tof_conversion_metadata(Q_from_wavelength, 'Q',
-                                  sc.units.one / sc.units.angstrom)
+    check_tof_conversion_metadata(
+        Q_from_wavelength, 'Q', sc.units.one / sc.units.angstrom
+    )
     # wavelength is intermediate in this case and thus kept but not in the other case.
     assert sc.identical(Q_from_tof, Q_from_wavelength)
 
     # Rule of thumb (c):
     # v [m/s] = 3956 / \lambda [ Angstrom ]
     tof_in_seconds = tof.coords['tof'] * 1e-6
 
     # Spectrum 0 is 11 m from source
     # Q = 4pi sin(theta) / lambda
     # theta = 45 deg => Q = 2 sqrt(2) pi / lambda
-    for val, t in zip(Q_from_wavelength.coords['Q']['spectrum', 0].values,
-                      tof_in_seconds.values):
+    for val, t in zip(
+        Q_from_wavelength.coords['Q']['spectrum', 0].values, tof_in_seconds.values
+    ):
         np.testing.assert_almost_equal(
-            val, 2.0 * math.sqrt(2.0) * math.pi / (3956.0 / (11.0 / t)), val * 1e-3)
+            val, 2.0 * math.sqrt(2.0) * math.pi / (3956.0 / (11.0 / t)), val * 1e-3
+        )
 
     # Spectrum 1
     # sin(2 theta) = 0.1/(L-10)
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
     lambda_to_Q = 4.0 * math.pi * math.sin(math.asin(0.1 / (L - 10.0)) / 2.0)
-    for val, t in zip(Q_from_wavelength.coords['Q']['spectrum', 1].values,
-                      tof_in_seconds.values):
-        np.testing.assert_almost_equal(val, lambda_to_Q / (3956.0 / (L / t)),
-                                       val * 1e-3)
+    for val, t in zip(
+        Q_from_wavelength.coords['Q']['spectrum', 1].values, tof_in_seconds.values
+    ):
+        np.testing.assert_almost_equal(
+            val, lambda_to_Q / (3956.0 / (L / t)), val * 1e-3
+        )
 
 
 def test_convert_Q_to_wavelength():
     tof = make_test_data(coords=('tof', 'Ltotal', 'two_theta'))
     Q = scn.convert(tof, origin='tof', target='Q', scatter=True)
     del Q.attrs['wavelength']
     wavelength_from_Q = scn.convert(Q, origin='Q', target='wavelength', scatter=True)
-    wavelength_from_tof = scn.convert(tof,
-                                      origin='tof',
-                                      target='wavelength',
-                                      scatter=True)
-    assert sc.allclose(wavelength_from_Q.coords['wavelength'],
-                       wavelength_from_tof.coords['wavelength'],
-                       rtol=1e-14 * sc.units.one)
+    wavelength_from_tof = scn.convert(
+        tof, origin='tof', target='wavelength', scatter=True
+    )
+    assert sc.allclose(
+        wavelength_from_Q.coords['wavelength'],
+        wavelength_from_tof.coords['wavelength'],
+        rtol=1e-14 * sc.units.one,
+    )
 
 
 def test_convert_tof_to_energy_elastic():
     tof = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
     energy = scn.convert(tof, origin='tof', target='energy', scatter=True)
     check_tof_conversion_metadata(energy, 'energy', sc.units.meV)
 
     tof_in_seconds = sc.to_unit(tof.coords['tof'], 's')
     # e [J] = 1/2 m(n) [kg] (l [m] / tof [s])^2
     joule_to_mev = sc.to_unit(1.0 * sc.Unit('J'), sc.units.meV).value
     neutron_mass = sc.to_unit(m_n, sc.units.kg).value
 
     # Spectrum 0 is 11 m from source
-    for val, t in zip(energy.coords['energy']['spectrum', 0].values,
-                      tof_in_seconds.values):
-        np.testing.assert_almost_equal(val,
-                                       joule_to_mev * neutron_mass / 2 * (11 / t)**2,
-                                       val * 1e-3)
+    for val, t in zip(
+        energy.coords['energy']['spectrum', 0].values, tof_in_seconds.values
+    ):
+        np.testing.assert_almost_equal(
+            val, joule_to_mev * neutron_mass / 2 * (11 / t) ** 2, val * 1e-3
+        )
     # Spectrum 1
     L = 10.0 + math.sqrt(1.0 * 1.0 + 0.1 * 0.1)
-    for val, t in zip(energy.coords['energy']['spectrum', 1].values,
-                      tof_in_seconds.values):
-        np.testing.assert_almost_equal(val,
-                                       joule_to_mev * 0.5 * neutron_mass * (L / t)**2,
-                                       val * 1e-3)
+    for val, t in zip(
+        energy.coords['energy']['spectrum', 1].values, tof_in_seconds.values
+    ):
+        np.testing.assert_almost_equal(
+            val, joule_to_mev * 0.5 * neutron_mass * (L / t) ** 2, val * 1e-3
+        )
 
 
 def test_convert_tof_to_energy_elastic_no_scatter():
     # scatter=True and scatter=False only differ in how Ltotal is computed.
     tof = make_test_data(coords=('tof', 'Ltotal'), dataset=True)
     no_scatter = scn.convert(tof, origin='tof', target='energy', scatter=False)
     scatter = scn.convert(tof, origin='tof', target='energy', scatter=True)
@@ -431,56 +457,61 @@
     tof.coords['incident_energy'] = ei
     direct = scn.convert(tof, origin='tof', target='energy_transfer', scatter=True)
     check_tof_conversion_metadata(direct, 'energy_transfer', sc.units.meV)
 
     t = tof.coords['tof']
     t0 = sc.to_unit(tof.coords['L1'] * sc.sqrt(m_n / 2 / ei), t.unit)
     assert sc.all(t0 < t).value  # only test physical region here
-    ref = ei - sc.to_unit(m_n / 2 * (tof.coords['L2'] / (t - t0))**2,
-                          ei.unit).rename_dims({'tof': 'energy_transfer'})
+    ref = ei - sc.to_unit(
+        m_n / 2 * (tof.coords['L2'] / (t - t0)) ** 2, ei.unit
+    ).rename_dims({'tof': 'energy_transfer'})
     assert sc.allclose(direct.coords['energy_transfer'], ref, rtol=sc.scalar(1e-13))
 
 
 def make_unphysical_tof(t0, da):
     # 0 < t < t0, t < 0, t > t0
     tof = sc.concat([t0 - t0 / 2, sc.full_like(t0, -2), 2 * t0], 'tof')
-    is_unphysical = sc.array(dims=['energy_transfer'],
-                             values=[True, True,
-                                     False]).broadcast(['energy_transfer', 'spectrum'],
-                                                       [3, da.sizes['spectrum']])
+    is_unphysical = sc.array(
+        dims=['energy_transfer'], values=[True, True, False]
+    ).broadcast(['energy_transfer', 'spectrum'], [3, da.sizes['spectrum']])
     return tof, is_unphysical
 
 
 def test_convert_tof_to_energy_transfer_direct_unphysical():
     tof = make_test_data(coords=('tof', 'L1', 'L2'), dataset=True)
     ei = 35.0 * sc.units.meV
     tof.coords['incident_energy'] = ei
     t0 = sc.to_unit(tof.coords['L1'] * sc.sqrt(m_n / ei), sc.units.s)
     coord, is_unphysical = make_unphysical_tof(t0, tof)
     tof.coords['tof'] = coord
 
     result = scn.convert(tof, origin='tof', target='energy_transfer', scatter=True)
-    assert sc.identical(sc.isnan(result.coords['energy_transfer']),
-                        is_unphysical.transpose(result.dims))
+    assert sc.identical(
+        sc.isnan(result.coords['energy_transfer']), is_unphysical.transpose(result.dims)
+    )
 
 
 def test_convert_tof_to_energy_transfer_indirect():
     tof = make_test_data(coords=('tof', 'L1', 'L2'), dataset=True)
     with pytest.raises(RuntimeError):
         scn.convert(tof, origin='tof', target='energy_transfer', scatter=True)
     ef = 25.0 * sc.units.meV
     tof.coords['final_energy'] = ef
     indirect = scn.convert(tof, origin='tof', target='energy_transfer', scatter=True)
     check_tof_conversion_metadata(indirect, 'energy_transfer', sc.units.meV)
 
     t = tof.coords['tof']
     t0 = sc.to_unit(tof.coords['L2'] * sc.sqrt(m_n / 2 / ef), t.unit)
     assert sc.all(t0 < t).value  # only test physical region here
-    ref = sc.to_unit(m_n / 2 * (tof.coords['L1'] / (t - t0))**2, ef.unit).rename_dims(
-        {'tof': 'energy_transfer'}) - ef
+    ref = (
+        sc.to_unit(m_n / 2 * (tof.coords['L1'] / (t - t0)) ** 2, ef.unit).rename_dims(
+            {'tof': 'energy_transfer'}
+        )
+        - ef
+    )
     assert sc.allclose(indirect.coords['energy_transfer'], ref, rtol=sc.scalar(1e-13))
 
 
 def test_convert_tof_to_energy_transfer_indirect_unphysical():
     tof = make_test_data(coords=('tof', 'L1', 'L2'), dataset=True)
     ef = 25.0 * sc.units.meV
     tof.coords['final_energy'] = ef
@@ -499,110 +530,116 @@
     with pytest.raises(RuntimeError):
         scn.convert(tof, origin='tof', target='energy_transfer', scatter=True)
 
 
 def test_convert_tof_to_energy_transfer_direct_indirect_are_distinct():
     tof_direct = make_test_data(coords=('tof', 'L1', 'L2'), dataset=True)
     tof_direct.coords['incident_energy'] = 22.0 * sc.units.meV
-    direct = scn.convert(tof_direct,
-                         origin='tof',
-                         target='energy_transfer',
-                         scatter=True)
+    direct = scn.convert(
+        tof_direct, origin='tof', target='energy_transfer', scatter=True
+    )
 
     tof_indirect = make_test_data(coords=('tof', 'L1', 'L2'), dataset=True)
     tof_indirect.coords['final_energy'] = 22.0 * sc.units.meV
-    indirect = scn.convert(tof_indirect,
-                           origin='tof',
-                           target='energy_transfer',
-                           scatter=True)
-    assert not sc.allclose(direct.coords['energy_transfer'],
-                           indirect.coords['energy_transfer'],
-                           rtol=0.0 * sc.units.one,
-                           atol=1e-11 * sc.units.meV)
+    indirect = scn.convert(
+        tof_indirect, origin='tof', target='energy_transfer', scatter=True
+    )
+    assert not sc.allclose(
+        direct.coords['energy_transfer'],
+        indirect.coords['energy_transfer'],
+        rtol=0.0 * sc.units.one,
+        atol=1e-11 * sc.units.meV,
+    )
 
 
 # Test conversions between quantities that are themselves
 # outputs of conversions from tof.
 @pytest.mark.parametrize('keep_tof', (False, True))
-@pytest.mark.parametrize(('target', 'target_unit'),
-                         (('energy', sc.units.meV), ('wavelength', sc.units.angstrom),
-                          ('dspacing', sc.units.angstrom)))
+@pytest.mark.parametrize(
+    ('target', 'target_unit'),
+    (
+        ('energy', sc.units.meV),
+        ('wavelength', sc.units.angstrom),
+        ('dspacing', sc.units.angstrom),
+    ),
+)
 @pytest.mark.parametrize('origin', ('energy', 'wavelength'))
 def test_convert_non_tof(origin, target, target_unit, keep_tof):
     tof = make_test_data(coords=('tof', 'Ltotal', 'two_theta'), dataset=True)
     original = scn.convert(tof, origin='tof', target=origin, scatter=True)
     if not keep_tof:
         del original['counts'].attrs['tof']
     converted = scn.convert(original, origin=origin, target=target, scatter=True)
     check_tof_conversion_metadata(converted, target, target_unit)
     converted_from_tof = scn.convert(tof, origin='tof', target=target, scatter=True)
-    assert sc.allclose(converted.coords[target],
-                       converted_from_tof.coords[target],
-                       rtol=1e-14 * sc.units.one)
+    assert sc.allclose(
+        converted.coords[target],
+        converted_from_tof.coords[target],
+        rtol=1e-14 * sc.units.one,
+    )
 
 
 def test_convert_with_factor_type_promotion():
     tof = make_test_data(coords=('tof', 'L1', 'L2', 'two_theta'))
-    tof.coords['tof'] = sc.array(dims=['tof'],
-                                 values=[4000, 5000, 6100, 7300],
-                                 unit='us',
-                                 dtype='float32')
+    tof.coords['tof'] = sc.array(
+        dims=['tof'], values=[4000, 5000, 6100, 7300], unit='us', dtype='float32'
+    )
     for target in TOF_TARGET_DIMS:
         res = scn.convert(tof, origin='tof', target=target, scatter=True)
         assert res.coords[target].dtype == sc.DType.float32
 
     for key in ('incident_energy', 'final_energy'):
         inelastic = tof.copy()
         inelastic.coords[key] = sc.scalar(35, dtype=sc.DType.float32, unit=sc.units.meV)
-        res = scn.convert(inelastic,
-                          origin='tof',
-                          target='energy_transfer',
-                          scatter=True)
+        res = scn.convert(
+            inelastic, origin='tof', target='energy_transfer', scatter=True
+        )
         assert res.coords['energy_transfer'].dtype == sc.DType.float32
 
 
 @pytest.mark.parametrize('target', TOF_TARGET_DIMS)
 def test_convert_integer_input_elastic(target):
     da_float_coord = make_test_data(coords=('tof', 'L1', 'L2', 'two_theta'))
     da_int_coord = da_float_coord.copy()
     da_int_coord.coords['tof'] = da_float_coord.coords['tof'].astype('int64')
 
     res = scn.convert(da_int_coord, origin='tof', target=target, scatter=True)
     expected = scn.convert(da_float_coord, origin='tof', target=target, scatter=True)
     assert res.coords[target].dtype == sc.DType.float64
-    assert sc.allclose(res.coords[target],
-                       expected.coords[target],
-                       rtol=1e-15 * sc.units.one)
+    assert sc.allclose(
+        res.coords[target], expected.coords[target], rtol=1e-15 * sc.units.one
+    )
 
 
 @pytest.mark.parametrize('input_energy', ('incident_energy', 'final_energy'))
-@pytest.mark.parametrize('input_dtypes', (('int64', 'float64'), ('float64', 'int64'),
-                                          ('int64', 'int64')))
+@pytest.mark.parametrize(
+    'input_dtypes', (('int64', 'float64'), ('float64', 'int64'), ('int64', 'int64'))
+)
 def test_convert_integer_input_inelastic(input_energy, input_dtypes):
     da_float_coord = make_test_data(coords=('tof', 'L1', 'L2', 'two_theta'))
-    da_float_coord.coords[input_energy] = sc.scalar(35,
-                                                    dtype=sc.DType.float64,
-                                                    unit=sc.units.meV)
+    da_float_coord.coords[input_energy] = sc.scalar(
+        35, dtype=sc.DType.float64, unit=sc.units.meV
+    )
 
     da_int_coord = da_float_coord.copy()
     for i, name in enumerate(('tof', input_energy)):
         da_int_coord.coords[name] = da_float_coord.coords[name].astype(input_dtypes[i])
 
-    res = scn.convert(da_int_coord,
-                      origin='tof',
-                      target='energy_transfer',
-                      scatter=True)
-    expected = scn.convert(da_float_coord,
-                           origin='tof',
-                           target='energy_transfer',
-                           scatter=True)
+    res = scn.convert(
+        da_int_coord, origin='tof', target='energy_transfer', scatter=True
+    )
+    expected = scn.convert(
+        da_float_coord, origin='tof', target='energy_transfer', scatter=True
+    )
     assert res.coords['energy_transfer'].dtype == sc.DType.float64
-    assert sc.allclose(res.coords['energy_transfer'],
-                       expected.coords['energy_transfer'],
-                       rtol=1e-14 * sc.units.one)
+    assert sc.allclose(
+        res.coords['energy_transfer'],
+        expected.coords['energy_transfer'],
+        rtol=1e-14 * sc.units.one,
+    )
 
 
 @pytest.mark.parametrize('target', TOF_TARGET_DIMS)
 def test_convert_binned_events_converted(target):
     tof = make_test_data(coords=('Ltotal', 'two_theta'), dataset=True)
     del tof['counts']
     tof['events'] = make_tof_binned_events()
@@ -624,13 +661,12 @@
 
 @pytest.mark.parametrize('target', TOF_TARGET_DIMS)
 def test_convert_binned_convert_slice(target):
     tof = make_test_data(coords=('tof', 'Ltotal', 'two_theta'))['tof', 0].copy()
     tof.data = make_tof_binned_events()
     original = tof.copy()
     full = scn.convert(tof, origin='tof', target=target, scatter=True)
-    sliced = scn.convert(tof['spectrum', 1:2],
-                         origin='tof',
-                         target=target,
-                         scatter=True)
+    sliced = scn.convert(
+        tof['spectrum', 1:2], origin='tof', target=target, scatter=True
+    )
     assert sc.identical(sliced, full['spectrum', 1:2])
     assert sc.identical(tof, original)
```

### Comparing `scippneutron-23.3.0/tests/data_stream_test.py` & `scippneutron-23.4.0/tests/data_stream_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import pytest
 import scipp as sc
 
 from scippneutron.data_streaming._consumer_type import ConsumerType
-from scippneutron.data_streaming._warnings import BufferSizeWarning, \
-    UnknownFlatbufferIdWarning
+from scippneutron.data_streaming._warnings import (
+    BufferSizeWarning,
+    UnknownFlatbufferIdWarning,
+)
 
 from .nexus_helpers import EventData, Log, NexusBuilder, Stream
 
 if platform.system() == "Darwin":
     pytest.skip(
         "Streaming tests disabled on MacOS because they tend to hang"
         " indefinitely for unknown reasons",
-        allow_module_level=True)
+        allow_module_level=True,
+    )
 
 try:
     import streaming_data_types  # noqa: F401
     from confluent_kafka import KafkaError, TopicPartition  # noqa: F401
     from streaming_data_types.eventdata_ev42 import serialise_ev42  # noqa: E402
     from streaming_data_types.logdata_f142 import serialise_f142
     from streaming_data_types.run_start_pl72 import serialise_pl72
@@ -36,31 +39,28 @@
     from scippneutron.data_streaming.data_stream import _data_stream  # noqa: E402
     from scippneutron.data_streaming.data_stream import StopTime
 except ImportError:
     pytest.skip("Kafka or Serialisation module is unavailable", allow_module_level=True)
 
 
 class FakeKafkaError:
-
     def __init__(self, kafka_error_code: int):
         self._error_code = kafka_error_code
 
     def code(self):
         return self._error_code
 
     def __str__(self):
         return f"FakeKafkaError: code {self._error_code}"
 
 
 class FakeMessage:
-
-    def __init__(self,
-                 payload: bytes,
-                 error_code: Optional[int] = None,
-                 timestamp: int = 0):
+    def __init__(
+        self, payload: bytes, error_code: Optional[int] = None, timestamp: int = 0
+    ):
         self._payload = payload
         self._error_code = error_code
         self._timestamp = timestamp
 
     def value(self):
         return self._payload
 
@@ -70,22 +70,23 @@
         return None
 
     def timestamp(self) -> Tuple[None, int]:
         return None, self._timestamp
 
 
 class FakeQueryConsumer:
-
-    def __init__(self,
-                 instrument_name: str = "",
-                 low_and_high_offset: Tuple[int, int] = (2, 10),
-                 streams: List[Stream] = None,
-                 start_time: Optional[Union[int, datetime.datetime]] = None,
-                 stop_time: Optional[Union[int, datetime.datetime]] = None,
-                 nexus_structure: Optional[str] = None):
+    def __init__(
+        self,
+        instrument_name: str = "",
+        low_and_high_offset: Tuple[int, int] = (2, 10),
+        streams: List[Stream] = None,
+        start_time: Optional[Union[int, datetime.datetime]] = None,
+        stop_time: Optional[Union[int, datetime.datetime]] = None,
+        nexus_structure: Optional[str] = None,
+    ):
         self._instrument_name = instrument_name
         self._low_and_high_offset = low_and_high_offset
         self._streams = streams
         self.queried_topics = []
         self.queried_timestamp = None
         self._start_time = start_time
         self._stop_time = stop_time
@@ -104,52 +105,55 @@
     @staticmethod
     def assign(partitions: List[TopicPartition]):
         pass
 
     def get_watermark_offsets(self, partition: TopicPartition) -> Tuple[int, int]:
         return self._low_and_high_offset
 
-    def get_topic_partitions(self,
-                             topic: str,
-                             offset: int = -1) -> List[TopicPartition]:
+    def get_topic_partitions(
+        self, topic: str, offset: int = -1
+    ) -> List[TopicPartition]:
         self.queried_topics.append(topic)
         return [TopicPartition(topic, partition=0, offset=offset)]
 
-    def poll(self, timeout=2.) -> FakeMessage:
+    def poll(self, timeout=2.0) -> FakeMessage:
         return FakeMessage(
-            serialise_pl72("",
-                           "",
-                           start_time=self._start_time,
-                           stop_time=self._stop_time,
-                           nexus_structure=self._nexus_structure))
+            serialise_pl72(
+                "",
+                "",
+                start_time=self._start_time,
+                stop_time=self._stop_time,
+                nexus_structure=self._nexus_structure,
+            )
+        )
 
     def seek(self, partition: TopicPartition):
         pass
 
     def offsets_for_times(self, partitions: List[TopicPartition]):
         self.queried_timestamp = partitions[0].offset
         return partitions
 
 
 # Short time to use for buffer emit and data_stream interval in tests
 # pass or fail fast!
-SHORT_TEST_INTERVAL = 100. * sc.Unit('milliseconds')
+SHORT_TEST_INTERVAL = 100.0 * sc.Unit('milliseconds')
 # Small buffer of 20 events is sufficient for the tests
 TEST_BUFFER_SIZE = 20
 
 TEST_STREAM_ARGS = {
     "kafka_broker": "broker",
     "topics": ["topic"],
     "interval": SHORT_TEST_INTERVAL,
     "event_buffer_size": TEST_BUFFER_SIZE,
     "slow_metadata_buffer_size": TEST_BUFFER_SIZE,
     "fast_metadata_buffer_size": TEST_BUFFER_SIZE,
     "chopper_buffer_size": TEST_BUFFER_SIZE,
     "consumer_type": ConsumerType.FAKE,
-    "timeout": 10. * sc.units.s
+    "timeout": 10.0 * sc.units.s,
 }
 # "timeout" arg: if something gets broken then this makes sure the
 # test will not get stuck in the _data_stream loop indefinitely.
 # A TimeoutError is raised by _data_stream if the timeout occurs.
 
 
 @pytest.fixture(scope="function")
@@ -163,52 +167,58 @@
     ctx = mp.get_context("spawn")
     return ctx.Queue(), ctx.Queue(), ctx.Queue()
 
 
 @pytest.mark.asyncio
 async def test_data_stream_returns_data_from_single_event_message(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
-    time_of_flight = np.array([1., 2., 3.])
+    time_of_flight = np.array([1.0, 2.0, 3.0])
     detector_ids = np.array([4, 5, 6])
     test_message = FakeMessage(
-        serialise_ev42("detector", 0, 0, time_of_flight, detector_ids))
+        serialise_ev42("detector", 0, 0, time_of_flight, detector_ids)
+    )
     test_message_queue.put(test_message)
 
     reached_assert = False
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   halt_after_n_data_chunks=1,
-                                   test_message_queue=test_message_queue,
-                                   query_consumer=FakeQueryConsumer(),
-                                   **TEST_STREAM_ARGS):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        halt_after_n_data_chunks=1,
+        test_message_queue=test_message_queue,
+        query_consumer=FakeQueryConsumer(),
+        **TEST_STREAM_ARGS,
+    ):
         assert np.allclose(data.coords['tof'].values, time_of_flight)
         reached_assert = True
     assert reached_assert
 
 
 @pytest.mark.asyncio
 async def test_data_stream_returns_data_from_multiple_event_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
-    first_tof = np.array([1., 2., 3.])
+    first_tof = np.array([1.0, 2.0, 3.0])
     first_detector_ids = np.array([4, 5, 6])
     first_test_message = serialise_ev42("detector", 0, 0, first_tof, first_detector_ids)
-    second_tof = np.array([1., 2., 3.])
+    second_tof = np.array([1.0, 2.0, 3.0])
     second_detector_ids = np.array([4, 5, 6])
-    second_test_message = serialise_ev42("detector", 0, 0, second_tof,
-                                         second_detector_ids)
+    second_test_message = serialise_ev42(
+        "detector", 0, 0, second_tof, second_detector_ids
+    )
     test_message_queue.put(FakeMessage(first_test_message))
     test_message_queue.put(FakeMessage(second_test_message))
 
     reached_asserts = False
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   halt_after_n_data_chunks=1,
-                                   test_message_queue=test_message_queue,
-                                   query_consumer=FakeQueryConsumer(),
-                                   **TEST_STREAM_ARGS):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        halt_after_n_data_chunks=1,
+        test_message_queue=test_message_queue,
+        query_consumer=FakeQueryConsumer(),
+        **TEST_STREAM_ARGS,
+    ):
         expected_tofs = np.concatenate((first_tof, second_tof))
         assert np.allclose(data.coords['tof'].values, expected_tofs)
         expected_ids = np.concatenate((first_detector_ids, second_detector_ids))
         assert np.array_equal(data.coords['detector_id'].values, expected_ids)
         reached_asserts = True
     assert reached_asserts
 
@@ -220,73 +230,80 @@
     # First 4 bytes of the message payload are the FlatBuffer schema identifier
     # "abcd" does not correspond to a FlatBuffer schema for data
     # that scipp is interested in
     test_message = b"abcd0000"
 
     with pytest.warns(UnknownFlatbufferIdWarning):
         test_message_queue.put(FakeMessage(test_message))
-        async for _ in _data_stream(data_queue,
-                                    worker_instruction_queue,
-                                    halt_after_n_warnings=1,
-                                    test_message_queue=test_message_queue,
-                                    query_consumer=FakeQueryConsumer(),
-                                    **TEST_STREAM_ARGS):
+        async for _ in _data_stream(
+            data_queue,
+            worker_instruction_queue,
+            halt_after_n_warnings=1,
+            test_message_queue=test_message_queue,
+            query_consumer=FakeQueryConsumer(),
+            **TEST_STREAM_ARGS,
+        ):
             test_message_queue.put(FakeMessage(test_message))
 
 
 @pytest.mark.asyncio
 async def test_warn_on_buffer_size_exceeded_by_single_message(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     buffer_size_2_events = 2
-    time_of_flight = np.array([1., 2., 3.])
+    time_of_flight = np.array([1.0, 2.0, 3.0])
     detector_ids = np.array([4, 5, 6])
     test_message = serialise_ev42("detector", 0, 0, time_of_flight, detector_ids)
 
     test_steam_args = TEST_STREAM_ARGS.copy()
     test_steam_args["event_buffer_size"] = buffer_size_2_events
 
     with pytest.warns(BufferSizeWarning):
         test_message_queue.put(FakeMessage(test_message))
-        async for _ in _data_stream(data_queue,
-                                    worker_instruction_queue,
-                                    halt_after_n_warnings=1,
-                                    test_message_queue=test_message_queue,
-                                    query_consumer=FakeQueryConsumer(),
-                                    **test_steam_args):
+        async for _ in _data_stream(
+            data_queue,
+            worker_instruction_queue,
+            halt_after_n_warnings=1,
+            test_message_queue=test_message_queue,
+            query_consumer=FakeQueryConsumer(),
+            **test_steam_args,
+        ):
             test_message_queue.put(FakeMessage(test_message))
 
 
 @pytest.mark.asyncio
 async def test_data_returned_when_buffer_size_exceeded_by_event_messages(queues):
     # Messages cumulatively exceed the buffer size, data_stream
     # will return multiple chunks of data to clear the buffer
     # between messages.
     data_queue, worker_instruction_queue, test_message_queue = queues
-    first_tof = np.array([1., 2., 3.])
+    first_tof = np.array([1.0, 2.0, 3.0])
     first_detector_ids = np.array([4, 5, 6])
     first_test_message = serialise_ev42("detector", 0, 0, first_tof, first_detector_ids)
-    second_tof = np.array([7., 8., 9.])
+    second_tof = np.array([7.0, 8.0, 9.0])
     second_detector_ids = np.array([4, 5, 6])
-    second_test_message = serialise_ev42("detector", 0, 0, second_tof,
-                                         second_detector_ids)
+    second_test_message = serialise_ev42(
+        "detector", 0, 0, second_tof, second_detector_ids
+    )
 
     # Event data buffer size is 5, so the second message
     # will not fit in the buffer
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["event_buffer_size"] = 5
     test_stream_args["run_info_topic"] = "run_info_topic"
 
     reached_asserts = False
     n_chunks = 0
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   halt_after_n_data_chunks=3,
-                                   test_message_queue=test_message_queue,
-                                   query_consumer=FakeQueryConsumer(),
-                                   **test_stream_args):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        halt_after_n_data_chunks=3,
+        test_message_queue=test_message_queue,
+        query_consumer=FakeQueryConsumer(),
+        **test_stream_args,
+    ):
         # n_chunks == 0 zeroth chunk contains data
         # from run start message
         if n_chunks == 0:
             test_message_queue.put(FakeMessage(first_test_message))
             test_message_queue.put(FakeMessage(second_test_message))
         elif n_chunks == 1:
             # Contain event data from first message
@@ -303,21 +320,22 @@
 @pytest.mark.asyncio
 async def test_data_are_loaded_from_run_start_message(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     reached_assert = False
     test_instrument_name = "DATA_STREAM_TEST"
     async for data in _data_stream(
-            data_queue,
-            worker_instruction_queue,
-            run_info_topic=run_info_topic,
-            halt_after_n_data_chunks=0,
-            test_message_queue=test_message_queue,
-            query_consumer=FakeQueryConsumer(test_instrument_name),
-            **TEST_STREAM_ARGS):
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        halt_after_n_data_chunks=0,
+        test_message_queue=test_message_queue,
+        query_consumer=FakeQueryConsumer(test_instrument_name),
+        **TEST_STREAM_ARGS,
+    ):
         assert data["instrument_name"].value == test_instrument_name
         reached_assert = True
     assert reached_assert
 
 
 @pytest.mark.asyncio
 async def test_error_raised_if_no_run_start_message_available(queues):
@@ -325,64 +343,70 @@
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # Low and high offset are the same value, indicates there are
     # no messages available in the partition
     low_and_high_offset = (0, 0)
     with pytest.raises(RunStartError):
-        async for _ in _data_stream(data_queue,
-                                    worker_instruction_queue,
-                                    run_info_topic=run_info_topic,
-                                    halt_after_n_data_chunks=0,
-                                    test_message_queue=test_message_queue,
-                                    query_consumer=FakeQueryConsumer(
-                                        test_instrument_name, low_and_high_offset),
-                                    **TEST_STREAM_ARGS):
+        async for _ in _data_stream(
+            data_queue,
+            worker_instruction_queue,
+            run_info_topic=run_info_topic,
+            halt_after_n_data_chunks=0,
+            test_message_queue=test_message_queue,
+            query_consumer=FakeQueryConsumer(test_instrument_name, low_and_high_offset),
+            **TEST_STREAM_ARGS,
+        ):
             pass
 
 
 @pytest.mark.asyncio
 async def test_error_if_both_topics_and_run_start_topic_not_specified(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     # At least one of "topics" and "run_start_topic" must be specified
     with pytest.raises(ValueError):
-        async for _ in _data_stream(data_queue,
-                                    worker_instruction_queue,
-                                    run_info_topic=None,
-                                    halt_after_n_data_chunks=0,
-                                    **test_stream_args,
-                                    query_consumer=FakeQueryConsumer(),
-                                    test_message_queue=test_message_queue):
+        async for _ in _data_stream(
+            data_queue,
+            worker_instruction_queue,
+            run_info_topic=None,
+            halt_after_n_data_chunks=0,
+            **test_stream_args,
+            query_consumer=FakeQueryConsumer(),
+            test_message_queue=test_message_queue,
+        ):
             pass
 
 
 @pytest.mark.asyncio
 async def test_specified_topics_override_run_start_message_topics(queues):
     # If "topics" argument is specified then they should be used, even if
     # a run start topic is provided
     data_queue, worker_instruction_queue, test_message_queue = queues
     test_topics = ["whiting", "snail", "porpoise"]
     topic_in_run_start_message = "test_topic"
     test_streams = [Stream("/entry", topic_in_run_start_message)]
     query_consumer = FakeQueryConsumer(streams=test_streams)
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = test_topics
-    async for _ in _data_stream(data_queue,
-                                worker_instruction_queue,
-                                run_info_topic=None,
-                                query_consumer=query_consumer,
-                                halt_after_n_data_chunks=0,
-                                **test_stream_args,
-                                test_message_queue=test_message_queue):
+    async for _ in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=None,
+        query_consumer=query_consumer,
+        halt_after_n_data_chunks=0,
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+    ):
         pass
-    assert not query_consumer.queried_topics, "Expected specified topics" \
-                                              " to be used and none queried"
+    assert not query_consumer.queried_topics, (
+        "Expected specified topics" " to be used and none queried"
+    )
 
 
 @pytest.mark.asyncio
 async def test_data_stream_returns_metadata(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
@@ -394,198 +418,269 @@
     f142_source_name = "f142_source"
     f142_log_name = "f142_log"
     senv_source_name = "senv_source"
     senv_log_name = "senv_log"
     tdct_source_name = "tdct_source"
     tdct_log_name = "tdct_log"
     streams = [
-        Stream(f"/entry/{f142_log_name}", "f142_topic", f142_source_name, "f142",
-               "double", "m"),
-        Stream(f"/entry/{senv_log_name}", "senv_topic", senv_source_name, "senv",
-               "double", "m"),
-        Stream(f"/entry/{tdct_log_name}", "tdct_topic", tdct_source_name, "tdct")
+        Stream(
+            f"/entry/{f142_log_name}",
+            "f142_topic",
+            f142_source_name,
+            "f142",
+            "double",
+            "m",
+        ),
+        Stream(
+            f"/entry/{senv_log_name}",
+            "senv_topic",
+            senv_source_name,
+            "senv",
+            "double",
+            "m",
+        ),
+        Stream(f"/entry/{tdct_log_name}", "tdct_topic", tdct_source_name, "tdct"),
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     n_chunks = 0
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name, streams=streams),
-                                   halt_after_n_data_chunks=2,
-                                   **test_stream_args,
-                                   test_message_queue=test_message_queue):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+        halt_after_n_data_chunks=2,
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+    ):
         data_from_stream = data
 
         if n_chunks == 0:
             # Fake receiving a Kafka message for each metadata schema
             # Do this after the run start message has been parsed, so that
             # a metadata buffer will have been created for each data source
             # described in the start message.
             f142_value = 26.1236
             f142_timestamp = 123456  # ns after epoch
-            f142_test_message = serialise_f142(f142_value, f142_source_name,
-                                               f142_timestamp)
+            f142_test_message = serialise_f142(
+                f142_value, f142_source_name, f142_timestamp
+            )
             test_message_queue.put(FakeMessage(f142_test_message))
             senv_values = np.array([26, 127, 52])
             senv_timestamp_ns = 123000  # ns after epoch
-            senv_timestamp = datetime.datetime.fromtimestamp(senv_timestamp_ns * 1e-9,
-                                                             datetime.timezone.utc)
+            senv_timestamp = datetime.datetime.fromtimestamp(
+                senv_timestamp_ns * 1e-9, datetime.timezone.utc
+            )
             senv_time_between_samples = 100  # ns
-            senv_test_message = serialise_senv(senv_source_name, -1, senv_timestamp,
-                                               senv_time_between_samples, 0,
-                                               senv_values, Location.Start)
+            senv_test_message = serialise_senv(
+                senv_source_name,
+                -1,
+                senv_timestamp,
+                senv_time_between_samples,
+                0,
+                senv_values,
+                Location.Start,
+            )
             test_message_queue.put(FakeMessage(senv_test_message))
             tdct_timestamps = np.array([1234, 2345, 3456])  # ns
             tdct_test_message = serialise_tdct(tdct_source_name, tdct_timestamps)
             test_message_queue.put(FakeMessage(tdct_test_message))
 
         n_chunks += 1
 
     assert isclose(data_from_stream.attrs[f142_source_name].value.values[0], f142_value)
     assert data_from_stream.attrs[f142_source_name].value.coords['time'].values[
-        0] == np.array(f142_timestamp, dtype=np.dtype('datetime64[ns]'))
-    assert np.array_equal(data_from_stream.attrs[senv_source_name].value.values,
-                          senv_values)
-    senv_expected_timestamps = np.array([
-        senv_timestamp_ns, senv_timestamp_ns + senv_time_between_samples,
-        senv_timestamp_ns + (2 * senv_time_between_samples)
-    ],
-                                        dtype=np.dtype('datetime64[ns]'))
+        0
+    ] == np.array(f142_timestamp, dtype=np.dtype('datetime64[ns]'))
+    assert np.array_equal(
+        data_from_stream.attrs[senv_source_name].value.values, senv_values
+    )
+    senv_expected_timestamps = np.array(
+        [
+            senv_timestamp_ns,
+            senv_timestamp_ns + senv_time_between_samples,
+            senv_timestamp_ns + (2 * senv_time_between_samples),
+        ],
+        dtype=np.dtype('datetime64[ns]'),
+    )
     assert np.array_equal(
         data_from_stream.attrs[senv_source_name].value.coords['time'].values,
-        senv_expected_timestamps)
-    assert np.array_equal(data_from_stream.attrs[tdct_source_name].value.values,
-                          tdct_timestamps)
+        senv_expected_timestamps,
+    )
+    assert np.array_equal(
+        data_from_stream.attrs[tdct_source_name].value.values, tdct_timestamps
+    )
 
 
 @pytest.mark.asyncio
 async def test_data_stream_returns_data_from_multiple_slow_metadata_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
     f142_source_name = "f142_source"
     f142_log_name = "f142_log"
     streams = [
-        Stream(f"/entry/{f142_log_name}", "f142_topic", f142_source_name, "f142",
-               "double", "m"),
+        Stream(
+            f"/entry/{f142_log_name}",
+            "f142_topic",
+            f142_source_name,
+            "f142",
+            "double",
+            "m",
+        ),
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     n_chunks = 0
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name, streams=streams),
-                                   halt_after_n_data_chunks=2,
-                                   **test_stream_args,
-                                   test_message_queue=test_message_queue):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+        halt_after_n_data_chunks=2,
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+    ):
         data_from_stream = data
 
         if n_chunks == 0:
             # Fake receiving a Kafka message for each metadata schema
             # Do this after the run start message has been parsed, so that
             # a metadata buffer will have been created for each data source
             # described in the start message.
             f142_value_1 = 26.1236
             f142_timestamp_1 = 123456  # ns after epoch
-            f142_test_message = serialise_f142(f142_value_1, f142_source_name,
-                                               f142_timestamp_1)
+            f142_test_message = serialise_f142(
+                f142_value_1, f142_source_name, f142_timestamp_1
+            )
             test_message_queue.put(FakeMessage(f142_test_message))
             f142_value_2 = 2.725
             f142_timestamp_2 = 234567  # ns after epoch
-            f142_test_message = serialise_f142(f142_value_2, f142_source_name,
-                                               f142_timestamp_2)
+            f142_test_message = serialise_f142(
+                f142_value_2, f142_source_name, f142_timestamp_2
+            )
             test_message_queue.put(FakeMessage(f142_test_message))
 
         n_chunks += 1
 
-    assert np.allclose(data_from_stream.attrs[f142_source_name].value.values,
-                       np.array([f142_value_1, f142_value_2]))
+    assert np.allclose(
+        data_from_stream.attrs[f142_source_name].value.values,
+        np.array([f142_value_1, f142_value_2]),
+    )
     assert np.array_equal(
         data_from_stream.attrs[f142_source_name].value.coords['time'].values,
-        np.array([f142_timestamp_1, f142_timestamp_2],
-                 dtype=np.dtype('datetime64[ns]')))
+        np.array(
+            [f142_timestamp_1, f142_timestamp_2], dtype=np.dtype('datetime64[ns]')
+        ),
+    )
 
 
 @pytest.mark.asyncio
 async def test_data_stream_returns_data_from_multiple_fast_metadata_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
     senv_source_name = "senv_source"
     senv_log_name = "senv_log"
     streams = [
-        Stream(f"/entry/{senv_log_name}", "senv_topic", senv_source_name, "senv",
-               "double", "m"),
+        Stream(
+            f"/entry/{senv_log_name}",
+            "senv_topic",
+            senv_source_name,
+            "senv",
+            "double",
+            "m",
+        ),
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     n_chunks = 0
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name, streams=streams),
-                                   halt_after_n_data_chunks=2,
-                                   **test_stream_args,
-                                   test_message_queue=test_message_queue):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+        halt_after_n_data_chunks=2,
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+    ):
         data_from_stream = data
 
         if n_chunks == 0:
             # Fake receiving a Kafka message for each metadata schema
             # Do this after the run start message has been parsed, so that
             # a metadata buffer will have been created for each data source
             # described in the start message.
             senv_values_1 = np.array([26, 127, 52])
             senv_timestamp_ns_1 = 123000  # ns after epoch
-            senv_timestamp = datetime.datetime.fromtimestamp(senv_timestamp_ns_1 * 1e-9,
-                                                             datetime.timezone.utc)
+            senv_timestamp = datetime.datetime.fromtimestamp(
+                senv_timestamp_ns_1 * 1e-9, datetime.timezone.utc
+            )
             senv_time_between_samples = 100  # ns
-            senv_test_message = serialise_senv(senv_source_name, -1, senv_timestamp,
-                                               senv_time_between_samples, 0,
-                                               senv_values_1, Location.Start)
+            senv_test_message = serialise_senv(
+                senv_source_name,
+                -1,
+                senv_timestamp,
+                senv_time_between_samples,
+                0,
+                senv_values_1,
+                Location.Start,
+            )
             test_message_queue.put(FakeMessage(senv_test_message))
             senv_values_2 = np.array([3832, 324, 3])
             senv_timestamp_ns_2 = 234000  # ns after epoch
-            senv_timestamp = datetime.datetime.fromtimestamp(senv_timestamp_ns_2 * 1e-9,
-                                                             datetime.timezone.utc)
-            senv_test_message = serialise_senv(senv_source_name, -1, senv_timestamp,
-                                               senv_time_between_samples, 0,
-                                               senv_values_2, Location.Start)
+            senv_timestamp = datetime.datetime.fromtimestamp(
+                senv_timestamp_ns_2 * 1e-9, datetime.timezone.utc
+            )
+            senv_test_message = serialise_senv(
+                senv_source_name,
+                -1,
+                senv_timestamp,
+                senv_time_between_samples,
+                0,
+                senv_values_2,
+                Location.Start,
+            )
             test_message_queue.put(FakeMessage(senv_test_message))
 
         n_chunks += 1
 
-    assert np.array_equal(data_from_stream.attrs[senv_source_name].value.values,
-                          np.concatenate((senv_values_1, senv_values_2)))
-    senv_expected_timestamps_1 = np.array([
-        senv_timestamp_ns_1, senv_timestamp_ns_1 + senv_time_between_samples,
-        senv_timestamp_ns_1 + (2 * senv_time_between_samples)
-    ],
-                                          dtype=np.dtype('datetime64[ns]'))
-    senv_expected_timestamps_2 = np.array([
-        senv_timestamp_ns_2, senv_timestamp_ns_2 + senv_time_between_samples,
-        senv_timestamp_ns_2 + (2 * senv_time_between_samples)
-    ],
-                                          dtype=np.dtype('datetime64[ns]'))
+    assert np.array_equal(
+        data_from_stream.attrs[senv_source_name].value.values,
+        np.concatenate((senv_values_1, senv_values_2)),
+    )
+    senv_expected_timestamps_1 = np.array(
+        [
+            senv_timestamp_ns_1,
+            senv_timestamp_ns_1 + senv_time_between_samples,
+            senv_timestamp_ns_1 + (2 * senv_time_between_samples),
+        ],
+        dtype=np.dtype('datetime64[ns]'),
+    )
+    senv_expected_timestamps_2 = np.array(
+        [
+            senv_timestamp_ns_2,
+            senv_timestamp_ns_2 + senv_time_between_samples,
+            senv_timestamp_ns_2 + (2 * senv_time_between_samples),
+        ],
+        dtype=np.dtype('datetime64[ns]'),
+    )
     assert np.array_equal(
         data_from_stream.attrs[senv_source_name].value.coords['time'].values,
-        np.concatenate((senv_expected_timestamps_1, senv_expected_timestamps_2)))
+        np.concatenate((senv_expected_timestamps_1, senv_expected_timestamps_2)),
+    )
 
 
 @pytest.mark.asyncio
 async def test_data_stream_returns_data_from_multiple_chopper_messages(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
@@ -597,22 +692,23 @@
     streams = [
         Stream(f"/entry/{tdct_log_name}", "tdct_topic", tdct_source_name, "tdct")
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     n_chunks = 0
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name, streams=streams),
-                                   halt_after_n_data_chunks=2,
-                                   **test_stream_args,
-                                   test_message_queue=test_message_queue):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+        halt_after_n_data_chunks=2,
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+    ):
         data_from_stream = data
 
         if n_chunks == 0:
             # Fake receiving a Kafka message for each metadata schema
             # Do this after the run start message has been parsed, so that
             # a metadata buffer will have been created for each data source
             # described in the start message.
@@ -621,60 +717,76 @@
             test_message_queue.put(FakeMessage(tdct_test_message))
             tdct_timestamps_2 = np.array([4567, 5678, 6789])  # ns
             tdct_test_message = serialise_tdct(tdct_source_name, tdct_timestamps_2)
             test_message_queue.put(FakeMessage(tdct_test_message))
 
         n_chunks += 1
 
-    assert np.array_equal(data_from_stream.attrs[tdct_source_name].value.values,
-                          np.concatenate((tdct_timestamps_1, tdct_timestamps_2)))
+    assert np.array_equal(
+        data_from_stream.attrs[tdct_source_name].value.values,
+        np.concatenate((tdct_timestamps_1, tdct_timestamps_2)),
+    )
 
 
 @pytest.mark.asyncio
 async def test_data_stream_warns_if_fast_metadata_message_exceeds_buffer(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
     buffer_size = 2
     run_info_topic = "fake_topic"
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
     senv_source_name = "senv_source"
     senv_log_name = "senv_log"
     streams = [
-        Stream(f"/entry/{senv_log_name}", "senv_topic", senv_source_name, "senv",
-               "double", "m"),
+        Stream(
+            f"/entry/{senv_log_name}",
+            "senv_topic",
+            senv_source_name,
+            "senv",
+            "double",
+            "m",
+        ),
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     test_stream_args["fast_metadata_buffer_size"] = buffer_size
     with pytest.warns(BufferSizeWarning):
-        async for _ in _data_stream(data_queue,
-                                    worker_instruction_queue,
-                                    run_info_topic=run_info_topic,
-                                    query_consumer=FakeQueryConsumer(
-                                        test_instrument_name, streams=streams),
-                                    halt_after_n_warnings=1,
-                                    **test_stream_args,
-                                    test_message_queue=test_message_queue):
+        async for _ in _data_stream(
+            data_queue,
+            worker_instruction_queue,
+            run_info_topic=run_info_topic,
+            query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+            halt_after_n_warnings=1,
+            **test_stream_args,
+            test_message_queue=test_message_queue,
+        ):
             # Fake receiving a Kafka message for each metadata schema
             # Do this after the run start message has been parsed, so that
             # a metadata buffer will have been created for each data source
             # described in the start message.
 
             # 3 values but buffer size is only 2!
             senv_values = np.array([26, 127, 52])
             senv_timestamp_ns = 123000  # ns after epoch
-            senv_timestamp = datetime.datetime.fromtimestamp(senv_timestamp_ns * 1e-9,
-                                                             datetime.timezone.utc)
+            senv_timestamp = datetime.datetime.fromtimestamp(
+                senv_timestamp_ns * 1e-9, datetime.timezone.utc
+            )
             senv_time_between_samples = 100  # ns
-            senv_test_message = serialise_senv(senv_source_name, -1, senv_timestamp,
-                                               senv_time_between_samples, 0,
-                                               senv_values, Location.Start)
+            senv_test_message = serialise_senv(
+                senv_source_name,
+                -1,
+                senv_timestamp,
+                senv_time_between_samples,
+                0,
+                senv_values,
+                Location.Start,
+            )
 
             test_message_queue.put(FakeMessage(senv_test_message))
 
 
 @pytest.mark.asyncio
 async def test_data_stream_warns_if_single_chopper_message_exceeds_buffer(queues):
     data_queue, worker_instruction_queue, test_message_queue = queues
@@ -690,22 +802,23 @@
         Stream(f"/entry/{tdct_log_name}", "tdct_topic", tdct_source_name, "tdct")
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     test_stream_args["chopper_buffer_size"] = buffer_size
     with pytest.warns(BufferSizeWarning):
-        async for _ in _data_stream(data_queue,
-                                    worker_instruction_queue,
-                                    run_info_topic=run_info_topic,
-                                    query_consumer=FakeQueryConsumer(
-                                        test_instrument_name, streams=streams),
-                                    halt_after_n_warnings=1,
-                                    **test_stream_args,
-                                    test_message_queue=test_message_queue):
+        async for _ in _data_stream(
+            data_queue,
+            worker_instruction_queue,
+            run_info_topic=run_info_topic,
+            query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+            halt_after_n_warnings=1,
+            **test_stream_args,
+            test_message_queue=test_message_queue,
+        ):
             # Fake receiving a Kafka message for each metadata schema
             # Do this after the run start message has been parsed, so that
             # a metadata buffer will have been created for each data source
             # described in the start message.
 
             # 3 values but buffer size is only 2!
             tdct_timestamps = np.array([1234, 2345, 3456])  # ns
@@ -721,50 +834,59 @@
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
     f142_source_name = "f142_source"
     f142_log_name = "f142_log"
     streams = [
-        Stream(f"/entry/{f142_log_name}", "f142_topic", f142_source_name, "f142",
-               "double", "m"),
+        Stream(
+            f"/entry/{f142_log_name}",
+            "f142_topic",
+            f142_source_name,
+            "f142",
+            "double",
+            "m",
+        ),
     ]
 
     first_f142_value = 26.1236
     f142_timestamp = 123456  # ns after epoch
     first_message = serialise_f142(first_f142_value, f142_source_name, f142_timestamp)
     second_f142_value = 62.721
     second_message = serialise_f142(second_f142_value, f142_source_name, f142_timestamp)
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["slow_metadata_buffer_size"] = 1
     test_stream_args["topics"] = None
     n_chunks = 0
     reached_asserts = False
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name, streams=streams),
-                                   halt_after_n_data_chunks=3,
-                                   **test_stream_args,
-                                   test_message_queue=test_message_queue):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+        halt_after_n_data_chunks=3,
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+    ):
         # n_chunks == 0 zeroth chunk contains data
         # from run start message
         if n_chunks == 0:
             test_message_queue.put(FakeMessage(first_message))
             test_message_queue.put(FakeMessage(second_message))
         elif n_chunks == 1:
             # Contains data from first message
-            assert isclose(data.attrs[f142_source_name].value.values[0],
-                           first_f142_value)
+            assert isclose(
+                data.attrs[f142_source_name].value.values[0], first_f142_value
+            )
         elif n_chunks == 2:
             # Contains data from second message
-            assert isclose(data.attrs[f142_source_name].value.values[0],
-                           second_f142_value)
+            assert isclose(
+                data.attrs[f142_source_name].value.values[0], second_f142_value
+            )
             reached_asserts = True
         n_chunks += 1
 
     assert reached_asserts
 
 
 @pytest.mark.asyncio
@@ -775,57 +897,79 @@
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
     senv_source_name = "senv_source"
     senv_log_name = "senv_log"
     streams = [
-        Stream(f"/entry/{senv_log_name}", "senv_topic", senv_source_name, "senv",
-               "double", "m"),
+        Stream(
+            f"/entry/{senv_log_name}",
+            "senv_topic",
+            senv_source_name,
+            "senv",
+            "double",
+            "m",
+        ),
     ]
 
     first_senv_values = np.array([26, 127, 52])
     second_senv_values = np.array([72, 94, 1])
     senv_timestamp_ns = 123000  # ns after epoch
-    senv_timestamp = datetime.datetime.fromtimestamp(senv_timestamp_ns * 1e-9,
-                                                     datetime.timezone.utc)
+    senv_timestamp = datetime.datetime.fromtimestamp(
+        senv_timestamp_ns * 1e-9, datetime.timezone.utc
+    )
     senv_time_between_samples = 100  # ns
-    first_message = serialise_senv(senv_source_name, -1, senv_timestamp,
-                                   senv_time_between_samples, 0, first_senv_values,
-                                   Location.Start)
-    second_message = serialise_senv(senv_source_name, -1, senv_timestamp,
-                                    senv_time_between_samples, 0, second_senv_values,
-                                    Location.Start)
+    first_message = serialise_senv(
+        senv_source_name,
+        -1,
+        senv_timestamp,
+        senv_time_between_samples,
+        0,
+        first_senv_values,
+        Location.Start,
+    )
+    second_message = serialise_senv(
+        senv_source_name,
+        -1,
+        senv_timestamp,
+        senv_time_between_samples,
+        0,
+        second_senv_values,
+        Location.Start,
+    )
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     test_stream_args["fast_metadata_buffer_size"] = buffer_size
     n_chunks = 0
     reached_asserts = False
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name, streams=streams),
-                                   halt_after_n_data_chunks=3,
-                                   **test_stream_args,
-                                   test_message_queue=test_message_queue):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+        halt_after_n_data_chunks=3,
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+    ):
         # n_chunks == 0 zeroth chunk contains data
         # from run start message
         if n_chunks == 0:
             test_message_queue.put(FakeMessage(first_message))
             test_message_queue.put(FakeMessage(second_message))
         elif n_chunks == 1:
             # Contains data from first message
-            assert np.array_equal(data.attrs[senv_source_name].value.values,
-                                  first_senv_values)
+            assert np.array_equal(
+                data.attrs[senv_source_name].value.values, first_senv_values
+            )
         elif n_chunks == 2:
             # Contains data from second message
-            assert np.array_equal(data.attrs[senv_source_name].value.values,
-                                  second_senv_values)
+            assert np.array_equal(
+                data.attrs[senv_source_name].value.values, second_senv_values
+            )
             reached_asserts = True
         n_chunks += 1
     assert reached_asserts
 
 
 @pytest.mark.asyncio
 async def test_data_returned_if_multiple_chopper_msgs_exceed_buffer(queues):
@@ -849,35 +993,38 @@
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     test_stream_args["chopper_buffer_size"] = buffer_size
 
     n_chunks = 0
     reached_asserts = False
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name, streams=streams),
-                                   **test_stream_args,
-                                   halt_after_n_data_chunks=3,
-                                   test_message_queue=test_message_queue):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(test_instrument_name, streams=streams),
+        **test_stream_args,
+        halt_after_n_data_chunks=3,
+        test_message_queue=test_message_queue,
+    ):
         # n_chunks == 0 zeroth chunk contains data
         # from run start message
         if n_chunks == 0:
             test_message_queue.put(FakeMessage(first_tdct_message))
             test_message_queue.put(FakeMessage(second_tdct_message))
         elif n_chunks == 1:
             # Contains data from first message
-            assert np.array_equal(data.attrs[tdct_source_name].value.values,
-                                  tdct_timestamps_1)
+            assert np.array_equal(
+                data.attrs[tdct_source_name].value.values, tdct_timestamps_1
+            )
         elif n_chunks == 2:
             # Contains data from second message
-            assert np.array_equal(data.attrs[tdct_source_name].value.values,
-                                  tdct_timestamps_2)
+            assert np.array_equal(
+                data.attrs[tdct_source_name].value.values, tdct_timestamps_2
+            )
             reached_asserts = True
         n_chunks += 1
     assert reached_asserts
 
 
 @pytest.mark.asyncio
 async def test_passes_with_missing_datasets_if_group_contains_stream(queues):
@@ -895,23 +1042,25 @@
 
     data_queue, worker_instruction_queue, test_message_queue = queues
     run_info_topic = "fake_topic"
     reached_assert = False
 
     with warnings.catch_warnings(record=True):
         warnings.filterwarnings("ignore", message='Failed to load')
-        async for _ in _data_stream(data_queue,
-                                    worker_instruction_queue,
-                                    run_info_topic=run_info_topic,
-                                    query_consumer=FakeQueryConsumer(
-                                        test_instrument_name,
-                                        nexus_structure=nexus_structure),
-                                    **TEST_STREAM_ARGS,
-                                    halt_after_n_data_chunks=0,
-                                    test_message_queue=test_message_queue):
+        async for _ in _data_stream(
+            data_queue,
+            worker_instruction_queue,
+            run_info_topic=run_info_topic,
+            query_consumer=FakeQueryConsumer(
+                test_instrument_name, nexus_structure=nexus_structure
+            ),
+            **TEST_STREAM_ARGS,
+            halt_after_n_data_chunks=0,
+            test_message_queue=test_message_queue,
+        ):
             reached_assert = True
             break
         assert reached_assert
 
 
 @pytest.mark.asyncio
 async def test_data_stream_times_out(queues):
@@ -920,25 +1069,26 @@
     test_instrument_name = "DATA_STREAM_TEST"
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     # "timeout" is only for use in tests, ensures that if something
     # gets broken then tests will not get stuck in the _data_stream
     # loop indefinitely.
-    test_stream_args["timeout"] = 2. * sc.units.s
+    test_stream_args["timeout"] = 2.0 * sc.units.s
     timed_out = False
     try:
         async for _ in _data_stream(
-                data_queue,
-                worker_instruction_queue,
-                run_info_topic=run_info_topic,
-                query_consumer=FakeQueryConsumer(test_instrument_name),
-                **test_stream_args,
-                test_message_queue=test_message_queue,
-                end_at=StopTime.END_OF_RUN):
+            data_queue,
+            worker_instruction_queue,
+            run_info_topic=run_info_topic,
+            query_consumer=FakeQueryConsumer(test_instrument_name),
+            **test_stream_args,
+            test_message_queue=test_message_queue,
+            end_at=StopTime.END_OF_RUN,
+        ):
             # Do nothing until it times out
             pass
     except TimeoutError:
         timed_out = True
     assert timed_out
 
 
@@ -951,22 +1101,25 @@
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     # System time is already after this stop time so the stream will stop
     # as soon as it sees the end of partition or a message with a
     # timestamp after the stop time
     stop_time_in_past = datetime.datetime(2017, 11, 28, 23, 55, 59, 342380)
     n_chunks = 0
-    async for _ in _data_stream(data_queue,
-                                worker_instruction_queue,
-                                run_info_topic=run_info_topic,
-                                query_consumer=FakeQueryConsumer(
-                                    test_instrument_name, stop_time=stop_time_in_past),
-                                **test_stream_args,
-                                test_message_queue=test_message_queue,
-                                end_at=StopTime.END_OF_RUN):
+    async for _ in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(
+            test_instrument_name, stop_time=stop_time_in_past
+        ),
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+        end_at=StopTime.END_OF_RUN,
+    ):
         if n_chunks == 0:
             # Tell consumer it has reached the end of the partition
             # Consumer will stop, data_consumption_manager will see the
             # consumer has stopped and stop the buffer and the
             # _data_stream will exit.
             # A TimeoutError would occur if the functionality is broken.
             test_message_queue.put(FakeMessage(b"", KafkaError._PARTITION_EOF))
@@ -980,65 +1133,80 @@
     test_instrument_name = "DATA_STREAM_TEST"
 
     # The Kafka topics to get metadata from are recorded as "stream" objects in
     # the nexus_structure field of the run start message
     f142_source_name = "f142_source"
     f142_log_name = "f142_log"
     streams = [
-        Stream(f"/entry/{f142_log_name}", "f142_topic", f142_source_name, "f142",
-               "double", "m"),
+        Stream(
+            f"/entry/{f142_log_name}",
+            "f142_topic",
+            f142_source_name,
+            "f142",
+            "double",
+            "m",
+        ),
     ]
 
     test_stream_args = TEST_STREAM_ARGS.copy()
     test_stream_args["topics"] = None
     # System time is already after this stop time so the stream will stop
     # as soon as it sees the end of partition or a message with a
     # timestamp after the stop time
     stop_time_in_past = datetime.datetime(2017, 11, 28, 23, 55, 59, 342380)
     n_chunks = 0
-    async for data in _data_stream(data_queue,
-                                   worker_instruction_queue,
-                                   run_info_topic=run_info_topic,
-                                   query_consumer=FakeQueryConsumer(
-                                       test_instrument_name,
-                                       stop_time=stop_time_in_past,
-                                       streams=streams),
-                                   **test_stream_args,
-                                   test_message_queue=test_message_queue,
-                                   end_at=StopTime.END_OF_RUN):
+    async for data in _data_stream(
+        data_queue,
+        worker_instruction_queue,
+        run_info_topic=run_info_topic,
+        query_consumer=FakeQueryConsumer(
+            test_instrument_name, stop_time=stop_time_in_past, streams=streams
+        ),
+        **test_stream_args,
+        test_message_queue=test_message_queue,
+        end_at=StopTime.END_OF_RUN,
+    ):
         if n_chunks == 0:
             # Publish a message with a timestamp before the stop time
             f142_value_1 = 26.1236
             timestamp_before_stop_dt = datetime.datetime(2017, 11, 28, 23, 55, 50, 0)
             # Convert to integer nanoseconds
             # (for timestamp in message payload)
-            timestamp_before_stop_ns = int(timestamp_before_stop_dt.timestamp() *
-                                           1_000_000_000)
+            timestamp_before_stop_ns = int(
+                timestamp_before_stop_dt.timestamp() * 1_000_000_000
+            )
             # Convert to integer milliseconds
             # (for Kafka message header)
             timestamp_before_stop_ms = int(timestamp_before_stop_dt.timestamp() * 1_000)
-            f142_test_message = serialise_f142(f142_value_1, f142_source_name,
-                                               timestamp_before_stop_ns)
+            f142_test_message = serialise_f142(
+                f142_value_1, f142_source_name, timestamp_before_stop_ns
+            )
             test_message_queue.put(
-                FakeMessage(f142_test_message, timestamp=timestamp_before_stop_ms))
+                FakeMessage(f142_test_message, timestamp=timestamp_before_stop_ms)
+            )
         elif n_chunks == 1:
             # The data from the first message will be returned
-            assert np.allclose(data.attrs[f142_source_name].value.values,
-                               np.array([f142_value_1]))
+            assert np.allclose(
+                data.attrs[f142_source_name].value.values, np.array([f142_value_1])
+            )
             assert np.array_equal(
                 data.attrs[f142_source_name].value.coords['time'].values,
-                np.array([timestamp_before_stop_ns], dtype=np.dtype('datetime64[ns]')))
+                np.array([timestamp_before_stop_ns], dtype=np.dtype('datetime64[ns]')),
+            )
 
             # Publish message with timestamp after stop time, this will trigger
             # the consumer to stop and data_stream to exit.
             # A TimeoutError would occur if the functionality is broken.
             f142_value_2 = 2.725
             timestamp_after_stop_dt = datetime.datetime(2017, 11, 28, 23, 56, 50, 0)
-            timestamp_after_stop_ns = int(timestamp_after_stop_dt.timestamp() *
-                                          1_000_000_000)
+            timestamp_after_stop_ns = int(
+                timestamp_after_stop_dt.timestamp() * 1_000_000_000
+            )
             timestamp_after_stop_ms = int(timestamp_after_stop_dt.timestamp() * 1_000)
-            f142_test_message = serialise_f142(f142_value_2, f142_source_name,
-                                               timestamp_after_stop_ns)
+            f142_test_message = serialise_f142(
+                f142_value_2, f142_source_name, timestamp_after_stop_ns
+            )
             test_message_queue.put(
-                FakeMessage(f142_test_message, timestamp=timestamp_after_stop_ms))
+                FakeMessage(f142_test_message, timestamp=timestamp_after_stop_ms)
+            )
 
         n_chunks += 1
```

### Comparing `scippneutron-23.3.0/tests/instrument_view_test.py` & `scippneutron-23.4.0/tests/instrument_view_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,103 +16,118 @@
     d = make_dataset_with_beamline()
     scn.instrument_view(d["a"])
 
 
 def test_neutron_instrument_view_with_masks():
     d = make_dataset_with_beamline()
     x = np.transpose(d.coords['position'].values)[0, :]
-    d['a'].masks['amask'] = sc.Variable(dims=['position'],
-                                        values=np.less(np.abs(x), 0.5))
+    d['a'].masks['amask'] = sc.Variable(
+        dims=['position'], values=np.less(np.abs(x), 0.5)
+    )
     scn.instrument_view(d["a"])
 
 
 def test_neutron_instrument_view_with_cmap_args():
     d = make_dataset_with_beamline()
-    scn.instrument_view(d["a"],
-                        vmin=0.001 * sc.units.one,
-                        vmax=5.0 * sc.units.one,
-                        cmap="magma",
-                        norm="log")
-
-
-def _make_component_settings(*,
-                             data,
-                             center='sample_position',
-                             type='box',
-                             size_unit=sc.units.m,
-                             wireframe=False,
-                             component_size=(0.1, 0.1, 0.1)):
-    comp_size = sc.vector(value=component_size, unit=size_unit) if isinstance(
-        component_size, tuple) else sc.scalar(value=component_size, unit=size_unit)
+    scn.instrument_view(
+        d["a"],
+        vmin=0.001 * sc.units.one,
+        vmax=5.0 * sc.units.one,
+        cmap="magma",
+        norm="log",
+    )
+
+
+def _make_component_settings(
+    *,
+    data,
+    center='sample_position',
+    type='box',
+    size_unit=sc.units.m,
+    wireframe=False,
+    component_size=(0.1, 0.1, 0.1),
+):
+    comp_size = (
+        sc.vector(value=component_size, unit=size_unit)
+        if isinstance(component_size, tuple)
+        else sc.scalar(value=component_size, unit=size_unit)
+    )
     center = data.meta[center] if isinstance(center, str) else center
     sample_settings = {'center': center, 'size': comp_size, 'type': type}
     return sample_settings
 
 
 def test_neutron_instrument_view_components_valid():
     d = make_dataset_with_beamline()
     scn.instrument_view(d["a"], components={'sample': _make_component_settings(data=d)})
 
 
 def test_neutron_instrument_view_with_size_scalar():
     d = make_dataset_with_beamline()
     scn.instrument_view(
         d["a"],
-        components={'sample': _make_component_settings(data=d, component_size=2.0)})
+        components={'sample': _make_component_settings(data=d, component_size=2.0)},
+    )
 
 
 def test_neutron_instrument_view_components_multiple_valid():
     d = make_dataset_with_beamline()
-    scn.instrument_view(d["a"],
-                        components={
-                            'sample':
-                            _make_component_settings(data=d, center='sample_position'),
-                            'source':
-                            _make_component_settings(data=d, center='source_position')
-                        })
+    scn.instrument_view(
+        d["a"],
+        components={
+            'sample': _make_component_settings(data=d, center='sample_position'),
+            'source': _make_component_settings(data=d, center='source_position'),
+        },
+    )
 
 
 def test_neutron_instrument_view_components_with_non_beamline_component():
     d = make_dataset_with_beamline()
     widget_center = sc.vector(value=[1, 1, 1], unit=sc.units.m)
     scn.instrument_view(
         d["a"],
-        components={'widget': _make_component_settings(data=d, center=widget_center)})
+        components={'widget': _make_component_settings(data=d, center=widget_center)},
+    )
 
 
 def test_neutron_instrument_view_components_with_wireframe():
     d = make_dataset_with_beamline()
     scn.instrument_view(
-        d["a"],
-        components={'sample': _make_component_settings(data=d, wireframe=False)})
+        d["a"], components={'sample': _make_component_settings(data=d, wireframe=False)}
+    )
     scn.instrument_view(
-        d["a"], components={'sample': _make_component_settings(data=d, wireframe=True)})
+        d["a"], components={'sample': _make_component_settings(data=d, wireframe=True)}
+    )
 
 
 def test_neutron_instrument_view_components_with_invalid_type():
     d = make_dataset_with_beamline()
     # Check that all our valid shape types work
     for shape_type in ['box', 'cylinder', 'disk']:
         scn.instrument_view(
             d["a"],
-            components={'sample': _make_component_settings(data=d, type=shape_type)})
+            components={'sample': _make_component_settings(data=d, type=shape_type)},
+        )
     with pytest.raises(ValueError):
-        scn.instrument_view(d["a"],
-                            components={
-                                'sample':
-                                _make_component_settings(data=d, type='trefoil_knot')
-                            })
+        scn.instrument_view(
+            d["a"],
+            components={
+                'sample': _make_component_settings(data=d, type='trefoil_knot')
+            },
+        )
 
 
 def test_neutron_instrument_view_components_with_invalid_size_unit():
     d = make_dataset_with_beamline()
     # mm is fine, source_position is set in meters. Just a scaling factor.
     scn.instrument_view(
         d["a"],
-        components={'sample': _make_component_settings(data=d, size_unit=sc.units.mm)})
+        components={'sample': _make_component_settings(data=d, size_unit=sc.units.mm)},
+    )
     # cannot scale us to meters. This should throw
     with pytest.raises(sc.core.UnitError):
-        scn.instrument_view(d["a"],
-                            components={
-                                'sample':
-                                _make_component_settings(data=d, size_unit=sc.units.us)
-                            })
+        scn.instrument_view(
+            d["a"],
+            components={
+                'sample': _make_component_settings(data=d, size_unit=sc.units.us)
+            },
+        )
```

### Comparing `scippneutron-23.3.0/tests/io/xye_test.py` & `scippneutron-23.4.0/tests/io/xye_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,30 @@
 from hypothesis import strategies as st
 from scipp.testing import strategies as scst
 
 import scippneutron as scn
 
 
 @st.composite
-def one_dim_data_arrays(draw: st.DrawFn,
-                        min_n_coords: int = 1,
-                        max_n_coords: int = 5) -> sc.DataArray:
+def one_dim_data_arrays(
+    draw: st.DrawFn, min_n_coords: int = 1, max_n_coords: int = 5
+) -> sc.DataArray:
     data = draw(scst.variables(ndim=1, dtype='float64', with_variances=True))
     # See https://github.com/scipp/scipp/issues/3052
     data.variances = abs(data.variances)
     coords = draw(
-        st.dictionaries(keys=st.text(),
-                        values=scst.variables(sizes=data.sizes,
-                                              dtype='float64',
-                                              with_variances=False),
-                        min_size=min_n_coords,
-                        max_size=max_n_coords))
+        st.dictionaries(
+            keys=st.text(),
+            values=scst.variables(
+                sizes=data.sizes, dtype='float64', with_variances=False
+            ),
+            min_size=min_n_coords,
+            max_size=max_n_coords,
+        )
+    )
     return sc.DataArray(data, coords=coords)
 
 
 def headers() -> st.SearchStrategy[str]:
     # Using only ASCII characters and excluding \r because Numpy and/or splitlines
     # do something funny with some other characters.
     return st.text(string.ascii_letters + string.digits + string.punctuation + ' \t\n')
@@ -48,36 +51,38 @@
 def roundtrip(da: sc.DataArray, coord: Optional[str] = None, **kwargs) -> sc.DataArray:
     buffer = save_to_buffer(da, coord, **kwargs)
     return scn.io.xye.load_xye(
         buffer,
         dim=da.dim,
         coord=coord,
         unit=da.unit,
-        coord_unit=da.coords[coord].unit if coord is not None else None)
+        coord_unit=da.coords[coord].unit if coord is not None else None,
+    )
 
 
 @given(initial=one_dim_data_arrays(), header=headers(), data=st.data())
 def test_roundtrip(initial, header, data):
     coord_name = data.draw(st.sampled_from(list(initial.coords.keys())))
     loaded = roundtrip(initial, coord=coord_name, header=header)
     assert set(loaded.coords.keys()) == {coord_name}
     # Using allclose instead of identical because the format might lose some precision.
     # Especially in the variances -> stddevs conversion.
-    assert sc.allclose(loaded.coords[coord_name],
-                       initial.coords[coord_name],
-                       equal_nan=True)
+    assert sc.allclose(
+        loaded.coords[coord_name], initial.coords[coord_name], equal_nan=True
+    )
     assert sc.allclose(loaded.data, initial.data, equal_nan=True)
 
 
 @given(da=one_dim_data_arrays(), data=st.data())
 def test_saved_file_contains_data_table(da, data):
     coord_name = data.draw(st.sampled_from(list(da.coords.keys())))
     file_contents = save_to_buffer(da, coord=coord_name).getvalue()
     for i, line in enumerate(
-            filter(lambda l: l and not l.startswith('#'), file_contents.split('\n'))):
+        filter(lambda l: l and not l.startswith('#'), file_contents.split('\n'))
+    ):
         x, y, e = map(float, line.split(' '))
         np.testing.assert_allclose(x, da.coords[coord_name][i].value)
         np.testing.assert_allclose(y, da[i].value)
         np.testing.assert_allclose(e, np.sqrt(da[i].variance))
 
 
 @given(initial=one_dim_data_arrays(max_n_coords=1))
@@ -93,15 +98,16 @@
 
 
 @given(initial=one_dim_data_arrays(), data=st.data())
 @settings(max_examples=20)
 def test_save_deduce_coord_dim_coord(initial, data):
     dim = initial.dim
     initial_coord = data.draw(
-        scst.variables(sizes=initial.sizes, dtype='float64', with_variances=False))
+        scst.variables(sizes=initial.sizes, dtype='float64', with_variances=False)
+    )
     initial.coords[dim] = initial_coord.rename({initial_coord.dim: dim})
 
     loaded = roundtrip(initial)
     # roundtrip cannot deduce coord name and unit in this case.
     # loaded_coord = next(iter(loaded.coords.values()))
     loaded_coord = loaded.coords[dim]
     loaded_coord.unit = initial.coords[dim].unit
@@ -136,54 +142,59 @@
 
 
 @given(da=one_dim_data_arrays(), data=st.data())
 @settings(max_examples=20)
 def test_cannot_save_data_with_bin_edges(da, data):
     coord_name = data.draw(st.sampled_from(list(da.coords.keys())))
     da.coords[coord_name] = sc.concat(
-        [da.coords[coord_name],
-         sc.scalar(0.0, unit=da.coords[coord_name].unit)],
-        dim=da.dim)
+        [da.coords[coord_name], sc.scalar(0.0, unit=da.coords[coord_name].unit)],
+        dim=da.dim,
+    )
     with pytest.raises(sc.CoordError):
         save_to_buffer(da, coord=coord_name)
 
 
 @given(da=one_dim_data_arrays(), data=st.data())
 @settings(max_examples=20)
 def test_cannot_save_data_with_masks(da, data):
     mask = data.draw(scst.variables(sizes=da.sizes, dtype=bool))
     da.masks[data.draw(st.text())] = mask
     with pytest.raises(ValueError):
         save_to_buffer(da, coord=next(iter(da.coords)))
 
 
-@given(da=scst.dataarrays(
-    data_args={
-        'ndim': st.integers(min_value=2, max_value=4),
-        'dtype': 'float64',
-        'with_variances': True
-    }),
-       data=st.data())
+@given(
+    da=scst.dataarrays(
+        data_args={
+            'ndim': st.integers(min_value=2, max_value=4),
+            'dtype': 'float64',
+            'with_variances': True,
+        }
+    ),
+    data=st.data(),
+)
 @settings(max_examples=20)
 def test_input_must_be_one_dimensional(da, data):
     coord_name = data.draw(st.sampled_from(list(da.coords.keys())))
     with pytest.raises(sc.DimensionError):
         save_to_buffer(da, coord=coord_name)
 
 
 @given(da=one_dim_data_arrays(), header=headers())
 def test_can_set_header(da, header):
     buffer = save_to_buffer(da, coord=next(iter(da.coords)), header=header)
-    commented_header = '\n'.join(f'# {line}'
-                                 for line in header.splitlines()) if header else ''
+    commented_header = (
+        '\n'.join(f'# {line}' for line in header.splitlines()) if header else ''
+    )
     assert buffer.getvalue().startswith(commented_header)
 
 
-@given(da=one_dim_data_arrays(),
-       coord_name=st.text(string.ascii_letters + string.digits))
+@given(
+    da=one_dim_data_arrays(), coord_name=st.text(string.ascii_letters + string.digits)
+)
 def test_generated_header_includes_coord_name_and_units(da, coord_name):
     # Detecting the coord name in the file can be tricky if it can contain arbitrary
     # characters (like '\n' or '#') because lines in the header start with '# '.
     initial_name = next(iter(da.coords))
     da.coords[coord_name] = da.coords.pop(initial_name)
 
     buffer = save_to_buffer(da, coord=coord_name)
@@ -197,18 +208,19 @@
 def test_loads_correct_values():
     file_contents = '''1 2 3
 1.003 32.1 5
 0.1111 0 2.1e-3
 '''
     buffer = StringIO(file_contents)
     loaded = scn.io.load_xye(buffer, dim='my-dim', unit='one', coord_unit='us')
-    expected = sc.DataArray(sc.array(dims=['my-dim'],
-                                     values=[2, 32.1, 0],
-                                     variances=np.power([3, 5, 2.1e-3], 2),
-                                     unit='one'),
-                            coords={
-                                'my-dim':
-                                sc.array(dims=['my-dim'],
-                                         values=[1, 1.003, 0.1111],
-                                         unit='us')
-                            })
+    expected = sc.DataArray(
+        sc.array(
+            dims=['my-dim'],
+            values=[2, 32.1, 0],
+            variances=np.power([3, 5, 2.1e-3], 2),
+            unit='one',
+        ),
+        coords={
+            'my-dim': sc.array(dims=['my-dim'], values=[1, 1.003, 0.1111], unit='us')
+        },
+    )
     assert sc.identical(loaded, expected)
```

### Comparing `scippneutron-23.3.0/tests/load_nexus_json_test.py` & `scippneutron-23.4.0/tests/load_nexus_json_test.py`

 * *Files identical despite different names*

### Comparing `scippneutron-23.3.0/tests/load_nexus_test.py` & `scippneutron-23.4.0/tests/load_nexus_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,17 +8,28 @@
 import pytest
 import scipp as sc
 from dateutil.parser import parse as parse_date
 
 import scippneutron
 from scippneutron.io.nexus.load_nexus import _load_nexus_json
 
-from .nexus_helpers import Chopper, Detector, EventData, Link, Log, Monitor, \
-    NexusBuilder, Sample, Source, Transformation, TransformationType, \
-    in_memory_hdf5_file_with_two_nxentry
+from .nexus_helpers import (
+    Chopper,
+    Detector,
+    EventData,
+    Link,
+    Log,
+    Monitor,
+    NexusBuilder,
+    Sample,
+    Source,
+    Transformation,
+    TransformationType,
+    in_memory_hdf5_file_with_two_nxentry,
+)
 
 # representative sample of UTF-8 test strings from
 # https://www.w3.org/2001/06/utf-8-test/UTF-8-demo.html
 UTF8_TEST_STRINGS = (
     "∮ E⋅da = Q,  n → ∞, ∑ f(i) = ∏ g(i), ∀x∈ℝ: ⌈x⌉ = −⌊−x⌋, α ∧ ¬β = ¬(¬α ∨ β)",
     "2H₂ + O₂ ⇌ 2H₂O, R = 4.7 kΩ, ⌀ 200 mm",
     "Σὲ γνωρίζω ἀπὸ τὴν κόψη",
@@ -38,38 +49,42 @@
 def test_no_exception_if_single_nxentry_found_below_root():
     with in_memory_hdf5_file_with_two_nxentry() as nexus_file:
         # There are 2 NXentry in the file, but root is used
         # to specify which to load data from
         assert scippneutron.load_nexus(nexus_file, root='/entry_1') is None
 
 
-def load_from_nexus(builder: NexusBuilder, *args, **kwargs)\
-        -> Union[sc.Dataset, sc.DataArray, None]:
+def load_from_nexus(
+    builder: NexusBuilder, *args, **kwargs
+) -> Union[sc.Dataset, sc.DataArray, None]:
     with builder.file() as nexus_file:
         return scippneutron.load_nexus(nexus_file, *args, **kwargs)
 
 
-def load_from_json(builder: NexusBuilder, *args, **kwargs)\
-        -> Union[sc.Dataset, sc.DataArray, None]:
+def load_from_json(
+    builder: NexusBuilder, *args, **kwargs
+) -> Union[sc.Dataset, sc.DataArray, None]:
     loaded_data, _ = _load_nexus_json(builder.json_string, *args, **kwargs)
     return loaded_data
 
 
 @pytest.fixture(params=[load_from_nexus, load_from_json])
 def load_function(request) -> Callable:
     """
     Each test with this fixture is executed with load_nexus_json
     loading JSON output from the NexusBuilder, and with load_nexus
     loading in-memory NeXus output from the NexusBuilder
     """
     return request.param
 
 
-@pytest.mark.skip(reason="The 'bigfake' file is partially broken and contains "
-                  "HDF5 groups without NX_class attribute.")
+@pytest.mark.skip(
+    reason="The 'bigfake' file is partially broken and contains "
+    "HDF5 groups without NX_class attribute."
+)
 @pytest.mark.parametrize('path_type', (str, pathlib.Path))
 def test_loads_from_file(path_type):
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", message='Skipped load', category=UserWarning)
         da = scippneutron.load_nexus(path_type(scippneutron.data.bigfake()))
     assert da.sizes == {'detector_id': 90000, 'tof': 1}
     assert 'tof' in da.coords
@@ -82,129 +97,155 @@
 
 
 def test_loads_data_from_single_event_data_group(load_function: Callable):
     event_time_offsets = np.array([456, 743, 347, 345, 632])
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets,
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
 
     builder = NexusBuilder()
     builder.add_event_data(event_data)
 
     loaded_data = load_function(builder)
 
     assert loaded_data.bins.constituents['data'].unit == 'counts'
 
     # Expect time of flight to match the values in the
     # event_time_offset dataset
     # May be reordered due to binning (hence np.sort)
     assert sc.identical(
-        sc.sort(loaded_data.bins.concat('detector_id').values[0].coords['tof'],
-                key="event"),
-        sc.sort(sc.array(dims=["event"], values=event_time_offsets, unit=sc.units.ns),
-                key="event"))
+        sc.sort(
+            loaded_data.bins.concat('detector_id').values[0].coords['tof'], key="event"
+        ),
+        sc.sort(
+            sc.array(dims=["event"], values=event_time_offsets, unit=sc.units.ns),
+            key="event",
+        ),
+    )
 
     counts_on_detectors = loaded_data.bins.sum()
     # No detector_number dataset in file so expect detector_id to be
     # binned according to whatever detector_ids are present in event_id
     # dataset: 2 on det 1, 1 on det 2, 2 on det 3
     expected_counts = np.array([[2], [1], [2]])
     assert sc.identical(
         counts_on_detectors.data,
-        sc.array(dims=['detector_id', 'tof'],
-                 unit='counts',
-                 dtype='float32',
-                 values=expected_counts))
+        sc.array(
+            dims=['detector_id', 'tof'],
+            unit='counts',
+            dtype='float32',
+            values=expected_counts,
+        ),
+    )
     expected_detector_ids = np.array([1, 2, 3])
-    assert np.array_equal(loaded_data.coords['detector_id'].values,
-                          expected_detector_ids)
+    assert np.array_equal(
+        loaded_data.coords['detector_id'].values, expected_detector_ids
+    )
 
 
-@pytest.mark.parametrize("unit,multiplier",
-                         (("ns", 1), ("us", 10**3), ("ms", 10**6), ("s", 10**9)))
+@pytest.mark.parametrize(
+    "unit,multiplier", (("ns", 1), ("us", 10**3), ("ms", 10**6), ("s", 10**9))
+)
 def test_loads_pulse_times_from_single_event_with_different_units(
-        load_function: Callable, unit: str, multiplier: float):
-
+    load_function: Callable, unit: str, multiplier: float
+):
     offsets = np.array([12, 34, 56, 78])
-    zeros = np.array([12., 34., 56., 78.], dtype="float64")
+    zeros = np.array([12.0, 34.0, 56.0, 78.0], dtype="float64")
     event_data = EventData(
         event_id=np.array([1, 2, 3, 4]),
         event_time_offset=offsets,
         event_time_zero=zeros,
         event_index=np.array([0, 3, 3, 4]),
         event_time_zero_unit=unit,
     )
 
     builder = NexusBuilder()
     builder.add_detector(
-        Detector(detector_numbers=np.array([1, 2, 3, 4]), event_data=event_data))
+        Detector(detector_numbers=np.array([1, 2, 3, 4]), event_data=event_data)
+    )
 
     loaded_data = load_function(builder)
 
     for event, pulse_time in enumerate([12, 12, 12, 56]):
-        _time = np.array("1970-01-01").astype("datetime64[ns]") \
-                + np.array(pulse_time).astype("timedelta64[ns]") * multiplier
+        _time = (
+            np.array("1970-01-01").astype("datetime64[ns]")
+            + np.array(pulse_time).astype("timedelta64[ns]") * multiplier
+        )
 
         # Allow 1ns difference for rounding errors between different routes
         assert all(
-            np.abs(loaded_data.values[event].coords['pulse_time'].values -
-                   _time) <= np.array(1).astype("timedelta64[ns]"))
+            np.abs(loaded_data.values[event].coords['pulse_time'].values - _time)
+            <= np.array(1).astype("timedelta64[ns]")
+        )
 
 
-@pytest.mark.parametrize("time_zero_offset,time_zero,time_zero_unit,expected_time", (
-    ("1980-01-01T00:00:00.0", 30, "s", "1980-01-01T00:00:30.0"),
-    ("1990-01-01T00:00:00.0", 5000, "ms", "1990-01-01T00:00:05.0"),
-    ("2000-01-01T00:00:00.0", 3 * 10**6, "us", "2000-01-01T00:00:03.0"),
-    ("2010-01-01T00:00:00.0", 12, "hour", "2010-01-01T12:00:00.0"),
-))
+@pytest.mark.parametrize(
+    "time_zero_offset,time_zero,time_zero_unit,expected_time",
+    (
+        ("1980-01-01T00:00:00.0", 30, "s", "1980-01-01T00:00:30.0"),
+        ("1990-01-01T00:00:00.0", 5000, "ms", "1990-01-01T00:00:05.0"),
+        ("2000-01-01T00:00:00.0", 3 * 10**6, "us", "2000-01-01T00:00:03.0"),
+        ("2010-01-01T00:00:00.0", 12, "hour", "2010-01-01T12:00:00.0"),
+    ),
+)
 def test_loads_pulse_times_with_combinations_of_offset_and_units(
-        load_function: Callable, time_zero_offset: str, time_zero: float,
-        time_zero_unit: str, expected_time: str):
-
+    load_function: Callable,
+    time_zero_offset: str,
+    time_zero: float,
+    time_zero_unit: str,
+    expected_time: str,
+):
     offsets = np.array([0])
     zeros = np.array([time_zero], dtype="float64")
     event_data = EventData(
         event_id=np.array([0]),
         event_time_offset=offsets,
         event_time_zero_offset=time_zero_offset,
         event_time_zero=zeros,
         event_index=np.array([0]),
         event_time_zero_unit=time_zero_unit,
     )
 
     builder = NexusBuilder()
-    builder.add_detector(Detector(detector_numbers=np.array([0]),
-                                  event_data=event_data))
+    builder.add_detector(
+        Detector(detector_numbers=np.array([0]), event_data=event_data)
+    )
 
     loaded_data = load_function(builder)
 
     _time = np.array(expected_time).astype("datetime64[ns]")
 
     # Allow 1ns difference for rounding errors between different routes
-    assert np.abs(loaded_data.values[0].coords['pulse_time'].values[0] -
-                  _time) <= np.array(1).astype("timedelta64[ns]")
+    assert np.abs(
+        loaded_data.values[0].coords['pulse_time'].values[0] - _time
+    ) <= np.array(1).astype("timedelta64[ns]")
 
 
 def test_does_not_load_events_if_index_not_ordered(load_function: Callable):
     event_data_1 = EventData(
         event_id=np.array([0, 1]),
         event_time_offset=np.array([0, 1]),
         event_time_zero=np.array([0, 1]),
         event_index=np.array([2, 0]),
     )
 
     builder = NexusBuilder()
     builder.add_detector(
-        Detector(detector_numbers=np.array([0, 1]), event_data=event_data_1))
+        Detector(detector_numbers=np.array([0, 1]), event_data=event_data_1)
+    )
 
     with pytest.warns(UserWarning, match="Invalid index in NXevent_data at "):
         load_function(builder)
 
 
 def test_loads_pulse_times_from_multiple_event_data_groups(load_function: Callable):
     offsets = np.array([0, 0, 0, 0])
@@ -223,37 +264,47 @@
         event_time_offset=offsets,
         event_time_zero=zeros_2,
         event_index=np.array([0, 3, 3, 4]),
     )
 
     builder = NexusBuilder()
     builder.add_detector(
-        Detector(detector_numbers=np.array([0, 1, 2, 3]), event_data=event_data_1))
+        Detector(detector_numbers=np.array([0, 1, 2, 3]), event_data=event_data_1)
+    )
     builder.add_detector(
-        Detector(detector_numbers=np.array([4, 5, 6, 7]), event_data=event_data_2))
+        Detector(detector_numbers=np.array([4, 5, 6, 7]), event_data=event_data_2)
+    )
 
     loaded_data = load_function(builder)
 
     for event, pulse_time in enumerate([12, 12, 12, 56, 87, 87, 87, 43]):
-        _time = np.array("1970-01-01").astype("datetime64[ns]") \
-                + np.array(pulse_time).astype("timedelta64[s]")
+        _time = np.array("1970-01-01").astype("datetime64[ns]") + np.array(
+            pulse_time
+        ).astype("timedelta64[s]")
 
         assert sc.identical(
             loaded_data.values[event].coords['pulse_time'],
-            sc.array(dims=["event"],
-                     values=[_time],
-                     unit=sc.units.ns,
-                     dtype=sc.DType.datetime64))
+            sc.array(
+                dims=["event"],
+                values=[_time],
+                unit=sc.units.ns,
+                dtype=sc.DType.datetime64,
+            ),
+        )
 
 
 def test_loads_data_from_multiple_event_data_groups(load_function: Callable):
-    pulse_times = np.array([
-        1600766730000000000, 1600766731000000000, 1600766732000000000,
-        1600766733000000000
-    ])
+    pulse_times = np.array(
+        [
+            1600766730000000000,
+            1600766731000000000,
+            1600766732000000000,
+            1600766733000000000,
+        ]
+    )
     event_time_offsets_1 = np.array([456, 743, 347, 345, 632])
     event_data_1 = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets_1,
         event_time_zero=pulse_times,
         event_index=np.array([0, 3, 3, 5]),
     )
@@ -274,95 +325,115 @@
     loaded_data = load_function(builder)
 
     # Expect time of flight to match the values in the
     # event_time_offset datasets
     # May be reordered due to binning (hence np.sort)
     assert np.array_equal(
         np.sort(loaded_data.bins.concat('detector_id').values[0].coords['tof'].values),
-        np.sort(np.concatenate((event_time_offsets_1, event_time_offsets_2))))
+        np.sort(np.concatenate((event_time_offsets_1, event_time_offsets_2))),
+    )
 
     counts_on_detectors = loaded_data.bins.sum()
     # There are detector_number datasets in the NXdetector for each
     # NXevent_data, these are used for detector_id binning
     expected_counts = np.array([[0], [2], [1], [2], [2], [1], [2], [0]])
     assert np.array_equal(counts_on_detectors.data.values, expected_counts)
     expected_detector_ids = np.concatenate((detector_1_ids, detector_2_ids))
-    assert np.array_equal(loaded_data.coords['detector_id'].values,
-                          expected_detector_ids)
+    assert np.array_equal(
+        loaded_data.coords['detector_id'].values, expected_detector_ids
+    )
 
 
 def test_skips_event_data_group_with_non_integer_event_ids(load_function: Callable):
     event_time_offsets = np.array([456, 743, 347, 345, 632])
     event_data = EventData(
         event_id=np.array([1.1, 2.2, 3.3, 1.1, 3.1]),
         event_time_offset=event_time_offsets,
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
 
     builder = NexusBuilder()
     builder.add_event_data(event_data)
 
     with pytest.warns(UserWarning):
         loaded_data = load_function(builder)
 
-    assert loaded_data is None, "Expected no data to be loaded as " \
-                                "event data has non integer event ids"
+    assert loaded_data is None, (
+        "Expected no data to be loaded as " "event data has non integer event ids"
+    )
 
 
 def test_skips_event_data_group_with_non_integer_detector_numbers(
-        load_function: Callable):
+    load_function: Callable,
+):
     event_time_offsets = np.array([456, 743, 347, 345, 632])
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets,
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
     detector_numbers = np.array([0.1, 1.2, 2.3, 3.4])
 
     builder = NexusBuilder()
     builder.add_detector(Detector(detector_numbers, event_data))
 
     with pytest.warns(UserWarning):
         loaded_data = load_function(builder)
 
-    assert loaded_data is None, "Expected no data to be loaded as " \
-                                "detector has non integer detector numbers"
+    assert loaded_data is None, (
+        "Expected no data to be loaded as " "detector has non integer detector numbers"
+    )
 
 
 def test_skips_data_with_event_id_and_detector_number_type_unequal(
-        load_function: Callable):
+    load_function: Callable,
+):
     event_time_offsets = np.array([456, 743, 347, 345, 632])
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3], dtype=np.int64),
         event_time_offset=event_time_offsets,
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
     detector_numbers = np.array([0, 1, 2, 3], dtype=np.float32)
 
     builder = NexusBuilder()
     builder.add_detector(Detector(detector_numbers, event_data))
 
     with pytest.warns(UserWarning):
         loaded_data = load_function(builder)
 
-    assert loaded_data is None, "Expected no data to be loaded as event " \
-                                "ids and detector numbers are of " \
-                                "different types"
+    assert loaded_data is None, (
+        "Expected no data to be loaded as event "
+        "ids and detector numbers are of "
+        "different types"
+    )
 
 
 def test_loads_data_from_single_log_with_no_units(load_function: Callable):
     values = np.array([1, 2, 3])
     times = np.array([4, 5, 6])
     name = "test_log"
     builder = NexusBuilder()
@@ -400,24 +471,32 @@
     # Expect a sc.Dataset with log names as keys
     assert np.allclose(loaded_data[log_1.name].data.values.values, log_1.value)
     assert np.array_equal(loaded_data[log_2.name].data.values.values, log_2.value)
 
 
 def test_loads_logs_with_non_supported_int_types(load_function: Callable):
     builder = NexusBuilder()
-    log_int8 = Log("test_log_int8",
-                   np.array([1, 2, 3]).astype(np.int8), np.array([4.4, 5.5, 6.6]))
-    log_int16 = Log("test_log_int16",
-                    np.array([123, 253, 756]).astype(np.int16),
-                    np.array([246, 1235, 2369]))
-    log_uint8 = Log("test_log_uint8",
-                    np.array([1, 2, 3]).astype(np.uint8), np.array([4.4, 5.5, 6.6]))
-    log_uint16 = Log("test_log_uint16",
-                     np.array([123, 253, 756]).astype(np.uint16),
-                     np.array([246, 1235, 2369]))
+    log_int8 = Log(
+        "test_log_int8", np.array([1, 2, 3]).astype(np.int8), np.array([4.4, 5.5, 6.6])
+    )
+    log_int16 = Log(
+        "test_log_int16",
+        np.array([123, 253, 756]).astype(np.int16),
+        np.array([246, 1235, 2369]),
+    )
+    log_uint8 = Log(
+        "test_log_uint8",
+        np.array([1, 2, 3]).astype(np.uint8),
+        np.array([4.4, 5.5, 6.6]),
+    )
+    log_uint16 = Log(
+        "test_log_uint16",
+        np.array([123, 253, 756]).astype(np.uint16),
+        np.array([246, 1235, 2369]),
+    )
     logs = (log_int8, log_int16, log_uint8, log_uint16)
     for log in logs:
         builder.add_log(log)
 
     loaded_data = load_function(builder)
 
     # Expect a sc.Dataset with log names as keys
@@ -433,15 +512,16 @@
     builder.add_log(Log(name, multidim_values, times, value_units=''))
 
     loaded_data = load_function(builder)
 
     log = loaded_data[name].data.value
     expected = sc.DataArray(sc.array(dims=['time', 'dim_1'], values=multidim_values))
     expected.coords['time'] = sc.epoch(unit='s') + sc.array(
-        dims=['time'], values=times, unit='s')
+        dims=['time'], values=times, unit='s'
+    )
     assert sc.identical(log, expected)
 
 
 def test_skips_log_with_no_value_dataset(load_function: Callable):
     name = "test_log"
     builder = NexusBuilder()
     builder.add_log(Log(name, None, np.array([4, 5, 6])))
@@ -498,20 +578,20 @@
     # Add one log to NXentry and the other to an NXdetector,
     # both have the same group name
     builder = NexusBuilder()
     builder.add_log(Log(name, values_1))
     builder.add_detector(Detector(log=Log(name, values_2)))
 
     with warnings.catch_warnings():
-        warnings.filterwarnings("ignore",
-                                message='Failed to load',
-                                category=UserWarning)
-        warnings.filterwarnings("ignore",
-                                message='Skipped loading',
-                                category=UserWarning)
+        warnings.filterwarnings(
+            "ignore", message='Failed to load', category=UserWarning
+        )
+        warnings.filterwarnings(
+            "ignore", message='Skipped loading', category=UserWarning
+        )
         loaded_data = load_function(builder)
 
     assert len(loaded_data) == 2
     for key, da in loaded_data.items():
         assert key.endswith('test_log')
         if 'detector_0' in key:
             assert np.allclose(da.value.values, values_2)
@@ -540,18 +620,22 @@
 
 
 def test_loads_event_and_log_data_from_single_file(load_function: Callable):
     event_time_offsets = np.array([456, 743, 347, 345, 632])
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets,
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
 
     log_1 = Log("test_log", np.array([1.1, 2.2, 3.3]), np.array([4.4, 5.5, 6.6]))
     log_2 = Log("test_log_2", np.array([123, 253, 756]), np.array([246, 1235, 2369]))
 
     builder = NexusBuilder()
@@ -562,38 +646,44 @@
     loaded_data = load_function(builder)
 
     # Expect time of flight to match the values in the
     # event_time_offset dataset
     # May be reordered due to binning (hence np.sort)
     assert np.allclose(
         np.sort(loaded_data.bins.concat('detector_id').values[0].coords['tof'].values),
-        np.sort(event_time_offsets))
+        np.sort(event_time_offsets),
+    )
 
     counts_on_detectors = loaded_data.bins.sum()
     # No detector_number dataset in file so expect detector_id to be
     # binned from the min to the max detector_id recorded in event_id
     # dataset: 2 on det 1, 1 on det 2, 2 on det 3
     expected_counts = np.array([[2], [1], [2]])
     assert np.allclose(counts_on_detectors.data.values, expected_counts)
     expected_detector_ids = np.array([1, 2, 3])
     assert np.allclose(loaded_data.coords['detector_id'].values, expected_detector_ids)
-    assert "position" not in loaded_data.meta.keys(
-    ), "The NXdetectors had no pixel position datasets so we " \
-       "should not find 'position' coord"
+    assert "position" not in loaded_data.meta.keys(), (
+        "The NXdetectors had no pixel position datasets so we "
+        "should not find 'position' coord"
+    )
 
     # Logs should have been added to the DataArray as attributes
     assert np.allclose(loaded_data.attrs[log_1.name].values.values, log_1.value)
     assert np.allclose(loaded_data.attrs[log_2.name].values.values, log_2.value)
 
 
 def test_loads_pixel_positions_with_event_data(load_function: Callable):
-    pulse_times = np.array([
-        1600766730000000000, 1600766731000000000, 1600766732000000000,
-        1600766733000000000
-    ])
+    pulse_times = np.array(
+        [
+            1600766730000000000,
+            1600766731000000000,
+            1600766732000000000,
+            1600766733000000000,
+        ]
+    )
     event_time_offsets_1 = np.array([456, 743, 347, 345, 632])
     event_data_1 = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets_1,
         event_time_zero=pulse_times,
         event_index=np.array([0, 3, 3, 5]),
     )
@@ -614,42 +704,52 @@
     detector_2_ids = np.array([[4, 5], [6, 7]])
     x_pixel_offset_2 = np.array([[1.1, 1.2], [1.1, 1.2]])
     y_pixel_offset_2 = np.array([[0.1, 0.1], [0.2, 0.2]])
 
     builder = NexusBuilder()
     offsets_units = "mm"
     builder.add_detector(
-        Detector(detector_1_ids,
-                 event_data_1,
-                 x_offsets=x_pixel_offset_1,
-                 y_offsets=y_pixel_offset_1,
-                 z_offsets=z_pixel_offset_1,
-                 offsets_unit=offsets_units))
+        Detector(
+            detector_1_ids,
+            event_data_1,
+            x_offsets=x_pixel_offset_1,
+            y_offsets=y_pixel_offset_1,
+            z_offsets=z_pixel_offset_1,
+            offsets_unit=offsets_units,
+        )
+    )
     builder.add_detector(
-        Detector(detector_2_ids,
-                 event_data_2,
-                 x_offsets=x_pixel_offset_2,
-                 y_offsets=y_pixel_offset_2,
-                 offsets_unit=offsets_units))
+        Detector(
+            detector_2_ids,
+            event_data_2,
+            x_offsets=x_pixel_offset_2,
+            y_offsets=y_pixel_offset_2,
+            offsets_unit=offsets_units,
+        )
+    )
 
     loaded_data = load_function(builder)
 
     # If z offsets are missing they should be zero
-    z_pixel_offset_2 = np.array([[0., 0.], [0., 0.]])
-    expected_pixel_positions = np.array([
-        np.concatenate((x_pixel_offset_1, x_pixel_offset_2.flatten())),
-        np.concatenate((y_pixel_offset_1, y_pixel_offset_2.flatten())),
-        np.concatenate((z_pixel_offset_1, z_pixel_offset_2.flatten()))
-    ]).T
+    z_pixel_offset_2 = np.array([[0.0, 0.0], [0.0, 0.0]])
+    expected_pixel_positions = np.array(
+        [
+            np.concatenate((x_pixel_offset_1, x_pixel_offset_2.flatten())),
+            np.concatenate((y_pixel_offset_1, y_pixel_offset_2.flatten())),
+            np.concatenate((z_pixel_offset_1, z_pixel_offset_2.flatten())),
+        ]
+    ).T
     assert np.allclose(loaded_data.coords['position'].values, expected_pixel_positions)
     assert loaded_data.meta['position'].unit == 'mm'
 
 
-@pytest.mark.skip(reason="It is unclear if NXdetector with neither data nor event_data "
-                  "needs to be considered valid.")
+@pytest.mark.skip(
+    reason="It is unclear if NXdetector with neither data nor event_data "
+    "needs to be considered valid."
+)
 def test_loads_pixel_positions_without_event_data(load_function: Callable):
     """
     This is important in the live-data feature as geometry and event data
     are streamed separately
     """
     detector_1_ids = np.array([0, 1, 2, 3])
     x_pixel_offset_1 = np.array([0.1, 0.2, 0.1, 0.2])
@@ -659,65 +759,83 @@
     detector_2_ids = np.array([[4, 5], [6, 7]])
     x_pixel_offset_2 = np.array([[1.1, 1.2], [1.1, 1.2]])
     y_pixel_offset_2 = np.array([[0.1, 0.1], [0.2, 0.2]])
 
     builder = NexusBuilder()
     offsets_units = "mm"
     builder.add_detector(
-        Detector(detector_numbers=detector_1_ids,
-                 x_offsets=x_pixel_offset_1,
-                 y_offsets=y_pixel_offset_1,
-                 z_offsets=z_pixel_offset_1,
-                 offsets_unit=offsets_units))
+        Detector(
+            detector_numbers=detector_1_ids,
+            x_offsets=x_pixel_offset_1,
+            y_offsets=y_pixel_offset_1,
+            z_offsets=z_pixel_offset_1,
+            offsets_unit=offsets_units,
+        )
+    )
     builder.add_detector(
-        Detector(detector_numbers=detector_2_ids,
-                 x_offsets=x_pixel_offset_2,
-                 y_offsets=y_pixel_offset_2,
-                 offsets_unit=offsets_units))
+        Detector(
+            detector_numbers=detector_2_ids,
+            x_offsets=x_pixel_offset_2,
+            y_offsets=y_pixel_offset_2,
+            offsets_unit=offsets_units,
+        )
+    )
 
     loaded_data = load_function(builder)
 
     # If z offsets are missing they should be zero
-    z_pixel_offset_2 = np.array([[0., 0.], [0., 0.]])
-    expected_pixel_positions = np.array([
-        np.concatenate((x_pixel_offset_1, x_pixel_offset_2.flatten())),
-        np.concatenate((y_pixel_offset_1, y_pixel_offset_2.flatten())),
-        np.concatenate((z_pixel_offset_1, z_pixel_offset_2.flatten()))
-    ]).T / 1_000  # Divide by 1000 for mm to metres
+    z_pixel_offset_2 = np.array([[0.0, 0.0], [0.0, 0.0]])
+    expected_pixel_positions = (
+        np.array(
+            [
+                np.concatenate((x_pixel_offset_1, x_pixel_offset_2.flatten())),
+                np.concatenate((y_pixel_offset_1, y_pixel_offset_2.flatten())),
+                np.concatenate((z_pixel_offset_1, z_pixel_offset_2.flatten())),
+            ]
+        ).T
+        / 1_000
+    )  # Divide by 1000 for mm to metres
     assert np.allclose(loaded_data.coords['position'].values, expected_pixel_positions)
-    assert loaded_data.meta[
-               'base_position'].unit == sc.units.m, \
-        "Expected positions to be converted to metres"
+    assert (
+        loaded_data.meta['base_position'].unit == sc.units.m
+    ), "Expected positions to be converted to metres"
 
 
 def test_loads_pixel_positions_with_no_units(load_function: Callable):
-    pulse_times = np.array([
-        1600766730000000000, 1600766731000000000, 1600766732000000000,
-        1600766733000000000
-    ])
+    pulse_times = np.array(
+        [
+            1600766730000000000,
+            1600766731000000000,
+            1600766732000000000,
+            1600766733000000000,
+        ]
+    )
     event_time_offsets = np.array([456, 743, 347, 345, 632])
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets,
         event_time_zero=pulse_times,
         event_index=np.array([0, 3, 3, 5]),
     )
     detector_ids = np.array([0, 1, 2, 3])
     x_pixel_offset = np.array([0.1, 0.2, 0.1, 0.2])
     y_pixel_offset = np.array([0.1, 0.1, 0.2, 0.2])
     z_pixel_offset = np.array([0.1, 0.2, 0.3, 0.4])
 
     builder = NexusBuilder()
     builder.add_detector(
-        Detector(detector_ids,
-                 event_data,
-                 x_offsets=x_pixel_offset,
-                 y_offsets=y_pixel_offset,
-                 z_offsets=z_pixel_offset,
-                 offsets_unit=None))
+        Detector(
+            detector_ids,
+            event_data,
+            x_offsets=x_pixel_offset,
+            y_offsets=y_pixel_offset,
+            z_offsets=z_pixel_offset,
+            offsets_unit=None,
+        )
+    )
 
     loaded_data = load_function(builder)
 
     assert loaded_data.coords['position'].unit is None
 
 
 def test_sample_position_at_origin_if_not_explicit_in_file(load_function: Callable):
@@ -745,512 +863,679 @@
 
     distance = 0.762
     units = "m"
     builder.add_sample(Sample(sample_2_name, distance=distance, distance_units=units))
     loaded_data = load_function(builder)
 
     origin = np.array([0, 0, 0])
-    assert np.allclose(
-        loaded_data[f"{sample_1_name}_position"].values, origin
-    ), "Sample did not have explicit location so expect position " \
-       "to be recorded as the origin"
+    assert np.allclose(loaded_data[f"{sample_1_name}_position"].values, origin), (
+        "Sample did not have explicit location so expect position "
+        "to be recorded as the origin"
+    )
     expected_position = np.array([0, 0, distance])
-    assert np.allclose(loaded_data[f"{sample_2_name}_position"].values,
-                       expected_position)
+    assert np.allclose(
+        loaded_data[f"{sample_2_name}_position"].values, expected_position
+    )
 
 
 def test_skips_loading_source_if_more_than_one_in_file(load_function: Callable):
     # More than one source is a serious error in the file, so load_nexus will not
     # define a source_position rather than guessing which is the "correct" one.
     builder = NexusBuilder()
     builder.add_source(Source("source_1"))
     builder.add_source(Source("source_2"))
     loaded_data = load_function(builder)
     assert 'source_1' in loaded_data
     assert 'source_2' in loaded_data
     assert 'source_position' not in loaded_data
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
 def test_component_position_from_distance_dataset_missing_unit(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    load_function: Callable,
+):
     builder = NexusBuilder()
     distance = 4.2
     builder.add_component(
-        component_class(component_name, distance=distance, distance_units=None))
+        component_class(component_name, distance=distance, distance_units=None)
+    )
     loaded_data = load_function(builder)
     assert loaded_data[f'{component_name}_position'].unit is None
 
 
-@pytest.mark.parametrize("component_class,component_name", [(Sample, "sample"),
-                                                            (Source, "source")])
-@pytest.mark.parametrize("transform_type,value,value_units,expected_position",
-                         ((TransformationType.ROTATION, 0.27, "rad", [0, 0, 0]),
-                          (TransformationType.TRANSLATION, 230, "cm", [0, 0, 2.3])))
+@pytest.mark.parametrize(
+    "component_class,component_name", [(Sample, "sample"), (Source, "source")]
+)
+@pytest.mark.parametrize(
+    "transform_type,value,value_units,expected_position",
+    (
+        (TransformationType.ROTATION, 0.27, "rad", [0, 0, 0]),
+        (TransformationType.TRANSLATION, 230, "cm", [0, 0, 2.3]),
+    ),
+)
 def test_loads_component_position_from_single_transformation(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        transform_type: TransformationType, value: float, value_units: str,
-        expected_position: List[float], load_function: Callable):
-    builder = NexusBuilder()
-    transformation = Transformation(transform_type,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(value),
-                                    value_units=value_units)
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    transform_type: TransformationType,
+    value: float,
+    value_units: str,
+    expected_position: List[float],
+    load_function: Callable,
+):
+    builder = NexusBuilder()
+    transformation = Transformation(
+        transform_type,
+        vector=np.array([0, 0, 1]),
+        value=np.array(value),
+        value_units=value_units,
+    )
     builder.add_component(component_class(component_name, depends_on=transformation))
     loaded_data = load_function(builder)
-    assert np.allclose(loaded_data[f"{component_name}_position"].values,
-                       expected_position)
+    assert np.allclose(
+        loaded_data[f"{component_name}_position"].values, expected_position
+    )
     # Resulting position will always be in metres, whatever units are
     # used in the NeXus file
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
-@pytest.mark.parametrize("component_class,component_name", [(Sample, "sample"),
-                                                            (Source, "source")])
-@pytest.mark.parametrize("transform_type,value,value_units,expected_position",
-                         ((TransformationType.ROTATION, 180, "deg", [-1, -2, 3]),
-                          (TransformationType.TRANSLATION, 230, "cm", [1, 2, 5.3])))
+@pytest.mark.parametrize(
+    "component_class,component_name", [(Sample, "sample"), (Source, "source")]
+)
+@pytest.mark.parametrize(
+    "transform_type,value,value_units,expected_position",
+    (
+        (TransformationType.ROTATION, 180, "deg", [-1, -2, 3]),
+        (TransformationType.TRANSLATION, 230, "cm", [1, 2, 5.3]),
+    ),
+)
 def test_loads_component_position_from_single_transformation_with_offset(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        transform_type: TransformationType, value: float, value_units: str,
-        expected_position: List[float], load_function: Callable):
-    builder = NexusBuilder()
-    transformation = Transformation(transform_type,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(value),
-                                    value_units=value_units,
-                                    offset=[1, 2, 3],
-                                    offset_unit='m')
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    transform_type: TransformationType,
+    value: float,
+    value_units: str,
+    expected_position: List[float],
+    load_function: Callable,
+):
+    builder = NexusBuilder()
+    transformation = Transformation(
+        transform_type,
+        vector=np.array([0, 0, 1]),
+        value=np.array(value),
+        value_units=value_units,
+        offset=[1, 2, 3],
+        offset_unit='m',
+    )
     builder.add_component(component_class(component_name, depends_on=transformation))
     loaded_data = load_function(builder)
-    assert np.allclose(loaded_data[f"{component_name}_position"].values,
-                       expected_position)
+    assert np.allclose(
+        loaded_data[f"{component_name}_position"].values, expected_position
+    )
     # Resulting position will always be in metres, whatever units are
     # used in the NeXus file
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
-@pytest.mark.parametrize("component_class,component_name", [(Sample, "sample"),
-                                                            (Source, "source")])
-@pytest.mark.parametrize("transform_type,value,value_units,expected_position",
-                         ((TransformationType.ROTATION, 180, "deg", [-1, -2, 3]),
-                          (TransformationType.TRANSLATION, 230, "cm", [1, 2, 5.3])))
+@pytest.mark.parametrize(
+    "component_class,component_name", [(Sample, "sample"), (Source, "source")]
+)
+@pytest.mark.parametrize(
+    "transform_type,value,value_units,expected_position",
+    (
+        (TransformationType.ROTATION, 180, "deg", [-1, -2, 3]),
+        (TransformationType.TRANSLATION, 230, "cm", [1, 2, 5.3]),
+    ),
+)
 def test_raises_if_offset_but_not_offset_units_found(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        transform_type: TransformationType, value: float, value_units: str,
-        expected_position: List[float], load_function: Callable):
-    builder = NexusBuilder()
-    transformation = Transformation(transform_type,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(value),
-                                    value_units=value_units,
-                                    offset=[1, 2, 3],
-                                    offset_unit=None)
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    transform_type: TransformationType,
+    value: float,
+    value_units: str,
+    expected_position: List[float],
+    load_function: Callable,
+):
+    builder = NexusBuilder()
+    transformation = Transformation(
+        transform_type,
+        vector=np.array([0, 0, 1]),
+        value=np.array(value),
+        value_units=value_units,
+        offset=[1, 2, 3],
+        offset_unit=None,
+    )
     builder.add_component(component_class(component_name, depends_on=transformation))
     with warnings.catch_warnings():
-        warnings.filterwarnings("ignore",
-                                message='Failed to load',
-                                category=UserWarning)
+        warnings.filterwarnings(
+            "ignore", message='Failed to load', category=UserWarning
+        )
         loaded_data = load_function(builder)
     assert isinstance(loaded_data[component_name].value['depends_on'], str)
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
-@pytest.mark.parametrize("transform_type,value,value_units,expected_position",
-                         ((TransformationType.ROTATION, 0.27, "rad", [0, 0, 0]),
-                          (TransformationType.TRANSLATION, 230, "cm", [0, 0, 2.3])))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
+@pytest.mark.parametrize(
+    "transform_type,value,value_units,expected_position",
+    (
+        (TransformationType.ROTATION, 0.27, "rad", [0, 0, 0]),
+        (TransformationType.TRANSLATION, 230, "cm", [0, 0, 2.3]),
+    ),
+)
 def test_loads_component_position_from_log_transformation(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        transform_type: TransformationType, value: float, value_units: str,
-        expected_position: List[float], load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    transform_type: TransformationType,
+    value: float,
+    value_units: str,
+    expected_position: List[float],
+    load_function: Callable,
+):
     builder = NexusBuilder()
     # Provide "time" data, the builder will write the transformation as
     # an NXlog
-    transformation = Transformation(transform_type,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(value),
-                                    value_units=value_units)
+    transformation = Transformation(
+        transform_type,
+        vector=np.array([0, 0, 1]),
+        value=np.array(value),
+        value_units=value_units,
+    )
     builder.add_component(component_class(component_name, depends_on=transformation))
     loaded_data = load_function(builder)
 
     # Should load as usual despite the transformation being an NXlog
     # as it only has a single value
-    assert np.allclose(loaded_data[f"{component_name}_position"].values,
-                       expected_position)
+    assert np.allclose(
+        loaded_data[f"{component_name}_position"].values, expected_position
+    )
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
 @pytest.mark.parametrize(
     "transform_type,value,value_units,expected_position",
-    ((TransformationType.ROTATION, [0.27, 0.73], "rad", [0, 0, 0]),
-     (TransformationType.TRANSLATION, [230, 310], "cm", [0, 0, 2.3])))
+    (
+        (TransformationType.ROTATION, [0.27, 0.73], "rad", [0, 0, 0]),
+        (TransformationType.TRANSLATION, [230, 310], "cm", [0, 0, 2.3]),
+    ),
+)
 def test_loads_component_position_with_multi_value_log_transformation(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        transform_type: TransformationType, value: List[float], value_units: str,
-        expected_position: float, load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    transform_type: TransformationType,
+    value: List[float],
+    value_units: str,
+    expected_position: float,
+    load_function: Callable,
+):
     builder = NexusBuilder()
     # Provide "time" data, the builder will write the transformation as
     # an NXlog. This would be encountered in a file from an experiment
     # involving a scan of a motion axis.
-    transformation = Transformation(transform_type,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(value),
-                                    time=np.array([1.3, 6.4]),
-                                    time_units="s",
-                                    value_units=value_units)
+    transformation = Transformation(
+        transform_type,
+        vector=np.array([0, 0, 1]),
+        value=np.array(value),
+        time=np.array([1.3, 6.4]),
+        time_units="s",
+        value_units=value_units,
+    )
     builder.add_component(component_class(component_name, depends_on=transformation))
     loaded_data = load_function(builder)
     assert sc.identical(
         loaded_data[component_name].value['depends_on'].coords["time"],
-        sc.Variable(dims=["time"],
-                    values=[1300000000, 6400000000],
-                    unit="ns",
-                    dtype=sc.DType.datetime64))
+        sc.Variable(
+            dims=["time"],
+            values=[1300000000, 6400000000],
+            unit="ns",
+            dtype=sc.DType.datetime64,
+        ),
+    )
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
 def test_loads_component_position_with_multiple_multi_valued_log_transformations(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    load_function: Callable,
+):
     builder = NexusBuilder()
     # Provide "time" data, the builder will write the transformation as
     # an NXlog. This would be encountered in a file from an experiment
     # involving a scan of a motion axis.
-    t1 = Transformation(TransformationType.TRANSLATION,
-                        vector=np.array([0, 0, 1]),
-                        value=np.array([1, 10]),
-                        time=np.array([0, 1]),
-                        time_units="s",
-                        value_units="m")
-
-    t2 = Transformation(TransformationType.TRANSLATION,
-                        vector=np.array([0, 0, 1]),
-                        value=np.array([5, 50]),
-                        time=np.array([0, 1]),
-                        time_units="s",
-                        value_units="m",
-                        depends_on=t1)
+    t1 = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array([1, 10]),
+        time=np.array([0, 1]),
+        time_units="s",
+        value_units="m",
+    )
+
+    t2 = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array([5, 50]),
+        time=np.array([0, 1]),
+        time_units="s",
+        value_units="m",
+        depends_on=t1,
+    )
 
     builder.add_component(component_class(component_name, depends_on=t2))
     loaded_data = load_function(builder)
     comp = loaded_data[component_name].value
     assert sc.identical(
         comp['depends_on'].coords["time"],
-        sc.Variable(dims=["time"], values=[0, 1], unit="s", dtype=sc.DType.datetime64))
+        sc.Variable(dims=["time"], values=[0, 1], unit="s", dtype=sc.DType.datetime64),
+    )
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
 def test_multi_valued_log_transformations_time_axis_interpolated_and_trimmed(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    load_function: Callable,
+):
     builder = NexusBuilder()
-    t1 = Transformation(TransformationType.TRANSLATION,
-                        vector=np.array([0, 0, 1]),
-                        value=np.array([1, 10]),
-                        time=np.array([0, 1]),
-                        time_units="s",
-                        value_units="m")
-    t2 = Transformation(TransformationType.TRANSLATION,
-                        vector=np.array([0, 0, 1]),
-                        value=np.array([5, 50]),
-                        time=np.array([0.1, 1.1]),
-                        time_units="s",
-                        value_units="m",
-                        depends_on=t1)
+    t1 = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array([1, 10]),
+        time=np.array([0, 1]),
+        time_units="s",
+        value_units="m",
+    )
+    t2 = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array([5, 50]),
+        time=np.array([0.1, 1.1]),
+        time_units="s",
+        value_units="m",
+        depends_on=t1,
+    )
     builder.add_component(component_class(component_name, depends_on=t2))
 
     loaded_data = load_function(builder)
 
     # Note the start at 100 ms, since there is no known value of t2 at 0 ms (when
     # t1 starts)
     comp = loaded_data[component_name].value
     assert sc.identical(
         comp['depends_on'].coords["time"],
-        sc.array(dims=["time"],
-                 values=[100, 1000, 1100],
-                 unit="ms",
-                 dtype=sc.DType.datetime64).to(unit="ns"))
+        sc.array(
+            dims=["time"],
+            values=[100, 1000, 1100],
+            unit="ms",
+            dtype=sc.DType.datetime64,
+        ).to(unit="ns"),
+    )
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
-@pytest.mark.parametrize("transform_type,value_units",
-                         ((TransformationType.ROTATION, "deg"),
-                          (TransformationType.TRANSLATION, "cm")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
+@pytest.mark.parametrize(
+    "transform_type,value_units",
+    ((TransformationType.ROTATION, "deg"), (TransformationType.TRANSLATION, "cm")),
+)
 def test_skips_component_position_with_empty_value_log_transformation(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        transform_type: TransformationType, value_units: str, load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    transform_type: TransformationType,
+    value_units: str,
+    load_function: Callable,
+):
     builder = NexusBuilder()
     empty_value = np.array([])
-    transformation = Transformation(transform_type,
-                                    vector=np.array([0, 0, 1]),
-                                    value=empty_value,
-                                    time=np.array([1.3, 6.4]),
-                                    time_units="s",
-                                    value_units=value_units)
+    transformation = Transformation(
+        transform_type,
+        vector=np.array([0, 0, 1]),
+        value=empty_value,
+        time=np.array([1.3, 6.4]),
+        time_units="s",
+        value_units=value_units,
+    )
     builder.add_component(component_class(component_name, depends_on=transformation))
     with pytest.warns(UserWarning):
         load_function(builder)
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
 def test_load_component_position_prefers_transform_over_distance(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    load_function: Callable,
+):
     # The "distance" dataset gives the position along the z axis.
     # If there is a "depends_on" pointing to transformations then we
     # prefer to use that instead as it is likely to be more accurate; it
     # can define position and orientation in 3D.
     builder = NexusBuilder()
-    transformation = Transformation(TransformationType.TRANSLATION,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(2.3),
-                                    value_units="m")
+    transformation = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array(2.3),
+        value_units="m",
+    )
     builder.add_component(
-        component_class(component_name,
-                        depends_on=transformation,
-                        distance=4.2,
-                        distance_units="m"))
+        component_class(
+            component_name, depends_on=transformation, distance=4.2, distance_units="m"
+        )
+    )
     loaded_data = load_function(builder)
 
     expected_position = np.array([0, 0, transformation.value])
-    assert np.allclose(loaded_data[f"{component_name}_position"].values,
-                       expected_position)
+    assert np.allclose(
+        loaded_data[f"{component_name}_position"].values, expected_position
+    )
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
-@pytest.mark.parametrize("transform_type",
-                         (TransformationType.ROTATION, TransformationType.TRANSLATION))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
+@pytest.mark.parametrize(
+    "transform_type", (TransformationType.ROTATION, TransformationType.TRANSLATION)
+)
 def test_skips_component_position_from_transformation_missing_unit(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        transform_type: TransformationType, load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    transform_type: TransformationType,
+    load_function: Callable,
+):
     builder = NexusBuilder()
-    transformation = Transformation(transform_type,
-                                    np.array([0, 0, -1]),
-                                    value=np.array(2.3))
+    transformation = Transformation(
+        transform_type, np.array([0, 0, -1]), value=np.array(2.3)
+    )
     builder.add_component(component_class(component_name, depends_on=transformation))
     with pytest.warns(UserWarning):
         load_function(builder)
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
 def test_loads_component_position_from_multiple_transformations(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        load_function: Callable):
-    builder = NexusBuilder()
-    transformation_1 = Transformation(TransformationType.ROTATION,
-                                      np.array([0, 1, 0]),
-                                      value=np.array(90),
-                                      value_units="deg")
-    transformation_2 = Transformation(TransformationType.TRANSLATION,
-                                      np.array([0, 0, 1]),
-                                      value=np.array(2.3),
-                                      value_units="m",
-                                      depends_on=transformation_1)
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    load_function: Callable,
+):
+    builder = NexusBuilder()
+    transformation_1 = Transformation(
+        TransformationType.ROTATION,
+        np.array([0, 1, 0]),
+        value=np.array(90),
+        value_units="deg",
+    )
+    transformation_2 = Transformation(
+        TransformationType.TRANSLATION,
+        np.array([0, 0, 1]),
+        value=np.array(2.3),
+        value_units="m",
+        depends_on=transformation_1,
+    )
     builder.add_component(component_class(component_name, depends_on=transformation_2))
     loaded_data = load_function(builder)
 
     expected_position = np.array([2.3, 0, 0])
-    assert np.allclose(loaded_data[f"{component_name}_position"].values,
-                       expected_position)
+    assert np.allclose(
+        loaded_data[f"{component_name}_position"].values, expected_position
+    )
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit("m")
 
 
 def test_skips_source_position_if_not_given_in_file(load_function: Callable):
     builder = NexusBuilder()
     builder.add_source(Source("source"))
     loaded_data = load_function(builder)
     assert 'source_position' not in loaded_data
 
 
-@pytest.mark.parametrize("component_class,component_name",
-                         ((Sample, "sample"), (Source, "source")))
+@pytest.mark.parametrize(
+    "component_class,component_name", ((Sample, "sample"), (Source, "source"))
+)
 def test_loads_component_position_from_distance_dataset(
-        component_class: Union[Type[Source], Type[Sample]], component_name: str,
-        load_function: Callable):
+    component_class: Union[Type[Source], Type[Sample]],
+    component_name: str,
+    load_function: Callable,
+):
     # If the NXsource or NXsample contains a "distance" dataset
     # this gives the position along the z axis. If there was a "depends_on"
     # pointing to transformations then we'd use that instead as it is
     # likely to be more accurate; it can define position and orientation in 3D.
     builder = NexusBuilder()
     distance = 4.2
     units = "m"
     builder.add_component(
-        component_class(component_name, distance=distance, distance_units=units))
+        component_class(component_name, distance=distance, distance_units=units)
+    )
     loaded_data = load_function(builder)
 
     expected_position = np.array([0, 0, distance])
-    assert np.allclose(loaded_data[f"{component_name}_position"].values,
-                       expected_position)
+    assert np.allclose(
+        loaded_data[f"{component_name}_position"].values, expected_position
+    )
     assert loaded_data[f"{component_name}_position"].unit == sc.Unit(units)
 
 
 def test_loads_source_position_dependent_on_sample_position(load_function: Callable):
     builder = NexusBuilder()
-    transformation_0 = Transformation(TransformationType.ROTATION,
-                                      np.array([0, 1, 0]),
-                                      value=np.array(90),
-                                      value_units="deg")
-    transformation_1 = Transformation(TransformationType.TRANSLATION,
-                                      np.array([0, 0, 1]),
-                                      value=np.array(2.3),
-                                      value_units="m",
-                                      depends_on=transformation_0)
+    transformation_0 = Transformation(
+        TransformationType.ROTATION,
+        np.array([0, 1, 0]),
+        value=np.array(90),
+        value_units="deg",
+    )
+    transformation_1 = Transformation(
+        TransformationType.TRANSLATION,
+        np.array([0, 0, 1]),
+        value=np.array(2.3),
+        value_units="m",
+        depends_on=transformation_0,
+    )
     builder.add_sample(Sample("sample", depends_on=transformation_1))
     transformation_2 = Transformation(
         TransformationType.TRANSLATION,
         np.array([0, 0, 1]),
         value=np.array(1.0),
         value_units="m",
-        depends_on="/entry/sample/transformations/transform_1")
+        depends_on="/entry/sample/transformations/transform_1",
+    )
     builder.add_source(Source("source", depends_on=transformation_2))
     loaded_data = load_function(builder)
 
     expected_position = np.array([3.3, 0, 0])
     assert np.allclose(loaded_data["source_position"].values, expected_position)
     assert loaded_data["source_position"].unit == sc.Unit("m")
 
 
 def test_loads_pixel_positions_with_transformations(load_function: Callable):
-    pulse_times = np.array([
-        1600766730000000000, 1600766731000000000, 1600766732000000000,
-        1600766733000000000
-    ])
+    pulse_times = np.array(
+        [
+            1600766730000000000,
+            1600766731000000000,
+            1600766732000000000,
+            1600766733000000000,
+        ]
+    )
     event_time_offsets_1 = np.array([456, 743, 347, 345, 632])
     event_data_1 = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets_1,
         event_time_zero=pulse_times,
         event_index=np.array([0, 3, 3, 5]),
     )
     detector_1_ids = np.array([0, 1, 2, 3])
     x_pixel_offset_1 = np.array([0.1, 0.2, 0.1, 0.2])
     y_pixel_offset_1 = np.array([0.1, 0.1, 0.2, 0.2])
     z_pixel_offset_1 = np.array([0.1, 0.2, 0.3, 0.4])
 
     distance = 57  # cm
-    transformation = Transformation(TransformationType.TRANSLATION,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(distance),
-                                    value_units="cm")
+    transformation = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array(distance),
+        value_units="cm",
+    )
 
     builder = NexusBuilder()
     builder.add_detector(
-        Detector(detector_1_ids,
-                 event_data_1,
-                 x_offsets=x_pixel_offset_1,
-                 y_offsets=y_pixel_offset_1,
-                 z_offsets=z_pixel_offset_1,
-                 offsets_unit="m",
-                 depends_on=transformation))
+        Detector(
+            detector_1_ids,
+            event_data_1,
+            x_offsets=x_pixel_offset_1,
+            y_offsets=y_pixel_offset_1,
+            z_offsets=z_pixel_offset_1,
+            offsets_unit="m",
+            depends_on=transformation,
+        )
+    )
 
     loaded_data = load_function(builder)
 
     expected_pixel_positions = np.array(
-        [x_pixel_offset_1, y_pixel_offset_1, z_pixel_offset_1]).T
-    assert np.allclose(loaded_data.meta['base_position'].values,
-                       expected_pixel_positions)
+        [x_pixel_offset_1, y_pixel_offset_1, z_pixel_offset_1]
+    ).T
+    assert np.allclose(
+        loaded_data.meta['base_position'].values, expected_pixel_positions
+    )
 
     expected_transform = sc.spatial.translation(unit=sc.units.m, value=[0, 0, 0.57])
 
-    assert np.allclose(loaded_data.meta['position_transformations'].value.values,
-                       expected_transform.values)
+    assert np.allclose(
+        loaded_data.meta['position_transformations'].value.values,
+        expected_transform.values,
+    )
 
     assert np.allclose(
-        (loaded_data.meta["position_transformations"].value *
-         loaded_data.meta["base_position"]["detector_id", 0]).values,
+        (
+            loaded_data.meta["position_transformations"].value
+            * loaded_data.meta["base_position"]["detector_id", 0]
+        ).values,
         [0.1, 0.1, 0.67],
     )
 
-    assert np.allclose(loaded_data.coords["position"]["detector_id", 0].values,
-                       [0.1, 0.1, 0.67])
+    assert np.allclose(
+        loaded_data.coords["position"]["detector_id", 0].values, [0.1, 0.1, 0.67]
+    )
 
 
 def test_loads_pixel_positions_with_multiple_transformations(load_function: Callable):
     event_data_1 = EventData(
         event_id=np.array([0, 0, 0, 0, 0]),
         event_time_offset=(np.array([456, 743, 347, 345, 632])),
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
     event_data_2 = EventData(
         event_id=np.array([1, 1, 1, 1, 1]),
         event_time_offset=(np.array([456, 743, 347, 345, 632])),
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
 
-    transformation1 = Transformation(TransformationType.TRANSLATION,
-                                     vector=np.array([0, 0, 1]),
-                                     value=np.array(12),
-                                     value_units="cm")
-    transformation2 = Transformation(TransformationType.TRANSLATION,
-                                     vector=np.array([0, 0, 1]),
-                                     value=np.array(34),
-                                     value_units="cm")
+    transformation1 = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array(12),
+        value_units="cm",
+    )
+    transformation2 = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array(34),
+        value_units="cm",
+    )
 
     builder = NexusBuilder()
     builder.add_detector(
-        Detector(np.array([0]),
-                 event_data_1,
-                 x_offsets=np.array([0.1]),
-                 y_offsets=np.array([0.1]),
-                 z_offsets=np.array([0.1]),
-                 offsets_unit="m",
-                 depends_on=transformation1))
+        Detector(
+            np.array([0]),
+            event_data_1,
+            x_offsets=np.array([0.1]),
+            y_offsets=np.array([0.1]),
+            z_offsets=np.array([0.1]),
+            offsets_unit="m",
+            depends_on=transformation1,
+        )
+    )
 
     builder.add_detector(
-        Detector(np.array([1]),
-                 event_data_2,
-                 x_offsets=np.array([0.6]),
-                 y_offsets=np.array([0.6]),
-                 z_offsets=np.array([0.6]),
-                 offsets_unit="m",
-                 depends_on=transformation2))
+        Detector(
+            np.array([1]),
+            event_data_2,
+            x_offsets=np.array([0.6]),
+            y_offsets=np.array([0.6]),
+            z_offsets=np.array([0.6]),
+            offsets_unit="m",
+            depends_on=transformation2,
+        )
+    )
 
     loaded_data = load_function(builder)
 
     assert np.allclose(
-        (loaded_data.meta["position_transformations"]["detector_id", 0].value *
-         loaded_data.meta["base_position"]["detector_id", 0]).values,
+        (
+            loaded_data.meta["position_transformations"]["detector_id", 0].value
+            * loaded_data.meta["base_position"]["detector_id", 0]
+        ).values,
         [0.1, 0.1, 0.1 + 0.12],
     )
     assert np.allclose(
-        (loaded_data.meta["position_transformations"]["detector_id", 1].value *
-         loaded_data.meta["base_position"]["detector_id", 1]).values,
+        (
+            loaded_data.meta["position_transformations"]["detector_id", 1].value
+            * loaded_data.meta["base_position"]["detector_id", 1]
+        ).values,
         [0.6, 0.6, 0.6 + 0.34],
     )
 
 
 def test_links_to_event_data_group_are_ignored(load_function: Callable):
     event_time_offsets = np.array([456, 743, 347, 345, 632])
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets,
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
 
     builder = NexusBuilder()
     builder.add_event_data(event_data)
     builder.add_hard_link(Link("/entry/hard_link_to_events", "/entry/events_0"))
     builder.add_soft_link(Link("/entry/soft_link_to_events", "/entry/events_0"))
@@ -1261,38 +1546,43 @@
     # dataset with no duplicate data due to the links
 
     # Expect time of flight to match the values in the
     # event_time_offset dataset
     # May be reordered due to binning (hence np.sort)
     assert np.array_equal(
         np.sort(loaded_data.bins.concat('detector_id').values[0].coords['tof'].values),
-        np.sort(event_time_offsets))
+        np.sort(event_time_offsets),
+    )
 
     counts_on_detectors = loaded_data.bins.sum()
     # No detector_number dataset in file so expect detector_id to be
     # binned according to whatever detector_ids are present in event_id
     # dataset: 2 on det 1, 1 on det 2, 2 on det 3
     expected_counts = np.array([[2], [1], [2]])
     assert np.array_equal(counts_on_detectors.data.values, expected_counts)
     expected_detector_ids = np.array([1, 2, 3])
-    assert np.array_equal(loaded_data.coords['detector_id'].values,
-                          expected_detector_ids)
+    assert np.array_equal(
+        loaded_data.coords['detector_id'].values, expected_detector_ids
+    )
 
 
 def test_links_in_transformation_paths_are_followed(load_function: Callable):
     builder = NexusBuilder()
     distance = 13.6
     builder.add_component(Source("source"))
     builder.add_dataset_at_path(
-        "/entry/transform", np.array(distance), {
+        "/entry/transform",
+        np.array(distance),
+        {
             "vector": np.array([0, 0, 1]),
             "units": "m",
             "transformation_type": "translation",
-            "depends_on": "."
-        })
+            "depends_on": ".",
+        },
+    )
     builder.add_dataset_at_path("/entry/source/depends_on", "/entry/transform_link", {})
     builder.add_soft_link(Link("/entry/transform_link", "/entry/transform"))
     loaded_data = load_function(builder)
 
     assert np.allclose(loaded_data["source_position"].values, [0, 0, distance])
     # Resulting position will always be in metres, whatever units are
     # used in the NeXus file
@@ -1300,44 +1590,54 @@
 
 
 def test_relative_links_in_transformation_paths_are_followed(load_function: Callable):
     builder = NexusBuilder()
     distance = 13.6
     builder.add_component(Source("source"))
     builder.add_dataset_at_path(
-        "/entry/transform1", np.array(distance), {
+        "/entry/transform1",
+        np.array(distance),
+        {
             "vector": np.array([0, 0, 1]),
             "units": "m",
             "transformation_type": "translation",
-            "depends_on": "."
-        })
+            "depends_on": ".",
+        },
+    )
     builder.add_dataset_at_path(
-        "/entry/transform2", np.array(distance), {
+        "/entry/transform2",
+        np.array(distance),
+        {
             "vector": np.array([0, 0, 1]),
             "units": "m",
             "transformation_type": "translation",
-            "depends_on": "transform1"
-        })
+            "depends_on": "transform1",
+        },
+    )
     builder.add_dataset_at_path("/entry/source/depends_on", "/entry/transform2", {})
     loaded_data = load_function(builder)
 
     assert np.allclose(loaded_data["source_position"].values, [0, 0, 2 * distance])
     # Resulting position will always be in metres, whatever units are
     # used in the NeXus file
     assert loaded_data["source_position"].unit == sc.Unit("m")
 
 
 def test_linked_datasets_are_found(load_function: Callable):
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=np.array([456, 743, 347, 345, 632]),
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
 
     builder = NexusBuilder()
     builder.add_event_data(event_data)
     replaced_ids = np.array([1, 1, 1, 2, 3])
     builder.add_dataset_at_path("/entry/ids", replaced_ids, {})
@@ -1348,60 +1648,68 @@
     builder.add_hard_link(Link("/entry/events_0/event_id", "/entry/ids"))
     builder.add_soft_link(Link("/entry/events_0/event_time_offset", "/entry/tofs"))
 
     loaded_data = load_function(builder)
 
     assert np.array_equal(
         np.sort(loaded_data.bins.concat('detector_id').values[0].coords['tof'].values),
-        np.sort(replaced_tofs))
+        np.sort(replaced_tofs),
+    )
 
     counts_on_detectors = loaded_data.bins.sum()
     expected_counts = np.array([[3], [1], [1]])
     assert np.array_equal(counts_on_detectors.data.values, expected_counts)
     expected_detector_ids = np.array([1, 2, 3])
-    assert np.array_equal(loaded_data.coords['detector_id'].values,
-                          expected_detector_ids)
+    assert np.array_equal(
+        loaded_data.coords['detector_id'].values, expected_detector_ids
+    )
 
 
 def test_loads_sample_ub_matrix(load_function: Callable):
     builder = NexusBuilder()
     builder.add_component(Sample("sample", ub_matrix=np.ones(shape=[3, 3])))
     loaded_data = load_function(builder)
     sample = loaded_data['sample'].value
     assert sc.identical(
         sample['ub_matrix'],
-        sc.spatial.linear_transform(value=np.ones(shape=[3, 3]),
-                                    unit=sc.units.angstrom**-1))
+        sc.spatial.linear_transform(
+            value=np.ones(shape=[3, 3]), unit=sc.units.angstrom**-1
+        ),
+    )
     assert "orientation_matrix" not in sample
 
 
 def test_loads_sample_orientation_matrix(load_function: Callable):
     builder = NexusBuilder()
     builder.add_component(Sample("sample", orientation_matrix=np.ones(shape=[3, 3])))
     loaded_data = load_function(builder)
     sample = loaded_data['sample'].value
     assert sc.identical(
         sample["orientation_matrix"],
-        sc.spatial.linear_transform(value=np.ones(shape=[3, 3]), unit=sc.units.one))
+        sc.spatial.linear_transform(value=np.ones(shape=[3, 3]), unit=sc.units.one),
+    )
     assert "ub_matrix" not in sample
 
 
 def test_loads_multiple_sample_ub_matrix(load_function: Callable):
     builder = NexusBuilder()
     builder.add_component(Sample("sample1", ub_matrix=np.ones(shape=[3, 3])))
     builder.add_component(Sample("sample2", ub_matrix=np.identity(3)))
     builder.add_component(Sample("sample3"))  # No ub specified
     loaded_data = load_function(builder)
     assert sc.identical(
         loaded_data["sample1"].value["ub_matrix"],
-        sc.spatial.linear_transform(value=np.ones(shape=[3, 3]),
-                                    unit=sc.units.angstrom**-1))
+        sc.spatial.linear_transform(
+            value=np.ones(shape=[3, 3]), unit=sc.units.angstrom**-1
+        ),
+    )
     assert sc.identical(
         loaded_data["sample2"].value["ub_matrix"],
-        sc.spatial.linear_transform(value=np.identity(3), unit=sc.units.angstrom**-1))
+        sc.spatial.linear_transform(value=np.identity(3), unit=sc.units.angstrom**-1),
+    )
     assert "ub_matrix" not in loaded_data['sample3'].value
 
 
 def test_warning_but_no_error_for_unrecognised_log_unit(load_function: Callable):
     values = np.array([1.1, 2.2, 3.3])
     times = np.array([4.4, 5.5, 6.6])
     name = "test_log"
@@ -1419,189 +1727,235 @@
 def test_start_and_end_times_appear_in_dataset_if_set(load_function: Callable):
     builder = NexusBuilder()
     builder.add_run_start_time("2001-01-01T00:00:00")
     builder.add_run_end_time("2002-02-02T00:00:00")
 
     loaded_data = load_function(builder)
 
-    assert sc.identical(loaded_data["start_time"],
-                        sc.DataArray(sc.scalar("2001-01-01T00:00:00")))
-    assert sc.identical(loaded_data["end_time"],
-                        sc.DataArray(sc.scalar("2002-02-02T00:00:00")))
+    assert sc.identical(
+        loaded_data["start_time"], sc.DataArray(sc.scalar("2001-01-01T00:00:00"))
+    )
+    assert sc.identical(
+        loaded_data["end_time"], sc.DataArray(sc.scalar("2002-02-02T00:00:00"))
+    )
 
 
-@pytest.mark.parametrize("log_start,scaling_factor",
-                         (("2000-01-01T01:00:00", 1000), ("2000-01-01T00:00:00", 0.001),
-                          ("2010-01-01T00:00:00", None)))
+@pytest.mark.parametrize(
+    "log_start,scaling_factor",
+    (
+        ("2000-01-01T01:00:00", 1000),
+        ("2000-01-01T00:00:00", 0.001),
+        ("2010-01-01T00:00:00", None),
+    ),
+)
 def test_load_log_times(log_start: str, scaling_factor: float, load_function: Callable):
-
-    times = np.array([0., 10., 20., 30., 40., 50.], dtype="float64")
+    times = np.array([0.0, 10.0, 20.0, 30.0, 40.0, 50.0], dtype="float64")
 
     builder = NexusBuilder()
     builder.add_log(
-        Log(name="test_log",
-            value=np.zeros(shape=(len(times), )),
+        Log(
+            name="test_log",
+            value=np.zeros(shape=(len(times),)),
             time=times,
             start_time=log_start,
-            scaling_factor=scaling_factor))
+            scaling_factor=scaling_factor,
+        )
+    )
 
     loaded_data = load_function(builder)
 
     times_ns = sc.to_unit(
-        sc.array(dims=["time"],
-                 values=times * (scaling_factor or 1.0),
-                 unit=sc.units.s,
-                 dtype=sc.DType.float64), sc.units.ns).astype(sc.DType.int64)
-
-    expected = sc.scalar(value=np.datetime64(log_start),
-                         unit=sc.units.ns,
-                         dtype=sc.DType.datetime64) + times_ns
+        sc.array(
+            dims=["time"],
+            values=times * (scaling_factor or 1.0),
+            unit=sc.units.s,
+            dtype=sc.DType.float64,
+        ),
+        sc.units.ns,
+    ).astype(sc.DType.int64)
+
+    expected = (
+        sc.scalar(
+            value=np.datetime64(log_start), unit=sc.units.ns, dtype=sc.DType.datetime64
+        )
+        + times_ns
+    )
 
     actual = loaded_data["test_log"].values.coords['time']
 
     diffs = np.abs(actual.values - expected.values)
 
     # Allow 1ns difference for rounding errors between different routes
     assert all(diffs <= np.array(1).astype("timedelta64[ns]"))
 
 
 def test_load_log_times_when_logs_do_not_have_start_time(load_function: Callable):
     # If an NXLog doesn't have a start time attribute then 1970-01-01 should be
     # assumed instead
 
-    times = np.array([-10., 0., 10., 20., 30., 40., 50.], dtype="float64")
+    times = np.array([-10.0, 0.0, 10.0, 20.0, 30.0, 40.0, 50.0], dtype="float64")
 
     builder = NexusBuilder()
     builder.add_log(
-        Log(name="test_log",
-            value=np.zeros(shape=(len(times), )),
+        Log(
+            name="test_log",
+            value=np.zeros(shape=(len(times),)),
             time=times,
-            start_time=None))
+            start_time=None,
+        )
+    )
 
     loaded_data = load_function(builder)
 
     times_ns = sc.to_unit(
         sc.array(dims=["time"], values=times, unit=sc.units.s, dtype=sc.DType.float64),
-        sc.units.ns).astype(sc.DType.int64)
+        sc.units.ns,
+    ).astype(sc.DType.int64)
 
-    expected = sc.scalar(value=np.datetime64("1970-01-01T00:00:00"),
-                         unit=sc.units.ns,
-                         dtype=sc.DType.datetime64) + times_ns
+    expected = (
+        sc.scalar(
+            value=np.datetime64("1970-01-01T00:00:00"),
+            unit=sc.units.ns,
+            dtype=sc.DType.datetime64,
+        )
+        + times_ns
+    )
 
     actual = loaded_data["test_log"].values.coords['time']
 
     diffs = np.abs(actual.values - expected.values)
 
     # Allow 1ns difference for rounding errors between different routes
     assert all(diffs <= np.array(1).astype("timedelta64[ns]"))
 
 
 @pytest.mark.parametrize("units", ("ps", "ns", "us", "ms", "s", "minute", "hour"))
 def test_adjust_log_times_with_different_time_units(units, load_function: Callable):
-
     times = [1, 2, 3]
 
     builder = NexusBuilder()
     builder.add_log(
-        Log(name="test_log",
-            value=np.zeros(shape=(len(times), )),
+        Log(
+            name="test_log",
+            value=np.zeros(shape=(len(times),)),
             time=np.array(times, dtype="float64"),
             time_units=units,
-            start_time="2000-01-01T00:00:00"), )
+            start_time="2000-01-01T00:00:00",
+        ),
+    )
 
     loaded_data = load_function(builder)
 
     times_ns = sc.to_unit(
         sc.array(dims=["time"], values=times, unit=units, dtype=sc.DType.int64),
-        sc.units.ns)
+        sc.units.ns,
+    )
 
-    expected = sc.scalar(value=np.datetime64("2000-01-01T00:00:00"),
-                         unit=sc.units.ns,
-                         dtype=sc.DType.datetime64) + times_ns
+    expected = (
+        sc.scalar(
+            value=np.datetime64("2000-01-01T00:00:00"),
+            unit=sc.units.ns,
+            dtype=sc.DType.datetime64,
+        )
+        + times_ns
+    )
 
     actual = loaded_data["test_log"].values.coords['time']
 
     diffs = np.abs(actual.values - expected.values)
 
     # Allow 1ns difference for rounding errors between different routes
     assert all(diffs <= np.array(1).astype("timedelta64[ns]"))
 
 
 def test_nexus_file_with_invalid_nxlog_time_units_loads_dataset_as_non_datetime(
-        load_function: Callable):
+    load_function: Callable,
+):
     builder = NexusBuilder()
     builder.add_log(
         Log(
             name="test_log_1",
-            value=np.zeros(shape=(1, )),
+            value=np.zeros(shape=(1,)),
             time=np.array([1.0]),
             time_units="m",  # Time in metres, should fail.
-            start_time="1970-01-01T00:00:00"))
+            start_time="1970-01-01T00:00:00",
+        )
+    )
 
     loaded_data = load_function(builder)
     assert loaded_data['test_log_1'].value.coords['time'].dtype == sc.DType('float64')
     assert loaded_data['test_log_1'].value.coords['time'].unit == 'm'
 
 
 def test_nexus_file_with_invalid_log_start_date_uses_epoch(load_function: Callable):
     builder = NexusBuilder()
     builder.add_log(
-        Log(name="test_log_1",
-            value=np.zeros(shape=(1, )),
+        Log(
+            name="test_log_1",
+            value=np.zeros(shape=(1,)),
             time=np.array([1]),
-            start_time="this_isnt_a_valid_log_start_time"))
+            start_time="this_isnt_a_valid_log_start_time",
+        )
+    )
     builder.add_log(
-        Log(name="test_log_2",
-            value=np.zeros(shape=(1, )),
+        Log(
+            name="test_log_2",
+            value=np.zeros(shape=(1,)),
             time=np.array([1]),
-            start_time="1970-01-01T00:00:00"))
+            start_time="1970-01-01T00:00:00",
+        )
+    )
 
     loaded_data = load_function(builder)
     assert sc.identical(
         loaded_data['test_log_1'].value.coords['time'],
-        sc.epoch(unit='s') +
-        sc.array(dims=['time'], values=[1], unit='s', dtype='int64'))
+        sc.epoch(unit='s')
+        + sc.array(dims=['time'], values=[1], unit='s', dtype='int64'),
+    )
 
 
 def test_extended_ascii_in_ascii_encoded_dataset(load_function: Callable):
     if load_function == load_from_json:
         pytest.skip("JSON serialiser can only serialize strings, not bytes.")
 
     builder = NexusBuilder()
     # When writing, if we use bytes h5py will write as ascii encoding
     # 0xb0 = degrees symbol in latin-1 encoding.
-    builder.add_title(b"run at rot=90" + bytes([0xb0]))
+    builder.add_title(b"run at rot=90" + bytes([0xB0]))
 
     with pytest.warns(UserWarning, match="contains characters in extended ascii range"):
         loaded_data = load_function(builder)
 
-        assert sc.identical(loaded_data["experiment_title"],
-                            sc.DataArray(data=sc.scalar("run at rot=90°")))
+        assert sc.identical(
+            loaded_data["experiment_title"],
+            sc.DataArray(data=sc.scalar("run at rot=90°")),
+        )
 
 
 @pytest.mark.parametrize("test_string", UTF8_TEST_STRINGS)
 def test_utf8_encoded_dataset(load_function: Callable, test_string):
     builder = NexusBuilder()
     # When writing, if we use str h5py will write as utf8 encoding
     builder.add_title(test_string)
 
     loaded_data = load_function(builder)
 
-    assert sc.identical(loaded_data["experiment_title"],
-                        sc.DataArray(data=sc.scalar(test_string)))
+    assert sc.identical(
+        loaded_data["experiment_title"], sc.DataArray(data=sc.scalar(test_string))
+    )
 
 
 def test_extended_ascii_in_ascii_encoded_attribute(load_function: Callable):
     if load_function == load_from_json:
         pytest.skip("JSON serialiser can only serialize strings, not bytes.")
 
     builder = NexusBuilder()
     # When writing, if we use bytes h5py will write as ascii encoding
     # 0xb0 = degrees symbol in latin-1 encoding.
-    builder.add_log(Log(name="testlog", value_units=bytes([0xb0]), value=np.array([0])))
+    builder.add_log(Log(name="testlog", value_units=bytes([0xB0]), value=np.array([0])))
 
     with pytest.warns(UserWarning, match="contains characters in extended ascii range"):
         loaded_data = load_function(builder)
 
         assert loaded_data["testlog"].data.values.unit == sc.units.deg
 
 
@@ -1617,69 +1971,87 @@
 
 
 def test_load_nexus_adds_single_tof_bin(load_function: Callable):
     event_time_offsets = np.array([456, 743, 347, 345, 632], dtype="float64")
     event_data = EventData(
         event_id=np.array([1, 2, 3, 1, 3]),
         event_time_offset=event_time_offsets,
-        event_time_zero=np.array([
-            1600766730000000000, 1600766731000000000, 1600766732000000000,
-            1600766733000000000
-        ]),
+        event_time_zero=np.array(
+            [
+                1600766730000000000,
+                1600766731000000000,
+                1600766732000000000,
+                1600766733000000000,
+            ]
+        ),
         event_index=np.array([0, 3, 3, 5]),
     )
 
     builder = NexusBuilder()
     builder.add_event_data(event_data)
 
     loaded_data = load_function(builder)
 
     # Size 2 for each of the two bin edges around a single bin
-    assert loaded_data.coords["tof"].shape == (2, )
+    assert loaded_data.coords["tof"].shape == (2,)
 
     # Assert bin edges correspond to smallest and largest+1 time-of-flights
     # in data.
-    assert sc.identical(loaded_data.coords["tof"]["tof", 0],
-                        sc.scalar(value=np.min(event_time_offsets), unit=sc.units.ns))
+    assert sc.identical(
+        loaded_data.coords["tof"]["tof", 0],
+        sc.scalar(value=np.min(event_time_offsets), unit=sc.units.ns),
+    )
     assert sc.identical(
         loaded_data.coords["tof"]["tof", 1],
-        sc.scalar(value=np.nextafter(np.max(event_time_offsets), float("inf")),
-                  unit=sc.units.ns))
+        sc.scalar(
+            value=np.nextafter(np.max(event_time_offsets), float("inf")),
+            unit=sc.units.ns,
+        ),
+    )
 
 
 def test_nexus_file_with_choppers(load_function: Callable):
     builder = NexusBuilder()
     builder.add_instrument("dummy")
     builder.add_chopper(
-        Chopper("chopper_1",
-                distance=10.0,
-                rotation_speed=60.0,
-                rotation_units="Hz",
-                distance_units="m"))
+        Chopper(
+            "chopper_1",
+            distance=10.0,
+            rotation_speed=60.0,
+            rotation_units="Hz",
+            distance_units="m",
+        )
+    )
     loaded_data = load_function(builder)
     chopper = loaded_data['chopper_1'].value
     assert sc.identical(chopper["rotation_speed"], 60.0 * sc.Unit("Hz"))
     assert sc.identical(chopper["distance"], 10.0 * sc.Unit("m"))
 
 
 def test_nexus_file_with_two_choppers(load_function: Callable):
     builder = NexusBuilder()
     builder.add_instrument("dummy")
     builder.add_chopper(
-        Chopper("chopper_1",
-                distance=11.0 * 1000,
-                rotation_speed=65.0 / 1000,
-                rotation_units="MHz",
-                distance_units="mm"))
+        Chopper(
+            "chopper_1",
+            distance=11.0 * 1000,
+            rotation_speed=65.0 / 1000,
+            rotation_units="MHz",
+            distance_units="mm",
+        )
+    )
     builder.add_chopper(
-        Chopper("chopper_2",
-                distance=10.0,
-                rotation_speed=60.0,
-                rotation_units="Hz",
-                distance_units="m"))
+        Chopper(
+            "chopper_2",
+            distance=10.0,
+            rotation_speed=60.0,
+            rotation_units="Hz",
+            distance_units="m",
+        )
+    )
     loaded_data = load_function(builder)
     chopper1 = loaded_data['chopper_1'].value
     chopper2 = loaded_data['chopper_2'].value
     assert sc.identical(chopper1["rotation_speed"], (65.0 / 1000) * sc.Unit("MHz"))
     assert sc.identical(chopper1["distance"], (11.0 * 1000) * sc.Unit("mm"))
     assert sc.identical(chopper2["rotation_speed"], 60.0 * sc.Unit("Hz"))
     assert sc.identical(chopper2["distance"], 10.0 * sc.Unit("m"))
@@ -1694,129 +2066,157 @@
             name="monitor1",
             data=np.ones(shape=(2, 4, 6), dtype="float64"),
             axes=[
                 ("event_index", np.arange(3, 5, dtype="float64")),
                 ("period_index", np.arange(3, 7, dtype="float64")),
                 ("time_of_flight", np.arange(3, 9, dtype="float64")),
             ],
-        ))
+        )
+    )
 
     # Monitor with only one "axis" and only one data item
     builder.add_monitor(
-        Monitor("monitor2",
-                data=np.array([1.]),
-                axes=[("time_of_flight", np.array([1.]))]))
+        Monitor(
+            "monitor2", data=np.array([1.0]), axes=[("time_of_flight", np.array([1.0]))]
+        )
+    )
 
     assert sc.identical(
         load_function(builder)["monitor1"].data.values,
-        sc.DataArray(data=sc.ones(
-            dims=["event_index", "period_index", "time_of_flight"],
-            shape=(2, 4, 6),
-            dtype=sc.DType.float64),
-                     coords={
-                         "event_index":
-                         sc.Variable(dims=["event_index"],
-                                     values=np.arange(3, 5, dtype="float64")),
-                         "period_index":
-                         sc.Variable(dims=["period_index"],
-                                     values=np.arange(3, 7, dtype="float64")),
-                         "time_of_flight":
-                         sc.Variable(dims=["time_of_flight"],
-                                     values=np.arange(3, 9, dtype="float64")),
-                     }))
+        sc.DataArray(
+            data=sc.ones(
+                dims=["event_index", "period_index", "time_of_flight"],
+                shape=(2, 4, 6),
+                dtype=sc.DType.float64,
+            ),
+            coords={
+                "event_index": sc.Variable(
+                    dims=["event_index"], values=np.arange(3, 5, dtype="float64")
+                ),
+                "period_index": sc.Variable(
+                    dims=["period_index"], values=np.arange(3, 7, dtype="float64")
+                ),
+                "time_of_flight": sc.Variable(
+                    dims=["time_of_flight"], values=np.arange(3, 9, dtype="float64")
+                ),
+            },
+        ),
+    )
 
     assert sc.identical(
         load_function(builder)["monitor2"].data.values,
-        sc.DataArray(data=sc.ones(dims=["time_of_flight"], shape=(1, )),
-                     coords={
-                         "time_of_flight":
-                         sc.Variable(dims=["time_of_flight"], values=np.array([1.])),
-                     }))
+        sc.DataArray(
+            data=sc.ones(dims=["time_of_flight"], shape=(1,)),
+            coords={
+                "time_of_flight": sc.Variable(
+                    dims=["time_of_flight"], values=np.array([1.0])
+                ),
+            },
+        ),
+    )
 
 
 def test_load_monitors_with_event_mode_data(load_function: Callable):
     builder = NexusBuilder()
 
     # Monitor with data
     builder.add_monitor(
-        Monitor(name="monitor1",
-                data=np.ones(shape=(2, 3, 4), dtype="float64"),
-                axes=[
-                    ("event_index", np.array([0, 5], dtype="int64")),
-                    ("period_index", np.array([2, 3, 4], dtype="int64")),
-                    ("time_of_flight", np.array([3, 4, 5, 6], dtype="float64")),
-                ],
-                events=EventData(
-                    event_id=np.array([0, 0, 0, 0, 0], dtype="int64"),
-                    event_time_offset=np.array([1, 2, 3, 4, 5], dtype="float64"),
-                    event_time_zero=np.array([0, 1], dtype="float64"),
-                    event_index=np.array([0, 5], dtype="int64"),
-                )))
+        Monitor(
+            name="monitor1",
+            data=np.ones(shape=(2, 3, 4), dtype="float64"),
+            axes=[
+                ("event_index", np.array([0, 5], dtype="int64")),
+                ("period_index", np.array([2, 3, 4], dtype="int64")),
+                ("time_of_flight", np.array([3, 4, 5, 6], dtype="float64")),
+            ],
+            events=EventData(
+                event_id=np.array([0, 0, 0, 0, 0], dtype="int64"),
+                event_time_offset=np.array([1, 2, 3, 4, 5], dtype="float64"),
+                event_time_zero=np.array([0, 1], dtype="float64"),
+                event_index=np.array([0, 5], dtype="int64"),
+            ),
+        )
+    )
 
     # Monitor with only one "axis" and only one data item
     builder.add_monitor(
-        Monitor("monitor2",
-                data=np.array([1.], dtype="float64"),
-                axes=[("time_of_flight", np.array([1.], dtype="float64"))],
-                events=EventData(
-                    event_id=np.array([1, 1, 1, 1, 1], dtype="int64"),
-                    event_time_offset=np.array([6, 7, 8, 9, 10], dtype="float64"),
-                    event_time_zero=np.array([0, 1], dtype="float64"),
-                    event_index=np.array([0, 5], dtype="int64"),
-                )))
+        Monitor(
+            "monitor2",
+            data=np.array([1.0], dtype="float64"),
+            axes=[("time_of_flight", np.array([1.0], dtype="float64"))],
+            events=EventData(
+                event_id=np.array([1, 1, 1, 1, 1], dtype="int64"),
+                event_time_offset=np.array([6, 7, 8, 9, 10], dtype="float64"),
+                event_time_zero=np.array([0, 1], dtype="float64"),
+                event_index=np.array([0, 5], dtype="int64"),
+            ),
+        )
+    )
 
     with warnings.catch_warnings():
-        warnings.filterwarnings("ignore",
-                                message='Failed to load',
-                                category=UserWarning)
+        warnings.filterwarnings(
+            "ignore", message='Failed to load', category=UserWarning
+        )
         warnings.filterwarnings("ignore", message='Skipped load', category=UserWarning)
         mon_1_events = load_function(builder)["monitor1"].data.values
         mon_2_events = load_function(builder)["monitor2"].data.values
 
     # Monitor 1 is too ambiguous for scippnexus to handle it
     assert isinstance(mon_1_events, sc.DataGroup)
     assert sc.identical(
         mon_1_events["event_time_offset"],
-        sc.array(dims=["event"],
-                 values=[1, 2, 3, 4, 5],
-                 unit=sc.units.ns,
-                 dtype=sc.DType.float64))
+        sc.array(
+            dims=["event"],
+            values=[1, 2, 3, 4, 5],
+            unit=sc.units.ns,
+            dtype=sc.DType.float64,
+        ),
+    )
     assert sc.identical(
         mon_2_events.values[0].coords["tof"],
-        sc.array(dims=["event"],
-                 values=[6, 7, 8, 9, 10],
-                 unit=sc.units.ns,
-                 dtype=sc.DType.float64))
+        sc.array(
+            dims=["event"],
+            values=[6, 7, 8, 9, 10],
+            unit=sc.units.ns,
+            dtype=sc.DType.float64,
+        ),
+    )
 
 
 def test_load_monitor_with_transformation(load_function: Callable):
     builder = NexusBuilder()
 
-    transformation = Transformation(TransformationType.TRANSLATION,
-                                    vector=np.array([0, 0, 1]),
-                                    value=np.array(6.5),
-                                    value_units='m',
-                                    offset=[1, 2, 3],
-                                    offset_unit='m')
+    transformation = Transformation(
+        TransformationType.TRANSLATION,
+        vector=np.array([0, 0, 1]),
+        value=np.array(6.5),
+        value_units='m',
+        offset=[1, 2, 3],
+        offset_unit='m',
+    )
 
     # Monitor with data and transformation
     builder.add_monitor(
-        Monitor(name="monitor1",
-                data=np.ones(shape=(2, 4, 6), dtype="float64"),
-                axes=[
-                    ("event_index", np.arange(3, 5, dtype="float64")),
-                    ("period_index", np.arange(3, 7, dtype="float64")),
-                    ("time_of_flight", np.arange(3, 9, dtype="float64")),
-                ],
-                depends_on=transformation))
+        Monitor(
+            name="monitor1",
+            data=np.ones(shape=(2, 4, 6), dtype="float64"),
+            axes=[
+                ("event_index", np.arange(3, 5, dtype="float64")),
+                ("period_index", np.arange(3, 7, dtype="float64")),
+                ("time_of_flight", np.arange(3, 9, dtype="float64")),
+            ],
+            depends_on=transformation,
+        )
+    )
 
     loaded = load_function(builder)["monitor1"].data.values
 
-    assert sc.identical(loaded.coords["position"],
-                        sc.vector(value=[1., 2., 9.5], unit="m"))
+    assert sc.identical(
+        loaded.coords["position"], sc.vector(value=[1.0, 2.0, 9.5], unit="m")
+    )
 
 
 def test_load_nexus_file_containing_empty_arrays(load_function: Callable):
     event_data = EventData(
         event_id=np.array([], dtype='int32'),
         event_time_offset=np.array([]),
         event_time_zero=np.array([]),
```

### Comparing `scippneutron-23.3.0/tests/load_nxdetector_test.py` & `scippneutron-23.4.0/tests/load_nxdetector_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import scipp as sc
 import scippnexus as snx
 
 
 def test_can_load_nxdetector_from_PG3():
     import scippneutron as scn
+
     with snx.File(scn.data.get_path('PG3_4844_event.nxs')) as f:
         det = f['entry/instrument/bank24']
         da = det[...]
         assert da.sizes == {'x_pixel_offset': 154, 'y_pixel_offset': 7}
         assert 'detector_number' not in da.coords
         assert da.coords['pixel_id'].sizes == da.sizes
         assert da.coords['distance'].sizes == da.sizes
```

### Comparing `scippneutron-23.3.0/tests/mantid_scipp_comparison/beamline_calculations_test.py` & `scippneutron-23.4.0/tests/mantid_scipp_comparison/beamline_calculations_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,57 +14,58 @@
     pytestmark = pytest.mark.skip('Mantid framework is unavailable')
     sapi = None
     kernel = None
 
 
 @pytest.fixture
 def in_ws():
-    ws = sapi.CreateSampleWorkspace(SourceDistanceFromSample=10.0,
-                                    BankDistanceFromSample=1.1,
-                                    BankPixelWidth=2,
-                                    NumBanks=1,
-                                    XMax=200,
-                                    StoreInADS=False)
+    ws = sapi.CreateSampleWorkspace(
+        SourceDistanceFromSample=10.0,
+        BankDistanceFromSample=1.1,
+        BankPixelWidth=2,
+        NumBanks=1,
+        XMax=200,
+        StoreInADS=False,
+    )
     return ws
 
 
 @pytest.fixture
 def in_da(in_ws):
     return scn.mantid.from_mantid(in_ws)
 
 
 def test_beamline_compute_l1(in_ws, in_da):
     out_mantid = in_ws.detectorInfo().l1() * sc.Unit('m')
     in_da = scn.mantid.from_mantid(in_ws)
     out_scipp = scn.L1(in_da)
-    assert sc.allclose(out_scipp,
-                       out_mantid,
-                       rtol=1e-15 * sc.units.one,
-                       atol=1e-15 * out_scipp.unit)
+    assert sc.allclose(
+        out_scipp, out_mantid, rtol=1e-15 * sc.units.one, atol=1e-15 * out_scipp.unit
+    )
 
 
 def test_beamline_compute_l2(in_ws, in_da):
     out_mantid = sc.array(
         dims=['spectrum'],
         unit='m',
-        values=[in_ws.detectorInfo().l2(i) for i in range(in_ws.detectorInfo().size())])
+        values=[in_ws.detectorInfo().l2(i) for i in range(in_ws.detectorInfo().size())],
+    )
     in_da = scn.mantid.from_mantid(in_ws)
     out_scipp = scn.L2(in_da)
-    assert sc.allclose(out_scipp,
-                       out_mantid,
-                       rtol=1e-15 * sc.units.one,
-                       atol=1e-15 * out_scipp.unit)
+    assert sc.allclose(
+        out_scipp, out_mantid, rtol=1e-15 * sc.units.one, atol=1e-15 * out_scipp.unit
+    )
 
 
 def test_beamline_compute_two_theta(in_ws, in_da):
-    out_mantid = sc.array(dims=['spectrum'],
-                          unit='rad',
-                          values=[
-                              in_ws.detectorInfo().twoTheta(i)
-                              for i in range(in_ws.detectorInfo().size())
-                          ])
+    out_mantid = sc.array(
+        dims=['spectrum'],
+        unit='rad',
+        values=[
+            in_ws.detectorInfo().twoTheta(i) for i in range(in_ws.detectorInfo().size())
+        ],
+    )
     in_da = scn.mantid.from_mantid(in_ws)
     out_scipp = scn.two_theta(in_da)
-    assert sc.allclose(out_scipp,
-                       out_mantid,
-                       rtol=1e-13 * sc.units.one,
-                       atol=1e-13 * out_scipp.unit)
+    assert sc.allclose(
+        out_scipp, out_mantid, rtol=1e-13 * sc.units.one, atol=1e-13 * out_scipp.unit
+    )
```

### Comparing `scippneutron-23.3.0/tests/mantid_scipp_comparison/histogram_events_test.py` & `scippneutron-23.4.0/tests/mantid_scipp_comparison/histogram_events_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 
 @pytest.fixture
 def in_da(in_ws):
     return scn.mantid.from_mantid(in_ws).astype('float64')
 
 
 def test_histogram_events(in_ws, in_da):
-    out_ws = sapi.Rebin(InputWorkspace=in_ws,
-                        Params=[0, 10, 1000],
-                        PreserveEvents=False,
-                        StoreInADS=False)
+    out_ws = sapi.Rebin(
+        InputWorkspace=in_ws,
+        Params=[0, 10, 1000],
+        PreserveEvents=False,
+        StoreInADS=False,
+    )
     out_mantid = scn.mantid.from_mantid(out_ws)
     out_scipp = in_da.hist(
-        tof=sc.linspace('tof', 0, 1000, num=101, dtype='float64', unit='us'))
+        tof=sc.linspace('tof', 0, 1000, num=101, dtype='float64', unit='us')
+    )
     assert sc.utils.comparison.isnear(out_scipp, out_mantid, rtol=1e-15 * sc.units.one)
```

### Comparing `scippneutron-23.3.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py` & `scippneutron-23.4.0/tests/mantid_scipp_comparison/neutron_convert_units_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,79 +20,93 @@
 
 def mantid_coord(scipp_coord: str) -> str:
     return {
         'tof': 'TOF',
         'wavelength': 'Wavelength',
         'dspacing': 'dSpacing',
         'energy': 'Energy',
-        'energy_transfer': 'DeltaE'
+        'energy_transfer': 'DeltaE',
     }[scipp_coord]
 
 
-def make_workspace(coord: str,
-                   emode: str = 'Elastic',
-                   efixed: Optional[sc.Variable] = None) -> 'sapi.Workspace':
+def make_workspace(
+    coord: str, emode: str = 'Elastic', efixed: Optional[sc.Variable] = None
+) -> 'sapi.Workspace':
     ws = sapi.CreateSampleWorkspace(XMin=1000, NumBanks=1, StoreInADS=False)
     # Crop out spectra index 0 as has two_theta=0, gives inf d-spacing
     ws = sapi.CropWorkspace(ws, StartWorkspaceIndex=1, StoreInADS=False)
-    ws = sapi.ConvertUnits(InputWorkspace=ws,
-                           Target=mantid_coord(coord),
-                           EMode=emode,
-                           EFixed=efixed.value if efixed is not None else None,
-                           StoreInADS=False)  # start in origin units
-    ws.mutableRun().addProperty('deltaE-mode',
-                                kernel.StringPropertyWithValue('deltaE-mode', emode),
-                                '', True)
+    ws = sapi.ConvertUnits(
+        InputWorkspace=ws,
+        Target=mantid_coord(coord),
+        EMode=emode,
+        EFixed=efixed.value if efixed is not None else None,
+        StoreInADS=False,
+    )  # start in origin units
+    ws.mutableRun().addProperty(
+        'deltaE-mode', kernel.StringPropertyWithValue('deltaE-mode', emode), '', True
+    )
     if efixed is not None:
-        ws.mutableRun().addProperty('Ei',
-                                    kernel.FloatPropertyWithValue('Ei', efixed.value),
-                                    str(efixed.unit), False)
+        ws.mutableRun().addProperty(
+            'Ei',
+            kernel.FloatPropertyWithValue('Ei', efixed.value),
+            str(efixed.unit),
+            False,
+        )
     return ws
 
 
-def mantid_convert_units(ws: 'sapi.Workspace',
-                         target: str,
-                         emode: str = 'Elastic',
-                         efixed: Optional[sc.Variable] = None) -> sc.DataArray:
-    out_ws = sapi.ConvertUnits(InputWorkspace=ws,
-                               Target=mantid_coord(target),
-                               EMode=emode,
-                               EFixed=efixed.value if efixed is not None else None,
-                               StoreInADS=False)
+def mantid_convert_units(
+    ws: 'sapi.Workspace',
+    target: str,
+    emode: str = 'Elastic',
+    efixed: Optional[sc.Variable] = None,
+) -> sc.DataArray:
+    out_ws = sapi.ConvertUnits(
+        InputWorkspace=ws,
+        Target=mantid_coord(target),
+        EMode=emode,
+        EFixed=efixed.value if efixed is not None else None,
+        StoreInADS=False,
+    )
     out = scn.mantid.from_mantid(out_ws)
     # broadcast to circumvent common-bins conversion in from_mantid
     spec_shape = out.coords['spectrum'].shape
-    out.coords[target] = sc.ones(dims=['spectrum'],
-                                 shape=spec_shape) * out.coords[target]
+    out.coords[target] = (
+        sc.ones(dims=['spectrum'], shape=spec_shape) * out.coords[target]
+    )
     return out
 
 
 def test_mantid_convert_tof_to_wavelength():
     in_ws = make_workspace('tof')
     out_mantid = mantid_convert_units(in_ws, 'wavelength')
 
     in_da = scn.mantid.from_mantid(in_ws)
     out_scipp = scn.convert(data=in_da, origin='tof', target='wavelength', scatter=True)
 
-    assert sc.allclose(out_scipp.coords['wavelength'],
-                       out_mantid.coords['wavelength'],
-                       rtol=1e-8 * sc.units.one)
+    assert sc.allclose(
+        out_scipp.coords['wavelength'],
+        out_mantid.coords['wavelength'],
+        rtol=1e-8 * sc.units.one,
+    )
     assert sc.identical(out_scipp.coords['spectrum'], out_mantid.coords['spectrum'])
 
 
 def test_mantid_convert_tof_to_dspacing():
     in_ws = make_workspace('tof')
     out_mantid = mantid_convert_units(in_ws, 'dspacing')
 
     in_da = scn.mantid.from_mantid(in_ws)
     out_scipp = scn.convert(data=in_da, origin='tof', target='dspacing', scatter=True)
 
-    assert sc.allclose(out_scipp.coords['dspacing'],
-                       out_mantid.coords['dspacing'],
-                       rtol=1e-8 * sc.units.one)
+    assert sc.allclose(
+        out_scipp.coords['dspacing'],
+        out_mantid.coords['dspacing'],
+        rtol=1e-8 * sc.units.one,
+    )
     assert sc.identical(out_scipp.coords['spectrum'], out_mantid.coords['spectrum'])
 
 
 def test_mantid_convert_tof_to_energy():
     in_ws = make_workspace('tof')
     out_mantid = mantid_convert_units(in_ws, 'energy')
 
@@ -100,37 +114,40 @@
     out_scipp = scn.convert(data=in_da, origin='tof', target='energy', scatter=True)
 
     # Mantid reverses the order of the energy dim.
     mantid_energy = sc.empty_like(out_mantid.coords['energy'])
     assert mantid_energy.dims[1] == 'energy'
     mantid_energy.values = out_mantid.coords['energy'].values[..., ::-1]
 
-    assert sc.allclose(out_scipp.coords['energy'],
-                       mantid_energy,
-                       rtol=1e-7 * sc.units.one)
+    assert sc.allclose(
+        out_scipp.coords['energy'], mantid_energy, rtol=1e-7 * sc.units.one
+    )
     assert sc.identical(out_scipp.coords['spectrum'], out_mantid.coords['spectrum'])
 
 
 def test_mantid_convert_tof_to_direct_energy_transfer():
     efixed = 1000.0 * sc.Unit('meV')
     in_ws = make_workspace('tof', emode='Direct', efixed=efixed)
-    out_mantid = mantid_convert_units(in_ws,
-                                      'energy_transfer',
-                                      emode='Direct',
-                                      efixed=efixed)
+    out_mantid = mantid_convert_units(
+        in_ws, 'energy_transfer', emode='Direct', efixed=efixed
+    )
 
     in_da = scn.mantid.from_mantid(in_ws)
-    out_scipp = scn.convert(data=in_da,
-                            origin='tof',
-                            target='energy_transfer',
-                            scatter=True)
+    out_scipp = scn.convert(
+        data=in_da, origin='tof', target='energy_transfer', scatter=True
+    )
 
     # The conversion consists of multiplications and additions, thus the relative error
     # changes with the inputs. In this case, small tof yields a large error due to
     # the 1/tof**2 factor in the conversion.
     # rtol is chosen to account for linearly changing tof in the input data.
     assert sc.allclose(
         out_scipp.coords['energy_transfer'],
         out_mantid.coords['energy_transfer'],
-        rtol=sc.linspace('energy_transfer', 1e-6, 1e-10,
-                         out_scipp.coords['energy_transfer'].sizes['energy_transfer']))
+        rtol=sc.linspace(
+            'energy_transfer',
+            1e-6,
+            1e-10,
+            out_scipp.coords['energy_transfer'].sizes['energy_transfer'],
+        ),
+    )
     assert sc.identical(out_scipp.coords['spectrum'], out_mantid.coords['spectrum'])
```

### Comparing `scippneutron-23.3.0/tests/mantid_test.py` & `scippneutron-23.4.0/tests/mantid_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,180 +15,198 @@
 import scippneutron as scn
 
 from .mantid_helper import mantid_is_available
 
 
 def memory_is_at_least_gb(required):
     import psutil
+
     total = psutil.virtual_memory().total / 1e9
     return total >= required
 
 
 @pytest.mark.skipif(not memory_is_at_least_gb(4), reason='Insufficient virtual memory')
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 class TestMantidConversion(unittest.TestCase):
-
     @classmethod
     def setUpClass(cls):
         import mantid.simpleapi as mantid
 
         # This is from the Mantid system-test data
         filename = "CNCS_51936_event.nxs"
         # This needs OutputWorkspace specified, as it doesn't
         # pick up the name from the class variable name
         cls.base_event_ws = mantid.LoadEventNexus(
             scn.data.get_path(filename),
             OutputWorkspace="test_ws{}".format(__file__),
             SpectrumMax=200,
-            StoreInADS=False)
+            StoreInADS=False,
+        )
 
     def test_Workspace2D(self):
         import mantid.simpleapi as mantid
+
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000, PreserveEvents=False)
         d = scn.mantid.convert_Workspace2D_to_data_array(ws)
         assert d.attrs["run_start"].value == "2012-05-21T15:14:56.279289666"
         assert d.data.unit == sc.units.counts
         for i in range(ws.getNumberHistograms()):
             assert np.all(np.equal(d.values[i], ws.readY(i)))
             assert np.all(np.equal(d.variances[i], ws.readE(i) * ws.readE(i)))
         assert d.coords['spectrum'].dtype == sc.DType.int32
         assert d.coords['spectrum'].unit is None
         assert d.coords['tof'].dtype == sc.DType.float64
 
     def test_EventWorkspace(self):
         import mantid.simpleapi as mantid
+
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000)
 
         binned_mantid = scn.mantid.convert_Workspace2D_to_data_array(ws)
 
         target_tof = binned_mantid.coords['tof']
-        d = scn.mantid.convert_EventWorkspace_to_data_array(eventWS,
-                                                            load_pulse_times=False)
+        d = scn.mantid.convert_EventWorkspace_to_data_array(
+            eventWS, load_pulse_times=False
+        )
         histogrammed = d.hist(tof=target_tof)
 
         delta = sc.sum(binned_mantid - histogrammed, 'spectrum')
         delta = sc.sum(delta, 'tof')
         self.assertLess(np.abs(delta.value), 1e-5)
 
     def test_EventWorkspace_empty_event_list_consistent_bin_indices(self):
         import mantid.simpleapi as mantid
+
         ws = mantid.CloneWorkspace(self.base_event_ws)
         ws.getSpectrum(ws.getNumberHistograms() - 1).clear(removeDetIDs=True)
 
         da = scn.mantid.convert_EventWorkspace_to_data_array(ws, load_pulse_times=False)
         assert da.bins.size()['spectrum', -1]['tof', 0].value == 0
         da.bins.coords['tof'] = da.bins.coords['tof'].copy()
 
     def test_comparison(self):
-        a = scn.mantid.convert_EventWorkspace_to_data_array(self.base_event_ws,
-                                                            load_pulse_times=False)
+        a = scn.mantid.convert_EventWorkspace_to_data_array(
+            self.base_event_ws, load_pulse_times=False
+        )
         b = a.copy()
         assert sc.identical(a, b)
 
     def test_advanced_geometry(self):
         # basic test that positions are approximately equal for detectors for
         # CNCS given advanced and basic geometry calculation routes
         x = scn.from_mantid(self.base_event_ws, advanced_geometry=False)
         y = scn.from_mantid(self.base_event_ws, advanced_geometry=True)
         assert np.all(
-            np.isclose(x.coords['position'].values, y.coords['position'].values))
+            np.isclose(x.coords['position'].values, y.coords['position'].values)
+        )
 
     def test_advanced_geometry_with_absent_shape(self):
         import mantid.simpleapi as mantid
 
         # single bank 3 by 3
-        ws = mantid.CreateSampleWorkspace(NumBanks=1,
-                                          BankPixelWidth=3,
-                                          StoreInADS=False)
+        ws = mantid.CreateSampleWorkspace(
+            NumBanks=1, BankPixelWidth=3, StoreInADS=False
+        )
         # Save and reload trick to purge sample shape info
         file_name = "example_geometry.nxs"
         geom_path = os.path.join(tempfile.gettempdir(), file_name)
         mantid.SaveNexusGeometry(ws, geom_path)  # Does not save shape info
         assert os.path.isfile(geom_path)  # sanity check
-        out = mantid.LoadEmptyInstrument(Filename=geom_path,
-                                         StoreInADS=False)  # reload without sample info
+        out = mantid.LoadEmptyInstrument(
+            Filename=geom_path, StoreInADS=False
+        )  # reload without sample info
         os.remove(geom_path)
 
         assert not out.componentInfo().hasValidShape(0)  # sanity check
         da = scn.mantid.from_mantid(out, advanced_geometry=True)
         # Shapes have zero size
-        assert sc.identical(sc.sum(da.meta['shape']),
-                            sc.vector(value=[0, 0, 0], unit=sc.units.m))
+        assert sc.identical(
+            sc.sum(da.meta['shape']), sc.vector(value=[0, 0, 0], unit=sc.units.m)
+        )
 
     def test_advanced_geometry_detector_info(self):
         da = scn.from_mantid(self.base_event_ws, advanced_geometry=True)
         detector_info = da.coords['detector_info'].value
         assert detector_info.dim == 'detector'
         assert detector_info.coords['detector'].unit is None
         assert detector_info.coords['spectrum'].unit is None
 
     def test_EventWorkspace_no_y_unit(self):
         import mantid.simpleapi as mantid
-        tiny_event_ws = mantid.CreateSampleWorkspace(WorkspaceType='Event',
-                                                     NumBanks=1,
-                                                     NumEvents=1)
-        d = scn.mantid.convert_EventWorkspace_to_data_array(tiny_event_ws,
-                                                            load_pulse_times=False)
+
+        tiny_event_ws = mantid.CreateSampleWorkspace(
+            WorkspaceType='Event', NumBanks=1, NumEvents=1
+        )
+        d = scn.mantid.convert_EventWorkspace_to_data_array(
+            tiny_event_ws, load_pulse_times=False
+        )
         self.assertEqual(d.data.bins.constituents['data'].unit, sc.units.counts)
         tiny_event_ws.setYUnit('')
-        d = scn.mantid.convert_EventWorkspace_to_data_array(tiny_event_ws,
-                                                            load_pulse_times=False)
+        d = scn.mantid.convert_EventWorkspace_to_data_array(
+            tiny_event_ws, load_pulse_times=False
+        )
         self.assertEqual(d.data.bins.constituents['data'].unit, sc.units.one)
 
     def test_from_mantid_LoadEmptyInstrument(self):
         import mantid.simpleapi as mantid
+
         ws = mantid.LoadEmptyInstrument(InstrumentName='PG3')
         scn.from_mantid(ws)
 
     def test_from_mantid_CreateWorkspace(self):
         import mantid.simpleapi as mantid
+
         dataX = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16]
         dataY = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]
-        ws = mantid.CreateWorkspace(DataX=dataX,
-                                    DataY=dataY,
-                                    NSpec=4,
-                                    UnitX="Wavelength")
+        ws = mantid.CreateWorkspace(
+            DataX=dataX, DataY=dataY, NSpec=4, UnitX="Wavelength"
+        )
         d = scn.from_mantid(ws)
         self.assertEqual(d.data.unit, sc.units.dimensionless)
 
     def test_unit_conversion(self):
         import mantid.simpleapi as mantid
+
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000, PreserveEvents=False)
         tmp = scn.mantid.convert_Workspace2D_to_data_array(ws)
         target_tof = tmp.coords['tof']
-        ws = mantid.ConvertUnits(InputWorkspace=ws,
-                                 Target="Wavelength",
-                                 EMode="Elastic")
+        ws = mantid.ConvertUnits(
+            InputWorkspace=ws, Target="Wavelength", EMode="Elastic"
+        )
         converted_mantid = scn.mantid.convert_Workspace2D_to_data_array(ws)
 
-        da = scn.mantid.convert_EventWorkspace_to_data_array(eventWS,
-                                                             load_pulse_times=False)
+        da = scn.mantid.convert_EventWorkspace_to_data_array(
+            eventWS, load_pulse_times=False
+        )
         da = da.hist(tof=target_tof)
         d = sc.Dataset(data={da.name: da})
         converted = scn.convert(d, 'tof', 'wavelength', scatter=True)
 
         self.assertTrue(
-            np.all(np.isclose(converted_mantid.values, converted[""].values)))
+            np.all(np.isclose(converted_mantid.values, converted[""].values))
+        )
         self.assertTrue(
             np.all(
                 np.isclose(
                     converted_mantid.coords['wavelength'].values,
                     converted.coords['wavelength'].values,
-                )))
+                )
+            )
+        )
 
     def test_inelastic_unit_conversion(self):
         import mantid.simpleapi as mantid
+
         eventWS = self.base_event_ws
-        ws_deltaE = mantid.ConvertUnits(eventWS,
-                                        Target='DeltaE',
-                                        EMode='Direct',
-                                        EFixed=3)
+        ws_deltaE = mantid.ConvertUnits(
+            eventWS, Target='DeltaE', EMode='Direct', EFixed=3
+        )
         ref = scn.from_mantid(ws_deltaE)
         da = scn.from_mantid(eventWS)
         # Boost and Mantid use CODATA 2006. This test passes if we manually
         # change the implementation to use the old constants. Alternatively
         # we can correct for this by scaling L1^2 or L2^2, and this was also
         # confirmed in C++. Unfortunately only positions are accessible to
         # correct for this here, and due to precision issues with
@@ -203,214 +221,240 @@
         da.coords['source_position'] *= np.sqrt(scale)
         da.coords['position'] *= np.sqrt(scale)
         low_tof = da.bins.constituents['data'].coords['tof'] < 49000.0 * sc.units.us
         da.coords['incident_energy'] = 3.0 * sc.units.meV
         da = scn.convert(da, 'tof', 'energy_transfer', scatter=True)
         assert sc.all(
             sc.isnan(da.coords['energy_transfer'])
-            | sc.isclose(da.coords['energy_transfer'],
-                         ref.coords['energy_transfer'],
-                         atol=1e-8 * sc.units.meV,
-                         rtol=1e-8 * sc.units.one)).value
+            | sc.isclose(
+                da.coords['energy_transfer'],
+                ref.coords['energy_transfer'],
+                atol=1e-8 * sc.units.meV,
+                rtol=1e-8 * sc.units.one,
+            )
+        ).value
         assert sc.all(
             low_tof
             | sc.isnan(da.bins.constituents['data'].coords['energy_transfer'])
-            | sc.isclose(da.bins.constituents['data'].coords['energy_transfer'],
-                         ref.bins.constituents['data'].coords['energy_transfer'],
-                         atol=1e-5 * sc.units.meV,
-                         rtol=1e-5 * sc.units.one)).value
+            | sc.isclose(
+                da.bins.constituents['data'].coords['energy_transfer'],
+                ref.bins.constituents['data'].coords['energy_transfer'],
+                atol=1e-5 * sc.units.meV,
+                rtol=1e-5 * sc.units.one,
+            )
+        ).value
 
     @staticmethod
     def _mask_bins_and_spectra(ws, xmin, xmax, num_spectra, indices=None):
         import mantid.simpleapi as mantid
-        masked_ws = mantid.MaskBins(ws,
-                                    XMin=xmin,
-                                    XMax=xmax,
-                                    InputWorkspaceIndexSet=indices)
+
+        masked_ws = mantid.MaskBins(
+            ws, XMin=xmin, XMax=xmax, InputWorkspaceIndexSet=indices
+        )
 
         # mask the first 3 spectra
         for i in range(num_spectra):
             masked_ws.spectrumInfo().setMasked(i, True)
 
         return masked_ws
 
     def test_Workspace2D_common_bins_masks(self):
         import mantid.simpleapi as mantid
+
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000, PreserveEvents=False)
         ws_x = ws.readX(0)
 
         # mask the first 3 bins, range is taken as [XMin, XMax)
-        masked_ws = self._mask_bins_and_spectra(ws,
-                                                xmin=ws_x[0],
-                                                xmax=ws_x[3],
-                                                num_spectra=3)
+        masked_ws = self._mask_bins_and_spectra(
+            ws, xmin=ws_x[0], xmax=ws_x[3], num_spectra=3
+        )
 
         self.assertTrue(masked_ws.isCommonBins())
 
         ds = scn.mantid.convert_Workspace2D_to_data_array(masked_ws)
 
         np.testing.assert_array_equal(ds.masks["bin"].values[0:3], [True, True, True])
 
-        np.testing.assert_array_equal(ds.masks["spectrum"].values[0:3],
-                                      [True, True, True])
+        np.testing.assert_array_equal(
+            ds.masks["spectrum"].values[0:3], [True, True, True]
+        )
 
     def test_Workspace2D_common_bins_not_common_masks(self):
         import mantid.simpleapi as mantid
+
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000, PreserveEvents=False)
         ws_x = ws.readX(0)
 
         # mask first 3 bins in first 3 spectra, range is taken as [XMin, XMax)
-        masked_ws = self._mask_bins_and_spectra(ws,
-                                                xmin=ws_x[0],
-                                                xmax=ws_x[3],
-                                                num_spectra=3,
-                                                indices='0-2')
+        masked_ws = self._mask_bins_and_spectra(
+            ws, xmin=ws_x[0], xmax=ws_x[3], num_spectra=3, indices='0-2'
+        )
 
         self.assertTrue(masked_ws.isCommonBins())
 
         ds = scn.mantid.convert_Workspace2D_to_data_array(masked_ws)
 
         mask = sc.zeros(dims=ds.dims, shape=ds.shape, dtype=sc.DType.bool)
         mask['spectrum', 0:3]['tof', 0:3] |= sc.scalar(True)
         assert sc.identical(ds.masks['bin'], mask)
 
-        np.testing.assert_array_equal(ds.masks["spectrum"].values[0:3],
-                                      [True, True, True])
+        np.testing.assert_array_equal(
+            ds.masks["spectrum"].values[0:3], [True, True, True]
+        )
 
     def test_Workspace2D_not_common_bins_masks(self):
         import mantid.simpleapi as mantid
+
         eventWS = self.base_event_ws
         ws = mantid.Rebin(eventWS, 10000, PreserveEvents=False)
         ws = mantid.ConvertUnits(ws, "Wavelength", EMode="Direct", EFixed=0.1231)
 
         # these X values will mask different number of bins
-        masked_ws = self._mask_bins_and_spectra(ws,
-                                                -214,
-                                                -192,
-                                                num_spectra=3,
-                                                indices='0-40')
+        masked_ws = self._mask_bins_and_spectra(
+            ws, -214, -192, num_spectra=3, indices='0-40'
+        )
 
         self.assertFalse(masked_ws.isCommonBins())
 
         ds = scn.mantid.convert_Workspace2D_to_data_array(masked_ws)
 
         # bin with 3 masks
         np.testing.assert_array_equal(ds.masks["bin"].values[0], [True, True, False])
 
         # bin with only 2
         np.testing.assert_array_equal(ds.masks["bin"].values[31], [True, True, False])
 
-        np.testing.assert_array_equal(ds.masks["spectrum"].values[0:3],
-                                      [True, True, True])
+        np.testing.assert_array_equal(
+            ds.masks["spectrum"].values[0:3], [True, True, True]
+        )
 
     @staticmethod
     def check_monitor_metadata(monitor):
         assert 'position' in monitor.coords
         assert 'source_position' in monitor.coords
         assert 'sample_position' not in monitor.coords
         assert 'sample_position' in monitor.attrs
         # Absence of the following is not crucial, but currently there is
         # no need for these, and it avoids duplication:
         assert 'detector_info' not in monitor.coords
         assert 'sample' not in monitor.coords
-        assert 'SampleTemp' not in monitor.coords, \
-            "Expect run logs not be duplicated in monitor workspaces"
+        assert (
+            'SampleTemp' not in monitor.coords
+        ), "Expect run logs not be duplicated in monitor workspaces"
 
     def test_Workspace2D_with_separate_monitors(self):
         from mantid.simpleapi import mtd
+
         mtd.clear()
         # This test would use 20 GB of memory if "SpectrumMax" was not set
-        ds = scn.load(scn.data.get_path("WISH00016748.raw"),
-                      mantid_args={
-                          "LoadMonitors": "Separate",
-                          "SpectrumMax": 10000
-                      })
+        ds = scn.load(
+            scn.data.get_path("WISH00016748.raw"),
+            mantid_args={"LoadMonitors": "Separate", "SpectrumMax": 10000},
+        )
         self.assertEqual(len(mtd), 0, mtd.getObjectNames())
         attrs = [str(key) for key in ds.attrs.keys()]
         expected_monitor_attrs = {
-            "monitor1", "monitor2", "monitor3", "monitor4", "monitor5"
+            "monitor1",
+            "monitor2",
+            "monitor3",
+            "monitor4",
+            "monitor5",
         }
         assert expected_monitor_attrs.issubset(attrs)
 
         for monitor_name in expected_monitor_attrs:
             monitor = ds.attrs[monitor_name].value
             assert isinstance(monitor, sc.DataArray)
-            assert monitor.shape == (4471, )
+            assert monitor.shape == (4471,)
             self.check_monitor_metadata(monitor)
 
     def test_Workspace2D_with_include_monitors(self):
         from mantid.simpleapi import mtd
+
         mtd.clear()
         # This test would use 20 GB of memory if "SpectrumMax" was not set
-        ds = scn.load(scn.data.get_path("WISH00016748.raw"),
-                      mantid_args={
-                          "LoadMonitors": "Include",
-                          "SpectrumMax": 100
-                      })
+        ds = scn.load(
+            scn.data.get_path("WISH00016748.raw"),
+            mantid_args={"LoadMonitors": "Include", "SpectrumMax": 100},
+        )
         self.assertEqual(len(mtd), 0, mtd.getObjectNames())
         attrs = [str(key) for key in ds.attrs.keys()]
         expected_monitor_attrs = {
-            "monitor1", "monitor2", "monitor3", "monitor4", "monitor5"
+            "monitor1",
+            "monitor2",
+            "monitor3",
+            "monitor4",
+            "monitor5",
         }
         assert expected_monitor_attrs.issubset(attrs)
         for monitor_name in expected_monitor_attrs:
             monitor = ds.attrs[monitor_name].value
             assert isinstance(monitor, sc.DataArray)
-            assert monitor.shape == (4471, )
+            assert monitor.shape == (4471,)
             self.check_monitor_metadata(monitor)
 
     def test_EventWorkspace_with_monitors(self):
         from mantid.simpleapi import mtd
+
         mtd.clear()
-        ds = scn.load(scn.data.get_path("CNCS_51936_event.nxs"),
-                      mantid_args={
-                          "LoadMonitors": True,
-                          "SpectrumMax": 1
-                      })
+        ds = scn.load(
+            scn.data.get_path("CNCS_51936_event.nxs"),
+            mantid_args={"LoadMonitors": True, "SpectrumMax": 1},
+        )
         self.assertEqual(len(mtd), 0, mtd.getObjectNames())
         attrs = [str(key) for key in ds.attrs.keys()]
         expected_monitor_attrs = {"monitor2", "monitor3"}
         assert expected_monitor_attrs.issubset(attrs)
         for monitor_name in expected_monitor_attrs:
             monitor = ds.attrs[monitor_name].value
             assert isinstance(monitor, sc.DataArray)
-            assert monitor.shape == (200001, )
+            assert monitor.shape == (200001,)
             self.check_monitor_metadata(monitor)
 
     def test_mdhisto_workspace_q(self):
         from mantid.simpleapi import BinMD, CreateMDWorkspace, FakeMDEventData
 
-        md_event = CreateMDWorkspace(Dimensions=3,
-                                     Extents=[-10, 10, -10, 10, -10, 10],
-                                     Names='Q_x,Q_y,Q_z',
-                                     Units='U,U,U',
-                                     Frames='QLab,QLab,QLab',
-                                     StoreInADS=False)
-        FakeMDEventData(InputWorkspace=md_event,
-                        PeakParams=[100000, 0, 0, 0, 1],
-                        StoreInADS=False)  # Add Peak
-        md_histo = BinMD(InputWorkspace=md_event,
-                         AlignedDim0='Q_y,-10,10,3',
-                         AlignedDim1='Q_x,-10,10,4',
-                         AlignedDim2='Q_z,-10,10,5',
-                         StoreInADS=False)
+        md_event = CreateMDWorkspace(
+            Dimensions=3,
+            Extents=[-10, 10, -10, 10, -10, 10],
+            Names='Q_x,Q_y,Q_z',
+            Units='U,U,U',
+            Frames='QLab,QLab,QLab',
+            StoreInADS=False,
+        )
+        FakeMDEventData(
+            InputWorkspace=md_event, PeakParams=[100000, 0, 0, 0, 1], StoreInADS=False
+        )  # Add Peak
+        md_histo = BinMD(
+            InputWorkspace=md_event,
+            AlignedDim0='Q_y,-10,10,3',
+            AlignedDim1='Q_x,-10,10,4',
+            AlignedDim2='Q_z,-10,10,5',
+            StoreInADS=False,
+        )
 
         histo_data_array = scn.mantid.convert_MDHistoWorkspace_to_data_array(md_histo)
 
-        self.assertEqual(histo_data_array.coords['Q_x'].shape, (4, ))
-        self.assertEqual(histo_data_array.coords['Q_y'].shape, (3, ))
-        self.assertEqual(histo_data_array.coords['Q_z'].shape, (5, ))
-        self.assertEqual(histo_data_array.coords['Q_x'].unit,
-                         sc.units.dimensionless / sc.units.angstrom)
-        self.assertEqual(histo_data_array.coords['Q_y'].unit,
-                         sc.units.dimensionless / sc.units.angstrom)
-        self.assertEqual(histo_data_array.coords['Q_z'].unit,
-                         sc.units.dimensionless / sc.units.angstrom)
+        self.assertEqual(histo_data_array.coords['Q_x'].shape, (4,))
+        self.assertEqual(histo_data_array.coords['Q_y'].shape, (3,))
+        self.assertEqual(histo_data_array.coords['Q_z'].shape, (5,))
+        self.assertEqual(
+            histo_data_array.coords['Q_x'].unit,
+            sc.units.dimensionless / sc.units.angstrom,
+        )
+        self.assertEqual(
+            histo_data_array.coords['Q_y'].unit,
+            sc.units.dimensionless / sc.units.angstrom,
+        )
+        self.assertEqual(
+            histo_data_array.coords['Q_z'].unit,
+            sc.units.dimensionless / sc.units.angstrom,
+        )
 
         self.assertEqual(histo_data_array.shape, (3, 4, 5))
 
         # Sum over 2 dimensions to simplify finding max.
         max_1d = sc.sum(sc.sum(histo_data_array, dim='Q_y'), dim='Q_x').values
         max_index = np.argmax(max_1d)
         # Check position of max 'peak'
@@ -419,52 +463,63 @@
         self.assertEqual(100000, max_1d[max_index])
 
         self.assertTrue('nevents' in histo_data_array.attrs)
 
     def test_mdhisto_workspace_many_dims(self):
         from mantid.simpleapi import BinMD, CreateMDWorkspace, FakeMDEventData
 
-        md_event = CreateMDWorkspace(Dimensions=4,
-                                     Extents=[-10, 10, -10, 10, -10, 10, -10, 10],
-                                     Names='deltae,y,z,T',
-                                     Units='U,U,U,U',
-                                     StoreInADS=False)
-        FakeMDEventData(InputWorkspace=md_event,
-                        PeakParams=[100000, 0, 0, 0, 0, 1],
-                        StoreInADS=False)  # Add Peak
-        md_histo = BinMD(InputWorkspace=md_event,
-                         AlignedDim0='deltae,-10,10,3',
-                         AlignedDim1='y,-10,10,4',
-                         AlignedDim2='z,-10,10,5',
-                         AlignedDim3='T,-10,10,7',
-                         StoreInADS=False)
+        md_event = CreateMDWorkspace(
+            Dimensions=4,
+            Extents=[-10, 10, -10, 10, -10, 10, -10, 10],
+            Names='deltae,y,z,T',
+            Units='U,U,U,U',
+            StoreInADS=False,
+        )
+        FakeMDEventData(
+            InputWorkspace=md_event,
+            PeakParams=[100000, 0, 0, 0, 0, 1],
+            StoreInADS=False,
+        )  # Add Peak
+        md_histo = BinMD(
+            InputWorkspace=md_event,
+            AlignedDim0='deltae,-10,10,3',
+            AlignedDim1='y,-10,10,4',
+            AlignedDim2='z,-10,10,5',
+            AlignedDim3='T,-10,10,7',
+            StoreInADS=False,
+        )
 
         histo_data_array = scn.mantid.convert_MDHistoWorkspace_to_data_array(md_histo)
         self.assertEqual(4, len(histo_data_array.dims))
 
     def test_to_workspace_2d_no_error(self):
         from mantid.simpleapi import mtd
+
         mtd.clear()
 
         # All Dims for which support is expected are
         # tested in the parametrized test.
         # Just set this one to a working one to avoid
         # generating many repetitive tests.
         param_dim = 'tof'
         data_len = 2
         expected_bins = data_len + 1
         expected_number_spectra = 10
 
-        y = sc.Variable(dims=['spectrum', param_dim],
-                        values=np.random.rand(expected_number_spectra, data_len))
-
-        x = sc.Variable(dims=['spectrum', param_dim],
-                        values=np.arange(expected_number_spectra * expected_bins,
-                                         dtype=np.float64).reshape(
-                                             (expected_number_spectra, expected_bins)))
+        y = sc.Variable(
+            dims=['spectrum', param_dim],
+            values=np.random.rand(expected_number_spectra, data_len),
+        )
+
+        x = sc.Variable(
+            dims=['spectrum', param_dim],
+            values=np.arange(
+                expected_number_spectra * expected_bins, dtype=np.float64
+            ).reshape((expected_number_spectra, expected_bins)),
+        )
         data = sc.DataArray(data=y, coords={param_dim: x})
 
         ws = scn.to_mantid(data, param_dim)
 
         assert len(ws.readX(0)) == expected_bins
         assert ws.getNumberHistograms() == expected_number_spectra
         # check that no workspaces have been leaked in the ADS
@@ -477,150 +532,181 @@
 
     def test_fit(self):
         """
         Tests that the fit executes, and the outputs
         are moved into the dataset. Does not check the fit values.
         """
         from mantid.simpleapi import mtd
+
         mtd.clear()
 
         data = scn.load(scn.data.get_path("iris26176_graphite002_sqw.nxs"))
 
-        params, diff = scn.fit(data['Q', 0],
-                               mantid_args={
-                                   'Function': 'name=LinearBackground,A0=0,A1=1',
-                                   'StartX': 0,
-                                   'EndX': 3
-                               })
+        params, diff = scn.fit(
+            data['Q', 0],
+            mantid_args={
+                'Function': 'name=LinearBackground,A0=0,A1=1',
+                'StartX': 0,
+                'EndX': 3,
+            },
+        )
 
         # check that no workspaces have been leaked in the ADS
         assert len(mtd) == 0
         assert 'data' in diff
         assert 'calculated' in diff
         assert 'diff' in diff
         assert 'status' in params.coords
         assert 'function' in params.coords
         assert 'cost_function' in params.coords
         assert 'chi^2/d.o.f.' in params.coords
 
     def test_convert_array_run_log_to_attrs(self):
         # Given a Mantid workspace with a run log
         import mantid.simpleapi as mantid
+
         target = mantid.CloneWorkspace(self.base_event_ws)
         log_name = "SampleTemp"
-        self.assertTrue(target.run().hasProperty(log_name),
-                        f"Expected input workspace to have a {log_name} run log")
+        self.assertTrue(
+            target.run().hasProperty(log_name),
+            f"Expected input workspace to have a {log_name} run log",
+        )
 
         # When the workspace is converted to a scipp data array
         d = scn.mantid.convert_EventWorkspace_to_data_array(target, False)
 
         # Then the data array contains the run log as an unaligned coord
         self.assertTrue(
-            np.allclose(target.run()[log_name].value,
-                        d.attrs[log_name].values.data.values),
+            np.allclose(
+                target.run()[log_name].value, d.attrs[log_name].values.data.values
+            ),
             "Expected values in the unaligned coord to match "
-            "the original run log from the Mantid workspace")
+            "the original run log from the Mantid workspace",
+        )
         self.assertEqual(d.attrs[log_name].values.unit, sc.units.K)
         self.assertTrue(
-            np.array_equal(target.run()[log_name].times.astype('datetime64[ns]'),
-                           d.attrs[log_name].values.coords["time"].values),
+            np.array_equal(
+                target.run()[log_name].times.astype('datetime64[ns]'),
+                d.attrs[log_name].values.coords["time"].values,
+            ),
             "Expected times in the unaligned coord to match "
-            "the original run log from the Mantid workspace")
+            "the original run log from the Mantid workspace",
+        )
 
     def test_convert_scalar_run_log_to_attrs(self):
         # Given a Mantid workspace with a run log
         import mantid.simpleapi as mantid
+
         target = mantid.CloneWorkspace(self.base_event_ws)
         log_name = "start_time"
-        self.assertTrue(target.run().hasProperty(log_name),
-                        f"Expected input workspace to have a {log_name} run log")
+        self.assertTrue(
+            target.run().hasProperty(log_name),
+            f"Expected input workspace to have a {log_name} run log",
+        )
 
         # When the workspace is converted to a scipp data array
         d = scn.mantid.convert_EventWorkspace_to_data_array(target, False)
 
         # Then the data array contains the run log as an unaligned coord
         self.assertEqual(
-            target.run()[log_name].value, d.attrs[log_name].value,
+            target.run()[log_name].value,
+            d.attrs[log_name].value,
             "Expected value of the unaligned coord to match "
-            "the original run log from the Mantid workspace")
+            "the original run log from the Mantid workspace",
+        )
 
     def test_warning_raised_when_convert_run_log_with_unrecognised_units(self):
         import mantid.simpleapi as mantid
+
         target = mantid.CloneWorkspace(self.base_event_ws)
         target.getRun()['LambdaRequest'].units = 'abcde'
         with warnings.catch_warnings(record=True) as caught_warnings:
             warnings.simplefilter("always")
             scn.mantid.convert_EventWorkspace_to_data_array(target, False)
-            assert len(
-                caught_warnings
-            ) > 0, "Expected warnings due to some run logs " \
-                   "having unrecognised units strings"
-            assert any("unrecognised units" in str(caught_warning.message)
-                       for caught_warning in caught_warnings)
+            assert len(caught_warnings) > 0, (
+                "Expected warnings due to some run logs "
+                "having unrecognised units strings"
+            )
+            assert any(
+                "unrecognised units" in str(caught_warning.message)
+                for caught_warning in caught_warnings
+            )
 
     def test_no_warning_raised_explicitly_dimensionless_run_log(self):
         import mantid.simpleapi as mantid
+
         target = mantid.CloneWorkspace(self.base_event_ws)
         with warnings.catch_warnings(record=True) as caught_warnings:
             scn.mantid.convert_EventWorkspace_to_data_array(target, False)
             original_number_of_warnings = len(caught_warnings)
 
         # Add an explicitly dimensionless log
-        mantid.AddSampleLog(Workspace=target,
-                            LogName='dimensionless_log',
-                            LogText='1',
-                            LogType='Number',
-                            LogUnit='dimensionless')
+        mantid.AddSampleLog(
+            Workspace=target,
+            LogName='dimensionless_log',
+            LogText='1',
+            LogType='Number',
+            LogUnit='dimensionless',
+        )
 
         with warnings.catch_warnings(record=True) as caught_warnings:
             scn.mantid.convert_EventWorkspace_to_data_array(target, False)
-            assert len(caught_warnings) == original_number_of_warnings,\
-                "Expected no extra warning about unrecognised units " \
+            assert len(caught_warnings) == original_number_of_warnings, (
+                "Expected no extra warning about unrecognised units "
                 "from explicitly dimensionless log"
+            )
 
     def test_set_sample(self):
         import mantid.simpleapi as mantid
+
         target = mantid.CloneWorkspace(self.base_event_ws)
         d = scn.mantid.convert_EventWorkspace_to_data_array(target, False)
         d.attrs["sample"].value.setThickness(3)
         # before
         self.assertNotEqual(3, target.sample().getThickness())
         target.setSample(d.attrs["sample"].value)
         # after
         self.assertEqual(3, target.sample().getThickness())
 
     def test_sample_ub(self):
         import mantid.simpleapi as mantid
+
         ws = mantid.CreateWorkspace(DataY=np.ones(1), DataX=np.arange(2))
         args = {'a': 1, 'b': 1, 'c': 1, 'alpha': 90, 'beta': 90, 'gamma': 90}
         mantid.SetUB(ws, **args)
         d = scn.mantid.from_mantid(ws)
         assert sc.identical(
             d.attrs['sample_ub'],
-            sc.spatial.linear_transform(value=ws.sample().getOrientedLattice().getUB(),
-                                        unit=sc.units.angstrom**-1))
+            sc.spatial.linear_transform(
+                value=ws.sample().getOrientedLattice().getUB(),
+                unit=sc.units.angstrom**-1,
+            ),
+        )
         assert sc.identical(
             d.attrs['sample_u'],
-            sc.spatial.linear_transform(value=ws.sample().getOrientedLattice().getU()))
+            sc.spatial.linear_transform(value=ws.sample().getOrientedLattice().getU()),
+        )
 
     def test_sample_without_ub(self):
         import mantid.simpleapi as mantid
+
         ws = mantid.CreateWorkspace(DataY=np.ones(1), DataX=np.arange(2))
         assert not ws.sample().hasOrientedLattice()  # Sanity check input
         d = scn.mantid.from_mantid(ws)
         assert "sample_ub" not in d.attrs
         assert "sample_u" not in d.attrs
 
     def _exec_to_spherical(self, x, y, z):
         in_out = sc.Dataset()
         in_out['x'] = sc.scalar(x, unit=sc.units.m)
         in_out['y'] = sc.scalar(y, unit=sc.units.m)
         in_out['z'] = sc.scalar(z, unit=sc.units.m)
-        point = sc.geometry.position(in_out['x'].data, in_out['y'].data,
-                                     in_out['z'].data)
+        point = sc.spatial.as_vectors(
+            in_out['x'].data, in_out['y'].data, in_out['z'].data
+        )
         scn.mantid._to_spherical(point, in_out)
         return in_out
 
     def test_spherical_conversion(self):
         x = 1.0
         y = 1.0
         z = 0.0
@@ -639,27 +725,30 @@
         spherical = self._exec_to_spherical(x, y, z)
         assert spherical['p-delta'].value == (1.0 / 4) * np.pi
         assert spherical['p-sign'].value < 0.0
 
     def test_detector_positions(self):
         import mantid.simpleapi as mantid
         from mantid.kernel import V3D
+
         eventWS = mantid.CloneWorkspace(self.base_event_ws)
         comp_info = eventWS.componentInfo()
         small_offset = V3D(0.01, 0.01, 0.01)
-        comp_info.setPosition(comp_info.source(),
-                              comp_info.samplePosition() + small_offset)
+        comp_info.setPosition(
+            comp_info.source(), comp_info.samplePosition() + small_offset
+        )
         moved = scn.mantid.convert_Workspace2D_to_data_array(eventWS)
         moved_det_position = moved.coords["position"]
         unmoved = scn.mantid.convert_Workspace2D_to_data_array(eventWS)
         unmoved_det_positions = unmoved.coords["position"]
         # Moving the sample accounted for in position calculations
         # but should not yield change to final detector positions
         self.assertTrue(
-            np.all(np.isclose(moved_det_position.values, unmoved_det_positions.values)))
+            np.all(np.isclose(moved_det_position.values, unmoved_det_positions.values))
+        )
 
     def test_validate_units(self):
         acceptable = ["wavelength", "Wavelength"]
         for i in acceptable:
             ret = scn.mantid.validate_dim_and_get_mantid_string(i)
             self.assertEqual(ret, "Wavelength")
 
@@ -667,14 +756,15 @@
         not_acceptable = [None, "None", "wavlength", 1, 1.0, ["wavelength"]]
         for i in not_acceptable:
             with self.assertRaises(RuntimeError):
                 scn.mantid.validate_dim_and_get_mantid_string(i)
 
     def test_WorkspaceGroup_parsed_correctly(self):
         from mantid.simpleapi import CreateSampleWorkspace, GroupWorkspaces, mtd
+
         CreateSampleWorkspace(OutputWorkspace="ws1")
         CreateSampleWorkspace(OutputWorkspace="ws2")
         CreateSampleWorkspace(OutputWorkspace="ws3")
         GroupWorkspaces(InputWorkspaces="ws1,ws2,ws3", OutputWorkspace="NewGroup")
 
         converted_group = scn.from_mantid(mtd["NewGroup"])
         converted_single = scn.from_mantid(mtd["ws1"])
@@ -685,30 +775,34 @@
         mtd.clear()
 
 
 @pytest.mark.skipif(not memory_is_at_least_gb(8), reason='Insufficient virtual memory')
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_load_mcstas_data():
     import mantid.simpleapi as mantid
-    wsg = mantid.LoadMcStas(scn.data.get_path('mcstas_sans.h5'),
-                            OutputWorkspace="test_mcstas_sans_wsg")
+
+    wsg = mantid.LoadMcStas(
+        scn.data.get_path('mcstas_sans.h5'), OutputWorkspace="test_mcstas_sans_wsg"
+    )
     ws = wsg[list(wsg.getNames()).index('EventData_test_mcstas_sans_wsg')]
     da = scn.from_mantid(ws)
 
     for i in range(ws.getNumberHistograms()):
         np.testing.assert_array_equal(da.coords['tof'].values, ws.readX(i))
         spec = ws.getSpectrum(i)
         da_spec = da['tof', 0]['spectrum', i]
         bin_sizes = da_spec.bins.size()
         assert spec.getNumberEvents() == bin_sizes.value
 
-        np.testing.assert_array_equal(spec.getTofs(),
-                                      da_spec.bins.coords['tof'].values.values)
-        np.testing.assert_array_equal(spec.getPulseTimesAsNumpy(),
-                                      da_spec.bins.coords['pulse_time'].value.values)
+        np.testing.assert_array_equal(
+            spec.getTofs(), da_spec.bins.coords['tof'].values.values
+        )
+        np.testing.assert_array_equal(
+            spec.getPulseTimesAsNumpy(), da_spec.bins.coords['pulse_time'].value.values
+        )
         np.testing.assert_array_equal(spec.getWeights(), da_spec.bins.data.value.values)
 
 
 def test_to_rot_from_vectors():
     a = sc.vector(value=[1, 0, 0])
     b = sc.vector(value=[0, 1, 0])
     rot = scn.mantid._rot_from_vectors(a, b)
@@ -717,31 +811,37 @@
     assert np.allclose((rot * b).value, a.value)
 
 
 @pytest.mark.skipif(not memory_is_at_least_gb(8), reason='Insufficient virtual memory')
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 @pytest.mark.parametrize(
     "param_dim",
-    ('tof', 'wavelength', 'energy', 'dspacing', 'Q', 'Q^2', 'energy_transfer'))
+    ('tof', 'wavelength', 'energy', 'dspacing', 'Q', 'Q^2', 'energy_transfer'),
+)
 def test_to_workspace_2d(param_dim):
     from mantid.simpleapi import mtd
+
     mtd.clear()
 
     data_len = 2
     expected_bins = data_len + 1
     expected_number_spectra = 10
 
-    y = sc.Variable(dims=['spectrum', param_dim],
-                    values=np.random.rand(expected_number_spectra, data_len),
-                    variances=np.random.rand(expected_number_spectra, data_len))
-
-    x = sc.Variable(dims=['spectrum', param_dim],
-                    values=np.arange(expected_number_spectra * expected_bins,
-                                     dtype=np.float64).reshape(
-                                         (expected_number_spectra, expected_bins)))
+    y = sc.Variable(
+        dims=['spectrum', param_dim],
+        values=np.random.rand(expected_number_spectra, data_len),
+        variances=np.random.rand(expected_number_spectra, data_len),
+    )
+
+    x = sc.Variable(
+        dims=['spectrum', param_dim],
+        values=np.arange(
+            expected_number_spectra * expected_bins, dtype=np.float64
+        ).reshape((expected_number_spectra, expected_bins)),
+    )
     data = sc.DataArray(data=y, coords={param_dim: x})
 
     ws = scn.to_mantid(data, param_dim)
 
     assert len(ws.readX(0)) == expected_bins
     assert ws.getNumberHistograms() == expected_number_spectra
     # check that no workspaces have been leaked in the ADS
@@ -752,19 +852,20 @@
         np.testing.assert_array_equal(ws.readY(i), y['spectrum', i].values)
         np.testing.assert_array_equal(ws.readE(i), np.sqrt(y['spectrum', i].variances))
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_to_workspace_2d_handles_single_spectra():
     from mantid.simpleapi import mtd
+
     mtd.clear()
 
-    expected_x = [0., 1., 2.]
-    expected_y = [10., 20., 30.]
-    expected_e = [4., 4., 4.]
+    expected_x = [0.0, 1.0, 2.0]
+    expected_y = [10.0, 20.0, 30.0]
+    expected_e = [4.0, 4.0, 4.0]
 
     x = sc.Variable(dims=['tof'], values=expected_x)
     y = sc.Variable(dims=['tof'], values=expected_y, variances=expected_e)
     data = sc.DataArray(data=y, coords={'tof': x})
 
     ws = scn.to_mantid(data, "tof")
 
@@ -774,24 +875,27 @@
     assert np.equal(ws.readY(0), expected_y).all()
     assert np.equal(ws.readE(0), np.sqrt(expected_e)).all()
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_to_workspace_2d_handles_single_x_array():
     from mantid.simpleapi import mtd
+
     mtd.clear()
 
-    expected_x = [0., 1., 2.]
-    expected_y = [[10., 20., 30.], [40., 50., 60.]]
-    expected_e = [[4., 4., 4.], [4., 4., 4.]]
+    expected_x = [0.0, 1.0, 2.0]
+    expected_y = [[10.0, 20.0, 30.0], [40.0, 50.0, 60.0]]
+    expected_e = [[4.0, 4.0, 4.0], [4.0, 4.0, 4.0]]
 
     x = sc.Variable(dims=['tof'], values=expected_x)
-    y = sc.Variable(dims=['spectrum', 'tof'],
-                    values=np.array(expected_y),
-                    variances=np.array(expected_e))
+    y = sc.Variable(
+        dims=['spectrum', 'tof'],
+        values=np.array(expected_y),
+        variances=np.array(expected_e),
+    )
     data = sc.DataArray(data=y, coords={'tof': x})
 
     ws = scn.to_mantid(data, "tof")
 
     assert ws.getNumberHistograms() == 2
     assert np.equal(ws.readX(0), expected_x).all()
     assert np.equal(ws.readX(1), expected_x).all()
@@ -801,14 +905,15 @@
         assert np.equal(ws.readE(i), np.sqrt(e_vals)).all()
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_attrs_with_dims():
     import mantid.simpleapi as sapi
     from mantid.kernel import FloatArrayProperty
+
     dataX = [1, 2, 3]
     dataY = [1, 2, 3]
     ws = sapi.CreateWorkspace(DataX=dataX, DataY=dataY, NSpec=1, UnitX="Wavelength")
     # Time series property
     sapi.AddSampleLog(ws, 'attr0', LogText='1', LogType='Number Series')
     # Single value property
     sapi.AddSampleLog(ws, 'attr1', LogText='1', LogType='Number')
@@ -822,178 +927,204 @@
     assert ds.attrs['attr0'].dtype == sc.DType.DataArray
     assert 'time' in ds.attrs['attr0'].value.coords
     # Variable (single value)
     assert ds.attrs['attr1'].dtype == sc.DType.int64
     # Variable (single value) wrapped Variable
     assert ds.attrs['attr2'].dtype == sc.DType.Variable
     assert ds.attrs['attr2'].shape == ()  # outer wrapper
-    assert ds.attrs['attr2'].value.shape == (10, )  # inner held
+    assert ds.attrs['attr2'].value.shape == (10,)  # inner held
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_time_series_log_extraction():
     import mantid.simpleapi as sapi
+
     ws = sapi.CreateWorkspace(DataX=[0, 1], DataY=[1])
     times = [
         np.datetime64(t)
         for t in ['2021-01-01T00:00:00', '2021-01-01T00:30:00', '2021-01-01T00:50:00']
     ]
     for i, t in enumerate(times):
         sapi.AddTimeSeriesLog(ws, Name='time_log', Time=str(t), Value=float(i))
     da = scn.from_mantid(ws)
     assert da.attrs['time_log'].value.coords['time'].dtype == sc.DType.datetime64
     # check times
     assert sc.identical(
         sc.Variable(dims=['time'], values=np.array(times).astype('datetime64[ns]')),
-        da.attrs['time_log'].value.coords['time'])
+        da.attrs['time_log'].value.coords['time'],
+    )
     # check values
-    assert sc.identical(sc.Variable(dims=['time'], values=np.arange(3.)),
-                        da.attrs['time_log'].value.data)
+    assert sc.identical(
+        sc.Variable(dims=['time'], values=np.arange(3.0)),
+        da.attrs['time_log'].value.data,
+    )
     sapi.DeleteWorkspace(ws)
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_from_mask_workspace():
     from os import path
 
     from mantid.simpleapi import LoadMask
+
     dir_path = path.dirname(path.realpath(__file__))
     mask = LoadMask('HYS', path.join(dir_path, 'HYS_mask.xml'))
     da = scn.from_mantid(mask)
+    assert da.unit is None
     assert da.data.dtype == sc.DType.bool
-    assert da.dims == ('spectrum', )
+    assert da.dims == ('spectrum',)
     assert da.variances is None
 
 
 def _all_indirect(blacklist):
     from mantid.simpleapi import config
 
     # Any indirect instrument considered
     for f in config.getFacilities():
         for i in f.instruments():
             if i.name() not in blacklist and [
-                    t for t in i.techniques() if 'Indirect' in t
+                t for t in i.techniques() if 'Indirect' in t
             ]:
                 yield i.name()
 
 
 def _load_indirect_instrument(instr, parameters):
-    from mantid.simpleapi import AddSampleLog, LoadEmptyInstrument, LoadParameterFile, \
-        config
+    from mantid.simpleapi import (
+        AddSampleLog,
+        LoadEmptyInstrument,
+        LoadParameterFile,
+        config,
+    )
 
     # Create a workspace from an indirect instrument
     out = LoadEmptyInstrument(InstrumentName=instr)
     if instr in parameters:
-        LoadParameterFile(out,
-                          Filename=os.path.join(config.getInstrumentDirectory(),
-                                                parameters[instr]))
+        LoadParameterFile(
+            out,
+            Filename=os.path.join(config.getInstrumentDirectory(), parameters[instr]),
+        )
     if not out.run().hasProperty('EMode'):
         # EMode would usually get attached via data loading
         # We skip that so have to apply manually
         AddSampleLog(out, LogName='EMode', LogText='Indirect', LogType='String')
     return out
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_extract_energy_final():
     # Efinal is often stored in a non-default parameter file
     parameters = {
         'IN16B': 'IN16B_silicon_311_Parameters.xml',
         'IRIS': 'IRIS_mica_002_Parameters.xml',
         'OSIRIS': 'OSIRIS_graphite_002_Parameters.xml',
-        'BASIS': 'BASIS_silicon_311_Parameters.xml'
+        'BASIS': 'BASIS_silicon_311_Parameters.xml',
     }
     unsupported = ['ZEEMANS', 'MARS', 'IN10', 'IN13', 'IN16', 'VISION', 'VESUVIO']
     for instr in _all_indirect(blacklist=unsupported):
         out = _load_indirect_instrument(instr, parameters)
         ds = scn.from_mantid(out)
         efs = ds.coords["final_energy"]
         assert not sc.all(sc.isnan(efs)).value
         assert efs.unit == sc.Unit("meV")
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_extract_energy_final_when_not_present():
     from mantid.kernel import DeltaEModeType
     from mantid.simpleapi import CreateSampleWorkspace
+
     ws = CreateSampleWorkspace(StoreInADS=False)
     assert ws.getEMode() == DeltaEModeType.Elastic
     ds = scn.from_mantid(ws)
     assert "final_energy" not in ds.coords
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_extract_energy_initial():
     from mantid.simpleapi import mtd
+
     mtd.clear()
-    ds = scn.load(scn.data.get_path("CNCS_51936_event.nxs"),
-                  mantid_args={"SpectrumMax": 1})
-    assert sc.identical(ds.coords["incident_energy"],
-                        sc.scalar(value=3.0, unit=sc.Unit("meV")))
+    ds = scn.load(
+        scn.data.get_path("CNCS_51936_event.nxs"), mantid_args={"SpectrumMax": 1}
+    )
+    assert sc.identical(
+        ds.coords["incident_energy"], sc.scalar(value=3.0, unit=sc.Unit("meV"))
+    )
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_extract_energy_inital_when_not_present():
     from mantid.kernel import DeltaEModeType
     from mantid.simpleapi import CreateSampleWorkspace
+
     ws = CreateSampleWorkspace(StoreInADS=False)
     assert ws.getEMode() == DeltaEModeType.Elastic
     ds = scn.from_mantid(ws)
     assert "incident_energy" not in ds.coords
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_EventWorkspace_with_pulse_times():
     import mantid.simpleapi as sapi
-    small_event_ws = sapi.CreateSampleWorkspace(WorkspaceType='Event',
-                                                NumBanks=1,
-                                                NumEvents=10)
-    d = scn.mantid.convert_EventWorkspace_to_data_array(small_event_ws,
-                                                        load_pulse_times=True)
+
+    small_event_ws = sapi.CreateSampleWorkspace(
+        WorkspaceType='Event', NumBanks=1, NumEvents=10
+    )
+    d = scn.mantid.convert_EventWorkspace_to_data_array(
+        small_event_ws, load_pulse_times=True
+    )
     assert d.data.values[0].coords['pulse_time'].dtype == sc.DType.datetime64
     assert sc.identical(
         d.data.values[0].coords['pulse_time']['event', 0],
         sc.scalar(
-            value=small_event_ws.getSpectrum(0).getPulseTimes()[0].to_datetime64()))
+            value=small_event_ws.getSpectrum(0).getPulseTimes()[0].to_datetime64()
+        ),
+    )
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_duplicate_monitor_names():
     from mantid.simpleapi import LoadEmptyInstrument
-    ws = LoadEmptyInstrument(InstrumentName='POLARIS',
-                             StoreInADS=False)  # Has many monitors named 'monitor'
+
+    ws = LoadEmptyInstrument(
+        InstrumentName='POLARIS', StoreInADS=False
+    )  # Has many monitors named 'monitor'
     da = scn.mantid.from_mantid(ws)
     assert da.attrs['monitor_1'].value.attrs['spectrum'].value == 1
     assert da.attrs['monitor_13'].value.attrs['spectrum'].value == 13
     assert da.attrs['monitor_14'].value.attrs['spectrum'].value == 14
 
 
 @pytest.mark.skipif(not mantid_is_available(), reason='Mantid framework is unavailable')
 def test_load_error_when_file_not_found_via_fuzzy_match():
     with pytest.raises(ValueError):
         scn.load("fictional.nxs")
 
 
 def make_dynamic_algorithm_without_fileproperty(alg_name):
-    from mantid.api import AlgorithmFactory, PythonAlgorithm, WorkspaceFactory, \
-        WorkspaceProperty
+    from mantid.api import (
+        AlgorithmFactory,
+        PythonAlgorithm,
+        WorkspaceFactory,
+        WorkspaceProperty,
+    )
     from mantid.kernel import Direction
 
     # Loader without FileProperty
     if AlgorithmFactory.exists(alg_name):
         return
 
     class Alg(PythonAlgorithm):
-
         def PyInit(self):
             self.declareProperty("Filename", "")
             self.declareProperty(
-                WorkspaceProperty(name="OutputWorkspace",
-                                  defaultValue="",
-                                  direction=Direction.Output))
+                WorkspaceProperty(
+                    name="OutputWorkspace", defaultValue="", direction=Direction.Output
+                )
+            )
 
         def PyExec(self):
             self.setProperty("OutputWorkspace", WorkspaceFactory.createTable())
 
     Alg.__name__ = alg_name
     AlgorithmFactory.subscribe(Alg)
     importlib.reload(sys.modules["mantid.simpleapi"])
```

### Comparing `scippneutron-23.3.0/tests/nexus_helpers.py` & `scippneutron-23.4.0/tests/nexus_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,32 +7,34 @@
 from enum import Enum
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
 
 import h5py
 import numpy as np
 import scipp as sc
 
-from scippneutron.io.nexus._json_nexus import JSONGroup, make_json_attr, \
-    make_json_dataset
+from scippneutron.io.nexus._json_nexus import (
+    JSONGroup,
+    make_json_attr,
+    make_json_dataset,
+)
 
 h5root = Union[h5py.File, h5py.Group]
 
 
 def _create_nx_class(group_name: str, nx_class_name: str, parent: h5root) -> h5py.Group:
     nx_class = parent.create_group(group_name)
     nx_class.attrs["NX_class"] = nx_class_name
     return nx_class
 
 
 @contextmanager
 def in_memory_hdf5_file_with_two_nxentry() -> Iterator[h5py.File]:
-    nexus_file = h5py.File('in_memory_events.nxs',
-                           mode='w',
-                           driver="core",
-                           backing_store=False)
+    nexus_file = h5py.File(
+        'in_memory_events.nxs', mode='w', driver="core", backing_store=False
+    )
     try:
         _create_nx_class("entry_1", "NXentry", nexus_file)
         _create_nx_class("entry_2", "NXentry", nexus_file)
         yield nexus_file
     finally:
         nexus_file.close()
 
@@ -145,14 +147,15 @@
 
 @dataclass
 class Stream:
     """
     Only present in the JSON NeXus file templates, not in HDF5 NeXus files.
     Records where to find data in Kafka that are streamed during an experiment.
     """
+
     # Where the builder should place the stream object
     path: str
 
     # The following members correspond to fields in stream object.
     # Some of them may not be of interest to Scipp but are to other
     # software which consume the json template, for example
     # the Filewriter (https://github.com/ess-dmsc/kafka-to-nexus)
@@ -182,32 +185,36 @@
     data: np.ndarray
     axes: List[Tuple[str, np.ndarray]]
     events: Optional[EventData] = None
     depends_on: Optional[Transformation] = None
 
 
 class InMemoryNeXusWriter:
-
-    def add_dataset_at_path(self, file_root: h5py.File, path: str, data: np.ndarray,
-                            attributes: Dict):
+    def add_dataset_at_path(
+        self, file_root: h5py.File, path: str, data: np.ndarray, attributes: Dict
+    ):
         path_split = path.split("/")
         dataset_name = path_split[-1]
         parent_path = "/".join(path_split[:-1])
         dataset = self.add_dataset(file_root[parent_path], dataset_name, data)
         for name, value in attributes.items():
             self.add_attribute(dataset, name, value)
 
     @staticmethod
-    def add_dataset(parent: h5py.Group, name: str,
-                    data: Union[str, bytes, np.ndarray]) -> h5py.Dataset:
+    def add_dataset(
+        parent: h5py.Group, name: str, data: Union[str, bytes, np.ndarray]
+    ) -> h5py.Dataset:
         return parent.create_dataset(name, data=data)
 
     @staticmethod
-    def add_attribute(parent: Union[h5py.Group, h5py.Dataset], name: str,
-                      value: Union[str, bytes, np.ndarray]):
+    def add_attribute(
+        parent: Union[h5py.Group, h5py.Dataset],
+        name: str,
+        value: Union[str, bytes, np.ndarray],
+    ):
         parent.attrs[name] = value
 
     @staticmethod
     def add_group(parent: h5py.Group, name: str) -> h5py.Group:
         return parent.create_group(name)
 
     @staticmethod
@@ -264,32 +271,34 @@
     name = path_split[-1]
     parent_path = '/'.join(path_split[:-1])
     parent_group = _get_object_by_path(file_root, parent_path)
     return parent_group, name
 
 
 class JsonWriter:
-
-    def add_dataset_at_path(self, file_root: Dict, path: str, data: np.ndarray,
-                            attributes: Dict):
+    def add_dataset_at_path(
+        self, file_root: Dict, path: str, data: np.ndarray, attributes: Dict
+    ):
         parent_group, dataset_name = _parent_and_name_from_path(file_root, path)
         dataset = self.add_dataset(parent_group, dataset_name, data)
         for name, value in attributes.items():
             self.add_attribute(dataset, name, value)
 
     @staticmethod
-    def add_dataset(parent: Dict, name: str, data: Union[str, bytes,
-                                                         np.ndarray]) -> Dict:
+    def add_dataset(
+        parent: Dict, name: str, data: Union[str, bytes, np.ndarray]
+    ) -> Dict:
         dataset = make_json_dataset(name, data)
         parent["children"].append(dataset)
         return dataset
 
     @staticmethod
-    def add_attribute(parent: Dict, name: str, value: Union[str, bytes, list,
-                                                            np.ndarray]):
+    def add_attribute(
+        parent: Dict, name: str, value: Union[str, bytes, list, np.ndarray]
+    ):
         attr = make_json_attr(name, value)
         parent["attributes"].append(attr)
 
     @staticmethod
     def add_group(parent: Dict, name: str) -> Dict:
         new_group = {"type": "group", "name": name, "children": [], "attributes": []}
         parent["children"].append(new_group)
@@ -307,25 +316,24 @@
         new_stream = {
             "type": "stream",
             "stream": {
                 "topic": stream.topic,
                 "source": stream.source,
                 "writer_module": stream.writer_module,
                 "type": stream.type,
-                "value_units": stream.value_units
-            }
+                "value_units": stream.value_units,
+            },
         }
         if (group := _get_object_by_path(file_root, stream.path)) is None:
             parent, name = _parent_and_name_from_path(file_root, stream.path)
             group = self.add_group(parent, name)
         group["children"].append(new_stream)
 
 
 class NumpyEncoder(json.JSONEncoder):
-
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         return json.JSONEncoder.default(self, obj)
 
 
 class NexusBuilder:
@@ -353,16 +361,17 @@
         self._datas = []
 
     def add_dataset_at_path(self, path: str, data: np.ndarray, attributes: Dict):
         self._datasets.append(DatasetAtPath(path, data, attributes))
 
     def _write_datasets(self, root: Union[Dict, h5py.File]):
         for dataset in self._datasets:
-            self._writer.add_dataset_at_path(root, dataset.path, dataset.data,
-                                             dataset.attributes)
+            self._writer.add_dataset_at_path(
+                root, dataset.path, dataset.data, dataset.attributes
+            )
 
     def add_stream(self, stream: Stream):
         self._streams.append(stream)
 
     def add_detector(self, detector: Detector):
         self._detectors.append(detector)
 
@@ -447,18 +456,17 @@
             pass
 
     @contextmanager
     def file(self) -> Iterator[h5py.File]:
         # "core" driver means file is "in-memory" not on disk.
         # backing_store=False prevents file being written to
         # disk on flush() or close().
-        nexus_file = h5py.File('in_memory_events.nxs',
-                               mode='w',
-                               driver="core",
-                               backing_store=False)
+        nexus_file = h5py.File(
+            'in_memory_events.nxs', mode='w', driver="core", backing_store=False
+        )
         self._writer = InMemoryNeXusWriter()
         try:
             self._write_file(nexus_file)
             yield nexus_file
         finally:
             nexus_file.close()
 
@@ -499,129 +507,143 @@
         try:
             self._write_file(nexus_file)
         finally:
             nexus_file.close()
 
     def _write_links(self, file_root: Union[h5py.Group, Dict]):
         for hard_link in self._hard_links:
-            self._writer.add_hard_link(file_root, hard_link.new_path,
-                                       hard_link.target_path)
+            self._writer.add_hard_link(
+                file_root, hard_link.new_path, hard_link.target_path
+            )
         for soft_link in self._soft_links:
-            self._writer.add_soft_link(file_root, soft_link.new_path,
-                                       soft_link.target_path)
+            self._writer.add_soft_link(
+                file_root, soft_link.new_path, soft_link.target_path
+            )
 
     def _write_sample(self, parent_group: Union[h5py.Group, Dict]):
         for sample in self._sample:
             sample_group = self._create_nx_class(sample.name, "NXsample", parent_group)
             if sample.depends_on is not None:
                 depends_on = self._add_transformations_to_file(
-                    sample.depends_on, sample_group, f"/entry/{sample.name}")
+                    sample.depends_on, sample_group, f"/entry/{sample.name}"
+                )
                 self._writer.add_dataset(sample_group, "depends_on", data=depends_on)
             if sample.distance is not None:
-                distance_ds = self._writer.add_dataset(sample_group,
-                                                       "distance",
-                                                       data=sample.distance)
+                distance_ds = self._writer.add_dataset(
+                    sample_group, "distance", data=sample.distance
+                )
                 if sample.distance_units is not None:
-                    self._writer.add_attribute(distance_ds, "units",
-                                               sample.distance_units)
+                    self._writer.add_attribute(
+                        distance_ds, "units", sample.distance_units
+                    )
 
             if sample.ub_matrix is not None:
-                self._writer.add_dataset(sample_group,
-                                         "ub_matrix",
-                                         data=sample.ub_matrix)
+                self._writer.add_dataset(
+                    sample_group, "ub_matrix", data=sample.ub_matrix
+                )
 
             if sample.orientation_matrix is not None:
-                self._writer.add_dataset(sample_group,
-                                         "orientation_matrix",
-                                         data=sample.orientation_matrix)
+                self._writer.add_dataset(
+                    sample_group, "orientation_matrix", data=sample.orientation_matrix
+                )
 
     def _write_source(self, parent_group: Union[h5py.Group, Dict]):
         for source in self._source:
             source_group = self._create_nx_class(source.name, "NXsource", parent_group)
             if source.depends_on is not None:
                 if isinstance(source.depends_on, str):
                     depends_on = source.depends_on
                 else:
                     depends_on = self._add_transformations_to_file(
-                        source.depends_on, source_group, f"/entry/{source.name}")
+                        source.depends_on, source_group, f"/entry/{source.name}"
+                    )
                 self._writer.add_dataset(source_group, "depends_on", data=depends_on)
             if source.distance is not None:
-                distance_ds = self._writer.add_dataset(source_group,
-                                                       "distance",
-                                                       data=source.distance)
+                distance_ds = self._writer.add_dataset(
+                    source_group, "distance", data=source.distance
+                )
                 if source.distance_units is not None:
-                    self._writer.add_attribute(distance_ds, "units",
-                                               source.distance_units)
+                    self._writer.add_attribute(
+                        distance_ds, "units", source.distance_units
+                    )
 
     def _write_instrument(
-            self, parent_group: Union[h5py.Group, Dict]) -> Union[h5py.Group, Dict]:
-        instrument_group = self._create_nx_class("instrument", "NXinstrument",
-                                                 parent_group)
+        self, parent_group: Union[h5py.Group, Dict]
+    ) -> Union[h5py.Group, Dict]:
+        instrument_group = self._create_nx_class(
+            "instrument", "NXinstrument", parent_group
+        )
         self._writer.add_dataset(instrument_group, "name", self._instrument_name)
         return instrument_group
 
     def _write_detectors(self, parent_group: Union[h5py.Group, Dict], parent_path: str):
         for detector_index, detector in enumerate(self._detectors):
             detector_name = f"detector_{detector_index}"
             detector_group = self._add_detector_group_to_file(
-                detector, parent_group, detector_name)
+                detector, parent_group, detector_name
+            )
             if detector.data is not None:
                 da = detector.data
                 ds = self._writer.add_dataset(detector_group, "data", data=da.values)
                 self._writer.add_attribute(ds, "units", str(da.unit))
                 axes = [dim if dim in da.coords else '.' for dim in da.dims]
                 self._writer.add_attribute(detector_group, "axes", axes)
                 for key, coord in da.coords.items():
-                    ds = self._writer.add_dataset(detector_group,
-                                                  key,
-                                                  data=coord.values)
+                    ds = self._writer.add_dataset(
+                        detector_group, key, data=coord.values
+                    )
                     self._writer.add_attribute(ds, "units", str(coord.unit))
 
             if detector.event_data is not None:
-                self._add_event_data_group_to_file(detector.event_data, detector_group,
-                                                   "events")
+                self._add_event_data_group_to_file(
+                    detector.event_data, detector_group, "events"
+                )
             if detector.log is not None:
                 self._add_log_group_to_file(detector.log, detector_group)
             if detector.depends_on is not None:
                 depends_on = self._add_transformations_to_file(
-                    detector.depends_on, detector_group,
-                    f"{parent_path}/{detector_name}")
+                    detector.depends_on,
+                    detector_group,
+                    f"{parent_path}/{detector_name}",
+                )
                 self._writer.add_dataset(detector_group, "depends_on", data=depends_on)
 
     def _write_choppers(self, parent_group: Union[h5py.Group, Dict]):
-
         for chopper in self._choppers:
-            chopper_group = self._create_nx_class(chopper.name, "NXdisk_chopper",
-                                                  parent_group)
-            distance_ds = self._writer.add_dataset(chopper_group,
-                                                   "distance",
-                                                   data=chopper.distance)
-            rotation_ds = self._writer.add_dataset(chopper_group,
-                                                   "rotation_speed",
-                                                   data=chopper.rotation_speed)
+            chopper_group = self._create_nx_class(
+                chopper.name, "NXdisk_chopper", parent_group
+            )
+            distance_ds = self._writer.add_dataset(
+                chopper_group, "distance", data=chopper.distance
+            )
+            rotation_ds = self._writer.add_dataset(
+                chopper_group, "rotation_speed", data=chopper.rotation_speed
+            )
             if chopper.distance_units is not None:
                 self._writer.add_attribute(distance_ds, "units", chopper.distance_units)
             if chopper.rotation_units is not None:
                 self._writer.add_attribute(rotation_ds, "units", chopper.rotation_units)
 
     def _write_event_data(self, parent_group: Union[h5py.Group, Dict]):
         for event_data_index, event_data in enumerate(self._event_data):
-            self._add_event_data_group_to_file(event_data, parent_group,
-                                               f"events_{event_data_index}")
+            self._add_event_data_group_to_file(
+                event_data, parent_group, f"events_{event_data_index}"
+            )
 
     def _write_monitors(self, parent_group: Union[h5py.Group, Dict]):
         for monitor in self._monitors:
             self._add_monitor_group_to_file(monitor, parent_group)
 
     def _add_monitor_group_to_file(self, monitor: Monitor, parent_group: h5py.Group):
         monitor_group = self._create_nx_class(monitor.name, "NXmonitor", parent_group)
         data_group = self._writer.add_dataset(monitor_group, "data", monitor.data)
         self._writer.add_attribute(data_group, "units", '')
-        self._writer.add_attribute(data_group, "axes",
-                                   ",".join(name for name, _ in monitor.axes))
+        self._writer.add_attribute(
+            data_group, "axes", ",".join(name for name, _ in monitor.axes)
+        )
 
         if monitor.events:
             self._write_event_data_to_group(monitor_group, monitor.events)
 
         for axis_name, axis_data in monitor.axes:
             # We write event data (if exists) first - if we've already written event
             # data the event index will already have been created so we skip writing
@@ -630,15 +652,16 @@
                 ds = self._writer.add_dataset(monitor_group, axis_name, axis_data)
                 self._writer.add_attribute(ds, "units", '')
         if monitor.depends_on is not None:
             if isinstance(monitor.depends_on, str):
                 depends_on = monitor.depends_on
             else:
                 depends_on = self._add_transformations_to_file(
-                    monitor.depends_on, monitor_group, f"/{monitor.name}")
+                    monitor.depends_on, monitor_group, f"/{monitor.name}"
+                )
             self._writer.add_dataset(monitor_group, "depends_on", data=depends_on)
 
     def _write_datas(self, parent_group: Union[h5py.Group, Dict]):
         for data in self._datas:
             self._add_data_group_to_file(data, parent_group)
 
     def _add_data_group_to_file(self, data: Data, parent_group: h5py.Group):
@@ -659,73 +682,93 @@
             for k, v in data.attrs.items():
                 self._writer.add_attribute(group, k, v)
 
     def _write_logs(self, parent_group: Union[h5py.Group, Dict]):
         for log in self._logs:
             self._add_log_group_to_file(log, parent_group)
 
-    def _add_event_data_group_to_file(self, data: EventData, parent_group: h5py.Group,
-                                      group_name: str):
+    def _add_event_data_group_to_file(
+        self, data: EventData, parent_group: h5py.Group, group_name: str
+    ):
         event_group = self._create_nx_class(group_name, "NXevent_data", parent_group)
         self._write_event_data_to_group(event_group, data)
 
     def _write_event_data_to_group(self, event_group: h5py.Group, data: EventData):
         if data.event_id is not None:
             self._writer.add_dataset(event_group, "event_id", data=data.event_id)
         if data.event_time_offset is not None:
-            event_time_offset_ds = self._writer.add_dataset(event_group,
-                                                            "event_time_offset",
-                                                            data=data.event_time_offset)
-            self._writer.add_attribute(event_time_offset_ds, "units",
-                                       data.event_time_offset_unit)
+            event_time_offset_ds = self._writer.add_dataset(
+                event_group, "event_time_offset", data=data.event_time_offset
+            )
+            self._writer.add_attribute(
+                event_time_offset_ds, "units", data.event_time_offset_unit
+            )
         if data.event_time_zero is not None:
-            event_time_zero_ds = self._writer.add_dataset(event_group,
-                                                          "event_time_zero",
-                                                          data=data.event_time_zero)
-            self._writer.add_attribute(event_time_zero_ds, "units",
-                                       data.event_time_zero_unit)
-            self._writer.add_attribute(event_time_zero_ds, "offset",
-                                       data.event_time_zero_offset)
+            event_time_zero_ds = self._writer.add_dataset(
+                event_group, "event_time_zero", data=data.event_time_zero
+            )
+            self._writer.add_attribute(
+                event_time_zero_ds, "units", data.event_time_zero_unit
+            )
+            self._writer.add_attribute(
+                event_time_zero_ds, "offset", data.event_time_zero_offset
+            )
         if data.event_index is not None:
             self._writer.add_dataset(event_group, "event_index", data=data.event_index)
 
-    def _add_transformations_to_file(self, transform: Transformation,
-                                     parent_group: h5py.Group, parent_path: str) -> str:
+    def _add_transformations_to_file(
+        self, transform: Transformation, parent_group: h5py.Group, parent_path: str
+    ) -> str:
         transform_chain = [transform]
         while transform.depends_on is not None and not isinstance(
-                transform.depends_on, str):
+            transform.depends_on, str
+        ):
             transform_chain.append(transform.depends_on)
             transform = transform.depends_on
 
         transforms_group_name = "transformations"
-        transforms_group = self._create_nx_class("transformations", "NXtransformations",
-                                                 parent_group)
+        transforms_group = self._create_nx_class(
+            "transformations", "NXtransformations", parent_group
+        )
         transform_chain.reverse()
-        depends_on_str = transform.depends_on if isinstance(transform.depends_on,
-                                                            str) else None
+        depends_on_str = (
+            transform.depends_on if isinstance(transform.depends_on, str) else None
+        )
         transform_group_path = f"{parent_path}/{transforms_group_name}"
         for transform_number, transform in enumerate(transform_chain):
             if transform.time is not None:
                 depends_on_str = self._add_transformation_as_log(
-                    transform, transform_number, transforms_group, transform_group_path,
-                    depends_on_str)
+                    transform,
+                    transform_number,
+                    transforms_group,
+                    transform_group_path,
+                    depends_on_str,
+                )
             else:
                 depends_on_str = self._add_transformation_as_dataset(
-                    transform, transform_number, transforms_group, transform_group_path,
-                    depends_on_str)
+                    transform,
+                    transform_number,
+                    transforms_group,
+                    transform_group_path,
+                    depends_on_str,
+                )
         return depends_on_str
 
-    def _add_transformation_as_dataset(self, transform: Transformation,
-                                       transform_number: int,
-                                       transforms_group: h5py.Group, group_path: str,
-                                       depends_on: Optional[str]) -> str:
+    def _add_transformation_as_dataset(
+        self,
+        transform: Transformation,
+        transform_number: int,
+        transforms_group: h5py.Group,
+        group_path: str,
+        depends_on: Optional[str],
+    ) -> str:
         transform_name = f"transform_{transform_number}"
-        added_transform = self._writer.add_dataset(transforms_group,
-                                                   f"transform_{transform_number}",
-                                                   data=transform.value)
+        added_transform = self._writer.add_dataset(
+            transforms_group, f"transform_{transform_number}", data=transform.value
+        )
         self._add_transform_attributes(added_transform, depends_on, transform)
         if transform.value_units is not None:
             self._writer.add_attribute(added_transform, "units", transform.value_units)
         return f"{group_path}/{transform_name}"
 
     def _add_log_group_to_file(self, log: Log, parent_group: h5py.Group) -> h5py.Group:
         log_group = self._create_nx_class(log.name, "NXlog", parent_group)
@@ -736,64 +779,90 @@
         if log.time is not None:
             time_ds = self._writer.add_dataset(log_group, "time", data=log.time)
             if log.time_units is not None:
                 self._writer.add_attribute(time_ds, "units", log.time_units)
             if log.start_time is not None:
                 self._writer.add_attribute(time_ds, "start", log.start_time)
             if log.scaling_factor is not None:
-                self._writer.add_attribute(time_ds, "scaling_factor",
-                                           log.scaling_factor)
+                self._writer.add_attribute(
+                    time_ds, "scaling_factor", log.scaling_factor
+                )
         return log_group
 
-    def _add_transformation_as_log(self, transform: Transformation,
-                                   transform_number: int, transforms_group: h5py.Group,
-                                   group_path: str, depends_on: Optional[str]) -> str:
+    def _add_transformation_as_log(
+        self,
+        transform: Transformation,
+        transform_number: int,
+        transforms_group: h5py.Group,
+        group_path: str,
+        depends_on: Optional[str],
+    ) -> str:
         transform_name = f"transform_{transform_number}"
         added_transform = self._add_log_group_to_file(
-            Log(transform_name, transform.value, transform.time, transform.value_units,
-                transform.time_units), transforms_group)
+            Log(
+                transform_name,
+                transform.value,
+                transform.time,
+                transform.value_units,
+                transform.time_units,
+            ),
+            transforms_group,
+        )
         self._add_transform_attributes(added_transform, depends_on, transform)
         return f"{group_path}/{transform_name}"
 
-    def _add_detector_group_to_file(self, detector: Detector, parent_group: h5py.Group,
-                                    group_name: str) -> h5py.Group:
+    def _add_detector_group_to_file(
+        self, detector: Detector, parent_group: h5py.Group, group_name: str
+    ) -> h5py.Group:
         detector_group = self._create_nx_class(group_name, "NXdetector", parent_group)
         if detector.detector_numbers is not None:
-            self._writer.add_dataset(detector_group, "detector_number",
-                                     detector.detector_numbers)
-        for dataset_name, array in (("x_pixel_offset", detector.x_offsets),
-                                    ("y_pixel_offset", detector.y_offsets),
-                                    ("z_pixel_offset", detector.z_offsets)):
+            self._writer.add_dataset(
+                detector_group, "detector_number", detector.detector_numbers
+            )
+        for dataset_name, array in (
+            ("x_pixel_offset", detector.x_offsets),
+            ("y_pixel_offset", detector.y_offsets),
+            ("z_pixel_offset", detector.z_offsets),
+        ):
             if array is not None:
-                offsets_ds = self._writer.add_dataset(detector_group, dataset_name,
-                                                      array)
+                offsets_ds = self._writer.add_dataset(
+                    detector_group, dataset_name, array
+                )
                 if detector.offsets_unit is not None:
-                    self._writer.add_attribute(offsets_ds, "units",
-                                               detector.offsets_unit)
+                    self._writer.add_attribute(
+                        offsets_ds, "units", detector.offsets_unit
+                    )
         return detector_group
 
-    def _add_transform_attributes(self, added_transform: Union[h5py.Group,
-                                                               h5py.Dataset],
-                                  depends_on: Optional[str], transform: Transformation):
+    def _add_transform_attributes(
+        self,
+        added_transform: Union[h5py.Group, h5py.Dataset],
+        depends_on: Optional[str],
+        transform: Transformation,
+    ):
         self._writer.add_attribute(added_transform, "vector", transform.vector)
-        self._writer.add_attribute(added_transform, "transformation_type",
-                                   transform.transform_type.value)
+        self._writer.add_attribute(
+            added_transform, "transformation_type", transform.transform_type.value
+        )
         if transform.offset is not None:
             self._writer.add_attribute(added_transform, "offset", transform.offset)
         if transform.offset_unit is not None:
-            self._writer.add_attribute(added_transform, "offset_units",
-                                       transform.offset_unit)
+            self._writer.add_attribute(
+                added_transform, "offset_units", transform.offset_unit
+            )
         if depends_on is not None:
             self._writer.add_attribute(added_transform, "depends_on", depends_on)
         else:
-            self._writer.add_attribute(added_transform, "depends_on",
-                                       ".")  # means end of chain
-
-    def _create_nx_class(self, group_name: str, nx_class_name: str,
-                         parent: h5root) -> h5py.Group:
+            self._writer.add_attribute(
+                added_transform, "depends_on", "."
+            )  # means end of chain
+
+    def _create_nx_class(
+        self, group_name: str, nx_class_name: str, parent: h5root
+    ) -> h5py.Group:
         nx_class = self._writer.add_group(parent, group_name)
         self._writer.add_attribute(nx_class, "NX_class", nx_class_name)
         return nx_class
 
     def _write_streams(self, root: Union[h5py.File, Dict]):
         if isinstance(self._writer, JsonWriter):
             for stream in self._streams:
```

### Comparing `scippneutron-23.3.0/tests/tof/frames_test.py` & `scippneutron-23.4.0/tests/tof/frames_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,91 +7,105 @@
 from hypothesis import given
 from hypothesis import strategies as st
 
 from scippneutron.tof import frames, unwrap_frames
 
 
 def make_array(*, npixel=3, nevent=1000, pulse_period=None, time_offset=None):
-    pulse_period = 71.0e3 * sc.Unit('us') if pulse_period is None else pulse_period.to(
-        unit='us')
+    pulse_period = (
+        71.0e3 * sc.Unit('us') if pulse_period is None else pulse_period.to(unit='us')
+    )
     if time_offset is None:
-        time_offset = sc.array(dims=['event'],
-                               values=np.random.rand(nevent) * pulse_period.value,
-                               unit='us')
+        time_offset = sc.array(
+            dims=['event'],
+            values=np.random.rand(nevent) * pulse_period.value,
+            unit='us',
+        )
     start = sc.datetime('now', unit='ns')
     npulse = 1234
     time_zero = start + (pulse_period * sc.linspace('event', 0, npulse, num=nevent)).to(
-        unit='ns', dtype='int64')
+        unit='ns', dtype='int64'
+    )
     pixel = sc.arange(dim='event', start=0, stop=nevent) % npixel
-    events = sc.DataArray(sc.ones(sizes=time_offset.sizes),
-                          coords={
-                              'event_time_offset': time_offset,
-                              'event_time_zero': time_zero,
-                              'pixel': pixel
-                          })
+    events = sc.DataArray(
+        sc.ones(sizes=time_offset.sizes),
+        coords={
+            'event_time_offset': time_offset,
+            'event_time_zero': time_zero,
+            'pixel': pixel,
+        },
+    )
     da = events.group(sc.arange(dim='pixel', start=0, stop=npixel, dtype=pixel.dtype))
     da.coords['L1'] = sc.scalar(value=160.0, unit='m')
     da.coords['L2'] = sc.array(dims=['pixel'], values=np.arange(npixel), unit='m')
     return da
 
 
 def test_unwrap_frames_given_tof_bins_meta_data_raises_ValueError():
     da = make_array()
     da.coords['tof'] = sc.scalar(1.0, unit='ms')
     with pytest.raises(ValueError):
-        unwrap_frames(da,
-                      scatter=True,
-                      pulse_period=71.0 * sc.Unit('ms'),
-                      frame_offset=30.1 * sc.Unit('ms'),
-                      lambda_min=2.5 * sc.Unit('Angstrom'))
+        unwrap_frames(
+            da,
+            scatter=True,
+            pulse_period=71.0 * sc.Unit('ms'),
+            frame_offset=30.1 * sc.Unit('ms'),
+            lambda_min=2.5 * sc.Unit('Angstrom'),
+        )
 
 
 def test_unwrap_frames_given_tof_event_meta_data_raises_ValueError():
     da = make_array()
     da.bins.coords['tof'] = da.bins.coords['event_time_offset']
     with pytest.raises(ValueError):
-        unwrap_frames(da,
-                      scatter=True,
-                      pulse_period=71.0 * sc.Unit('ms'),
-                      frame_offset=30.1 * sc.Unit('ms'),
-                      lambda_min=2.5 * sc.Unit('Angstrom'))
+        unwrap_frames(
+            da,
+            scatter=True,
+            pulse_period=71.0 * sc.Unit('ms'),
+            frame_offset=30.1 * sc.Unit('ms'),
+            lambda_min=2.5 * sc.Unit('Angstrom'),
+        )
 
 
 def test_unwrap_frames_no_shift_and_infinite_energy_yields_tof_equal_time_offset():
     da = make_array(pulse_period=71.0 * sc.Unit('ms'))
-    da = unwrap_frames(da,
-                       scatter=True,
-                       pulse_period=71.0 * sc.Unit('ms'),
-                       frame_offset=0.0 * sc.Unit('ms'),
-                       lambda_min=0.0 * sc.Unit('Angstrom'))
+    da = unwrap_frames(
+        da,
+        scatter=True,
+        pulse_period=71.0 * sc.Unit('ms'),
+        frame_offset=0.0 * sc.Unit('ms'),
+        lambda_min=0.0 * sc.Unit('Angstrom'),
+    )
     assert sc.identical(da.bins.coords['tof'], da.bins.attrs['event_time_offset'])
 
 
-def test_unwrap_frames_no_shift_and_no_events_below_lambda_min_yields_tof_equal_time_offset(  # noqa #501
-):
+def test_unwrap_frames_no_shift_and_no_events_below_lambda_min_yields_tof_equal_time_offset():  # noqa #501
     da = make_array(pulse_period=71.0 * sc.Unit('ms'))
     da.bins.coords['event_time_offset'] += sc.to_unit(
-        10.0 * sc.Unit('ms'), da.bins.coords['event_time_offset'].bins.unit)
-    da = unwrap_frames(da,
-                       scatter=True,
-                       pulse_period=81.0 * sc.Unit('ms'),
-                       frame_offset=0.0 * sc.Unit('ms'),
-                       lambda_min=0.2 * sc.Unit('Angstrom'))
+        10.0 * sc.Unit('ms'), da.bins.coords['event_time_offset'].bins.unit
+    )
+    da = unwrap_frames(
+        da,
+        scatter=True,
+        pulse_period=81.0 * sc.Unit('ms'),
+        frame_offset=0.0 * sc.Unit('ms'),
+        lambda_min=0.2 * sc.Unit('Angstrom'),
+    )
     assert sc.identical(da.bins.coords['tof'], da.bins.attrs['event_time_offset'])
 
 
 def test_unwrap_frames_time_offset_pivot_and_min_define_frames():
     # events [before, after, after, before] pivot point
     time_offset = sc.array(dims=['event'], values=[5.0, 70.0, 21.0, 6.0], unit='ms')
-    da = make_array(pulse_period=71.0 * sc.Unit('ms'),
-                    npixel=1,
-                    nevent=4,
-                    time_offset=time_offset)
-    pivot = sc.to_unit(10.0 * sc.Unit('ms'),
-                       da.bins.coords['event_time_offset'].bins.unit)
+    da = make_array(
+        pulse_period=71.0 * sc.Unit('ms'), npixel=1, nevent=4, time_offset=time_offset
+    )
+    pivot = sc.to_unit(
+        10.0 * sc.Unit('ms'), da.bins.coords['event_time_offset'].bins.unit
+    )
     da.coords['time_offset_pivot'] = pivot
     da.coords['tof_min'] = 200.0 * sc.Unit('ms')
     da.coords['pulse_period'] = 71.0 * sc.Unit('ms')
     da = da.transform_coords('tof', graph=frames.to_tof())
     tof = da.bins.coords['tof'].values[0]
     tof_values = [
         71.0 - 10.0 + 5.0 + 200.0,
@@ -101,124 +115,149 @@
     ]
     assert sc.identical(tof, sc.array(dims=['event'], unit='ms', values=tof_values))
 
 
 def tof_array(*, npixel=3, nevent=1000, pulse_period=None, tof_min=None):
     pulse_period = 71.0 * sc.Unit('ms') if pulse_period is None else pulse_period
     tof_min = 234.0 * sc.Unit('ms') if tof_min is None else tof_min
-    tof = sc.array(dims=['event'], values=np.random.rand(nevent)) * pulse_period.to(
-        unit=tof_min.unit) + tof_min
+    tof = (
+        sc.array(dims=['event'], values=np.random.rand(nevent))
+        * pulse_period.to(unit=tof_min.unit)
+        + tof_min
+    )
     pixel = sc.arange(dim='event', start=0, stop=nevent) % npixel
     events = sc.DataArray(sc.ones(sizes=tof.sizes), coords={'tof': tof, 'pixel': pixel})
     da = events.group(sc.arange(dim='pixel', start=0, stop=npixel, dtype=pixel.dtype))
     da.coords['L1'] = sc.scalar(value=160.0, unit='m')
     da.coords['L2'] = sc.array(dims=['pixel'], values=np.arange(npixel), unit='m')
     return da
 
 
 def tof_to_time_offset(tof, *, pulse_period, frame_offset):
     unit = tof.bins.unit
     return (frame_offset.to(unit=unit) + tof) % pulse_period.to(unit=unit)
 
 
 @pytest.mark.parametrize(
-    "tof_min", [234.0 * sc.Unit('ms'), 37000.0 * sc.Unit('us'), 337.0 * sc.Unit('ms')])
+    "tof_min", [234.0 * sc.Unit('ms'), 37000.0 * sc.Unit('us'), 337.0 * sc.Unit('ms')]
+)
 @pytest.mark.parametrize(
-    "frame_offset", [0.0 * sc.Unit('ms'), 11.0 * sc.Unit('ms'), 9999.0 * sc.Unit('us')])
+    "frame_offset", [0.0 * sc.Unit('ms'), 11.0 * sc.Unit('ms'), 9999.0 * sc.Unit('us')]
+)
 def test_unwrap_frames_reproduces_true_pulses(tof_min, frame_offset):
     from scippneutron.conversion.tof import wavelength_from_tof
+
     pulse_period = 71.0 * sc.Unit('ms')
     # Setup data with known 'tof' coord, which will serve as a reference
     da = tof_array(pulse_period=pulse_period, tof_min=tof_min)
     reference = da.bins.coords['tof'].copy()
     # Compute backwards to "raw" input with 'event_time_offset'. 'tof' coord is removed
-    da.bins.coords['event_time_offset'] = tof_to_time_offset(da.bins.coords.pop('tof'),
-                                                             pulse_period=pulse_period,
-                                                             frame_offset=frame_offset)
-    lambda_min = wavelength_from_tof(tof=tof_min,
-                                     Ltotal=da.coords['L1'] + da.coords['L2'])
-
-    da = unwrap_frames(da,
-                       scatter=True,
-                       pulse_period=pulse_period,
-                       frame_offset=frame_offset,
-                       lambda_min=lambda_min)
+    da.bins.coords['event_time_offset'] = tof_to_time_offset(
+        da.bins.coords.pop('tof'), pulse_period=pulse_period, frame_offset=frame_offset
+    )
+    lambda_min = wavelength_from_tof(
+        tof=tof_min, Ltotal=da.coords['L1'] + da.coords['L2']
+    )
+
+    da = unwrap_frames(
+        da,
+        scatter=True,
+        pulse_period=pulse_period,
+        frame_offset=frame_offset,
+        lambda_min=lambda_min,
+    )
 
     # Should reproduce reference 'tof' within rounding errors
-    assert sc.allclose(da.bins.coords['tof'],
-                       reference,
-                       atol=sc.scalar(1e-12, unit=reference.bins.unit),
-                       rtol=sc.scalar(1e-12))
-
-
-def fake_pulse_skipping_data(*,
-                             npixel=3,
-                             nevent,
-                             nframe,
-                             pulse_period,
-                             pulse_stride: int = 2,
-                             frame_offset,
-                             tof_min):
+    assert sc.allclose(
+        da.bins.coords['tof'],
+        reference,
+        atol=sc.scalar(1e-12, unit=reference.bins.unit),
+        rtol=sc.scalar(1e-12),
+    )
+
+
+def fake_pulse_skipping_data(
+    *,
+    npixel=3,
+    nevent,
+    nframe,
+    pulse_period,
+    pulse_stride: int = 2,
+    frame_offset,
+    tof_min,
+):
     from scippneutron.conversion.tof import wavelength_from_tof
+
     rng = np.random.default_rng(1234)
 
     # Setup data with known 'tof' coord, which will serve as a reference
     frame_period = (pulse_period * pulse_stride).to(unit=tof_min.unit)
     tof = sc.array(dims=['event'], values=rng.random(nevent)) * frame_period + tof_min
     start = sc.datetime('now', unit='ns')
-    time_zero = start + (frame_period * sc.linspace(
-        'event', 0, nframe, num=nevent, dtype='int64')).to(unit='ns', dtype='int64')
+    time_zero = start + (
+        frame_period * sc.linspace('event', 0, nframe, num=nevent, dtype='int64')
+    ).to(unit='ns', dtype='int64')
 
     pixel = sc.arange(dim='event', start=0, stop=nevent) % npixel
     events = sc.DataArray(sc.ones(sizes=tof.sizes), coords={'tof': tof, 'pixel': pixel})
     events.coords['time_zero'] = time_zero
     da = events.group(sc.arange(dim='pixel', start=0, stop=npixel, dtype=pixel.dtype))
     da.coords['L1'] = sc.scalar(value=160.0, unit='m')
     da.coords['L2'] = sc.array(dims=['pixel'], values=np.arange(npixel), unit='m')
     reference = da.copy()
 
     # Compute backwards to "raw" input with 'event_time_offset'. 'tof' coord is removed
-    time_offset = tof_to_time_offset(da.bins.coords.pop('tof'),
-                                     pulse_period=frame_period,
-                                     frame_offset=frame_offset)
+    time_offset = tof_to_time_offset(
+        da.bins.coords.pop('tof'), pulse_period=frame_period, frame_offset=frame_offset
+    )
     event_time_offset = time_offset % pulse_period.to(unit=time_offset.bins.unit)
     da.bins.coords['event_time_offset'] = event_time_offset
     da.bins.coords['event_time_zero'] = da.bins.coords.pop('time_zero') + (
-        time_offset - event_time_offset).to(unit='ns', dtype='int64')
-    lambda_min = wavelength_from_tof(tof=tof_min,
-                                     Ltotal=da.coords['L1'] + da.coords['L2'])
+        time_offset - event_time_offset
+    ).to(unit='ns', dtype='int64')
+    lambda_min = wavelength_from_tof(
+        tof=tof_min, Ltotal=da.coords['L1'] + da.coords['L2']
+    )
     return reference, da, start, lambda_min
 
 
-@given(nevent=st.integers(min_value=0, max_value=10000),
-       nframe=st.integers(min_value=1, max_value=1000000),
-       frame_offset=st.floats(min_value=0.0, max_value=10000.0),
-       tof_min=st.floats(min_value=0.1, max_value=100000.0))
+@given(
+    nevent=st.integers(min_value=0, max_value=10000),
+    nframe=st.integers(min_value=1, max_value=1000000),
+    frame_offset=st.floats(min_value=0.0, max_value=10000.0),
+    tof_min=st.floats(min_value=0.1, max_value=100000.0),
+)
 @pytest.mark.parametrize("pulse_stride", [1, 2, 3, 4, 5])
 def test_unwrap_frames_with_pulse_stride_reproduces_true_pulses(
-        nevent, nframe, tof_min, frame_offset, pulse_stride):
+    nevent, nframe, tof_min, frame_offset, pulse_stride
+):
     frame_offset = frame_offset * sc.Unit('ms')
     tof_min = tof_min * sc.Unit('us')
     pulse_period = 71.0 * sc.Unit('ms')
     # Setup data with known 'tof' coord, which will serve as a reference
     reference, da, first_pulse_time, lambda_min = fake_pulse_skipping_data(
         pulse_period=pulse_period,
         pulse_stride=pulse_stride,
         frame_offset=frame_offset,
         nevent=nevent,
         nframe=nframe,
-        tof_min=tof_min)
+        tof_min=tof_min,
+    )
 
-    da = unwrap_frames(da,
-                       scatter=True,
-                       pulse_period=pulse_period,
-                       pulse_stride=pulse_stride,
-                       first_pulse_time=first_pulse_time,
-                       frame_offset=frame_offset,
-                       lambda_min=lambda_min)
+    da = unwrap_frames(
+        da,
+        scatter=True,
+        pulse_period=pulse_period,
+        pulse_stride=pulse_stride,
+        first_pulse_time=first_pulse_time,
+        frame_offset=frame_offset,
+        lambda_min=lambda_min,
+    )
 
     # Should reproduce reference 'tof' within rounding errors
     expected = reference.bins.coords['tof']
-    assert sc.allclose(da.bins.coords['tof'],
-                       expected,
-                       atol=sc.scalar(1e-9, unit=expected.bins.unit),
-                       rtol=sc.scalar(1e-9))
+    assert sc.allclose(
+        da.bins.coords['tof'],
+        expected,
+        atol=sc.scalar(1e-9, unit=expected.bins.unit),
+        rtol=sc.scalar(1e-9),
+    )
```

### Comparing `scippneutron-23.3.0/tools/make_tutorial_data.ipynb` & `scippneutron-23.4.0/tools/make_tutorial_data.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969494047619047%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, '\\n'), (10, 'for i in [1, 2, 3, 4, 5]:\\n')], delete: "*

 * *            "[9]}}, 1: {'source': {insert: [(1, '\\n')]}}, 2: {'source': {insert: [(2, '\\n'), "*

 * *            '(10, "delta = sc.to_unit(tmax - tmin, \'us\')\\n"), (12, "scale = '*

 * *            'sc.to_unit(da.bins.coords[\'pulse_time\'] - tmin, \'us\') * sc.scalar(\\n"), (13, '*

 * *            '"    1, unit=\'Angstrom/us\'\\n"), (14, \')\\n\'), (15, "da.bins.coords[\'dspacing\'] '*

 * *            '+= 0.02 * scale / delta\ […]*

```diff
@@ -7,65 +7,74 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import scipp as sc\n",
                 "import scippneutron as scn\n",
                 "import urllib.request\n",
+                "\n",
                 "url = 'https://github.com/ess-dmsc-dram/loki_tube_scripts/raw/master/test/test_data/LARMOR00049338.nxs'\n",
                 "filename, _ = urllib.request.urlretrieve(url)\n",
                 "data = scn.load(filename=filename)\n",
                 "edges = sc.array(dims=['tof'], unit='us', values=np.linspace(5.0, 100000.0, num=201))\n",
                 "data = sc.rebin(data, 'tof', edges)\n",
-                "for i in [1,2,3,4,5]:\n",
+                "for i in [1, 2, 3, 4, 5]:\n",
                 "    mon = data.attrs[f'monitor{i}']\n",
                 "    mon.value = sc.rebin(mon.value, 'tof', edges)\n",
                 "data.to_hdf5(filename='loki-at-larmor.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5328874d-f101-43ea-82aa-41f97d360247",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import urllib\n",
+                "\n",
                 "url = 'http://198.74.56.37/ftp/external-data/MD5/d5ae38871d0a09a28ae01f85d969de1e'\n",
                 "filename, _ = urllib.request.urlretrieve(url, filename='PG3_4844_event.nxs')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "71896365-76be-426d-986f-7aeffd8d3acb",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import scipp as sc\n",
                 "import scippneutron as scn\n",
+                "\n",
                 "da = scn.load(filename=f'PG3_4844_event.nxs', load_pulse_times=True)\n",
                 "\n",
                 "# Fake d-spacing shift\n",
                 "da = scn.convert(da, 'tof', 'dspacing', scatter=True)\n",
                 "proton_charge = da.attrs['proton_charge'].value\n",
                 "tmin = proton_charge.coords['time'].min()\n",
                 "tmax = proton_charge.coords['time'].max()\n",
-                "delta = sc.to_unit(tmax-tmin, 'us')\n",
+                "delta = sc.to_unit(tmax - tmin, 'us')\n",
                 "delta.unit = ''\n",
-                "scale = sc.to_unit(da.bins.coords['pulse_time'] - tmin, 'us')* sc.scalar(1, unit='Angstrom/us')\n",
-                "da.bins.coords['dspacing'] += 0.02*scale/delta\n",
+                "scale = sc.to_unit(da.bins.coords['pulse_time'] - tmin, 'us') * sc.scalar(\n",
+                "    1, unit='Angstrom/us'\n",
+                ")\n",
+                "da.bins.coords['dspacing'] += 0.02 * scale / delta\n",
                 "da = scn.convert(da, 'dspacing', 'tof', scatter=True)\n",
                 "da.coords['tof'] = da.coords['tof']['spectrum', 0]\n",
                 "\n",
                 "# Fake prompt pulse\n",
                 "prompt_start = 4000.0 * sc.Unit('us')\n",
                 "prompt_stop = 5000.0 * sc.Unit('us')\n",
                 "tof = da.bins.coords['tof']\n",
-                "da.bins.data *= sc.where((prompt_start <= tof) & (tof < prompt_stop), 1.0+3.0*sc.exp(-(tof-prompt_start)/sc.scalar(200.0, unit='us')), sc.scalar(1.0))\n",
+                "da.bins.data *= sc.where(\n",
+                "    (prompt_start <= tof) & (tof < prompt_stop),\n",
+                "    1.0 + 3.0 * sc.exp(-(tof - prompt_start) / sc.scalar(200.0, unit='us')),\n",
+                "    sc.scalar(1.0),\n",
+                ")\n",
                 "\n",
                 "# Reduce data size to 1/3\n",
                 "da['spectrum', 14100:].to_hdf5(filename='powder-event.h5')"
             ]
         }
     ],
     "metadata": {
```

### Comparing `scippneutron-23.3.0/tox.ini` & `scippneutron-23.4.0/tox.ini`

 * *Files identical despite different names*

