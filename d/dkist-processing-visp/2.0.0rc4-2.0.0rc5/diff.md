# Comparing `tmp/dkist_processing_visp-2.0.0rc4.tar.gz` & `tmp/dkist_processing_visp-2.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.0.0rc4.tar", last modified: Thu Mar 30 21:10:41 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.0.0rc5.tar", last modified: Fri Mar 31 21:38:30 2023, max compression
```

## Comparing `dkist_processing_visp-2.0.0rc4.tar` & `dkist_processing_visp-2.0.0rc5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.728894 dkist_processing_visp-2.0.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    16806 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4692 2023-03-30 21:10:41.728894 dkist_processing_visp-2.0.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4121 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3548 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.720894 dkist_processing_visp-2.0.0rc4/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/changelog/104.misc.rst
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/changelog/105.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/changelog/106.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/changelog/107.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/changelog/108.feature.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/changelog/109.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.720894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.720894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.724894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     9775 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1380 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.724894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.724894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    15383 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    37463 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    23315 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5883 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.724894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10489 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4602 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28203 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6258 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.728894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16085 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6595 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    17704 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    19981 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4490 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)    13735 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    11320 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5633 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11821 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16323 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9696 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5097 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5489 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.728894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp/workflows/single_task_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.720894 dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4692 2023-03-30 21:10:41.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3572 2023-03-30 21:10:41.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-30 21:10:41.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-03-30 21:10:41.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-30 21:10:41.000000 dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.728894 dkist_processing_visp-2.0.0rc4/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/docs/requirements_table.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-30 21:10:41.728894 dkist_processing_visp-2.0.0rc4/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-03-30 21:10:41.732894 dkist_processing_visp-2.0.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-03-30 21:10:36.000000 dkist_processing_visp-2.0.0rc4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    16806 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4692 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4121 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3548 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/104.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/105.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/106.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/107.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/108.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/changelog/109.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.119971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     9775 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1380 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.119971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    15383 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    38179 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    23315 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5883 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4689 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10489 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4602 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28203 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6258 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16085 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    17704 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    19981 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4490 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    13876 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    11320 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5633 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11821 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16323 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9696 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5097 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5489 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.123971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/single_task_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.115971 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4692 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3572 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-31 21:38:30.000000 dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/docs/requirements_table.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-03-31 21:38:30.127971 dkist_processing_visp-2.0.0rc5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-03-31 21:38:22.000000 dkist_processing_visp-2.0.0rc5/setup.py
```

### Comparing `dkist_processing_visp-2.0.0rc4/.gitignore` & `dkist_processing_visp-2.0.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/.pre-commit-config.yaml` & `dkist_processing_visp-2.0.0rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/CHANGELOG.rst` & `dkist_processing_visp-2.0.0rc5/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/PKG-INFO` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist_processing_visp
-Version: 2.0.0rc4
+Name: dkist-processing-visp
+Version: 2.0.0rc5
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.0.0rc4/README.rst` & `dkist_processing_visp-2.0.0rc5/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/bitbucket-pipelines.yml` & `dkist_processing_visp-2.0.0rc5/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/check_changelog_updated.sh` & `dkist_processing_visp-2.0.0rc5/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/spectral_line.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/spectral_line.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/geometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,53 +357,64 @@
         angle_list = []
         for modstate in range(1, self.constants.num_modstates + 1):
             data = self.basic_corrected_lamp_data(beam=beam, modstate=modstate)
             angle = self._compute_single_modstate_angle(data)
             logger.info(f"Angle for {beam = } and {modstate = } = {np.rad2deg(angle):0.4f} deg")
             angle_list.append(angle)
 
-        theta = float(np.mean(angle_list))
+        theta = float(np.nanmedian(angle_list))
         logger.info(f"Beam angle for {beam = }: {np.rad2deg(theta):0.4f} deg")
         return theta
 
     def _compute_single_modstate_angle(self, array: np.ndarray) -> float:
         """
         Compute the angle of a single array.
 
         The angle is computed by simply looking at the slope of the two hairlines. The hairlines are identified
         by fitting a Gaussian to each spectral pixel based on an initial guess from the center of mass of a binarized
         image.
         """
+        # Compute the optimal number of Otsu iterations on the full array (instead of each individual hairline region)
+        # so that the signals of the strong, but narrow hairlines combine to increase hairline SNR.
+        ideal_num_otsu = self._compute_ideal_num_otsu(
+            array, max_num_otsu=self.parameters.geo_max_num_otsu
+        )
+        logger.info(f"Ideal number of Otsu iterations is {ideal_num_otsu} ")
+
         # The 2 hairlines aren't exactly centered in these regions, but we don't care because we'll find the rough
         # locations with a center of mass below.
         half_idx = array.shape[1] // 2
         hairline_1_region = array[:, :half_idx]
         hairline_2_region = array[:, half_idx:]
 
         angles = []
         for h, data in enumerate([hairline_1_region, hairline_2_region], start=1):
-            ideal_num_otsu = self._compute_ideal_num_otsu(
-                data, max_num_otsu=self.parameters.geo_max_num_otsu
-            )
-            logger.info(f"Hairline region {h} has {ideal_num_otsu = } ")
-
             # binary will be 1 on the hairlines and 0 elsewhere
             binary = make_binary(data, ideal_num_otsu)
             wave_size, spatial_size = data.shape
             wave_x = np.arange(wave_size)
             spatial_x = np.arange(spatial_size)
 
             # Calculate the center of mass (COM) of the hairline for each spectral pixel. These will be the initial
             # guesses. (The [None, :] and axis=1 allow us to compute the COM for all spectral pixels at once, so
             # hailine_COM will have shape (wave_size, )).
             hairline_COM = np.sum(spatial_x[None, :] * binary, axis=1) / np.sum(binary, axis=1)
 
             # Now refine hairline center with a gaussian fit at each spectral pixel
-            hairline_centers = np.zeros(wave_size)
+            #
+            # Initialize gaussian fit centers with NaN so any bad pixels can easily be ignored during the line fit.
+            hairline_centers = np.zeros(wave_size) * np.nan
             for i in range(wave_size):
+                if np.isnan(hairline_COM[i]):
+                    # NaNs happen when there's no identified hairline pixels at all for a particular spectral pixel.
+                    logger.info(
+                        f"Hairline region {h} and spectral pixel {i} has a NaN initial guess. Ignoring pixel in line fit."
+                    )
+                    continue
+
                 x0 = int(hairline_COM[i])
                 fit_slice = slice(
                     x0 - self.parameters.geo_hairline_fit_width_px,
                     x0 + self.parameters.geo_hairline_fit_width_px,
                 )
                 hairline_profile = data[i, fit_slice]
                 abscissa = spatial_x[fit_slice]
@@ -422,15 +433,15 @@
                         p0=[a0, x0, sig0, bg0, slope0],
                     )[0]
                     fit_center = fit_pars[1]
                 except RuntimeError:
                     logger.info(
                         f"Hairline fit in hairline region {h} and pixel {i} failed. Ignoring pixel in line fit."
                     )
-                    fit_center = np.nan
+                    continue
 
                 hairline_centers[i] = fit_center
 
             # Fit the hairlines with a simple line
             non_nan_idx = ~np.isnan(hairline_centers)
             coeffs = np.polyfit(wave_x[non_nan_idx], hairline_centers[non_nan_idx], 1)
```

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/e2e_helpers.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/e2e_test.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_geometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,16 @@
                     true_solar = 10 * (np.ones(array_shape[1:]) + modstate + beam)
                     translated_solar = next(
                         transform.translate_arrays(
                             arrays=true_solar, translation=task.offsets[beam - 1][modstate - 1]
                         )
                     )
                     translated_solar[translated_solar == 0] = 10 * (modstate + beam + 1)
+
+                    # Hairlines
                     translated_solar[:, 30] = 5.0
                     translated_solar[:, 70] = 5.0
                     distorted_solar = next(
                         transform.rotate_arrays_about_point(
                             arrays=translated_solar, angle=task.angles[beam - 1]
                         )
                     )
@@ -117,19 +119,22 @@
                     true_lamp = 10 * (np.ones(array_shape[1:]) + modstate + beam)
                     translated_lamp = next(
                         transform.translate_arrays(
                             arrays=true_lamp, translation=task.offsets[beam - 1][modstate - 1]
                         )
                     )
                     translated_lamp[translated_lamp == 0] = 10 * (modstate + beam + 1)
-                    translated_lamp[:, 7] = 5.0
-                    translated_lamp[:, 21] = 5.0
+
+                    # Hairlines
+                    translated_lamp[:, 30] = 5.0
+                    translated_lamp[:, 70] = 5.0
+                    translated_lamp[5:15, 70] = 10 * (modstate + beam + 1)
                     distorted_lamp = next(
                         transform.rotate_arrays_about_point(
-                            arrays=translated_solar, angle=task.angles[beam - 1]
+                            arrays=translated_lamp, angle=task.angles[beam - 1]
                         )
                     )
                     raw_lamp = distorted_lamp + raw_dark
                     lamp_hdul = generate_214_l0_fits_frame(data=raw_lamp, s122_header=lamp_header)
                     task.fits_data_write(
                         hdu_list=lamp_hdul,
                         tags=[
```

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.0.0rc5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist-processing-visp
-Version: 2.0.0rc4
+Name: dkist_processing_visp
+Version: 2.0.0rc5
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.0.0rc5/dkist_processing_visp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/docs/Makefile` & `dkist_processing_visp-2.0.0rc5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/docs/background_light.rst` & `dkist_processing_visp-2.0.0rc5/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/docs/conf.py` & `dkist_processing_visp-2.0.0rc5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.0.0rc5/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/docs/make.bat` & `dkist_processing_visp-2.0.0rc5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/licenses/LICENSE.rst` & `dkist_processing_visp-2.0.0rc5/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/pyproject.toml` & `dkist_processing_visp-2.0.0rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.0.0rc4/setup.cfg` & `dkist_processing_visp-2.0.0rc5/setup.cfg`

 * *Files identical despite different names*

