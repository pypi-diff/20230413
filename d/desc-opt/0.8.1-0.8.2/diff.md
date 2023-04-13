# Comparing `tmp/desc-opt-0.8.1.tar.gz` & `tmp/desc-opt-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "desc-opt-0.8.1.tar", last modified: Fri Mar 17 23:28:34 2023, max compression
+gzip compressed data, was "desc-opt-0.8.2.tar", last modified: Thu Apr 13 10:59:21 2023, max compression
```

## Comparing `desc-opt-0.8.1.tar` & `desc-opt-0.8.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.332149 desc-opt-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-17 23:27:31.000000 desc-opt-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-17 23:27:31.000000 desc-opt-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-03-17 23:28:34.332149 desc-opt-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-03-17 23:27:31.000000 desc-opt-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.332149 desc-opt-0.8.1/desc/
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-17 23:28:34.332149 desc-opt-0.8.1/desc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    44961 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/coils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.292148 desc-opt-0.8.1/desc/compute/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18361 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_basis_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_equil.py
--rw-r--r--   0 runner    (1001) docker     (123)    78741 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20829 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    25271 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_qs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/data_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    25508 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/compute/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16566 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/continuation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/derivatives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.292148 desc-opt-0.8.1/desc/equilibrium/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/equilibrium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44938 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/equilibrium/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/equilibrium/coords.py
--rw-r--r--   0 runner    (1001) docker     (123)    38627 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/equilibrium/equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/equilibrium/initial_guess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/equilibrium/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.320149 desc-opt-0.8.1/desc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  2781266 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/ARIES-CS_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1854489 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/ATF_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/DSHAPE_CURRENT_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/DSHAPE_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1515598 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/ESTELL_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1003793 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/HELIOTRON_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  3109450 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/NCSX_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  2669839 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/QAS_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)   650984 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/SOLOVEV_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  3500803 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/W7-X_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1942753 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/WISTELL-A_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/precise_QA.py
--rw-r--r--   0 runner    (1001) docker     (123)  4020724 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/precise_QA_output.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/precise_QH.py
--rw-r--r--   0 runner    (1001) docker     (123)  4017915 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/examples/precise_QH_output.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.324149 desc-opt-0.8.1/desc/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/geometry/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    40658 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/geometry/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    35071 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/geometry/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/geometry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35160 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.324149 desc-opt-0.8.1/desc/io/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/io/ascii_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/io/core_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/io/equilibrium_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/io/hdf5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    55967 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/io/input_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/io/pickle_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    24850 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/magnetic_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.324149 desc-opt-0.8.1/desc/objectives/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29224 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    14989 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    25650 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/_qs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)    77854 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/linear_objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/nae_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26756 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/objective_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13834 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/objectives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.328149 desc-opt-0.8.1/desc/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20441 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/_constraint_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/_desc_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/_scipy_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/fmin_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/least_squares.py
--rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/tr_subproblems.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/optimize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25751 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/perturbations.py
--rw-r--r--   0 runner    (1001) docker     (123)   123146 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    43789 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    29582 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    59530 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/vmec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-03-17 23:27:31.000000 desc-opt-0.8.1/desc/vmec_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.328149 desc-opt-0.8.1/desc_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-03-17 23:28:34.000000 desc-opt-0.8.1/desc_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-17 23:28:34.000000 desc-opt-0.8.1/desc_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 23:28:34.000000 desc-opt-0.8.1/desc_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-17 23:28:34.000000 desc-opt-0.8.1/desc_opt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-17 23:28:34.000000 desc-opt-0.8.1/desc_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-17 23:28:34.000000 desc-opt-0.8.1/desc_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-17 23:27:31.000000 desc-opt-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-17 23:28:34.332149 desc-opt-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-17 23:27:31.000000 desc-opt-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 23:28:34.332149 desc-opt-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)    56948 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_coils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35072 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_compute_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_compute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_constrain_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    23693 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_input_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    27137 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_linear_objectives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_magnetic_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_objective_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13895 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_perturbations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25689 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_stability_funs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    21693 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-03-17 23:27:32.000000 desc-opt-0.8.1/tests/test_vmec.py
--rw-r--r--   0 runner    (1001) docker     (123)    68590 2023-03-17 23:27:32.000000 desc-opt-0.8.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.784757 desc-opt-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-13 10:58:10.000000 desc-opt-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 10:58:10.000000 desc-opt-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-13 10:59:21.784757 desc-opt-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-13 10:58:10.000000 desc-opt-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.784757 desc-opt-0.8.2/desc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 10:59:21.784757 desc-opt-0.8.2/desc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44961 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/coils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.724754 desc-opt-0.8.2/desc/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18361 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_basis_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_equil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80058 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10129 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45013 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25271 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_qs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/data_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25508 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/compute/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24391 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/continuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18594 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/derivatives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.728754 desc-opt-0.8.2/desc/equilibrium/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/equilibrium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44938 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/equilibrium/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/equilibrium/coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38401 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/equilibrium/equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11150 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/equilibrium/initial_guess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/equilibrium/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.764756 desc-opt-0.8.2/desc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)  2781266 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/ARIES-CS_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1854489 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/ATF_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/DSHAPE_CURRENT_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   974880 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/DSHAPE_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1515598 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/ESTELL_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1003793 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/HELIOTRON_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  3109450 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/NCSX_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  2669839 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/QAS_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   650984 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/SOLOVEV_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  3500803 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/W7-X_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1942753 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/WISTELL-A_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/precise_QA.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4020724 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/precise_QA_output.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/precise_QH.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4017915 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/examples/precise_QH_output.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.768756 desc-opt-0.8.2/desc/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/geometry/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40845 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/geometry/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35258 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/geometry/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/geometry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38623 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.772756 desc-opt-0.8.2/desc/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/io/ascii_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/io/core_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/io/equilibrium_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/io/hdf5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54732 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/io/input_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/io/pickle_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24850 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/magnetic_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.776756 desc-opt-0.8.2/desc/objectives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29439 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15247 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25695 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21241 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/_qs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13156 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/_stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81717 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/linear_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/nae_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27241 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/objective_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/objectives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.776756 desc-opt-0.8.2/desc/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22438 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/_constraint_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/_desc_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/_scipy_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/fmin_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/least_squares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/tr_subproblems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/optimize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27420 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121835 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43789 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29582 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59646 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/vmec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-04-13 10:58:10.000000 desc-opt-0.8.2/desc/vmec_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.776756 desc-opt-0.8.2/desc_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-13 10:59:21.000000 desc-opt-0.8.2/desc_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-13 10:59:21.000000 desc-opt-0.8.2/desc_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 10:59:21.000000 desc-opt-0.8.2/desc_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-13 10:59:21.000000 desc-opt-0.8.2/desc_opt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-13 10:59:21.000000 desc-opt-0.8.2/desc_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 10:59:21.000000 desc-opt-0.8.2/desc_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-13 10:58:10.000000 desc-opt-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-13 10:59:21.784757 desc-opt-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-13 10:58:10.000000 desc-opt-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 10:59:21.784757 desc-opt-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57032 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_coils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37458 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_compute_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_compute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_constrain_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32467 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_input_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24497 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_linear_objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_magnetic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_objective_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13780 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_perturbations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27108 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14773 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_stability_funs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21693 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26178 2023-04-13 10:58:11.000000 desc-opt-0.8.2/tests/test_vmec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68590 2023-04-13 10:58:11.000000 desc-opt-0.8.2/versioneer.py
```

### Comparing `desc-opt-0.8.1/LICENSE` & `desc-opt-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/PKG-INFO` & `desc-opt-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desc-opt
-Version: 0.8.1
+Version: 0.8.2
 Summary: Computes, analyzes and optimizes 3D MHD equilibria for stellarators and tokamaks
 Home-page: https://github.com/PlasmaControl/DESC/
 Author: Daniel Dudt, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Project-URL: Issues Tracker, https://github.com/PlasmaControl/DESC/issues
 Project-URL: Contributing, https://github.com/PlasmaControl/DESC/blob/master/CONTRIBUTING.rst
@@ -28,26 +28,24 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/PlasmaControl/DESC/master/docs/_static/images/logo_med_clear.png
 
 .. inclusion-marker-do-not-remove
 
-##############################
-Stellarator Equilibrium Solver
-##############################
+################################
+Stellarator Optimization Package
+################################
 |License| |DOI| |Issues| |Pypi|
 
 |Docs| |UnitTests| |RegressionTests| |Codecov|
 
-DESC computes 3D MHD equilibria by solving the force balance equations.
-It can also be used for perturbation analysis and sensitivity studies to see how the equilibria change as input parameters are varied.
+DESC solves for and optimizes 3D MHD equilibria using pseudo-spectral numerical methods and automatic differentiation.
 
-The theoretical approach and numerical methods used by DESC are presented in these papers [1]_ [2]_ [3]_ [4]_
-and documented at Theory_.
+The theoretical approach and implementation details used by DESC are presented in these papers [1]_ [2]_ [3]_ [4]_ and documented at Theory_.
 Please cite our work if you use DESC!
 
 .. [1] Dudt, D. & Kolemen, E. (2020). DESC: A Stellarator Equilibrium Solver. [`Physics of Plasmas <https://aip.scitation.org/doi/full/10.1063/5.0020743>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/master/docs/Dudt_Kolemen_PoP_2020.pdf>`__]
 .. [2] Panici, D. et al (2022). The DESC Stellarator Code Suite Part I: Quick and accurate equilibria computations. [`arxiv <https://arxiv.org/abs/2203.17173>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/panici2022/panici2022equilibria.pdf>`__]
 .. [3] Conlin, R. et al. (2022). The DESC Stellarator Code Suite Part II: Perturbation and continuation methods. [`arxiv <https://arxiv.org/abs/2203.15927>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/conlin2022/conlin2022perturbations.pdf>`__]
 .. [4] Dudt, D. et al. (2022). The DESC Stellarator Code Suite Part III: Quasi-symmetry optimization. [`arxiv <https://arxiv.org/abs/2204.00078>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/dudt2022/dudt2022optimization.pdf>`__]
 .. _Theory: https://desc-docs.readthedocs.io/en/latest/theory_general.html
```

### Comparing `desc-opt-0.8.1/README.rst` & `desc-opt-0.8.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 .. image:: https://raw.githubusercontent.com/PlasmaControl/DESC/master/docs/_static/images/logo_med_clear.png
 
 .. inclusion-marker-do-not-remove
 
-##############################
-Stellarator Equilibrium Solver
-##############################
+################################
+Stellarator Optimization Package
+################################
 |License| |DOI| |Issues| |Pypi|
 
 |Docs| |UnitTests| |RegressionTests| |Codecov|
 
-DESC computes 3D MHD equilibria by solving the force balance equations.
-It can also be used for perturbation analysis and sensitivity studies to see how the equilibria change as input parameters are varied.
+DESC solves for and optimizes 3D MHD equilibria using pseudo-spectral numerical methods and automatic differentiation.
 
-The theoretical approach and numerical methods used by DESC are presented in these papers [1]_ [2]_ [3]_ [4]_
-and documented at Theory_.
+The theoretical approach and implementation details used by DESC are presented in these papers [1]_ [2]_ [3]_ [4]_ and documented at Theory_.
 Please cite our work if you use DESC!
 
 .. [1] Dudt, D. & Kolemen, E. (2020). DESC: A Stellarator Equilibrium Solver. [`Physics of Plasmas <https://aip.scitation.org/doi/full/10.1063/5.0020743>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/master/docs/Dudt_Kolemen_PoP_2020.pdf>`__]
 .. [2] Panici, D. et al (2022). The DESC Stellarator Code Suite Part I: Quick and accurate equilibria computations. [`arxiv <https://arxiv.org/abs/2203.17173>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/panici2022/panici2022equilibria.pdf>`__]
 .. [3] Conlin, R. et al. (2022). The DESC Stellarator Code Suite Part II: Perturbation and continuation methods. [`arxiv <https://arxiv.org/abs/2203.15927>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/conlin2022/conlin2022perturbations.pdf>`__]
 .. [4] Dudt, D. et al. (2022). The DESC Stellarator Code Suite Part III: Quasi-symmetry optimization. [`arxiv <https://arxiv.org/abs/2204.00078>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/dudt2022/dudt2022optimization.pdf>`__]
 .. _Theory: https://desc-docs.readthedocs.io/en/latest/theory_general.html
```

### Comparing `desc-opt-0.8.1/desc/__init__.py` & `desc-opt-0.8.2/desc/__init__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/__main__.py` & `desc-opt-0.8.2/desc/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,41 +20,60 @@
     import desc
 
     if ir.args.verbose:
         print(desc.BANNER)
 
     import matplotlib.pyplot as plt
 
-    from desc.equilibrium import EquilibriaFamily
+    from desc.equilibrium import EquilibriaFamily, Equilibrium
     from desc.plotting import plot_section, plot_surfaces
 
     if ir.args.verbose:
         print("Reading input from {}".format(ir.input_path))
         print("Outputs will be written to {}".format(ir.output_path))
 
-    # initialize
     inputs = ir.inputs
-    equil_fam = EquilibriaFamily(inputs)
-    # check vmec path input
-    if ir.args.guess is not None:
-        if ir.args.verbose:
-            print("Initial guess from {}".format(ir.args.guess))
-        equil_fam[0].set_initial_guess(ir.args.guess)
-    # solve equilibrium
-    equil_fam.solve_continuation(
-        objective=inputs[0]["objective"],
-        optimizer=inputs[0]["optimizer"],
-        pert_order=[inp["pert_order"] for inp in inputs],
-        ftol=[inp["ftol"] for inp in inputs],
-        xtol=[inp["xtol"] for inp in inputs],
-        gtol=[inp["gtol"] for inp in inputs],
-        nfev=[inp["nfev"] for inp in inputs],
-        verbose=ir.args.verbose,
-        checkpoint_path=ir.output_path,
-    )
+    if (
+        len(inputs) == 1
+        and (inputs[-1]["pres_ratio"] is None)
+        and (inputs[-1]["bdry_ratio"] is None)
+    ):
+        eq = Equilibrium(**inputs[-1])
+        equil_fam = EquilibriaFamily.solve_continuation_automatic(
+            eq,
+            objective=inputs[-1]["objective"],
+            optimizer=inputs[-1]["optimizer"],
+            pert_order=inputs[-1]["pert_order"],
+            ftol=inputs[-1]["ftol"],
+            xtol=inputs[-1]["xtol"],
+            gtol=inputs[-1]["gtol"],
+            nfev=inputs[-1]["nfev"],
+            verbose=ir.args.verbose,
+            checkpoint_path=ir.output_path,
+        )
+    else:
+        # initialize
+        equil_fam = EquilibriaFamily(inputs)
+        # check vmec path input
+        if ir.args.guess is not None:
+            if ir.args.verbose:
+                print("Initial guess from {}".format(ir.args.guess))
+            equil_fam[0].set_initial_guess(ir.args.guess)
+        # solve equilibrium
+        equil_fam.solve_continuation(
+            objective=inputs[0]["objective"],
+            optimizer=inputs[0]["optimizer"],
+            pert_order=[inp["pert_order"] for inp in inputs],
+            ftol=[inp["ftol"] for inp in inputs],
+            xtol=[inp["xtol"] for inp in inputs],
+            gtol=[inp["gtol"] for inp in inputs],
+            nfev=[inp["nfev"] for inp in inputs],
+            verbose=ir.args.verbose,
+            checkpoint_path=ir.output_path,
+        )
 
     if ir.args.plot > 1:
         for i, eq in enumerate(equil_fam[:-1]):
             print("Plotting solution at step {}".format(i + 1))
             _ = plot_surfaces(eq)
             plt.show()
             _ = plot_section(eq, "|F|", log=True, norm_F=True)
```

### Comparing `desc-opt-0.8.1/desc/backend.py` & `desc-opt-0.8.2/desc/backend.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/basis.py` & `desc-opt-0.8.2/desc/basis.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/coils.py` & `desc-opt-0.8.2/desc/coils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compat.py` & `desc-opt-0.8.2/desc/compat.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/__init__.py` & `desc-opt-0.8.2/desc/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/_basis_vectors.py` & `desc-opt-0.8.2/desc/compute/_basis_vectors.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/_bootstrap.py` & `desc-opt-0.8.2/desc/compute/_bootstrap.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/_core.py` & `desc-opt-0.8.2/desc/compute/_core.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/_equil.py` & `desc-opt-0.8.2/desc/compute/_equil.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/_field.py` & `desc-opt-0.8.2/desc/compute/_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -2571,14 +2571,37 @@
     data["|grad(|B|^2)|/2mu0"] = jnp.linalg.norm(data["grad(|B|^2)"], axis=-1) / (
         2 * mu_0
     )
     return data
 
 
 @register_compute_fun(
+    name="<|grad(|B|^2)|/2mu0>_vol",
+    label="\\langle |\\nabla B^{2}/(2\\mu_0)| \\rangle_{vol}",
+    units="N \\cdot m^{-3}",
+    units_long="Newtons per cubic meter",
+    description="Volume average of magnitude of magnetic pressure gradient",
+    dim=0,
+    params=[],
+    transforms={"grid": []},
+    profiles=[],
+    coordinates="",
+    data=["|grad(|B|^2)|/2mu0", "sqrt(g)", "V"],
+)
+def _gradB2mag_vol(params, transforms, profiles, data, **kwargs):
+    data["<|grad(|B|^2)|/2mu0>_vol"] = (
+        jnp.sum(
+            data["|grad(|B|^2)|/2mu0"] * data["sqrt(g)"] * transforms["grid"].weights
+        )
+        / data["V"]
+    )
+    return data
+
+
+@register_compute_fun(
     name="(curl(B)xB)_rho",
     label="((\\nabla \\times \\mathbf{B}) \\times \\mathbf{B})_{\\rho}",
     units="T^{2}",
     units_long="Tesla squared",
     description="Covariant radial component of Lorentz force",
     dim=1,
     params=[],
@@ -2748,14 +2771,35 @@
 )
 def _B_dot_grad_B_mag(params, transforms, profiles, data, **kwargs):
     data["|(B*grad)B|"] = jnp.linalg.norm(data["(B*grad)B"], axis=-1)
     return data
 
 
 @register_compute_fun(
+    name="<|(B*grad)B|>_vol",
+    label="\\langle |(\\mathbf{B} \\cdot \\nabla) \\mathbf{B}| \\rangle_{vol}",
+    units="T^{2} \\cdot m^{-1}",
+    units_long="Tesla squared / meters",
+    description="Volume average magnetic tension magnitude",
+    dim=0,
+    params=[],
+    transforms={"grid": []},
+    profiles=[],
+    coordinates="",
+    data=["|(B*grad)B|", "sqrt(g)", "V"],
+)
+def _B_dot_grad_B_mag_vol(params, transforms, profiles, data, **kwargs):
+    data["<|(B*grad)B|>_vol"] = (
+        jnp.sum(data["|(B*grad)B|"] * data["sqrt(g)"] * transforms["grid"].weights)
+        / data["V"]
+    )
+    return data
+
+
+@register_compute_fun(
     name="B*grad(|B|)",
     label="\\mathbf{B} \\cdot \\nabla B",
     units="T^2 \\cdot m^{-1}",
     units_long="Tesla squared / meters",
     description="",
     dim=1,
     params=[],
```

### Comparing `desc-opt-0.8.1/desc/compute/_geometry.py` & `desc-opt-0.8.2/desc/compute/_geometry.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/_profiles.py` & `desc-opt-0.8.2/desc/compute/_profiles.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/_qs.py` & `desc-opt-0.8.2/desc/compute/_qs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Compute functions for quasisymmetry objectives."""
 
 import numpy as np
 
 from desc.backend import jnp, put, sign
 
 from .data_index import register_compute_fun
+from .utils import cross, dot
 
 
 @register_compute_fun(
     name="B_theta_mn",
     label="B_{\\theta, m, n}",
     units="T \\cdot m}",
     units_long="Tesla * meters",
@@ -350,7 +351,28 @@
 )
 def _f_T(params, transforms, profiles, data, **kwargs):
     data["f_T"] = (data["psi_r"] / data["sqrt(g)"]) * (
         data["|B|_t"] * data["(B*grad(|B|))_z"]
         - data["|B|_z"] * data["(B*grad(|B|))_t"]
     )
     return data
+
+
+@register_compute_fun(
+    name="isodynamicity",
+    label="1/B^2 (\\mathbf{b} \\times \\nabla B) \\cdot \\nabla \\psi",
+    units="~",
+    units_long="None",
+    description="Measure of cross field drift at each point, "
+    + "unweighted by particle energy",
+    dim=1,
+    params=[],
+    transforms={},
+    profiles=[],
+    coordinates="rtz",
+    data=["b", "grad(|B|)", "|B|", "grad(psi)"],
+)
+def _isodynamicity(params, transforms, profiles, data, **kwargs):
+    data["isodynamicity"] = (
+        dot(cross(data["b"], data["grad(|B|)"]), data["grad(psi)"]) / data["|B|"] ** 2
+    )
+    return data
```

### Comparing `desc-opt-0.8.1/desc/compute/_stability.py` & `desc-opt-0.8.2/desc/compute/_stability.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/data_index.py` & `desc-opt-0.8.2/desc/compute/data_index.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/compute/utils.py` & `desc-opt-0.8.2/desc/compute/utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/derivatives.py` & `desc-opt-0.8.2/desc/derivatives.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/equilibrium/configuration.py` & `desc-opt-0.8.2/desc/equilibrium/configuration.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/equilibrium/coords.py` & `desc-opt-0.8.2/desc/equilibrium/coords.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/equilibrium/equilibrium.py` & `desc-opt-0.8.2/desc/equilibrium/equilibrium.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,15 +339,15 @@
             if N == np.inf:
                 N = int((na_eq.nphi - 1) / 2)
 
             if ntheta is None:
                 ntheta = 2 * M + 1
 
             inputs = {}
-            inputs["Psi"] = np.pi * r**2 * na_eq.spsi * na_eq.Bbar
+            inputs["Psi"] = np.pi * r**2 * na_eq.Bbar
             inputs["NFP"] = na_eq.nfp
             inputs["L"] = L
             inputs["M"] = M
             inputs["N"] = N
             inputs["sym"] = not na_eq.lasym
             inputs["spectral_indexing "] = spectral_indexing
             inputs["pressure"] = np.array(
@@ -363,15 +363,15 @@
             inputs["surface"] = None
         except AttributeError as e:
             raise ValueError("Input must be a pyQSC or pyQIC solution.") from e
 
         rho, _ = special.js_roots(L, 2, 2)
         # TODO: could make this an OCS grid to improve fitting, need to figure out
         # how concentric grids work with QSC
-        grid = LinearGrid(rho=rho, theta=ntheta, zeta=na_eq.nphi, NFP=na_eq.nfp)
+        grid = LinearGrid(rho=rho, theta=ntheta, zeta=na_eq.phi, NFP=na_eq.nfp)
         basis_R = FourierZernikeBasis(
             L=L,
             M=M,
             N=N,
             NFP=na_eq.nfp,
             sym="cos" if not na_eq.lasym else False,
             spectral_indexing=spectral_indexing,
@@ -428,15 +428,15 @@
         constraints=None,
         optimizer="lsq-exact",
         ftol=None,
         xtol=None,
         gtol=None,
         maxiter=50,
         x_scale="auto",
-        options={},
+        options=None,
         verbose=1,
         copy=False,
     ):
         """Solve to find the equilibrium configuration.
 
         Parameters
         ----------
@@ -546,15 +546,15 @@
         constraints=None,
         optimizer="proximal-lsq-exact",
         ftol=None,
         xtol=None,
         gtol=None,
         maxiter=50,
         x_scale="auto",
-        options={},
+        options=None,
         verbose=1,
         copy=False,
     ):
         """Optimize an equilibrium for an objective.
 
         Parameters
         ----------
@@ -856,20 +856,14 @@
             objective = get_equilibrium_objective()
         if constraints is None:
             constraints = get_fixed_boundary_constraints(
                 iota=self.iota is not None,
                 kinetic=self.electron_temperature is not None,
             )
 
-        if not objective.built:
-            objective.build(self, verbose=verbose)
-        for constraint in constraints:
-            if not constraint.built:
-                constraint.build(self, verbose=verbose)
-
         eq = perturb(
             self,
             objective,
             constraints,
             deltas,
             order=order,
             tr_ratio=tr_ratio,
```

### Comparing `desc-opt-0.8.1/desc/equilibrium/initial_guess.py` & `desc-opt-0.8.2/desc/equilibrium/initial_guess.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/equilibrium/utils.py` & `desc-opt-0.8.2/desc/equilibrium/utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/ARIES-CS_output.h5` & `desc-opt-0.8.2/desc/examples/ARIES-CS_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/ATF_output.h5` & `desc-opt-0.8.2/desc/examples/ATF_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/DSHAPE_CURRENT_output.h5` & `desc-opt-0.8.2/desc/examples/DSHAPE_CURRENT_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/DSHAPE_output.h5` & `desc-opt-0.8.2/desc/examples/DSHAPE_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/ESTELL_output.h5` & `desc-opt-0.8.2/desc/examples/ESTELL_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/HELIOTRON_output.h5` & `desc-opt-0.8.2/desc/examples/HELIOTRON_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/NCSX_output.h5` & `desc-opt-0.8.2/desc/examples/NCSX_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/QAS_output.h5` & `desc-opt-0.8.2/desc/examples/QAS_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/SOLOVEV_output.h5` & `desc-opt-0.8.2/desc/examples/SOLOVEV_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/W7-X_output.h5` & `desc-opt-0.8.2/desc/examples/W7-X_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/WISTELL-A_output.h5` & `desc-opt-0.8.2/desc/examples/WISTELL-A_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/__init__.py` & `desc-opt-0.8.2/desc/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/precise_QA.py` & `desc-opt-0.8.2/desc/examples/precise_QA.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/precise_QA_output.h5` & `desc-opt-0.8.2/desc/examples/precise_QA_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/precise_QH.py` & `desc-opt-0.8.2/desc/examples/precise_QH.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/examples/precise_QH_output.h5` & `desc-opt-0.8.2/desc/examples/precise_QH_output.h5`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/geometry/core.py` & `desc-opt-0.8.2/desc/geometry/core.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/geometry/curve.py` & `desc-opt-0.8.2/desc/geometry/curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,18 @@
         ):
             self._NFP = NFP if NFP is not None else self.NFP
             N = N if N is not None else self.N
             R_modes_old = self.R_basis.modes
             Z_modes_old = self.Z_basis.modes
             self.R_basis.change_resolution(N=N, NFP=self.NFP)
             self.Z_basis.change_resolution(N=N, NFP=self.NFP)
+            if hasattr(self.grid, "change_resolution"):
+                self.grid.change_resolution(
+                    self.grid.L, self.grid.M, self.grid.N, self.NFP
+                )
             self._R_transform, self._Z_transform = self._get_transforms(self.grid)
             self.R_n = copy_coeffs(self.R_n, R_modes_old, self.R_basis.modes)
             self.Z_n = copy_coeffs(self.Z_n, Z_modes_old, self.Z_basis.modes)
 
     def get_coeffs(self, n):
         """Get Fourier coefficients for given mode number(s)."""
         n = np.atleast_1d(n).astype(int)
```

### Comparing `desc-opt-0.8.1/desc/geometry/surface.py` & `desc-opt-0.8.2/desc/geometry/surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,18 @@
         ):
             M = M if M is not None else self.M
             N = N if N is not None else self.N
             R_modes_old = self.R_basis.modes
             Z_modes_old = self.Z_basis.modes
             self.R_basis.change_resolution(M=M, N=N, NFP=self.NFP)
             self.Z_basis.change_resolution(M=M, N=N, NFP=self.NFP)
+            if hasattr(self.grid, "change_resolution"):
+                self.grid.change_resolution(
+                    self.grid.L, self.grid.M, self.grid.N, self.NFP
+                )
             self._R_transform, self._Z_transform = self._get_transforms(self.grid)
             self.R_lmn = copy_coeffs(self.R_lmn, R_modes_old, self.R_basis.modes)
             self.Z_lmn = copy_coeffs(self.Z_lmn, Z_modes_old, self.Z_basis.modes)
             self._M = M
             self._N = N
 
     @property
```

### Comparing `desc-opt-0.8.1/desc/geometry/utils.py` & `desc-opt-0.8.2/desc/geometry/utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/grid.py` & `desc-opt-0.8.2/desc/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,58 +49,77 @@
     def __init__(self, nodes, sort=True):
         self._NFP = 1
         self._sym = False
         self._node_pattern = "custom"
 
         self._nodes, self._spacing = self._create_nodes(nodes)
 
-        dtheta_scale = self._enforce_symmetry()
+        self._enforce_symmetry()
         if sort:
             self._sort_nodes()
         self._find_axis()
         self._count_nodes()
-        self._scale_weights(dtheta_scale)
+        self._scale_weights()
 
     def _enforce_symmetry(self):
         """Enforce stellarator symmetry.
 
         1. Remove nodes with theta > pi.
         2. Rescale theta spacing to preserve dtheta weight.
             Need to rescale on each theta coordinate curve by a different factor.
-            dtheta should = 2pi / number of nodes remaining on that theta curve
-
-        Returns
-        -------
-        dtheta_scale : ndarray
-            The multiplicative factor to scale the theta spacing for each theta curve.
-                number of nodes / (number of nodes - number of nodes to delete)
+            dtheta should = 2pi / number of nodes remaining on that theta curve.
+            Nodes on the symmetry line should not be rescaled.
 
         """
         if self.sym:
-            non_sym_idx = np.where(self.nodes[:, 1] > np.pi)
-            __, inverse, nodes_per_rho_surf = np.unique(
-                self.nodes[:, 0], return_inverse=True, return_counts=True
+            # indices where theta coordinate is off the symmetry line of theta=0 or pi
+            off_sym_line_idx = np.where(self.nodes[:, 1] % np.pi != 0)[0]
+            __, inverse, off_sym_line_per_rho_surf_count = np.unique(
+                self.nodes[off_sym_line_idx, 0], return_inverse=True, return_counts=True
+            )
+            # indices of nodes to be deleted
+            to_delete_idx = np.where(self.nodes[:, 1] > np.pi)[0]
+            __, to_delete_per_rho_surf_count = np.unique(
+                self.nodes[to_delete_idx, 0], return_counts=True
             )
-            __, non_sym_per_rho_surf = np.unique(
-                self.nodes[non_sym_idx, 0], return_counts=True
+            assert (
+                2 * np.pi not in self.nodes[:, 1]
+                and off_sym_line_per_rho_surf_count.size
+                >= to_delete_per_rho_surf_count.size
             )
-            if len(nodes_per_rho_surf) > len(non_sym_per_rho_surf):
+            if off_sym_line_per_rho_surf_count.size > to_delete_per_rho_surf_count.size:
                 # edge case where surfaces closest to axis lack theta > pi nodes
-                pad_count = len(nodes_per_rho_surf) - len(non_sym_per_rho_surf)
-                non_sym_per_rho_surf = np.pad(non_sym_per_rho_surf, (pad_count, 0))
-            # assumes number of theta nodes to delete is constant over zeta
-            scale = nodes_per_rho_surf / (nodes_per_rho_surf - non_sym_per_rho_surf)
-            # arrange scale factors to match spacing's arbitrary ordering
+                # The number of nodes to delete on those surfaces is zero.
+                pad_count = (
+                    off_sym_line_per_rho_surf_count.size
+                    - to_delete_per_rho_surf_count.size
+                )
+                to_delete_per_rho_surf_count = np.pad(
+                    to_delete_per_rho_surf_count, (pad_count, 0)
+                )
+            # The computation of this scale factor assumes
+            # 1. number of nodes to delete is constant over zeta
+            # 2. number of nodes off symmetry line is constant over zeta
+            # 3. uniform theta spacing between nodes
+            # The first two assumptions let _per_theta_curve = _per_rho_surf.
+            # The third assumption lets the scale factor be constant over a
+            # particular theta curve, so that each node in the open interval
+            # (0, pi) has its spacing scaled up by the same factor.
+            # Nodes at endpoints 0, pi should not be scaled.
+            scale = off_sym_line_per_rho_surf_count / (
+                off_sym_line_per_rho_surf_count - to_delete_per_rho_surf_count
+            )
+            # Arrange scale factors to match spacing's arbitrary ordering.
             scale = scale[inverse]
 
-            self._spacing[:, 1] *= scale
-            self._nodes = np.delete(self.nodes, non_sym_idx, axis=0)
-            self._spacing = np.delete(self.spacing, non_sym_idx, axis=0)
-            return np.delete(scale, non_sym_idx)
-        return 1
+            # Scale up all nodes so that their spacing accounts for the node
+            # that is their reflection across the symmetry line.
+            self._spacing[off_sym_line_idx, 1] *= scale
+            self._nodes = np.delete(self.nodes, to_delete_idx, axis=0)
+            self._spacing = np.delete(self.spacing, to_delete_idx, axis=0)
 
     def _sort_nodes(self):
         """Sort nodes for use with FFT."""
         sort_idx = np.lexsort((self.nodes[:, 1], self.nodes[:, 0], self.nodes[:, 2]))
         self._nodes = self.nodes[sort_idx]
         self._spacing = self.spacing[sort_idx]
 
@@ -119,35 +138,26 @@
         __, self._unique_zeta_idx, self._inverse_zeta_idx = np.unique(
             self.nodes[:, 2], return_index=True, return_inverse=True
         )
         self._num_rho = self._unique_rho_idx.size
         self._num_theta = self._unique_theta_idx.size
         self._num_zeta = self._unique_zeta_idx.size
 
-    def _scale_weights(self, dtheta_scale):
-        """Scale weights sum to full volume and reduce weights for duplicated nodes.
-
-        Parameters
-        ----------
-        dtheta_scale : ndarray
-            The multiplicative factor to scale the theta spacing for each theta curve.
-
-        """
+    def _scale_weights(self):
+        """Scale weights sum to full volume and reduce duplicate node weights."""
         nodes = self.nodes.copy().astype(float)
         nodes[:, 1] %= 2 * np.pi
         nodes[:, 2] %= 2 * np.pi / self.NFP
         # reduce weights for duplicated nodes
         _, inverse, counts = np.unique(
             nodes, axis=0, return_inverse=True, return_counts=True
         )
         duplicates = np.tile(np.atleast_2d(counts[inverse]).T, 3)
         temp_spacing = np.copy(self.spacing)
         temp_spacing /= duplicates ** (1 / 3)
-        # assign weights pretending _enforce_symmetry didn't change theta spacing
-        temp_spacing[:, 1] /= dtheta_scale
         # scale weights sum to full volume
         temp_spacing *= (4 * np.pi**2 / temp_spacing.prod(axis=1).sum()) ** (1 / 3)
         self._weights = temp_spacing.prod(axis=1)
 
         # Spacing is the differential element used for integration over surfaces.
         # For this, 2 columns of the matrix are used.
         # Spacing is rescaled below to get the correct double product for each pair
@@ -160,14 +170,15 @@
         # Because a surface integral always ignores 1 column, with this approach,
         # duplicates nodes are scaled down properly regardless of which two columns
         # span the surface.
 
         # scale areas sum to full area
         # The following operation is not a general solution to return the weight
         # removed from the duplicate nodes back to the unique nodes.
+        # (For the 3 predefined grid types this line of code has no effect).
         # For this reason, duplicates should typically be deleted rather than rescaled.
         # Note we multiply each column by duplicates^(1/6) to account for the extra
         # division by duplicates^(1/2) in one of the columns above.
         self._spacing *= (
             4 * np.pi**2 / (self.spacing * duplicates ** (1 / 6)).prod(axis=1).sum()
         ) ** (1 / 3)
 
@@ -184,16 +195,19 @@
         nodes : ndarray of float, size(num_nodes,3)
             Node coordinates, in (rho,theta,zeta).
         spacing : ndarray of float, size(num_nodes,3)
             Node spacing, in (rho,theta,zeta).
 
         """
         nodes = np.atleast_2d(nodes).reshape((-1, 3)).astype(float)
-        nodes[nodes[:, 1] > 2 * np.pi, 1] %= 2 * np.pi
-        nodes[nodes[:, 2] > 2 * np.pi / self.NFP, 2] %= 2 * np.pi / self.NFP
+        # Do not alter nodes given by the user for custom grids.
+        # In particular, do not modulo nodes by 2pi or 2pi/NFP.
+        # This may cause the surface_integrals() function to fail recognizing
+        # surfaces outside the interval [0, 2pi] as duplicates. However, most
+        # surface integral computations are done with LinearGrid anyway.
         spacing = (  # make weights sum to 4pi^2
             np.ones_like(nodes) * np.array([1, 2 * np.pi, 2 * np.pi]) / nodes.shape[0]
         )
         self._L = len(np.unique(nodes[:, 0]))
         self._M = len(np.unique(nodes[:, 1]))
         self._N = len(np.unique(nodes[:, 2]))
         return nodes, spacing
@@ -371,34 +385,34 @@
 
         self._L = L
         self._M = M
         self._N = N
         self._NFP = NFP
         self._axis = axis
         self._sym = sym
-        self._endpoint = endpoint
+        self._endpoint = bool(endpoint)
         self._node_pattern = "linear"
 
         self._nodes, self._spacing = self._create_nodes(
             L=self.L,
             M=self.M,
             N=self.N,
             NFP=self.NFP,
             axis=self.axis,
             endpoint=self.endpoint,
             rho=rho,
             theta=theta,
             zeta=zeta,
         )
 
-        dtheta_scale = self._enforce_symmetry()
+        # symmetry handled in create_nodes()
         self._sort_nodes()
         self._find_axis()
         self._count_nodes()
-        self._scale_weights(dtheta_scale)
+        self._scale_weights()
 
     def _create_nodes(  # noqa: C901
         self,
         L=None,
         M=None,
         N=None,
         NFP=1,
@@ -450,15 +464,15 @@
         if self.L is not None:
             rho = self.L + 1
         else:
             self._L = len(np.atleast_1d(rho))
         if np.isscalar(rho) and (int(rho) == rho) and rho > 0:
             r = np.flipud(np.linspace(1, 0, int(rho), endpoint=axis))
             # choose dr such that each node has the same weight
-            dr = 1 / r.size * np.ones_like(r)
+            dr = np.ones_like(r) / r.size
         else:
             # need to sort to compute correct spacing
             r = np.sort(np.atleast_1d(rho))
             dr = np.zeros_like(r)
             if r.size > 1:
                 # choose dr such that cumulative sums of dr[] are node midpoints
                 # and the total sum is 1
@@ -473,53 +487,95 @@
             if self.sym:
                 theta = 2 * (self.M + 1)
             else:
                 theta = 2 * self.M + 1
         else:
             self._M = len(np.atleast_1d(theta))
         if np.isscalar(theta) and (int(theta) == theta) and theta > 0:
-            t = np.linspace(0, 2 * np.pi, int(theta), endpoint=endpoint)
-            if self.sym and t.size > 1:
+            theta = int(theta)
+            if self.sym and theta > 1:
+                # Enforce that no node lies on theta=0 or theta=2pi, so that
+                # each node has a symmetric counterpart, and that, for all i,
+                # t[i]-t[i-1] = 2 t[0] = 2 (pi - t[last node before pi]).
+                # Both conditions necessary to evenly space nodes with constant dt.
+                # This can be done by making (theta + endpoint) an even integer.
+                if (theta + endpoint) % 2 != 0:
+                    theta += 1
+                t = np.linspace(0, 2 * np.pi, theta, endpoint=endpoint)
                 t += t[1] / 2
+                # delete theta > pi nodes
+                t = t[: np.searchsorted(t, np.pi, side="right")]
+            else:
+                t = np.linspace(0, 2 * np.pi, theta, endpoint=endpoint)
             dt = 2 * np.pi / t.size * np.ones_like(t)
             if (endpoint and not self.sym) and t.size > 1:
                 # increase node weight to account for duplicate node
                 dt *= t.size / (t.size - 1)
                 # scale_weights() will reduce endpoint (dt[0] and dt[-1])
                 # duplicate node weight
         else:
             t = np.atleast_1d(theta).astype(float)
+            SUP = 2 * np.pi  # supremum
+            # enforce periodicity
+            t[t != SUP] %= SUP
             # need to sort to compute correct spacing
-            t[t > 2 * np.pi] %= 2 * np.pi
             t = np.sort(t)
+            if self.sym:
+                # cut domain to relevant subdomain: delete theta > pi nodes
+                t = t[: np.searchsorted(t, np.pi, side="right")]
             dt = np.zeros_like(t)
             if t.size > 1:
-                # choose dt to be half the cyclic distance of the surrounding two nodes
-                SUP = 2 * np.pi  # supremum
-                dt[0] = t[1] + (SUP - (t[-1] % SUP)) % SUP
+                # choose dt to be the cyclic distance of the surrounding two nodes
                 dt[1:-1] = t[2:] - t[:-2]
-                dt[-1] = t[0] + (SUP - (t[-2] % SUP)) % SUP
-                dt /= 2
-                if t.size == 2:
-                    dt[-1] = dt[0]
-                if t[0] == 0 and t[-1] == SUP:
-                    # The cyclic distance algorithm above correctly weights
-                    # the duplicate endpoint node spacing at theta = 0 and 2pi
-                    # to be half the weight of the other nodes.
-                    if not self.sym:
+                if not self.sym:
+                    dt[0] = t[1] + (SUP - t[-1]) % SUP
+                    dt[-1] = t[0] + (SUP - t[-2]) % SUP
+                    dt /= 2  # choose dt to be half the cyclic distance
+                    if t.size == 2:
+                        assert dt[0] == np.pi and dt[-1] == 0
+                        dt[-1] = dt[0]
+                    if t[0] == 0 and t[-1] == SUP:
+                        # The cyclic distance algorithm above correctly weights
+                        # the duplicate endpoint node spacing at theta = 0 and 2pi
+                        # to be half the weight of the other nodes.
                         # However, scale_weights() is not aware of this, so we
                         # counteract the reduction that will be done there.
                         dt[0] += dt[-1]
                         dt[-1] = dt[0]
+                else:
+                    first_positive_idx = np.searchsorted(t, 0, side="right")
+                    if first_positive_idx == 0:
+                        # then there are no nodes at theta=0
+                        dt[0] = t[0] + t[1]
                     else:
-                        # Symmetry deletion will delete the duplicate node at 2pi.
-                        # Need to move weight from non-duplicate nodes back to the
-                        # node at theta = 0 pi.
-                        dt[0] += dt[-1]
-                        dt *= (t.size - 1) / t.size
+                        # total spacing of nodes at theta=0 should be half the
+                        # distance between first positive node and its
+                        # reflection across the theta=0 line.
+                        dt[0] = t[first_positive_idx]
+                        assert (first_positive_idx == 1) or (
+                            dt[0] == dt[first_positive_idx - 1]
+                        )
+                        # If the first condition is false and the latter true,
+                        # then both of those dt should be halved.
+                        # The scale_weights() function will handle this.
+                    first_pi_idx = np.searchsorted(t, np.pi, side="left")
+                    if first_pi_idx == t.size:
+                        # then there are no nodes at theta=pi
+                        dt[-1] = (SUP - t[-1]) - t[-2]
+                    else:
+                        # total spacing of nodes at theta=pi should be half the
+                        # distance between first node < pi and its
+                        # reflection across the theta=pi line.
+                        dt[-1] = (SUP - t[-1]) - t[first_pi_idx - 1]
+                        assert (first_pi_idx == t.size - 1) or (
+                            dt[first_pi_idx] == dt[-1]
+                        )
+                        # If the first condition is false and the latter true,
+                        # then both of those dt should be halved.
+                        # The scale_weights() function will handle this.
             else:
                 dt = np.array([2 * np.pi])
 
         # zeta
         # note: dz spacing should not depend on NFP
         # spacing corresponds to a node's weight in an integral --
         # such as integral = sum(dt * dz * data["B"]) -- not the node's coordinates
@@ -533,40 +589,44 @@
             if endpoint and z.size > 1:
                 # increase node weight to account for duplicate node
                 dz *= z.size / (z.size - 1)
                 # scale_weights() will reduce endpoint (dz[0] and dz[-1])
                 # duplicate node weight
         else:
             z = np.atleast_1d(zeta).astype(float)
+            # enforce periodicity
+            SUP = 2 * np.pi / self.NFP  # supremum
+            z[z != SUP] %= SUP
             # need to sort to compute correct spacing
-            z[z > 2 * np.pi / self.NFP] %= 2 * np.pi / self.NFP
             z = np.sort(z)
             dz = np.zeros_like(z)
             if z.size > 1:
                 # choose dz to be half the cyclic distance of the surrounding two nodes
-                SUP = 2 * np.pi / self.NFP  # supremum
-                dz[0] = z[1] + (SUP - (z[-1] % SUP)) % SUP
+                dz[0] = z[1] + (SUP - z[-1]) % SUP
                 dz[1:-1] = z[2:] - z[:-2]
-                dz[-1] = z[0] + (SUP - (z[-2] % SUP)) % SUP
+                dz[-1] = z[0] + (SUP - z[-2]) % SUP
                 dz /= 2
                 dz *= self.NFP
                 if z.size == 2:
                     dz[-1] = dz[0]
                 if z[0] == 0 and z[-1] == SUP:
                     # The cyclic distance algorithm above correctly weights
                     # the duplicate node spacing at zeta = 0 and 2pi / NFP.
                     # However, scale_weights() is not aware of this, so we
                     # counteract the reduction that will be done there.
                     dz[0] += dz[-1]
                     dz[-1] = dz[0]
             else:
                 dz = np.array([2 * np.pi])
 
-        self._endpoint = (t[0] == 0 and t[-1] == 2 * np.pi) and (
-            z[0] == 0 and z[-1] == 2 * np.pi / self.NFP
+        self._endpoint = (
+            t.size > 0
+            and z.size > 0
+            and (t[0] == 0 and t[-1] == 2 * np.pi)
+            and (z[0] == 0 and z[-1] == 2 * np.pi / self.NFP)
         )
 
         r, t, z = np.meshgrid(r, t, z, indexing="ij")
         r = r.flatten()
         t = t.flatten()
         z = z.flatten()
 
@@ -604,18 +664,18 @@
                 L=L,
                 M=M,
                 N=N,
                 NFP=self.NFP,
                 axis=len(self.axis) > 0,
                 endpoint=self.endpoint,
             )
-            dtheta_scale = self._enforce_symmetry()
+            self._enforce_symmetry()
             self._sort_nodes()
             self._find_axis()
-            self._scale_weights(dtheta_scale)
+            self._scale_weights()
 
     @property
     def endpoint(self):
         """bool: Whether the grid is made of open or closed intervals."""
         return self.__dict__.setdefault("_endpoint", False)
 
 
@@ -727,20 +787,17 @@
         """
         self._NFP = NFP if NFP is not None else self.NFP
         if L != self.L or M != self.M or N != self.N:
             self._L = L
             self._M = M
             self._N = N
             self._nodes, self._spacing = self._create_nodes(L=L, M=M, N=N, NFP=self.NFP)
-            dtheta_scale = self._enforce_symmetry()
             self._sort_nodes()
             self._find_axis()
-            temp_spacing = np.copy(self.spacing)
-            temp_spacing[:, 1] /= dtheta_scale
-            self._weights = temp_spacing.prod(axis=1)  # instead of _scale_weights
+            self._weights = self.spacing.prod(axis=1)  # instead of _scale_weights
 
 
 class ConcentricGrid(Grid):
     """Grid in which the nodes are arranged in concentric circles.
 
     Nodes are arranged concentrically within each toroidal cross-section, with more
     nodes per flux surface at larger radius. Typically used as the solution grid,
@@ -788,19 +845,19 @@
             M=self.M,
             N=self.N,
             NFP=self.NFP,
             axis=self.axis,
             node_pattern=self.node_pattern,
         )
 
-        dtheta_scale = self._enforce_symmetry()
+        self._enforce_symmetry()
         self._sort_nodes()
         self._find_axis()
         self._count_nodes()
-        self._scale_weights(dtheta_scale)
+        self._scale_weights()
 
     def _create_nodes(self, L, M, N, NFP=1, axis=False, node_pattern="jacobi"):
         """Create grid nodes and weights.
 
         Parameters
         ----------
         L : int
@@ -933,18 +990,18 @@
                 L=L,
                 M=M,
                 N=N,
                 NFP=self.NFP,
                 axis=len(self.axis) > 0,
                 node_pattern=self.node_pattern,
             )
-            dtheta_scale = self._enforce_symmetry()
+            self._enforce_symmetry()
             self._sort_nodes()
             self._find_axis()
-            self._scale_weights(dtheta_scale)
+            self._scale_weights()
 
 
 # these functions are currently unused ---------------------------------------
 
 # TODO: finish option for placing nodes at irrational surfaces
```

### Comparing `desc-opt-0.8.1/desc/interpolate.py` & `desc-opt-0.8.2/desc/interpolate.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/io/ascii_io.py` & `desc-opt-0.8.2/desc/io/ascii_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/io/core_io.py` & `desc-opt-0.8.2/desc/io/core_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/io/equilibrium_io.py` & `desc-opt-0.8.2/desc/io/equilibrium_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/io/hdf5_io.py` & `desc-opt-0.8.2/desc/io/hdf5_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/io/input_reader.py` & `desc-opt-0.8.2/desc/io/input_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,18 +159,18 @@
             "Psi": 1.0,
             "L": np.atleast_1d(None),
             "M": np.atleast_1d(0),
             "N": np.atleast_1d(0),
             "L_grid": np.atleast_1d(None),
             "M_grid": np.atleast_1d(0),
             "N_grid": np.atleast_1d(0),
-            "pres_ratio": np.atleast_1d(1.0),
-            "curr_ratio": np.atleast_1d(1.0),
-            "bdry_ratio": np.atleast_1d(1.0),
-            "pert_order": np.atleast_1d(1),
+            "pres_ratio": np.atleast_1d(None),
+            "curr_ratio": np.atleast_1d(None),
+            "bdry_ratio": np.atleast_1d(None),
+            "pert_order": np.atleast_1d(2),
             "ftol": np.atleast_1d(None),
             "xtol": np.atleast_1d(None),
             "gtol": np.atleast_1d(None),
             "nfev": np.atleast_1d(None),
             "objective": "force",
             "optimizer": "lsq-exact",
             "spectral_indexing": "ansi",
@@ -621,24 +621,28 @@
                 if key in arrs:
                     inputs_ii[key] = inputs[key][ii]
                 elif isinstance(inputs[key], np.ndarray):
                     inputs_ii[key] = inputs[key].copy()
                 else:
                     inputs_ii[key] = inputs[key]
             # apply pressure ratio
-            inputs_ii["pressure"][:, 1] *= inputs_ii["pres_ratio"]
+            if inputs_ii["pres_ratio"] is not None:
+                inputs_ii["pressure"][:, 1] *= inputs_ii["pres_ratio"]
             # apply current ratio
-            if "current" in inputs_ii:
+            if "current" in inputs_ii and inputs_ii["curr_ratio"] is not None:
                 inputs_ii["current"][:, 1] *= inputs_ii["curr_ratio"]
+            else:
+                del inputs_ii["curr_ratio"]
             # apply boundary ratio
             bdry_factor = np.where(
                 inputs_ii["surface"][:, 2] != 0, inputs_ii["bdry_ratio"], 1.0
             )
-            inputs_ii["surface"][:, 3] *= bdry_factor
-            inputs_ii["surface"][:, 4] *= bdry_factor
+            if inputs_ii["bdry_ratio"] is not None:
+                inputs_ii["surface"][:, 3] *= bdry_factor
+                inputs_ii["surface"][:, 4] *= bdry_factor
             inputs_list.append(inputs_ii)
 
         return inputs_list
 
     @staticmethod
     def write_desc_input(filename, inputs, header=""):  # noqa: C901 - fxn too complex
         """Generate a DESC input file from a dictionary of parameters.
@@ -681,17 +685,26 @@
         }.items():
             f.write(
                 key + " = {}\n".format(", ".join([str(inp[val]) for inp in inputs]))
             )
 
         f.write("\n# continuation parameters\n")
         for key in ["bdry_ratio", "pres_ratio", "curr_ratio", "pert_order"]:
+            inputs_not_None = []
+            for inp in inputs:
+                if inp.get(key) is not None:
+                    inputs_not_None.append(inp)
+            if not inputs_not_None:  # an  empty list evals to False
+                continue  # don't write line if all input tolerance are None
+
             f.write(
                 key
-                + " = {} \n".format(", ".join([str(float(inp[key])) for inp in inputs]))
+                + " = {} \n".format(
+                    ", ".join([str(float(inp[key])) for inp in inputs_not_None])
+                )
             )
 
         f.write("\n# solver tolerances\n")
         for key in ["ftol", "xtol", "gtol", "nfev"]:
             inputs_not_None = []
             for inp in inputs:
                 if inp[key] is not None:
@@ -806,18 +819,18 @@
             "Psi": 1.0,
             "L": None,
             "M": 0,
             "N": 0,
             "L_grid": None,
             "M_grid": 0,
             "N_grid": 0,
-            "pres_ratio": 1.0,
-            "curr_ratio": 1.0,
-            "bdry_ratio": 1.0,
-            "pert_order": 1,
+            "pres_ratio": None,
+            "curr_ratio": None,
+            "bdry_ratio": None,
+            "pert_order": 2,
             "ftol": None,
             "xtol": None,
             "gtol": None,
             "nfev": None,
             "objective": "force",
             "optimizer": "lsq-exact",
             "spectral_indexing": "ansi",
@@ -1338,57 +1351,15 @@
         if iota_flag:
             del inputs["current"]
         else:
             del inputs["iota"]
 
         vmec_file.close()
 
-        # default continuation stuff
-        res_step = 6
-        pres_step = 1 / 2
-        bdry_step = 1 / 4
-
-        # first we solve vacuum until we reach full L,M
-        # then pressure
-        # then 3d shaping
-        res_steps = max(inputs["L"] // res_step, 1)
-        pres_steps = (
-            0 if (inputs["pressure"][:, 1] == 0).all() else int(np.ceil(1 / pres_step))
-        )
-        bdry_steps = 0 if inputs["N"] == 0 else int(np.ceil(1 / bdry_step))
-
-        total_steps = res_steps + pres_steps + bdry_steps
-        inputs_arr = [inputs.copy() for _ in range(total_steps)]
-        for i in range(total_steps):
-            if i < res_steps:
-                inputs_arr[i]["L"] = min((i + 1) * res_step, inputs["L"])
-                inputs_arr[i]["L_grid"] = 2 * inputs_arr[i]["L"]
-                inputs_arr[i]["N"] = 0
-                inputs_arr[i]["N_grid"] = 0
-                inputs_arr[i]["pres_ratio"] = 0.0
-                inputs_arr[i]["curr_ratio"] = 0.0
-                if bdry_steps != 0:
-                    inputs_arr[i]["bdry_ratio"] = 0.0
-                else:
-                    inputs_arr[i]["bdry_ratio"] = 1.0
-            elif i < (res_steps + pres_steps):
-                inputs_arr[i]["N"] = 0
-                inputs_arr[i]["N_grid"] = 0
-                inputs_arr[i]["pres_ratio"] = (i - res_steps + 1) * pres_step
-                inputs_arr[i]["curr_ratio"] = (i - res_steps + 1) * pres_step
-                inputs_arr[i]["pert_order"] = 2
-                if bdry_steps != 0:
-                    inputs_arr[i]["bdry_ratio"] = 0.0
-                else:
-                    inputs_arr[i]["bdry_ratio"] = 1.0
-            else:
-                inputs_arr[i]["pert_order"] = 2
-                inputs_arr[i]["bdry_ratio"] = (
-                    i - res_steps - pres_steps + 1
-                ) * bdry_step
+        inputs_arr = [inputs]
 
         return inputs_arr
 
 
 # NOTE: this has to be outside the class to work with autodoc
```

### Comparing `desc-opt-0.8.1/desc/io/pickle_io.py` & `desc-opt-0.8.2/desc/io/pickle_io.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/magnetic_fields.py` & `desc-opt-0.8.2/desc/magnetic_fields.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/objectives/__init__.py` & `desc-opt-0.8.2/desc/objectives/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,24 @@
     AspectRatio,
     Elongation,
     MeanCurvature,
     PlasmaVesselDistance,
     PrincipalCurvature,
     Volume,
 )
-from ._qs import QuasisymmetryBoozer, QuasisymmetryTripleProduct, QuasisymmetryTwoTerm
+from ._qs import (
+    Isodynamicity,
+    QuasisymmetryBoozer,
+    QuasisymmetryTripleProduct,
+    QuasisymmetryTwoTerm,
+)
 from ._stability import MagneticWell, MercierStability
 from .linear_objectives import (
+    BoundaryRSelfConsistency,
+    BoundaryZSelfConsistency,
     FixAtomicNumber,
     FixAxisR,
     FixAxisZ,
     FixBoundaryR,
     FixBoundaryZ,
     FixCurrent,
     FixElectronDensity,
```

### Comparing `desc-opt-0.8.1/desc/objectives/_bootstrap.py` & `desc-opt-0.8.2/desc/objectives/_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         grid=None,
         helicity=(1, 0),
         name="Bootstrap current self-consistency (Redl)",
     ):
 
         assert (len(helicity) == 2) and (int(helicity[1]) == helicity[1])
         assert helicity[0] == 1, "Redl bootstrap current model assumes helicity[0] == 1"
-        self.grid = grid
+        self._grid = grid
         self.helicity = helicity
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
@@ -101,27 +101,29 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(
+        if self._grid is None:
+            grid = LinearGrid(
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 rho=np.linspace(1 / 5, 1, 5),
             )
+        else:
+            grid = self._grid
 
         assert (
             self.helicity[1] == 0 or abs(self.helicity[1]) == eq.NFP
         ), "Helicity toroidal mode number should be 0 (QA) or +/- NFP (QH)"
-        self._dim_f = self.grid.num_rho
+        self._dim_f = grid.num_rho
         self._data_keys = ["<J*B>", "<J*B> Redl"]
         self._args = get_params(self._data_keys)
 
         if eq.electron_temperature is None:
             raise RuntimeError(
                 "Bootstrap current calculation requires an electron temperature "
                 "profile."
@@ -133,15 +135,15 @@
         if eq.ion_temperature is None:
             raise RuntimeError(
                 "Bootstrap current calculation requires an ion temperature profile."
             )
 
         # Try to catch cases in which density or temperatures are specified in the
         # wrong units. Densities should be ~ 10^20, temperatures are ~ 10^3.
-        rho = eq.compute("rho", grid=self.grid)["rho"]
+        rho = eq.compute("rho", grid=grid)["rho"]
         if jnp.any(eq.electron_density(rho) > 1e22):
             warnings.warn(
                 "Electron density is surprisingly high. It should have units of "
                 "1/meters^3"
             )
         if jnp.any(eq.electron_temperature(rho) > 50e3):
             warnings.warn(
@@ -168,16 +170,16 @@
             )
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -200,20 +202,26 @@
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
             helicity=self.helicity,
         )
 
         return compress(
-            self.grid, data["<J*B>"] - data["<J*B> Redl"], surface_label="rho"
+            self._transforms["grid"],
+            data["<J*B>"] - data["<J*B> Redl"],
+            surface_label="rho",
         )
 
     def compute_scaled(self, *args, **kwargs):
         """Compute and apply the target/bounds, weighting, and normalization."""
-        w = compress(self.grid, self.grid.spacing[:, 0], surface_label="rho")
+        w = compress(
+            self._transforms["grid"],
+            self._transforms["grid"].spacing[:, 0],
+            surface_label="rho",
+        )
         return super().compute_scaled(*args, **kwargs) * jnp.sqrt(w)
 
     def print_value(self, *args, **kwargs):
         """Print the value of the objective."""
         f = self.compute(*args, **kwargs)
         print("Maximum " + self._print_value_fmt.format(jnp.max(f)) + self._units)
         print("Minimum " + self._print_value_fmt.format(jnp.min(f)) + self._units)
```

### Comparing `desc-opt-0.8.1/desc/objectives/_equilibrium.py` & `desc-opt-0.8.2/desc/objectives/_equilibrium.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="force",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -87,56 +87,58 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
+        if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
             ]:
-                self.grid = ConcentricGrid(
+                grid = ConcentricGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                     sym=eq.sym,
                     axis=False,
                     node_pattern=eq.node_pattern,
                 )
             elif eq.node_pattern == "quad":
-                self.grid = QuadratureGrid(
+                grid = QuadratureGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                 )
+        else:
+            grid = self._grid
 
-        self._dim_f = 2 * self.grid.num_nodes
+        self._dim_f = 2 * grid.num_nodes
         self._data_keys = [
             "F_rho",
             "|grad(rho)|",
             "sqrt(g)",
             "F_helical",
             "|e^helical|",
         ]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -183,18 +185,18 @@
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
         fr = data["F_rho"] * data["|grad(rho)|"]
-        fr = fr * data["sqrt(g)"] * self.grid.weights
+        fr = fr * data["sqrt(g)"] * self._transforms["grid"].weights
 
         fb = data["F_helical"] * data["|e^helical|"]
-        fb = fb * data["sqrt(g)"] * self.grid.weights
+        fb = fb * data["sqrt(g)"] * self._transforms["grid"].weights
 
         return jnp.concatenate([fr, fb])
 
 
 class RadialForceBalance(_Objective):
     """Radial MHD force balance.
 
@@ -240,15 +242,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="radial force",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -264,50 +266,52 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
+        if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
             ]:
-                self.grid = ConcentricGrid(
+                grid = ConcentricGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                     sym=eq.sym,
                     axis=False,
                     node_pattern=eq.node_pattern,
                 )
             elif eq.node_pattern == "quad":
-                self.grid = QuadratureGrid(
+                grid = QuadratureGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                 )
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_nodes
+        self._dim_f = grid.num_nodes
         self._data_keys = ["F_rho", "|grad(rho)|", "sqrt(g)"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -354,15 +358,15 @@
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
         f = data["F_rho"] * data["|grad(rho)|"]
-        return f * data["sqrt(g)"] * self.grid.weights
+        return f * data["sqrt(g)"] * self._transforms["grid"].weights
 
 
 class HelicalForceBalance(_Objective):
     """Helical MHD force balance.
 
     F_helical = sqrt(g) J^rho
     e^helical = -B^zeta grad(theta) + B^theta grad(zeta)
@@ -407,15 +411,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="helical force",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -431,50 +435,52 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
+        if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
             ]:
-                self.grid = ConcentricGrid(
+                grid = ConcentricGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                     sym=eq.sym,
                     axis=False,
                     node_pattern=eq.node_pattern,
                 )
             elif eq.node_pattern == "quad":
-                self.grid = QuadratureGrid(
+                grid = QuadratureGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                 )
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_nodes
+        self._dim_f = grid.num_nodes
         self._data_keys = ["F_helical", "|e^helical|", "sqrt(g)"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -521,15 +527,15 @@
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
         f = data["F_helical"] * data["|e^helical|"]
-        return f * data["sqrt(g)"] * self.grid.weights
+        return f * data["sqrt(g)"] * self._transforms["grid"].weights
 
 
 class Energy(_Objective):
     """MHD energy.
 
     W = integral( B^2 / (2*mu0) + p / (gamma - 1) ) dV  (J)
 
@@ -577,15 +583,15 @@
         normalize=True,
         normalize_target=True,
         grid=None,
         gamma=0,
         name="energy",
     ):
 
-        self.grid = grid
+        self._grid = grid
         self.gamma = gamma
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
@@ -602,15 +608,15 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
+        if self._grid is None:
             if eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
             ]:
@@ -618,43 +624,45 @@
                     colored(
                         "Energy objective built using grid "
                         + "that is not the quadrature grid! "
                         + "This is not recommended and may result in poor convergence. "
                         "yellow",
                     )
                 )
-                self.grid = ConcentricGrid(
+                grid = ConcentricGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                     sym=eq.sym,
                     axis=False,
                     node_pattern=eq.node_pattern,
                 )
 
             else:
-                self.grid = QuadratureGrid(
+                grid = QuadratureGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                 )
+        else:
+            grid = self._grid
 
         self._dim_f = 1
         self._data_keys = ["W"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -760,15 +768,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="current density",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -784,50 +792,52 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
+        if self._grid is None:
             if eq.node_pattern is None or eq.node_pattern in [
                 "jacobi",
                 "cheb1",
                 "cheb2",
                 "ocs",
                 "linear",
             ]:
-                self.grid = ConcentricGrid(
+                grid = ConcentricGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                     sym=eq.sym,
                     axis=False,
                     node_pattern=eq.node_pattern,
                 )
             elif eq.node_pattern == "quad":
-                self.grid = QuadratureGrid(
+                grid = QuadratureGrid(
                     L=eq.L_grid,
                     M=eq.M_grid,
                     N=eq.N_grid,
                     NFP=eq.NFP,
                 )
+        else:
+            grid = self._grid
 
-        self._dim_f = 3 * self.grid.num_nodes
+        self._dim_f = 3 * grid.num_nodes
         self._data_keys = ["J^rho", "J^theta", "J^zeta", "sqrt(g)"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -863,12 +873,12 @@
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
-        jr = data["J^rho"] * data["sqrt(g)"] * self.grid.weights
-        jt = data["J^theta"] * data["sqrt(g)"] * self.grid.weights
-        jz = data["J^zeta"] * data["sqrt(g)"] * self.grid.weights
+        jr = data["J^rho"] * data["sqrt(g)"] * self._transforms["grid"].weights
+        jt = data["J^theta"] * data["sqrt(g)"] * self._transforms["grid"].weights
+        jz = data["J^zeta"] * data["sqrt(g)"] * self._transforms["grid"].weights
 
         return jnp.concatenate([jr, jt, jz])
```

### Comparing `desc-opt-0.8.1/desc/objectives/_generic.py` & `desc-opt-0.8.2/desc/objectives/_generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         normalize=True,
         normalize_target=True,
         grid=None,
         name="generic",
     ):
 
         self.f = f
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -84,26 +84,28 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = QuadratureGrid(eq.L_grid, eq.M_grid, eq.N_grid, eq.NFP)
+        if self._grid is None:
+            grid = QuadratureGrid(eq.L_grid, eq.M_grid, eq.N_grid, eq.NFP)
+        else:
+            grid = self._grid
 
         if data_index[self.f]["dim"] == 0:
             self._dim_f = 1
             self._scalar = True
         else:
-            self._dim_f = self.grid.num_nodes * data_index[self.f]["dim"]
+            self._dim_f = grid.num_nodes * data_index[self.f]["dim"]
             self._scalar = False
         self._args = get_params(self.f)
-        self._profiles = get_profiles(self.f, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self.f, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self.f, eq=eq, grid=grid)
+        self._transforms = get_transforms(self.f, eq=eq, grid=grid)
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, *args, **kwargs):
         """Compute the quantity.
 
         Parameters
         ----------
@@ -121,15 +123,15 @@
             self.f,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
         f = data[self.f]
         if not self.scalar:
-            f = (f.T * self.grid.weights).flatten()
+            f = (f.T * self._transforms["grid"].weights).flatten()
         return f
 
 
 class ToroidalCurrent(_Objective):
     """Target toroidal current profile.
 
     Parameters
@@ -171,15 +173,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="toroidal current",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -195,38 +197,40 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(
+        if self._grid is None:
+            grid = LinearGrid(
                 L=eq.L_grid,
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 axis=False,
             )
+        else:
+            grid = self._grid
 
         if isinstance(self._target, Profile):
-            self._target = self._target(self.grid.nodes[self.grid.unique_rho_idx])
+            self._target = self._target(grid.nodes[grid.unique_rho_idx])
 
-        self._dim_f = self.grid.num_rho
+        self._dim_f = grid.num_rho
         self._data_keys = ["current"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -261,19 +265,23 @@
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
-        return compress(self.grid, data["current"], surface_label="rho")
+        return compress(self._transforms["grid"], data["current"], surface_label="rho")
 
     def compute_scaled(self, *args, **kwargs):
         """Compute and apply the target/bounds, weighting, and normalization."""
-        w = compress(self.grid, self.grid.spacing[:, 0], surface_label="rho")
+        w = compress(
+            self._transforms["grid"],
+            self._transforms["grid"].spacing[:, 0],
+            surface_label="rho",
+        )
         return super().compute_scaled(*args, **kwargs) * jnp.sqrt(w)
 
     def print_value(self, *args, **kwargs):
         """Print the value of the objective."""
         f = self.compute(*args, **kwargs)
         print("Maximum " + self._print_value_fmt.format(jnp.max(f)) + self._units)
         print("Minimum " + self._print_value_fmt.format(jnp.min(f)) + self._units)
@@ -341,15 +349,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="rotational transform",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -365,37 +373,40 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(
+        if self._grid is None:
+            grid = LinearGrid(
                 L=eq.L_grid,
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 axis=False,
             )
+        else:
+            grid = self._grid
+
         if isinstance(self._target, Profile):
-            self._target = self._target(self.grid.nodes[self.grid.unique_rho_idx])
+            self._target = self._target(grid.nodes[grid.unique_rho_idx])
 
-        self._dim_f = self.grid.num_rho
+        self._dim_f = grid.num_rho
         self._data_keys = ["iota"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
@@ -426,19 +437,23 @@
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
-        return compress(self.grid, data["iota"], surface_label="rho")
+        return compress(self._transforms["grid"], data["iota"], surface_label="rho")
 
     def compute_scaled(self, *args, **kwargs):
         """Compute and apply the target/bounds, weighting, and normalization."""
-        w = compress(self.grid, self.grid.spacing[:, 0], surface_label="rho")
+        w = compress(
+            self._transforms["grid"],
+            self._transforms["grid"].spacing[:, 0],
+            surface_label="rho",
+        )
         return super().compute_scaled(*args, **kwargs) * jnp.sqrt(w)
 
     def print_value(self, *args, **kwargs):
         """Print the value of the objective."""
         f = self.compute(*args, **kwargs)
         print("Maximum " + self._print_value_fmt.format(jnp.max(f)) + self._units)
         print("Minimum " + self._print_value_fmt.format(jnp.min(f)) + self._units)
```

### Comparing `desc-opt-0.8.1/desc/objectives/_geometry.py` & `desc-opt-0.8.2/desc/objectives/_geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="aspect ratio",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -82,30 +82,30 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = QuadratureGrid(
-                L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP
-            )
+        if self._grid is None:
+            grid = QuadratureGrid(L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        else:
+            grid = self._grid
 
         self._dim_f = 1
         self._data_keys = ["R0/a"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
@@ -178,15 +178,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="elongation",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -202,30 +202,30 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = QuadratureGrid(
-                L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP
-            )
+        if self._grid is None:
+            grid = QuadratureGrid(L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        else:
+            grid = self._grid
 
         self._dim_f = 1
         self._data_keys = ["a_major/a_minor"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
@@ -298,15 +298,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="volume",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -322,30 +322,30 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = QuadratureGrid(
-                L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP
-            )
+        if self._grid is None:
+            grid = QuadratureGrid(L=eq.L_grid, M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        else:
+            grid = self._grid
 
         self._dim_f = 1
         self._data_keys = ["V"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -457,38 +457,40 @@
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
         if self._surface_grid is None:
-            self._surface_grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+            surface_grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        else:
+            surface_grid = self._surface_grid
         if self._plasma_grid is None:
-            self._plasma_grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
-        if not np.allclose(self._surface_grid.nodes[:, 0], 1):
+            plasma_grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        else:
+            plasma_grid = self._plasma_grid
+        if not np.allclose(surface_grid.nodes[:, 0], 1):
             warnings.warn("Surface grid includes off-surface pts, should be rho=1")
-        if not np.allclose(self._plasma_grid.nodes[:, 0], 1):
+        if not np.allclose(plasma_grid.nodes[:, 0], 1):
             warnings.warn("Plasma grid includes interior points, should be rho=1")
 
-        self._dim_f = self._surface_grid.num_nodes
+        self._dim_f = surface_grid.num_nodes
         self._data_keys = ["R", "phi", "Z"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
         self._surface_coords = self._surface.compute_coordinates(
-            grid=self._surface_grid, basis="xyz"
-        )
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self._plasma_grid)
-        self._transforms = get_transforms(
-            self._data_keys, eq=eq, grid=self._plasma_grid
+            grid=surface_grid, basis="xyz"
         )
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=plasma_grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=plasma_grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -574,15 +576,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="mean-curvature",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -598,28 +600,30 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        if self._grid is None:
+            grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_nodes
+        self._dim_f = grid.num_nodes
         self._data_keys = ["curvature_H"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -635,15 +639,15 @@
         R_lmn : ndarray
             Spectral coefficients of R(rho,theta,zeta) -- flux surface R coordinate (m).
         Z_lmn : ndarray
             Spectral coefficients of Z(rho,theta,zeta) -- flux surface Z coordinate (m).
 
         Returns
         -------
-        H : ndarray, shape(self.grid.num_nodes,)
+        H : ndarray
             Mean curvature at each point (m^-1).
 
         """
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
@@ -704,15 +708,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="principal-curvature",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -728,28 +732,30 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        if self._grid is None:
+            grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP)
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_nodes
+        self._dim_f = grid.num_nodes
         self._data_keys = ["curvature_k1", "curvature_k2"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -765,15 +771,15 @@
         R_lmn : ndarray
             Spectral coefficients of R(rho,theta,zeta) -- flux surface R coordinate (m).
         Z_lmn : ndarray
             Spectral coefficients of Z(rho,theta,zeta) -- flux surface Z coordinate (m).
 
         Returns
         -------
-        k : ndarray, shape(self.grid.num_nodes,)
+        k : ndarray
             Max absolute principal curvature at each point (m^-1).
 
         """
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
```

### Comparing `desc-opt-0.8.1/desc/objectives/_qs.py` & `desc-opt-0.8.2/desc/objectives/_qs.py`

 * *Files 10% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         M_booz=None,
         N_booz=None,
         name="QS Boozer",
     ):
 
         assert len(helicity) == 2
         assert (int(helicity[0]) == helicity[0]) and (int(helicity[1]) == helicity[1])
-        self.grid = grid
+        self._grid = grid
         self.helicity = helicity
         self.M_booz = M_booz
         self.N_booz = N_booz
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
@@ -103,40 +103,40 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.M_booz is None:
-            self.M_booz = 2 * eq.M
-        if self.N_booz is None:
-            self.N_booz = 2 * eq.N
-        if self.grid is None:
-            self.grid = LinearGrid(
-                M=2 * self.M_booz, N=2 * self.N_booz, NFP=eq.NFP, sym=False
-            )
+        M_booz = self.M_booz or 2 * eq.M
+        N_booz = self.N_booz or 2 * eq.N
+
+        if self._grid is None:
+            grid = LinearGrid(M=2 * M_booz, N=2 * N_booz, NFP=eq.NFP, sym=False)
+        else:
+            grid = self._grid
+
         self._data_keys = ["|B|_mn"]
         self._args = get_params(self._data_keys)
 
-        assert self.grid.sym is False
-        assert self.grid.num_rho == 1
+        assert grid.sym is False
+        assert grid.num_rho == 1
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
         self._transforms = get_transforms(
             self._data_keys,
             eq=eq,
-            grid=self.grid,
-            M_booz=self.M_booz,
-            N_booz=self.N_booz,
+            grid=grid,
+            M_booz=M_booz,
+            N_booz=N_booz,
         )
         self._matrix, self._modes, self._idx = ptolemy_linear_transform(
             self._transforms["B"].basis.modes,
             helicity=self.helicity,
             NFP=self._transforms["B"].basis.NFP,
         )
 
@@ -258,15 +258,15 @@
         normalize=True,
         normalize_target=True,
         grid=None,
         helicity=(1, 0),
         name="QS two-term",
     ):
 
-        self.grid = grid
+        self._grid = grid
         self.helicity = helicity
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
@@ -290,28 +290,30 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
+        if self._grid is None:
+            grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_nodes
+        self._dim_f = grid.num_nodes
         self._data_keys = ["f_C"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -347,15 +349,15 @@
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
             helicity=self.helicity,
         )
-        return data["f_C"] * self.grid.weights
+        return data["f_C"] * self._transforms["grid"].weights
 
     @property
     def helicity(self):
         """tuple: Type of quasi-symmetry (M, N)."""
         return self._helicity
 
     @helicity.setter
@@ -421,15 +423,15 @@
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="QS triple product",
     ):
 
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -445,28 +447,30 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
+        if self._grid is None:
+            grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_nodes
+        self._dim_f = grid.num_nodes
         self._data_keys = ["f_T"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -503,8 +507,141 @@
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
-        return data["f_T"] * self.grid.weights
+        return data["f_T"] * self._transforms["grid"].weights
+
+
+class Isodynamicity(_Objective):
+    """Isodynamicity metric for cross field transport.
+
+    Note: This is NOT the same as Quasi-isodynamicity (QI), which is a more general
+    condition. This specifically penalizes the local cross field transport, rather than
+    just the average.
+
+    Parameters
+    ----------
+    eq : Equilibrium, optional
+        Equilibrium that will be optimized to satisfy the Objective.
+    target : float, ndarray, optional
+        Target value(s) of the objective. Only used if bounds is None.
+        len(target) must be equal to Objective.dim_f
+    bounds : tuple, optional
+        Lower and upper bounds on the objective. Overrides target.
+        len(bounds[0]) and len(bounds[1]) must be equal to Objective.dim_f
+    weight : float, ndarray, optional
+        Weighting to apply to the Objective, relative to other Objectives.
+        len(weight) must be equal to Objective.dim_f
+    normalize : bool
+        Whether to compute the error in physical units or non-dimensionalize.
+        Has no effect for this objective.
+    normalize_target : bool
+       Whether target and bounds should be normalized before comparing to computed
+        values. If `normalize` is `True` and the target is in physical units,
+        this should also be set to True.
+        Has no effect for this objective.
+    grid : Grid, ndarray, optional
+        Collocation grid containing the nodes to evaluate at.
+    name : str
+        Name of the objective function.
+
+    """
+
+    _scalar = False
+    _linear = False
+    _units = "(dimensionless)"
+    _print_value_fmt = "Isodynamicity error: {:10.3e} "
+
+    def __init__(
+        self,
+        eq=None,
+        target=0,
+        bounds=None,
+        weight=1,
+        normalize=False,
+        normalize_target=False,
+        grid=None,
+        name="Isodynamicity",
+    ):
+
+        self._grid = grid
+        super().__init__(
+            eq=eq,
+            target=target,
+            bounds=bounds,
+            weight=weight,
+            normalize=normalize,
+            normalize_target=normalize_target,
+            name=name,
+        )
+
+    def build(self, eq, use_jit=True, verbose=1):
+        """Build constant arrays.
+
+        Parameters
+        ----------
+        eq : Equilibrium, optional
+            Equilibrium that will be optimized to satisfy the Objective.
+        use_jit : bool, optional
+            Whether to just-in-time compile the objective and derivatives.
+        verbose : int, optional
+            Level of output.
+
+        """
+        if self._grid is None:
+            grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym)
+        else:
+            grid = self._grid
+
+        self._dim_f = grid.num_nodes
+        self._data_keys = ["isodynamicity"]
+        self._args = get_params(self._data_keys)
+
+        timer = Timer()
+        if verbose > 0:
+            print("Precomputing transforms")
+        timer.start("Precomputing transforms")
+
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
+
+        timer.stop("Precomputing transforms")
+        if verbose > 1:
+            timer.disp("Precomputing transforms")
+
+        super().build(eq=eq, use_jit=use_jit, verbose=verbose)
+
+    def compute(self, *args, **kwargs):
+        """Compute isodynamicity errors.
+
+        Parameters
+        ----------
+        R_lmn : ndarray
+            Spectral coefficients of R(rho,theta,zeta) -- flux surface R coordinate (m).
+        Z_lmn : ndarray
+            Spectral coefficients of Z(rho,theta,zeta) -- flux surface Z coordinate (m).
+        L_lmn : ndarray
+            Spectral coefficients of lambda(rho,theta,zeta) -- poloidal stream function.
+        i_l : ndarray
+            Spectral coefficients of iota(rho) -- rotational transform profile.
+        c_l : ndarray
+            Spectral coefficients of I(rho) -- toroidal current profile.
+        Psi : float
+            Total toroidal magnetic flux within the last closed flux surface (Wb).
+
+        Returns
+        -------
+        f : ndarray
+            Isodynamicity error at each node (~).
+
+        """
+        params = self._parse_args(*args, **kwargs)
+        data = compute_fun(
+            self._data_keys,
+            params=params,
+            transforms=self._transforms,
+            profiles=self._profiles,
+        )
+        return data["isodynamicity"] * self._transforms["grid"].weights
```

### Comparing `desc-opt-0.8.1/desc/objectives/_stability.py` & `desc-opt-0.8.2/desc/objectives/_stability.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         bounds=(0, np.inf),
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="Mercier Stability",
     ):
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -86,34 +86,36 @@
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
-        if self.grid is None:
-            self.grid = LinearGrid(
+        if self._grid is None:
+            grid = LinearGrid(
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 rho=np.linspace(1 / 5, 1, 5),
             )
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_rho
+        self._dim_f = grid.num_rho
         self._data_keys = ["D_Mercier"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
@@ -158,19 +160,25 @@
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
-        return compress(self.grid, data["D_Mercier"], surface_label="rho")
+        return compress(
+            self._transforms["grid"], data["D_Mercier"], surface_label="rho"
+        )
 
     def compute_scaled(self, *args, **kwargs):
         """Compute and apply the target/bounds, weighting, and normalization."""
-        w = compress(self.grid, self.grid.spacing[:, 0], surface_label="rho")
+        w = compress(
+            self._transforms["grid"],
+            self._transforms["grid"].spacing[:, 0],
+            surface_label="rho",
+        )
         return super().compute_scaled(*args, **kwargs) * jnp.sqrt(w)
 
     def print_value(self, *args, **kwargs):
         """Print the value of the objective."""
         f = self.compute(*args, **kwargs)
         print("Maximum " + self._print_value_fmt.format(jnp.max(f)) + self._units)
         print("Minimum " + self._print_value_fmt.format(jnp.min(f)) + self._units)
@@ -244,15 +252,15 @@
         bounds=(0, np.inf),
         weight=1,
         normalize=True,
         normalize_target=True,
         grid=None,
         name="Magnetic Well",
     ):
-        self.grid = grid
+        self._grid = grid
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -267,34 +275,36 @@
         eq : Equilibrium, optional
             Equilibrium that will be optimized to satisfy the Objective.
         use_jit : bool, optional
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
         """
-        if self.grid is None:
-            self.grid = LinearGrid(
+        if self._grid is None:
+            grid = LinearGrid(
                 M=eq.M_grid,
                 N=eq.N_grid,
                 NFP=eq.NFP,
                 sym=eq.sym,
                 rho=np.linspace(1 / 5, 1, 5),
             )
+        else:
+            grid = self._grid
 
-        self._dim_f = self.grid.num_rho
+        self._dim_f = grid.num_rho
         self._data_keys = ["magnetic well"]
         self._args = get_params(self._data_keys)
 
         timer = Timer()
         if verbose > 0:
             print("Precomputing transforms")
         timer.start("Precomputing transforms")
 
-        self._profiles = get_profiles(self._data_keys, eq=eq, grid=self.grid)
-        self._transforms = get_transforms(self._data_keys, eq=eq, grid=self.grid)
+        self._profiles = get_profiles(self._data_keys, eq=eq, grid=grid)
+        self._transforms = get_transforms(self._data_keys, eq=eq, grid=grid)
 
         timer.stop("Precomputing transforms")
         if verbose > 1:
             timer.disp("Precomputing transforms")
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
@@ -335,19 +345,25 @@
         params = self._parse_args(*args, **kwargs)
         data = compute_fun(
             self._data_keys,
             params=params,
             transforms=self._transforms,
             profiles=self._profiles,
         )
-        return compress(self.grid, data["magnetic well"], surface_label="rho")
+        return compress(
+            self._transforms["grid"], data["magnetic well"], surface_label="rho"
+        )
 
     def compute_scaled(self, *args, **kwargs):
         """Compute and apply the target/bounds, weighting, and normalization."""
-        w = compress(self.grid, self.grid.spacing[:, 0], surface_label="rho")
+        w = compress(
+            self._transforms["grid"],
+            self._transforms["grid"].spacing[:, 0],
+            surface_label="rho",
+        )
         return super().compute_scaled(*args, **kwargs) * jnp.sqrt(w)
 
     def print_value(self, *args, **kwargs):
         """Print the value of the objective."""
         f = self.compute(*args, **kwargs)
         print("Maximum " + self._print_value_fmt.format(jnp.max(f)) + self._units)
         print("Minimum " + self._print_value_fmt.format(jnp.min(f)) + self._units)
```

### Comparing `desc-opt-0.8.1/desc/objectives/linear_objectives.py` & `desc-opt-0.8.2/desc/objectives/linear_objectives.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,177 @@
 
 from desc.backend import jnp
 from desc.basis import zernike_radial, zernike_radial_coeffs
 
 from .normalization import compute_scaling_factors
 from .objective_funs import _Objective
 
-# TODO: need dim_x attribute
+
+class BoundaryRSelfConsistency(_Objective):
+    """Ensure that the boundary and interior surfaces are self consistent.
+
+    Note: this constraint is automatically applied when needed, and does not need to be
+    included by the user.
+
+    Parameters
+    ----------
+    eq : Equilibrium, optional
+        Equilibrium that will be optimized to satisfy the Objective.
+    surface_label : float
+        Surface to enforce boundary conditions on. Defaults to Equilibrium.surface.rho
+    name : str
+        Name of the objective function.
+
+    """
+
+    _scalar = False
+    _linear = True
+    _fixed = False
+    _units = "(m)"
+    _print_value_fmt = "R boundary self consistency error: {:10.3e} "
+
+    def __init__(
+        self,
+        eq=None,
+        surface_label=None,
+        name="self_consistency R",
+    ):
+
+        self._surface_label = surface_label
+        self._args = ["R_lmn", "Rb_lmn"]
+        super().__init__(
+            eq=eq,
+            target=0,
+            bounds=None,
+            weight=1,
+            normalize=False,
+            normalize_target=False,
+            name=name,
+        )
+
+    def build(self, eq, use_jit=False, verbose=1):
+        """Build constant arrays.
+
+        Parameters
+        ----------
+        eq : Equilibrium, optional
+            Equilibrium that will be optimized to satisfy the Objective.
+        use_jit : bool, optional
+            Whether to just-in-time compile the objective and derivatives.
+        verbose : int, optional
+            Level of output.
+
+        """
+        modes = eq.surface.R_basis.modes
+        idx = np.arange(eq.surface.R_basis.num_modes)
+
+        self._dim_f = idx.size
+        self._A = np.zeros((self._dim_f, eq.R_basis.num_modes))
+        for i, (l, m, n) in enumerate(eq.R_basis.modes):
+            if eq.bdry_mode == "lcfs":
+                j = np.argwhere((modes[:, 1:] == [m, n]).all(axis=1))
+                surf = (
+                    eq.surface.rho
+                    if self._surface_label is None
+                    else self._surface_label
+                )
+                self._A[j, i] = zernike_radial(surf, l, m)
+            else:
+                raise NotImplementedError(
+                    "bdry_mode is not lcfs, yell at Dario to finish poincare stuff"
+                )
+
+        super().build(eq=eq, use_jit=use_jit, verbose=verbose)
+
+    def compute(self, *args, **kwargs):
+        """Compute boundary self consistency errror."""
+        params = self._parse_args(*args, **kwargs)
+        return jnp.dot(self._A, params["R_lmn"]) - params["Rb_lmn"]
+
+
+class BoundaryZSelfConsistency(_Objective):
+    """Ensure that the boundary and interior surfaces are self consistent.
+
+    Note: this constraint is automatically applied when needed, and does not need to be
+    included by the user.
+
+    Parameters
+    ----------
+    eq : Equilibrium, optional
+        Equilibrium that will be optimized to satisfy the Objective.
+    surface_label : float
+        Surface to enforce boundary conditions on. Defaults to Equilibrium.surface.rho
+    name : str
+        Name of the objective function.
+
+    """
+
+    _scalar = False
+    _linear = True
+    _fixed = False
+    _units = "(m)"
+    _print_value_fmt = "Z boundary self consistency error: {:10.3e} "
+
+    def __init__(
+        self,
+        eq=None,
+        surface_label=None,
+        name="self_consistency Z",
+    ):
+
+        self._surface_label = surface_label
+        self._args = ["Z_lmn", "Zb_lmn"]
+        super().__init__(
+            eq=eq,
+            target=0,
+            bounds=None,
+            weight=1,
+            normalize=False,
+            normalize_target=False,
+            name=name,
+        )
+
+    def build(self, eq, use_jit=False, verbose=1):
+        """Build constant arrays.
+
+        Parameters
+        ----------
+        eq : Equilibrium, optional
+            Equilibrium that will be optimized to satisfy the Objective.
+        use_jit : bool, optional
+            Whether to just-in-time compile the objective and derivatives.
+        verbose : int, optional
+            Level of output.
+
+        """
+        modes = eq.surface.Z_basis.modes
+        idx = np.arange(eq.surface.Z_basis.num_modes)
+
+        self._dim_f = idx.size
+        self._A = np.zeros((self._dim_f, eq.Z_basis.num_modes))
+        for i, (l, m, n) in enumerate(eq.Z_basis.modes):
+            if eq.bdry_mode == "lcfs":
+                j = np.argwhere((modes[:, 1:] == [m, n]).all(axis=1))
+                surf = (
+                    eq.surface.rho
+                    if self._surface_label is None
+                    else self._surface_label
+                )
+                self._A[j, i] = zernike_radial(surf, l, m)
+            else:
+                raise NotImplementedError(
+                    "bdry_mode is not lcfs, yell at Dario to finish poincare stuff"
+                )
+
+        super().build(eq=eq, use_jit=use_jit, verbose=verbose)
+
+    def compute(self, *args, **kwargs):
+        """Compute boundary self consistency errror."""
+        params = self._parse_args(*args, **kwargs)
+        return jnp.dot(self._A, params["Z_lmn"]) - params["Zb_lmn"]
 
 
 class FixBoundaryR(_Objective):
     """Boundary condition on the R boundary parameters.
 
     Parameters
     ----------
@@ -38,17 +200,14 @@
         len(weight) must be equal to Objective.dim_f
     normalize : bool
         Whether to compute the error in physical units or non-dimensionalize.
     normalize_target : bool
         Whether target should be normalized before comparing to computed values.
         if `normalize` is `True` and the target is in physical units, this should also
         be set to True.
-    fixed_boundary : bool, optional
-        True to enforce the boundary condition on flux surfaces,
-        or False to fix the boundary surface coefficients (default).
     modes : ndarray, optional
         Basis modes numbers [l,m,n] of boundary modes to fix.
         len(target) = len(weight) = len(modes).
         If True/False uses all/none of the profile modes.
     surface_label : float
         Surface to enforce boundary conditions on. Defaults to Equilibrium.surface.rho
     name : str
@@ -60,36 +219,35 @@
     If specifying particular modes to fix, the rows of the resulting constraint `A`
     matrix and `target` vector will be re-sorted according to the ordering of
     `basis.modes` which may be different from the order that was passed in.
     """
 
     _scalar = False
     _linear = True
-    _fixed = False  # TODO: can we dynamically detect this instead?
+    _fixed = False
     _units = "(m)"
     _print_value_fmt = "R boundary error: {:10.3e} "
 
     def __init__(
         self,
         eq=None,
         target=None,
         bounds=None,
         weight=1,
         normalize=True,
         normalize_target=True,
-        fixed_boundary=False,
         modes=True,
         surface_label=None,
         name="lcfs R",
     ):
 
-        self._fixed_boundary = fixed_boundary
         self._modes = modes
+        self._target_from_user = target
         self._surface_label = surface_label
-        self._args = ["R_lmn"] if self._fixed_boundary else ["Rb_lmn"]
+        self._args = ["Rb_lmn"]
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -137,56 +295,42 @@
                         "Some of the given modes are not in the surface, "
                         + "these modes will not be fixed.",
                         "yellow",
                     )
                 )
 
         self._dim_f = idx.size
-        if self.target is not None:  # rearrange given target to match modes order
+        if self._target_from_user is not None:
             if self._modes is True or self._modes is False:
                 raise RuntimeError(
                     "Attempting to provide target for R boundary modes without "
                     + "providing modes array!"
                     + "You must pass in the modes corresponding to the"
                     + "provided target"
                 )
-            self.target = self.target[modes_idx]
+            # rearrange given target to match modes order
+            self.target = self._target_from_user[modes_idx]
 
-        if self._fixed_boundary:  # R_lmn -> Rb_lmn boundary condition
-            self._A = np.zeros((self._dim_f, eq.R_basis.num_modes))
-            for i, (l, m, n) in enumerate(eq.R_basis.modes):
-                if eq.bdry_mode == "lcfs":
-                    j = np.argwhere((modes[:, 1:] == [m, n]).all(axis=1))
-                    surf = (
-                        eq.surface.rho
-                        if self._surface_label is None
-                        else self._surface_label
-                    )
-                    self._A[j, i] = zernike_radial(surf, l, m)
-
-        else:  # Rb_lmn -> Rb optimization space
-            self._A = np.eye(eq.surface.R_basis.num_modes)[idx, :]
+        # Rb_lmn -> Rb optimization space
+        self._A = np.eye(eq.surface.R_basis.num_modes)[idx, :]
 
         # use surface parameters as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = eq.surface.R_lmn[idx]
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
             self._normalization = scales["a"]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, *args, **kwargs):
         """Compute deviation from desired boundary."""
-        if len(args):
-            x = kwargs.get(self.args[0], args[0])
-        else:
-            x = kwargs.get(self.args[0])
-        return jnp.dot(self._A, x)
+        params = self._parse_args(*args, **kwargs)
+        return jnp.dot(self._A, params["Rb_lmn"])
 
     @property
     def target_arg(self):
         """str: Name of argument corresponding to the target."""
         return "Rb_lmn"
 
 
@@ -207,17 +351,14 @@
         len(weight) must be equal to Objective.dim_f
     normalize : bool
         Whether to compute the error in physical units or non-dimensionalize.
     normalize_target : bool
         Whether target should be normalized before comparing to computed values.
         if `normalize` is `True` and the target is in physical units, this should also
         be set to True.
-    fixed_boundary : bool, optional
-        True to enforce the boundary condition on flux surfaces,
-        or False to fix the boundary surface coefficients (default).
     modes : ndarray, optional
         Basis modes numbers [l,m,n] of boundary modes to fix.
         len(target) = len(weight) = len(modes).
         If True/False uses all/none of the surface modes.
     surface_label : float
         Surface to enforce boundary conditions on. Defaults to Equilibrium.surface.rho
     name : str
@@ -241,24 +382,23 @@
         self,
         eq=None,
         target=None,
         bounds=None,
         weight=1,
         normalize=True,
         normalize_target=True,
-        fixed_boundary=False,
         modes=True,
         surface_label=None,
         name="lcfs Z",
     ):
 
-        self._fixed_boundary = fixed_boundary
         self._modes = modes
+        self._target_from_user = target
         self._surface_label = surface_label
-        self._args = ["Z_lmn"] if self._fixed_boundary else ["Zb_lmn"]
+        self._args = ["Zb_lmn"]
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -306,64 +446,54 @@
                         "Some of the given modes are not in the surface, "
                         + "these modes will not be fixed.",
                         "yellow",
                     )
                 )
 
         self._dim_f = idx.size
-        if self.target is not None:  # rearrange given target to match modes order
+        if self._target_from_user is not None:
             if self._modes is True or self._modes is False:
                 raise RuntimeError(
                     "Attempting to provide target for Z boundary modes without "
                     + "providing modes array!"
                     + "You must pass in the modes corresponding to the"
                     + "provided target"
                 )
-            self.target = self.target[modes_idx]
+            # rearrange given target to match modes order
+            self.target = self._target_from_user[modes_idx]
 
-        if self._fixed_boundary:  # Z_lmn -> Zb_lmn boundary condition
-            self._A = np.zeros((self._dim_f, eq.Z_basis.num_modes))
-            for i, (l, m, n) in enumerate(eq.Z_basis.modes):
-                if eq.bdry_mode == "lcfs":
-                    j = np.argwhere((modes[:, 1:] == [m, n]).all(axis=1))
-                    surf = (
-                        eq.surface.rho
-                        if self._surface_label is None
-                        else self._surface_label
-                    )
-                    self._A[j, i] = zernike_radial(surf, l, m)
-        else:  # Zb_lmn -> Zb optimization space
-            self._A = np.eye(eq.surface.Z_basis.num_modes)[idx, :]
+        # Zb_lmn -> Zb optimization space
+        self._A = np.eye(eq.surface.Z_basis.num_modes)[idx, :]
 
         # use surface parameters as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = eq.surface.Z_lmn[idx]
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
             self._normalization = scales["a"]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, *args, **kwargs):
         """Compute deviation from desired boundary."""
-        if len(args):
-            x = kwargs.get(self.args[0], args[0])
-        else:
-            x = kwargs.get(self.args[0])
-        return jnp.dot(self._A, x)
+        params = self._parse_args(*args, **kwargs)
+        return jnp.dot(self._A, params["Zb_lmn"])
 
     @property
     def target_arg(self):
         """str: Name of argument corresponding to the target."""
         return "Zb_lmn"
 
 
 class FixLambdaGauge(_Objective):
-    """Fixes gauge freedom for lambda: lambda(rho=0)=0 and lambda(theta=0,zeta=0)=0.
+    """Fixes gauge freedom for lambda: lambda(theta=0,zeta=0)=0.
+
+    Note: this constraint is automatically applied when needed, and does not need to be
+    included by the user.
 
     Parameters
     ----------
     eq : Equilibrium, optional
         Equilibrium that will be optimized to satisfy the Objective.
     target : float, ndarray, optional
         Value to fix lambda to at rho=0 and (theta=0,zeta=0)
@@ -581,14 +711,15 @@
         modes=True,
         normalize=True,
         normalize_target=True,
         name="axis R",
     ):
 
         self._modes = modes
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -656,28 +787,28 @@
                 j = np.argwhere(n == ns)
                 self._A[j, i] = 1
             else:
                 j = np.argwhere(n == ns)
                 self._A[j, i] = -1
 
         # use axis parameters as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = np.zeros(self._dim_f)
             for n, Rn in zip(eq.axis.R_basis.modes[:, 2], eq.axis.R_n):
                 j = np.argwhere(ns == n)
                 self.target[j] = Rn
         else:  # rearrange given target to match modes order
             if self._modes is True or self._modes is False:
                 raise RuntimeError(
                     "Attempting to provide target for R axis modes without "
                     + "providing modes array!"
                     + "You must pass in the modes corresponding to the"
                     + "provided target axis"
                 )
-            self.target = self.target[modes_idx]
+            self.target = self._target_from_user[modes_idx]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, R_lmn, **kwargs):
         """Compute axis R errors.
 
         Parameters
@@ -730,14 +861,15 @@
         modes=True,
         name="axis Z",
         normalize=True,
         normalize_target=True,
     ):
 
         self._modes = modes
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -803,28 +935,28 @@
                 j = np.argwhere(n == ns)
                 self._A[j, i] = 1
             else:
                 j = np.argwhere(n == ns)
                 self._A[j, i] = -1
 
         # use axis parameters as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = np.zeros(self._dim_f)
             for n, Zn in zip(eq.axis.Z_basis.modes[:, 2], eq.axis.Z_n):
                 j = np.argwhere(ns == n)
                 self.target[j] = Zn
         else:  # rearrange given target to match modes order
             if self._modes is True or self._modes is False:
                 raise RuntimeError(
                     "Attempting to provide target for Z axis modes without "
                     + "providing modes array!"
                     + "You must pass in the modes corresponding to the"
                     + "provided target axis"
                 )
-            self.target = self.target[modes_idx]
+            self.target = self._target_from_user[modes_idx]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, Z_lmn, **kwargs):
         """Compute axis Z errors.
 
         Parameters
@@ -883,14 +1015,15 @@
     ):
 
         self._modes = modes
         if modes is None or modes is False:
             raise ValueError(
                 f"modes kwarg must be specified or True with FixModeR! got {modes}"
             )
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -933,25 +1066,25 @@
                         "yellow",
                     )
                 )
 
         self._dim_f = modes_idx.size
 
         # use current eq's coefficients as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = eq.R_lmn[self._idx]
         else:  # rearrange given target to match modes order
             if self._modes is True or self._modes is False:
                 raise RuntimeError(
                     "Attempting to provide target for R fixed modes without "
                     + "providing modes array!"
                     + "You must pass in the modes corresponding to the"
                     + "provided target modes"
                 )
-            self.target = self.target[modes_idx]
+            self.target = self._target_from_user[modes_idx]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, R_lmn, **kwargs):
         """Compute Fixed mode R errors.
 
         Parameters
@@ -1015,15 +1148,15 @@
     ):
 
         self._modes = modes
         if modes is None or modes is False:
             raise ValueError(
                 f"modes kwarg must be specified or True with FixModeZ! got {modes}"
             )
-
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -1066,25 +1199,25 @@
                         "yellow",
                     )
                 )
 
         self._dim_f = modes_idx.size
 
         # use current eq's coefficients as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = eq.Z_lmn[self._idx]
         else:  # rearrange given target to match modes order
             if self._modes is True or self._modes is False:
                 raise RuntimeError(
                     "Attempting to provide target for Z fixed modes without "
                     + "providing modes array!"
                     + "You must pass in the modes corresponding to the"
                     + "provided target modes"
                 )
-            self.target = self.target[modes_idx]
+            self.target = self._target_from_user[modes_idx]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, Z_lmn, **kwargs):
         """Compute Fixed mode Z errors.
 
         Parameters
@@ -1163,14 +1296,15 @@
         if target is not None:
             if target.size > 1:
                 raise ValueError(
                     "FixSumModesR only accepts 1 target value, please use multiple"
                     + " FixSumModesR objectives if you wish to have multiple"
                     + " sets of constrained mode sums!"
                 )
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -1219,23 +1353,23 @@
                         "yellow",
                     )
                 )
         if self._sum_weights is None:
             sum_weights = np.ones(modes.shape[0])
         else:
             sum_weights = np.atleast_1d(self._sum_weights)
-        self._dim_f = np.array([1])
+        self._dim_f = 1
 
         self._A = np.zeros((1, eq.R_basis.num_modes))
         for i, (l, m, n) in enumerate(modes):
             j = eq.R_basis.get_idx(L=l, M=m, N=n)
             self._A[0, j] = sum_weights[i]
 
         # use current sum as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = np.dot(sum_weights.T, eq.R_lmn[self._idx])
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, R_lmn, **kwargs):
         """Compute Sum mode R errors.
 
@@ -1315,14 +1449,15 @@
         if target is not None:
             if target.size > 1:
                 raise ValueError(
                     "FixSumModesZ only accepts 1 target value, please use multiple"
                     + " FixSumModesZ objectives if you wish to have multiple sets of"
                     + " constrained mode sums!"
                 )
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             weight=weight,
             name=name,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -1372,23 +1507,23 @@
                         "yellow",
                     )
                 )
         if self._sum_weights is None:
             sum_weights = np.ones(modes.shape[0])
         else:
             sum_weights = np.atleast_1d(self._sum_weights)
-        self._dim_f = np.array([1])
+        self._dim_f = 1
 
         self._A = np.zeros((1, eq.Z_basis.num_modes))
         for i, (l, m, n) in enumerate(modes):
             j = eq.Z_basis.get_idx(L=l, M=m, N=n)
             self._A[0, j] = sum_weights[i]
 
         # use current sum as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = np.dot(sum_weights.T, eq.Z_lmn[self._idx])
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
     def compute(self, Z_lmn, **kwargs):
         """Compute Sum mode Z errors.
 
@@ -1465,14 +1600,15 @@
         profile=None,
         indices=True,
         name="",
     ):
 
         self._profile = profile
         self._indices = indices
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -1503,15 +1639,15 @@
         elif self._indices is True:  # all indices of Profile.params
             self._idx = np.arange(np.size(self._profile.params))
         else:  # specified indices
             self._idx = np.atleast_1d(self._indices)
 
         self._dim_f = self._idx.size
         # use profile parameters as target if needed
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = self._profile.params[self._idx]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
 
 
 class FixPressure(_FixProfile):
     """Fixes pressure coefficients.
@@ -2331,15 +2467,15 @@
         target=None,
         bounds=None,
         weight=1,
         normalize=True,
         normalize_target=True,
         name="fixed-Psi",
     ):
-
+        self._target_from_user = target
         super().__init__(
             eq=eq,
             target=target,
             bounds=bounds,
             weight=weight,
             normalize=normalize,
             normalize_target=normalize_target,
@@ -2357,15 +2493,15 @@
             Whether to just-in-time compile the objective and derivatives.
         verbose : int, optional
             Level of output.
 
         """
         self._dim_f = 1
 
-        if self.target is None:
+        if self._target_from_user is None:
             self.target = eq.Psi
 
         if self._normalize:
             scales = compute_scaling_factors(eq)
             self._normalization = scales["Psi"]
 
         super().build(eq=eq, use_jit=use_jit, verbose=verbose)
```

### Comparing `desc-opt-0.8.1/desc/objectives/nae_utils.py` & `desc-opt-0.8.2/desc/objectives/nae_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         tuple of constraints of type FixSumModesR, which enforce
         the O(rho) behavior of the equilibrium R coefficents to match the NAE.
     Zconstraints : tuple of Objective
         tuple of constraints of type FixSumModesZ, which enforce
         the O(rho) behavior of the equilibrium Z coefficents to match the NAE.
     """
     # r is the ratio  r_NAE / rho_DESC
-    r = np.sqrt(2 * desc_eq.Psi / qsc.Bbar / 2 / np.pi)
+    r = np.sqrt(2 * abs(desc_eq.Psi / qsc.Bbar) / 2 / np.pi)
 
     Rconstraints = ()
     Zconstraints = ()
     Rbasis_cos = bases["Rbasis_cos"]
     Zbasis_cos = bases["Zbasis_cos"]
     Rbasis_sin = bases["Rbasis_sin"]
     Zbasis_sin = bases["Zbasis_sin"]
@@ -163,15 +163,14 @@
         target = NAEcoeff * r
         for k in range(1, int((desc_eq.L + 1) / 2) + 1):
             modes.append([2 * k - 1, 1, n])
             sum_weights.append([(-1) ** k * k])
         modes = np.atleast_2d(modes)
         sum_weights = -np.atleast_1d(sum_weights)
         Rcon = FixSumModesR(target=target, sum_weights=sum_weights, modes=modes)
-        desc_eq.R_lmn
         Rconstraints += (Rcon,)
     # Z_1_neg1_n
     for n, NAEcoeff in zip(Zbasis_cos.modes[:, 2], coeffs["Z_1_neg1_n"]):
         sum_weights = []
         modes = []
         target = NAEcoeff * r
         for k in range(1, int((desc_eq.L + 1) / 2) + 1):
```

### Comparing `desc-opt-0.8.1/desc/objectives/normalization.py` & `desc-opt-0.8.2/desc/objectives/normalization.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/objectives/objective_funs.py` & `desc-opt-0.8.2/desc/objectives/objective_funs.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,19 +52,26 @@
         self._deriv_mode = deriv_mode
         self._built = False
         self._compiled = False
 
         if eq is not None:
             self.build(eq, use_jit=self._use_jit, verbose=verbose)
 
-    def _set_state_vector(self):
-        """Set state vector components, dimensions, and indices."""
-        self._args = np.concatenate([obj.args for obj in self.objectives])
+    def set_args(self, *args):
+        """Set which arguments the objective should expect.
+
+        Defaults to args from all sub-objectives. Additional arguments can be passed in.
+        """
+        self._args = list(np.concatenate([obj.args for obj in self.objectives]))
+        self._args += list(args)
         self._args = [arg for arg in arg_order if arg in self._args]
+        self._set_state_vector()
 
+    def _set_state_vector(self):
+        """Set state vector components, dimensions, and indices."""
         self._dimensions = self.objectives[0].dimensions
 
         self._dim_x = 0
         self._x_idx = {}
         for arg in self.args:
             self.x_idx[arg] = np.arange(self._dim_x, self._dim_x + self.dimensions[arg])
             self._dim_x += self.dimensions[arg]
@@ -175,15 +182,15 @@
             objective.build(eq, use_jit=self.use_jit, verbose=verbose)
             self._dim_f += objective.dim_f
         if self._dim_f == 1:
             self._scalar = True
         else:
             self._scalar = False
 
-        self._set_state_vector()
+        self.set_args()
         self._set_derivatives()
         if self.use_jit:
             self.jit()
 
         self._built = True
         timer.stop("Objective build")
         if verbose > 1:
@@ -263,15 +270,18 @@
 
         """
         if not self.built:
             raise RuntimeError("ObjectiveFunction must be built first.")
 
         x = jnp.atleast_1d(x)
         if x.size != self.dim_x:
-            raise ValueError("Input vector dimension is invalid.")
+            raise ValueError(
+                "Input vector dimension is invalid, expected "
+                + f"{self.dim_x} got {x.size}."
+            )
 
         kwargs = {}
         for arg in self.args:
             kwargs[arg] = jnp.atleast_1d(x[self.x_idx[arg]])
         return kwargs
 
     def _kwargs_to_args(self, kwargs, args):
@@ -536,21 +546,27 @@
                 )
                 self._derivatives["hess"][arg] = Derivative(
                     self.compute_scalar,
                     argnum=self.args.index(arg),
                     mode="hess",
                 )
             else:  # these derivatives are always zero
-                self._derivatives["jac"][arg] = lambda *args, **kwargs: jnp.zeros(
+                self._derivatives["jac"][
+                    arg
+                ] = lambda *args, arg=arg, **kwargs: jnp.zeros(
                     (self.dim_f, self.dimensions[arg])
                 )
-                self._derivatives["grad"][arg] = lambda *args, **kwargs: jnp.zeros(
+                self._derivatives["grad"][
+                    arg
+                ] = lambda *args, arg=arg, **kwargs: jnp.zeros(
                     (1, self.dimensions[arg])
                 )
-                self._derivatives["hess"][arg] = lambda *args, **kwargs: jnp.zeros(
+                self._derivatives["hess"][
+                    arg
+                ] = lambda *args, arg=arg, **kwargs: jnp.zeros(
                     (self.dimensions[arg], self.dimensions[arg])
                 )
 
     def jit(self):
         """Apply JIT to compute methods, or re-apply after updating self."""
         # doing str name type checking to avoid importing weird jax private stuff
         # for proper isinstance check
```

### Comparing `desc-opt-0.8.1/desc/objectives/utils.py` & `desc-opt-0.8.2/desc/objectives/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """Functions for getting common objectives and constraints."""
 
 import numpy as np
 
-from desc.backend import block_diag, jnp, put
+from desc.backend import jnp, put
 from desc.compute import arg_order
-from desc.utils import svd_inv_null
+from desc.utils import Index, svd_inv_null
 
 from ._equilibrium import (
     CurrentDensity,
     Energy,
     ForceBalance,
     HelicalForceBalance,
     RadialForceBalance,
 )
 from .linear_objectives import (
+    BoundaryRSelfConsistency,
+    BoundaryZSelfConsistency,
     FixAtomicNumber,
     FixAxisR,
     FixAxisZ,
     FixBoundaryR,
     FixBoundaryZ,
     FixCurrent,
     FixElectronDensity,
@@ -51,21 +53,16 @@
     Returns
     -------
     constraints, tuple of _Objectives
         A list of the linear constraints used in fixed-boundary problems.
 
     """
     constraints = (
-        FixBoundaryR(
-            fixed_boundary=True, normalize=normalize, normalize_target=normalize
-        ),
-        FixBoundaryZ(
-            fixed_boundary=True, normalize=normalize, normalize_target=normalize
-        ),
-        FixLambdaGauge(normalize=normalize, normalize_target=normalize),
+        FixBoundaryR(normalize=normalize, normalize_target=normalize),
+        FixBoundaryZ(normalize=normalize, normalize_target=normalize),
         FixPsi(normalize=normalize, normalize_target=normalize),
     )
     if profiles:
         if kinetic:
             constraints += (
                 FixElectronDensity(normalize=normalize, normalize_target=normalize),
                 FixElectronTemperature(normalize=normalize, normalize_target=normalize),
@@ -82,14 +79,29 @@
         else:
             constraints += (
                 FixCurrent(normalize=normalize, normalize_target=normalize),
             )
     return constraints
 
 
+def maybe_add_self_consistency(constraints):
+    """Add self consistency constraints if needed."""
+
+    def _is_any_instance(things, cls):
+        return any([isinstance(t, cls) for t in things])
+
+    if not _is_any_instance(constraints, BoundaryRSelfConsistency):
+        constraints += (BoundaryRSelfConsistency(),)
+    if not _is_any_instance(constraints, BoundaryZSelfConsistency):
+        constraints += (BoundaryZSelfConsistency(),)
+    if not _is_any_instance(constraints, FixLambdaGauge):
+        constraints += (FixLambdaGauge(),)
+    return constraints
+
+
 def get_fixed_axis_constraints(profiles=True, iota=True):
     """Get the constraints necessary for a fixed-axis equilibrium problem.
 
     Parameters
     ----------
     profiles : bool
         Whether to also return constraints to fix input profiles.
@@ -140,15 +152,14 @@
     constraints, tuple of _Objectives
         A list of the linear constraints used in fixed-axis problems.
     """
 
     constraints = (
         FixAxisR(),
         FixAxisZ(),
-        FixLambdaGauge(),
         FixPsi(),
     )
     if profiles:
         constraints += (FixPressure(),)
 
         if iota:
             constraints += (FixIota(),)
@@ -210,22 +221,20 @@
     objective_args : list of str
         names of all arguments used by the desired objective.
 
     Returns
     -------
     xp : ndarray
         particular solution to Ax=b
-    A : dict of ndarray
-        Individual constraint matrices, keyed by argument
-    Ainv : dict of ndarray
-        Individual pseudoinverses of constraint matrices
-    b : dict of ndarray
-        Individual rhs vectors
+    A : ndarray ndarray
+        Combined constraint matrix, such that A @ x[unfixed_idx] == b
+    b : list of ndarray
+        Combined rhs vector
     Z : ndarray
-        Null space operator for full combined A
+        Null space operator for full combined A such that A @ Z == 0
     unfixed_idx : ndarray
         indices of x that correspond to non-fixed values
     project, recover : function
         functions to project full vector x into reduced vector y,
         and recovering x from y.
 
     """
@@ -233,130 +242,103 @@
     args = np.concatenate([obj.args for obj in constraints])
     args = np.concatenate((args, objective_args))
     # this is all args used by both constraints and objective
     args = [arg for arg in arg_order if arg in args]
     dimensions = constraints[0].dimensions
     dim_x = 0
     x_idx = {}
-    for arg in objective_args:
+    for arg in args:
         x_idx[arg] = np.arange(dim_x, dim_x + dimensions[arg])
         dim_x += dimensions[arg]
 
-    A = {}
-    _A_unweighted = {}  # keep unweighted A here and use this to find Ainv
-    b = {}
-    Ainv = {}
-    arg_obj_lists = {}
+    A = []
+    b = []
     xp = jnp.zeros(dim_x)  # particular solution to Ax=b
-    constraint_args = []  # all args used in constraints
-    unfixed_args = []  # subset of constraint args for unfixed objectives
 
     # linear constraint matrices for each objective
     for obj_ind, obj in enumerate(constraints):
-        if len(obj.args) > 1:
-            raise ValueError("Linear constraints must have only 1 argument.")
         if obj.bounds is not None:
             raise ValueError("Linear constraints must use target instead of bounds.")
-        arg = obj.args[0]
-        if arg not in objective_args:
-            continue
-        if arg not in constraint_args:  # hope this does not mess
-            constraint_args.append(arg)
-        if obj.fixed and obj.dim_f == dimensions[obj.target_arg]:
-            # if all coefficients are fixed the constraint matrices are not needed
-            xp = put(xp, x_idx[obj.target_arg], obj.target)
-
-        else:
-            A_ = obj.derivatives["jac"][arg](jnp.zeros(obj.dimensions[arg]))
-            # using obj.compute instead of obj.target to allow for correct scale/weight
-            b_ = -obj.compute_scaled(jnp.zeros(obj.dimensions[arg]))
-            if arg not in A.keys():
-                A[arg] = A_
-
-                _A_unweighted[arg] = (
-                    obj.normalization * (A_.T / obj.weight).T
-                )  # undo normalization here for each indiv A
-                b[arg] = b_
-                unfixed_args.append(arg)
-                arg_obj_lists[arg] = [obj]
-            elif b_.size > 0:  # we want to stack these vertically if the same arg
-                # but only if the constraint actually constrains anything
-                # if not, i.e. if attempted to fix a mode that is not in the basis,
-                # b_ is an empty array and does not need to be added
-                rk_before = jnp.linalg.matrix_rank(A[arg])
-                A[arg] = jnp.vstack((A[arg], A_))
-                rk_after = jnp.linalg.matrix_rank(A[arg])
-                if (
-                    rk_after < rk_before + A_.shape[0]
-                ):  # if less, there are some lin dependent rows of A_ and A[arg]
-                    # for example, could be trying to constrain same mode with 2
-                    # different values
-                    raise RuntimeError(
-                        f"Incompatible constraints given for {arg}!"
-                        + f" constraint {obj} is incompatible with"
-                        + f" {*arg_obj_lists[arg],}"
-                    )
-                _A_unweighted[arg] = jnp.vstack(
-                    (A[arg], A_ / obj.weight * obj.normalization)
-                )
-                arg_obj_lists[arg] += [obj]
-
-                b[arg] = jnp.hstack((b[arg], b_))
-    # find inverse of the now-combined constraint matrices for each arg
-    for key in list(A.keys()):
-        if A[key].shape[0]:
-            Ainv[key], Z_ = svd_inv_null(_A_unweighted[key])
-        else:
-            Ainv[key] = _A_unweighted[
-                key
-            ].T  # make inverse matrices using already unweighted A
-
-    # catch any arguments that are not constrained
-    for arg in x_idx.keys():
-        if arg not in constraint_args:
-            unfixed_args.append(arg)
-            A[arg] = jnp.zeros((1, dimensions[arg]))
-            b[arg] = jnp.zeros((1,))
-
-    # full A matrix for all unfixed constraints
-    if len(A):
-        unfixed_idx = jnp.concatenate(
-            [x_idx[arg] for arg in arg_order if arg in A.keys()]
+        A_ = {
+            arg: obj.derivatives["jac"][arg](
+                *[jnp.zeros(obj.dimensions[arg]) for arg in obj.args]
+            )
+            for arg in args
+        }
+        # using obj.compute instead of obj.target to allow for correct scale/weight
+        b_ = -obj.compute_scaled(*[jnp.zeros(obj.dimensions[arg]) for arg in obj.args])
+        A.append(A_)
+        b.append(b_)
+
+    A_full = jnp.vstack([jnp.hstack([Ai[arg] for arg in args]) for Ai in A])
+    b_full = jnp.concatenate(b)
+    # fixed just means there is a single element in A, so A_ij*x_j = b_i
+    fixed_rows = np.where(np.count_nonzero(A_full, axis=1) == 1)[0]
+    # indices of x that are fixed = cols of A where rows have 1 nonzero val.
+    _, fixed_idx = np.where(A_full[fixed_rows])
+    unfixed_rows = np.setdiff1d(np.arange(A_full.shape[0]), fixed_rows)
+    unfixed_idx = np.setdiff1d(np.arange(xp.size), fixed_idx)
+    if len(fixed_rows):
+        # something like 0.5 x1 = 2 is the same as x1 = 4
+        b_full = put(
+            b_full, fixed_rows, b_full[fixed_rows] / np.sum(A_full[fixed_rows], axis=1)
+        )
+        A_full = put(
+            A_full,
+            Index[fixed_rows, :],
+            A_full[fixed_rows] / np.sum(A_full[fixed_rows], axis=1)[:, None],
+        )
+        xp = put(xp, fixed_idx, b_full[fixed_rows])
+        # some values might be fixed, but they still show up in other constraints
+        # this is where the fixed cols have >1 nonzero val
+        # for fixed variables, we delete that row and col of A, but that means
+        # we need to subtract the fixed value from b so that the equation is balanced.
+        # eg 2 x1 + 3 x2 + 1 x3= 4 ;    4 x1 = 2
+        # combining gives 3 x2 + 1 x3 = 3, with x1 now removed
+        b_full = put(
+            b_full,
+            unfixed_rows,
+            b_full[unfixed_rows]
+            - A_full[unfixed_rows][:, fixed_idx] @ b_full[fixed_rows],
         )
-        A_full = block_diag(*[A[arg] for arg in arg_order if arg in A.keys()])
-        b_full = jnp.concatenate([b[arg] for arg in arg_order if arg in b.keys()])
+    A_full = A_full[unfixed_rows][:, unfixed_idx]
+    b_full = b_full[unfixed_rows]
+    if A_full.size:
         Ainv_full, Z = svd_inv_null(A_full)
-        xp = put(xp, unfixed_idx, Ainv_full @ b_full)
+    else:
+        Ainv_full = A_full.T
+        Z = np.eye(A_full.shape[1])
+    xp = put(xp, unfixed_idx, Ainv_full @ b_full)
 
     def project(x):
         """Project a full state vector into the reduced optimization vector."""
         x_reduced = jnp.dot(Z.T, (x - xp)[unfixed_idx])
         return jnp.atleast_1d(jnp.squeeze(x_reduced))
 
     def recover(x_reduced):
         """Recover the full state vector from the reduced optimization vector."""
         dx = put(jnp.zeros(dim_x), unfixed_idx, Z @ x_reduced)
         return jnp.atleast_1d(jnp.squeeze(xp + dx))
 
     # check that all constraints are actually satisfiable
     xp_dict = {arg: xp[x_idx[arg]] for arg in x_idx.keys()}
     for con in constraints:
-        arg = con.args[0]
-        if arg not in objective_args:
-            continue
         res = con.compute_scaled(**xp_dict)
-        x = xp_dict[arg]
+        x = np.concatenate([xp_dict[arg] for arg in con.args])
         # stuff like density is O(1e19) so need some adjustable tolerance here.
-        atol = max(1e-8, np.finfo(x).eps * np.linalg.norm(x) / x.size)
-        if not np.allclose(res, 0, atol=atol):
-            raise ValueError(
-                f"Incompatible constraints detected, cannot satisfy constraint {con}"
-            )
+        atol = max(1e-8, np.finfo(x.dtype).eps * np.linalg.norm(x) / x.size)
+        np.testing.assert_allclose(
+            res,
+            0,
+            atol=atol,
+            err_msg="Incompatible constraints detected, cannot satisfy "
+            + f"constraint {con}",
+        )
 
-    return xp, A, Ainv, b, Z, unfixed_idx, project, recover
+    return xp, A_full, b_full, Z, unfixed_idx, project, recover
 
 
 def align_jacobian(Fx, objective_f, objective_g):
     """Pad Jacobian with zeros in the right places so that the arguments line up.
 
     Parameters
     ----------
```

### Comparing `desc-opt-0.8.1/desc/optimize/_constraint_wrappers.py` & `desc-opt-0.8.2/desc/optimize/_constraint_wrappers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 """Wrappers for doing STELLOPT/SIMSOPT like optimization."""
 
 import numpy as np
 
 from desc.backend import jnp
 from desc.compute import arg_order
 from desc.objectives import (
+    BoundaryRSelfConsistency,
+    BoundaryZSelfConsistency,
     CurrentDensity,
     ForceBalance,
     HelicalForceBalance,
     ObjectiveFunction,
     RadialForceBalance,
 )
 from desc.objectives.utils import (
     align_jacobian,
     factorize_linear_constraints,
     get_fixed_boundary_constraints,
+    maybe_add_self_consistency,
 )
-from desc.utils import Timer
+from desc.utils import Timer, get_instance
 
 from .utils import compute_jac_scale, f_where_x
 
 
 class LinearConstraintProjection(ObjectiveFunction):
     """Remove linear constraints via orthogonal projection.
 
     Given a problem of the form
 
     min_x f(x)  subject to A*x=b
 
     We can write any feasible x=xp + Z*x_reduced where xp is a particular solution to
     Ax=b (taken to be the least norm solution), Z is a representation for the null
-    space of A (A*Z=0) and x_reduced is conconstrained. This transforms the problem into
+    space of A (A*Z=0) and x_reduced is unconstrained. This transforms the problem into
 
     min_x_reduced f(x_reduced)
 
     Parameters
     ----------
     objective : ObjectiveFunction
         Objective function to optimize.
@@ -54,14 +57,15 @@
         for con in constraints:
             if not con.linear:
                 raise ValueError(
                     "LinearConstraintProjection method "
                     + "cannot handle nonlinear constraint {}.".format(con)
                 )
         self._objective = objective
+        self._objectives = [objective]
         self._constraints = constraints
         self._built = False
         # don't want to compile this, just use the compiled objective
         self._use_jit = False
         self._compiled = False
 
         if eq is not None:
@@ -80,37 +84,46 @@
         verbose : int, optional
             Level of output.
 
         """
         timer = Timer()
         timer.start("Linear constraint projection build")
 
+        # we don't always build here because in ~all cases the user doesn't interact
+        # with this directly, so if the user wants to manually rebuild they should
+        # do it before this wrapper is created for them.
         if not self._objective.built:
             self._objective.build(eq, verbose=verbose)
         for con in self._constraints:
             if not con.built:
                 con.build(eq, verbose=verbose)
-        self._args = self._objective.args
+
+        args = np.concatenate([obj.args for obj in self._constraints])
+        args = np.concatenate((args, self._objective.args))
+        # this is all args used by both constraints and objective
+        self._args = [arg for arg in arg_order if arg in args]
         self._dim_f = self._objective.dim_f
         self._scalar = self._objective.scalar
+        self._dimensions = self._objective.dimensions
+        self._objective.set_args(*self._args)
+        self.set_args()
         (
             self._xp,
             self._A,
-            self._Ainv,
             self._b,
             self._Z,
             self._unfixed_idx,
             self._project,
             self._recover,
         ) = factorize_linear_constraints(
             self._constraints,
-            self._objective.args,
+            self._args,
         )
+        self._dim_x_full = self._dim_x
         self._dim_x = self._Z.shape[1]
-        self._dim_x_full = self._objective.dim_x
 
         self._built = True
         timer.stop("Linear constraint projection build")
         if verbose > 1:
             timer.disp("Linear constraint projection build")
 
     def compile(self, mode="lsq", verbose=1):
@@ -134,15 +147,17 @@
 
     def recover(self, x_reduced):
         """Recover the full state vector from the reduced optimization vector."""
         return self._recover(x_reduced)
 
     def x(self, eq):
         """Return the reduced state vector from the Equilibrium eq."""
-        x = self._objective.x(eq)
+        x = np.zeros((self._dim_x_full,))
+        for arg in self.args:
+            x[self.x_idx[arg]] = getattr(eq, arg)
         return self.project(x)
 
     def unpack_state(self, x):
         """Unpack the state vector into its components.
 
         Parameters
         ----------
@@ -151,16 +166,20 @@
 
         Returns
         -------
         kwargs : dict
             Dictionary of the state components with argument names as keys.
 
         """
-        if len(x) == self._dim_x:
-            x = self.recover(x)
+        if x.size != self.dim_x:
+            raise ValueError(
+                "Input vector dimension is invalid, expected "
+                + f"{self.dim_x} got {x.size}."
+            )
+        x = self.recover(x)
         return self._objective.unpack_state(x)
 
     def compute(self, x_reduced):
         """Compute the objective function.
 
         Parameters
         ----------
@@ -300,91 +319,58 @@
             ):
                 raise ValueError(
                     "ProximalProjection method "
                     + "cannot handle general nonlinear constraint {}.".format(con)
                 )
         self._objective = objective
         self._constraint = constraint
+        self._objectives = [objective, constraint]
         perturb_options.setdefault("verbose", 0)
         perturb_options.setdefault("include_f", False)
         solve_options.setdefault("verbose", 0)
         self._perturb_options = perturb_options
         self._solve_options = solve_options
         self._built = False
         # don't want to compile this, just use the compiled objective and constraint
         self._use_jit = False
         self._compiled = False
 
         if eq is not None:
             self.build(eq, verbose=verbose)
 
-    def build(self, eq, use_jit=None, verbose=1):  # noqa: C901
-        """Build the objective.
-
-        Parameters
-        ----------
-        eq : Equilibrium, optional
-            Equilibrium that will be optimized to satisfy the Objective.
-        use_jit : bool, optional
-            Whether to just-in-time compile the objective and derivatives.
-            Note: unused by this class, should pass to sub-objectives directly.
-        verbose : int, optional
-            Level of output.
+    def set_args(self, *args):
+        """Set which arguments the objective should expect.
 
+        Defaults to args from all sub-objectives. Additional arguments can be passed in.
         """
-        timer = Timer()
-        timer.start("Proximal projection build")
-
-        self._eq = eq.copy()
-        self._linear_constraints = get_fixed_boundary_constraints(
-            iota=not isinstance(self._constraint.objectives[0], CurrentDensity)
-            and self._eq.iota is not None,
-            kinetic=eq.electron_temperature is not None,
-        )
-
-        if not self._objective.built:
-            self._objective.build(self._eq, verbose=verbose)
-        if not self._constraint.built:
-            self._constraint.build(self._eq, verbose=verbose)
-        # remove constraints that aren't necessary
-        self._linear_constraints = tuple(
-            [
-                con
-                for con in self._linear_constraints
-                if con.args[0] in self._constraint.args
-            ]
-        )
-        for constraint in self._linear_constraints:
-            constraint.build(self._eq, verbose=verbose)
-        self._objectives = self._objective.objectives
-
-        self._dim_f = self._objective.dim_f
-        if self._dim_f == 1:
-            self._scalar = True
-        else:
-            self._scalar = False
-
         # this is everything taken by either objective
-        self._full_args = self._constraint.args + self._objective.args
+        self._full_args = (
+            self._constraint.args
+            + self._objective.args
+            + list(np.concatenate([obj.args for obj in self._linear_constraints]))
+        )
         self._full_args = [arg for arg in arg_order if arg in self._full_args]
 
         # arguments being optimized are all args, but with internal degrees of freedom
         # replaced by boundary terms
-        self._args = self._full_args.copy()
+        self._args = self._full_args.copy() + list(args)
+        self._args = [arg for arg in arg_order if arg in self._args]
         if "L_lmn" in self._args:
             self._args.remove("L_lmn")
         if "R_lmn" in self._args:
             self._args.remove("R_lmn")
             if "Rb_lmn" not in self._args:
                 self._args.append("Rb_lmn")
         if "Z_lmn" in self._args:
             self._args.remove("Z_lmn")
             if "Zb_lmn" not in self._args:
                 self._args.append("Zb_lmn")
+        self._set_state_vector()
 
+    def _set_state_vector(self):
         self._dimensions = self._objective.dimensions
         self._dim_x = 0
         self._x_idx = {}
         for arg in self.args:
             self.x_idx[arg] = np.arange(self._dim_x, self._dim_x + self.dimensions[arg])
             self._dim_x += self.dimensions[arg]
         self._dim_x_full = 0
@@ -394,15 +380,14 @@
                 self._dim_x_full, self._dim_x_full + self.dimensions[arg]
             )
             self._dim_x_full += self.dimensions[arg]
 
         (
             xp,
             A,
-            self._Ainv,
             b,
             self._Z,
             self._unfixed_idx,
             project,
             recover,
         ) = factorize_linear_constraints(self._linear_constraints, self._full_args)
 
@@ -413,26 +398,77 @@
                 for arg in self._args
                 if arg not in ["Rb_lmn", "Zb_lmn"]
             ]
         )
         x_idx.sort(kind="mergesort")
         self._dxdc = np.eye(self._dim_x_full)[:, x_idx]
         if "Rb_lmn" in self._args:
-            dxdRb = (
-                np.eye(self._dim_x_full)[:, self._x_idx_full["R_lmn"]]
-                @ self._Ainv["R_lmn"]
+            c = get_instance(self._linear_constraints, BoundaryRSelfConsistency)
+            A = c.derivatives["jac"]["R_lmn"](
+                *[jnp.zeros(c.dimensions[arg]) for arg in c.args]
             )
+            A = (c.normalization * (A.T / c.weight)).T
+            Ainv = np.linalg.pinv(A)
+            dxdRb = np.eye(self._dim_x_full)[:, self._x_idx_full["R_lmn"]] @ Ainv
             self._dxdc = np.hstack((self._dxdc, dxdRb))
         if "Zb_lmn" in self._args:
-            dxdZb = (
-                np.eye(self._dim_x_full)[:, self._x_idx_full["Z_lmn"]]
-                @ self._Ainv["Z_lmn"]
+            c = get_instance(self._linear_constraints, BoundaryZSelfConsistency)
+            A = c.derivatives["jac"]["Z_lmn"](
+                *[jnp.zeros(c.dimensions[arg]) for arg in c.args]
             )
+            A = (c.normalization * (A.T / c.weight)).T
+            Ainv = np.linalg.pinv(A)
+            dxdZb = np.eye(self._dim_x_full)[:, self._x_idx_full["Z_lmn"]] @ Ainv
             self._dxdc = np.hstack((self._dxdc, dxdZb))
 
+    def build(self, eq, use_jit=None, verbose=1):  # noqa: C901
+        """Build the objective.
+
+        Parameters
+        ----------
+        eq : Equilibrium, optional
+            Equilibrium that will be optimized to satisfy the Objective.
+        use_jit : bool, optional
+            Whether to just-in-time compile the objective and derivatives.
+            Note: unused by this class, should pass to sub-objectives directly.
+        verbose : int, optional
+            Level of output.
+
+        """
+        timer = Timer()
+        timer.start("Proximal projection build")
+
+        self._eq = eq.copy()
+        self._linear_constraints = get_fixed_boundary_constraints(
+            iota=not isinstance(self._constraint.objectives[0], CurrentDensity)
+            and self._eq.iota is not None,
+            kinetic=eq.electron_temperature is not None,
+        )
+        self._linear_constraints = maybe_add_self_consistency(self._linear_constraints)
+
+        # we don't always build here because in ~all cases the user doesn't interact
+        # with this directly, so if the user wants to manually rebuild they should
+        # do it before this wrapper is created for them.
+        if not self._objective.built:
+            self._objective.build(self._eq, verbose=verbose)
+        if not self._constraint.built:
+            self._constraint.build(self._eq, verbose=verbose)
+
+        for constraint in self._linear_constraints:
+            constraint.build(self._eq, verbose=verbose)
+
+        self._dim_f = self._objective.dim_f
+        if self._dim_f == 1:
+            self._scalar = True
+        else:
+            self._scalar = False
+
+        self.set_args()
+        self._objective.set_args(*self._full_args)
+        self._constraint.set_args(*self._full_args)
         # history and caching
         self._x_old = np.zeros((self._dim_x,))
         for arg in self.args:
             self._x_old[self.x_idx[arg]] = getattr(eq, arg)
 
         self._allx = [self._x_old]
         self._allxopt = [self._objective.x(eq)]
@@ -487,20 +523,20 @@
             x_dict = self.unpack_state(x)
             x_dict_old = self.unpack_state(self._x_old)
             deltas = {str(key): x_dict[key] - x_dict_old[key] for key in x_dict}
             self._eq = self._eq.perturb(
                 objective=self._constraint,
                 constraints=self._linear_constraints,
                 deltas=deltas,
-                **self._perturb_options
+                **self._perturb_options,
             )
             self._eq.solve(
                 objective=self._constraint,
                 constraints=self._linear_constraints,
-                **self._solve_options
+                **self._solve_options,
             )
             xopt = self._objective.x(self._eq)
             xeq = self._constraint.x(self._eq)
             self._allx.append(x)
             self._allxopt.append(xopt)
             self._allxeq.append(xeq)
```

### Comparing `desc-opt-0.8.1/desc/optimize/_desc_wrappers.py` & `desc-opt-0.8.2/desc/optimize/_desc_wrappers.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/optimize/_scipy_wrappers.py` & `desc-opt-0.8.2/desc/optimize/_scipy_wrappers.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,17 +73,19 @@
        Important attributes are: ``x`` the solution array, ``success`` a
        Boolean flag indicating if the optimizer exited successfully and
        ``message`` which describes the cause of the termination. See
        `OptimizeResult` for a description of other attributes.
 
     """
     assert constraint is None, f"method {method} doesn't support constraints"
+    x_scale = 1 if x_scale == "auto" else x_scale
     options = {} if options is None else options
     options.setdefault("maxiter", np.iinfo(np.int32).max)
-    x_scale = 1 if x_scale == "auto" else x_scale
+    if method in ["scipy-trust-exact", "scipy-trust-ncg"]:
+        options.setdefault("initial_trust_radius", 1e-2 * np.linalg.norm(x0))
     if isinstance(x_scale, str):
         raise ValueError(f"Method {method} does not support x_scale type {x_scale}")
     fun, grad, hess = objective.compute_scalar, objective.grad, objective.hess
 
     # need to use some "global" variables here
     allx = []
     func_allx = []
@@ -120,31 +122,31 @@
         hess_allx.append(x)
         H = hess(x)
         hess_allf.append(H)
         return H / (np.atleast_2d(x_scale).T * np.atleast_2d(x_scale))
 
     def callback(x1):
         allx.append(x1)
-        f1 = f_where_x(x1, func_allx, func_allf)
-        g1 = f_where_x(x1, grad_allx, grad_allf)
+        f1 = f_where_x(x1, func_allx, func_allf, dim=0)
+        g1 = f_where_x(x1, grad_allx, grad_allf, dim=1)
         g_norm = np.linalg.norm(g1, ord=np.inf)
         x_norm = np.linalg.norm(x1)
 
         if len(allx) < 2:
             df = np.inf
             dx_norm = np.inf
             reduction_ratio = 0
         else:
             x2 = allx[-2]
-            f2 = f_where_x(x2, func_allx, func_allf)
+            f2 = f_where_x(x2, func_allx, func_allf, dim=0)
             df = f2 - f1
             dx = x1 - x2
             dx_norm = jnp.linalg.norm(dx)
             if len(hess_allx):
-                H1 = f_where_x(x1, hess_allx, hess_allf)
+                H1 = f_where_x(x1, hess_allx, hess_allf, dim=2)
             else:
                 H1 = np.eye(x1.size) / dx_norm
             if not H1.size:
                 H1 = np.eye(x1.size) / dx_norm
             predicted_reduction = -evaluate_quadratic_form_hess(dx, 0, g1, H1)
             if predicted_reduction > 0:
                 reduction_ratio = df / predicted_reduction
@@ -199,18 +201,18 @@
         result["allx"] = allx
         result["nfev"] = len(func_allx)
         result["ngev"] = len(grad_allx)
         result["nhev"] = len(hess_allx)
         result["nit"] = len(allx)
     except StopIteration:
         x = grad_allx[-1]
-        f = f_where_x(x, func_allx, func_allf)
-        g = f_where_x(x, grad_allx, grad_allf)
+        f = f_where_x(x, func_allx, func_allf, dim=0)
+        g = f_where_x(x, grad_allx, grad_allf, dim=1)
         if len(hess_allx):
-            H = f_where_x(x, hess_allx, hess_allf)
+            H = f_where_x(x, hess_allx, hess_allf, dim=2)
         else:
             H = None
         result = OptimizeResult(
             x=x,
             success=success[0],
             fun=f,
             grad=g,
@@ -301,45 +303,46 @@
     jac_allf = []
     message = [""]
     success = [None]
 
     def fun_wrapped(x):
         # record all the xs and fs we see
         fun_allx.append(x)
-        f = fun(x)
+        f = jnp.atleast_1d(fun(x))
         fun_allf.append(f)
         return f
 
     def jac_wrapped(x):
         # record all the xs and jacs we see
         jac_allx.append(x)
         J = jac(x)
         jac_allf.append(J)
         callback(x)
         return J
 
     def callback(x1):
-        f1 = f_where_x(x1, fun_allx, fun_allf)
+        f1 = f_where_x(x1, fun_allx, fun_allf, dim=1)
         c1 = 1 / 2 * np.dot(f1, f1)
-        J1 = f_where_x(x1, jac_allx, jac_allf)
+        J1 = f_where_x(x1, jac_allx, jac_allf, dim=2)
         g1 = J1.T @ f1
+
         g_norm = np.linalg.norm(g1, ord=np.inf)
         x_norm = np.linalg.norm(x1)
 
         if len(jac_allx) < 2:
             df = np.inf
             dx_norm = np.inf
             reduction_ratio = 0
         else:
             x2 = jac_allx[-2]
-            f2 = f_where_x(x2, fun_allx, fun_allf)
+            f2 = f_where_x(x2, fun_allx, fun_allf, dim=1)
             c2 = 1 / 2 * np.dot(f2, f2)
             df = c2 - c1
-            dx = x1 - x2
-            dx_norm = jnp.linalg.norm(dx)
+            dx = np.atleast_1d(x1 - x2)
+            dx_norm = np.linalg.norm(dx)
 
             predicted_reduction = -evaluate_quadratic_form_jac(J1, g1, dx)
             if predicted_reduction > 0:
                 reduction_ratio = df / predicted_reduction
             elif predicted_reduction == df == 0:
                 reduction_ratio = 1
             else:
@@ -394,18 +397,18 @@
         )
         result["allx"] = jac_allx
         result["nfev"] = len(fun_allx)
         result["njev"] = len(jac_allx)
         result["nit"] = len(jac_allx)
     except StopIteration:
         x = jac_allx[-1]
-        f = f_where_x(x, fun_allx, fun_allf)
+        f = f_where_x(x, fun_allx, fun_allf, dim=1)
         c = 1 / 2 * np.dot(f, f)
-        J = f_where_x(x, jac_allx, jac_allf)
-        g = J.T @ f
+        J = f_where_x(x, jac_allx, jac_allf, dim=2)
+        g = np.atleast_1d(J.T @ f)
         result = OptimizeResult(
             x=x,
             success=success[0],
             cost=c,
             fun=f,
             grad=g,
             jac=J,
```

### Comparing `desc-opt-0.8.1/desc/optimize/fmin_scalar.py` & `desc-opt-0.8.2/desc/optimize/fmin_scalar.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/optimize/least_squares.py` & `desc-opt-0.8.2/desc/optimize/least_squares.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/optimize/optimizer.py` & `desc-opt-0.8.2/desc/optimize/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import warnings
 
 import numpy as np
 from termcolor import colored
 
 from desc.io import IOAble
 from desc.objectives import FixCurrent, FixIota, ObjectiveFunction
+from desc.objectives.utils import maybe_add_self_consistency
 from desc.utils import Timer
 
 from ._constraint_wrappers import LinearConstraintProjection, ProximalProjection
 
 
 class Optimizer(IOAble):
     """A helper class to wrap several optimization routines.
@@ -71,15 +72,15 @@
         constraints=(),
         ftol=None,
         xtol=None,
         gtol=None,
         x_scale="auto",
         verbose=1,
         maxiter=None,
-        options={},
+        options=None,
     ):
         """Optimize an objective function.
 
         Parameters
         ----------
         eq : Equilibrium
             Initial equilibrium.
@@ -128,27 +129,36 @@
             Boolean flag indicating if the optimizer exited successfully and
             ``message`` which describes the cause of the termination. See
             `OptimizeResult` for a description of other attributes.
 
         """
         # TODO: document options
         timer = Timer()
+        options = {} if options is None else options
         wrapper, method = _parse_method(self.method)
 
         linear_constraints, nonlinear_constraint = _parse_constraints(constraints)
         objective, nonlinear_constraint = _maybe_wrap_nonlinear_constraints(
             objective, nonlinear_constraint, self.method, options
         )
+
+        if not isinstance(objective, ProximalProjection):
+            # need to include self consistency constraints
+            linear_constraints = maybe_add_self_consistency(linear_constraints)
         if len(linear_constraints):
             objective = LinearConstraintProjection(objective, linear_constraints)
         if not objective.built:
             objective.build(eq, verbose=verbose)
         if not objective.compiled:
             mode = "scalar" if optimizers[method]["scalar"] else "lsq"
-            objective.compile(mode, verbose)
+            try:
+                objective.compile(mode, verbose)
+            except ValueError:
+                objective.build(eq, verbose=verbose)
+                objective.compile(mode, verbose=verbose)
 
         if objective.scalar and (not optimizers[method]["scalar"]):
             warnings.warn(
                 colored(
                     "method {} is not intended for scalar objective function".format(
                         ".".join([method])
                     ),
```

### Comparing `desc-opt-0.8.1/desc/optimize/stochastic.py` & `desc-opt-0.8.2/desc/optimize/stochastic.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/optimize/tr_subproblems.py` & `desc-opt-0.8.2/desc/optimize/tr_subproblems.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/optimize/utils.py` & `desc-opt-0.8.2/desc/optimize/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,33 +337,40 @@
     scale_inv = jnp.where(scale_inv == 0, 1, scale_inv)
 
     if prev_scale_inv is not None:
         scale_inv = jnp.maximum(scale_inv, prev_scale_inv)
     return 1 / scale_inv, scale_inv
 
 
-def f_where_x(x, xs, fs):
+def f_where_x(x, xs, fs, dim=0):
     """Return fs where x==xs.
 
     Parameters
     ----------
     x : ndarray, shape(k,)
         array to find
     xs : list of ndarray of shape(k,)
         list to compare x against
     fs : list of float, ndarray
         list of values to return value from
+    dim : int
+        number of dimensions the output should have
 
     Returns
     -------
     f : float or ndarray
         value of fs[i] where x==xs[i]
     """
     x, xs, fs = map(np.asarray, (x, xs, fs))
     assert len(xs) == len(fs)
     assert len(xs) == 0 or x.shape == xs[0].shape
     eps = np.finfo(x.dtype).eps
     i = np.where(np.all(np.isclose(x, xs, rtol=eps, atol=eps), axis=1))[0]
     # sometimes two things are within eps of x, we want the most recent one
     if len(i) > 1:
         i = i[-1]
-    return fs[i].squeeze()
+    f = fs[i].squeeze()
+    if dim == 1:
+        f = np.atleast_1d(f)
+    if dim == 2:
+        f = np.atleast_2d(f.T).T
+    return f
```

### Comparing `desc-opt-0.8.1/desc/perturbations.py` & `desc-opt-0.8.2/desc/perturbations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 """Functions for perturbing equilibria."""
 
 import warnings
 
-import numpy as np
 from termcolor import colored
 
-from desc.backend import put, use_jax
+from desc.backend import jnp, put, use_jax
 from desc.compute import arg_order, profile_names
-from desc.objectives import get_fixed_boundary_constraints
-from desc.objectives.utils import align_jacobian, factorize_linear_constraints
+from desc.objectives import (
+    BoundaryRSelfConsistency,
+    BoundaryZSelfConsistency,
+    get_fixed_boundary_constraints,
+)
+from desc.objectives.utils import (
+    align_jacobian,
+    factorize_linear_constraints,
+    maybe_add_self_consistency,
+)
 from desc.optimize.tr_subproblems import trust_region_step_exact_svd
 from desc.optimize.utils import compute_jac_scale, evaluate_quadratic_form_jac
-from desc.utils import Timer
+from desc.utils import Timer, get_instance
 
 __all__ = ["get_deltas", "perturb", "optimal_perturb"]
 
 
 def get_deltas(things1, things2):
     """Compute differences between parameters for perturbations.
 
@@ -39,35 +46,35 @@
     if "surface" in things1:
         s1 = things1.pop("surface")
         s2 = things2.pop("surface")
         if s1 is not None and s2 is not None:
             s1 = s1.copy()
             s2 = s2.copy()
             s1.change_resolution(s2.L, s2.M, s2.N)
-            if not np.allclose(s2.R_lmn, s1.R_lmn):
+            if not jnp.allclose(s2.R_lmn, s1.R_lmn):
                 deltas["Rb_lmn"] = s2.R_lmn - s1.R_lmn
-            if not np.allclose(s2.Z_lmn, s1.Z_lmn):
+            if not jnp.allclose(s2.Z_lmn, s1.Z_lmn):
                 deltas["Zb_lmn"] = s2.Z_lmn - s1.Z_lmn
 
     for key, val in profile_names.items():
         if key in things1:
             t1 = things1.pop(key)
             t2 = things2.pop(key)
             if t1 is not None and t2 is not None:
                 t1 = t1.copy()
                 t2 = t2.copy()
                 if hasattr(t1, "change_resolution") and hasattr(t2, "basis"):
                     t1.change_resolution(t2.basis.L)
-                if not np.allclose(t2.params, t1.params):
+                if not jnp.allclose(t2.params, t1.params):
                     deltas[val] = t2.params - t1.params
 
     if "Psi" in things1:
         psi1 = things1.pop("Psi")
         psi2 = things2.pop("Psi")
-        if psi1 is not None and not np.allclose(psi2, psi1):
+        if psi1 is not None and not jnp.allclose(psi2, psi1):
             deltas["Psi"] = psi2 - psi1
 
     assert len(things1) == 0, "get_deltas got an unexpected key: {}".format(
         things1.keys()
     )
     return deltas
 
@@ -126,35 +133,39 @@
         warnings.warn(
             colored(
                 "Computing perturbations with finite differences can be "
                 + "highly inaccurate. Consider using JAX for exact derivatives.",
                 "yellow",
             )
         )
-    if np.isscalar(tr_ratio):
-        tr_ratio = tr_ratio * np.ones(order)
+    if jnp.isscalar(tr_ratio):
+        tr_ratio = tr_ratio * jnp.ones(order)
     elif len(tr_ratio) < order:
         raise ValueError(
             "Got only {} tr_ratios for order {} perturbations.".format(
                 len(tr_ratio), order
             )
         )
     # remove deltas that are zero
-    deltas = {key: val for key, val in deltas.items() if np.any(val)}
+    deltas = {key: val for key, val in deltas.items() if jnp.any(val)}
 
-    # make sure things are at least 1D for np.concatenate later
+    # make sure things are at least 1D for jnp.concatenate later
     # in case only a single delta is being passed
     for key in deltas.keys():
-        deltas[key] = np.atleast_1d(deltas[key])
+        deltas[key] = jnp.atleast_1d(deltas[key])
 
     if not objective.built:
         objective.build(eq, verbose=verbose)
-    for constraint in constraints:
-        if not constraint.built:
-            constraint.build(eq, verbose=verbose)
+    constraints = maybe_add_self_consistency(constraints)
+    con_args = []
+    for con in constraints:
+        con_args += con.args
+        if not con.built:
+            con.build(eq, verbose=verbose)
+    objective.set_args(*con_args)
 
     if objective.scalar:  # FIXME: change to num objectives >= num parameters
         raise AttributeError(
             "Cannot perturb with a scalar objective: {}.".format(objective)
         )
 
     if verbose > 0:
@@ -162,91 +173,105 @@
 
     timer = Timer()
     timer.start("Total perturbation")
 
     if verbose > 0:
         print("Factorizing linear constraints")
     timer.start("linear constraint factorize")
-    xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+    xp, _, _, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints, objective.args
     )
     timer.stop("linear constraint factorize")
     if verbose > 1:
         timer.disp("linear constraint factorize")
 
     # state vector
     x = objective.x(eq)
     x_reduced = project(x)
-    x_norm = np.linalg.norm(x_reduced)
+    x_norm = jnp.linalg.norm(x_reduced)
 
     # perturbation vectors
-    dx1_reduced = np.zeros_like(x_reduced)
-    dx2_reduced = np.zeros_like(x_reduced)
-    dx3_reduced = np.zeros_like(x_reduced)
+    dx1_reduced = jnp.zeros_like(x_reduced)
+    dx2_reduced = jnp.zeros_like(x_reduced)
+    dx3_reduced = jnp.zeros_like(x_reduced)
 
     # tangent vectors
-    tangents = np.zeros((objective.dim_x,))
+    tangents = jnp.zeros((objective.dim_x,))
     if "Rb_lmn" in deltas.keys():
-        dc = deltas["Rb_lmn"]
-        tangents += (
-            np.eye(objective.dim_x)[:, objective.x_idx["R_lmn"]] @ Ainv["R_lmn"] @ dc
+        con = get_instance(constraints, BoundaryRSelfConsistency)
+        A = con.derivatives["jac"]["R_lmn"](
+            *[jnp.zeros(con.dimensions[arg]) for arg in con.args]
         )
+        A = (con.normalization * (A.T / con.weight)).T
+        Ainv = jnp.linalg.pinv(A)
+        dc = deltas["Rb_lmn"]
+        tangents += jnp.eye(objective.dim_x)[:, objective.x_idx["R_lmn"]] @ Ainv @ dc
     if "Zb_lmn" in deltas.keys():
-        dc = deltas["Zb_lmn"]
-        tangents += (
-            np.eye(objective.dim_x)[:, objective.x_idx["Z_lmn"]] @ Ainv["Z_lmn"] @ dc
+        con = get_instance(constraints, BoundaryZSelfConsistency)
+        A = con.derivatives["jac"]["Z_lmn"](
+            *[jnp.zeros(con.dimensions[arg]) for arg in con.args]
         )
+        A = (con.normalization * (A.T / con.weight)).T
+        Ainv = jnp.linalg.pinv(A)
+        dc = deltas["Zb_lmn"]
+        tangents += jnp.eye(objective.dim_x)[:, objective.x_idx["Z_lmn"]] @ Ainv @ dc
     # all other perturbations besides the boundary
     other_args = [arg for arg in arg_order if arg not in ["Rb_lmn", "Zb_lmn"]]
     if len([arg for arg in other_args if arg in deltas.keys()]):
-        dc = np.concatenate(
+        dc = jnp.concatenate(
             [
                 deltas[arg]
                 for arg in other_args
                 if arg in deltas.keys() and arg in objective.args
             ]
         )
-        x_idx = np.concatenate(
+        x_idx = jnp.concatenate(
             [
                 objective.x_idx[arg]
                 for arg in other_args
                 if arg in deltas.keys() and arg in objective.args
             ]
         )
-        x_idx.sort(kind="mergesort")
-        tangents += np.eye(objective.dim_x)[:, x_idx] @ dc
+        x_idx = jnp.sort(x_idx)
+        tangents += jnp.eye(objective.dim_x)[:, x_idx] @ dc
 
     # 1st order
     if order > 0:
 
         if (weight is None) or (weight == "auto"):
-            w = np.ones((objective.dim_x,))
+            w = jnp.ones((objective.dim_x,))
             if weight == "auto" and (("p_l" in deltas) or ("i_l" in deltas)):
-                w[objective.x_idx["R_lmn"]] = (
-                    abs(eq.R_basis.modes[:, :2]).sum(axis=1) + 1
+                w = put(
+                    w,
+                    objective.x_idx["R_lmn"],
+                    (abs(eq.R_basis.modes[:, :2]).sum(axis=1) + 1),
                 )
-                w[objective.x_idx["Z_lmn"]] = (
-                    abs(eq.Z_basis.modes[:, :2]).sum(axis=1) + 1
+                w = put(
+                    w,
+                    objective.x_idx["Z_lmn"],
+                    (abs(eq.Z_basis.modes[:, :2]).sum(axis=1) + 1),
                 )
-                w[objective.x_idx["L_lmn"]] = (
-                    abs(eq.L_basis.modes[:, :2]).sum(axis=1) + 1
+                w = put(
+                    w,
+                    objective.x_idx["L_lmn"],
+                    (abs(eq.L_basis.modes[:, :2]).sum(axis=1) + 1),
                 )
             weight = w
-        weight = np.atleast_1d(weight)
+        weight = jnp.atleast_1d(weight)
         assert (
             len(weight) == objective.dim_x
         ), "Size of weight supplied to perturbation does not match objective.dim_x."
         if weight.ndim == 1:
             weight = weight[unfixed_idx]
-            weight = np.diag(weight)
+            weight = jnp.diag(weight)
         else:
             weight = weight[unfixed_idx, unfixed_idx]
         W = Z.T @ weight @ Z
         scale_inv = W
-        scale = np.linalg.inv(scale_inv)
+        scale = jnp.linalg.inv(scale_inv)
 
         # 1st partial derivatives wrt both state vector (x) and input parameters (c)
         if verbose > 0:
             print("Computing df")
         timer.start("df computation")
         Jx = objective.jac(x)
         Jx_reduced = Jx[:, unfixed_idx] @ Z @ scale
@@ -257,25 +282,25 @@
         timer.stop("df computation")
         if verbose > 1:
             timer.disp("df computation")
 
         if verbose > 0:
             print("Factoring df")
         timer.start("df/dx factorization")
-        u, s, vt = np.linalg.svd(Jx_reduced, full_matrices=False)
+        u, s, vt = jnp.linalg.svd(Jx_reduced, full_matrices=False)
         timer.stop("df/dx factorization")
         if verbose > 1:
             timer.disp("df/dx factorization")
 
         dx1_h, hit, alpha = trust_region_step_exact_svd(
             RHS1,
             u,
             s,
             vt.T,
-            tr_ratio[0] * np.linalg.norm(scale_inv @ x_reduced),
+            tr_ratio[0] * jnp.linalg.norm(scale_inv @ x_reduced),
             initial_alpha=None,
             rtol=0.01,
             max_iter=10,
         )
         dx1_reduced = scale @ dx1_h
         dx1 = recover(dx1_reduced) - xp
 
@@ -293,15 +318,15 @@
             timer.disp("d^2f computation")
 
         dx2_h, hit, alpha = trust_region_step_exact_svd(
             RHS2,
             u,
             s,
             vt.T,
-            tr_ratio[1] * np.linalg.norm(dx1_h),
+            tr_ratio[1] * jnp.linalg.norm(dx1_h),
             initial_alpha=alpha / tr_ratio[1],
             rtol=0.01,
             max_iter=10,
         )
         dx2_reduced = scale @ dx2_h
         dx2 = recover(dx2_reduced) - xp
 
@@ -319,15 +344,15 @@
             timer.disp("d^3f computation")
 
         dx3_h, hit, alpha = trust_region_step_exact_svd(
             RHS3,
             u,
             s,
             vt.T,
-            tr_ratio[2] * np.linalg.norm(dx2_h),
+            tr_ratio[2] * jnp.linalg.norm(dx2_h),
             initial_alpha=alpha / tr_ratio[2],
             rtol=0.01,
             max_iter=10,
         )
         dx3_reduced = scale @ dx3_h
 
     if order > 3:
@@ -341,34 +366,34 @@
         eq_new = eq
 
     # update perturbation attributes
     for key, value in deltas.items():
         setattr(eq_new, key, getattr(eq_new, key) + value)
     for constraint in constraints:
         constraint.update_target(eq_new)
-    xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+    xp, _, _, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints, objective.args
     )
 
     # update other attributes
     dx_reduced = dx1_reduced + dx2_reduced + dx3_reduced
     x_new = recover(x_reduced + dx_reduced)
     args = objective.unpack_state(x_new)
     for key, value in args.items():
         if key not in deltas:
             value = put(  # parameter values below threshold are set to 0
-                value, np.where(np.abs(value) < 10 * np.finfo(value.dtype).eps)[0], 0
+                value, jnp.where(jnp.abs(value) < 10 * jnp.finfo(value.dtype).eps)[0], 0
             )
             # don't set nonexistent profile (values are empty ndarrays)
             if value.size:
                 setattr(eq_new, key, value)
 
     timer.stop("Total perturbation")
     if verbose > 0:
-        print("||dx||/||x|| = {:10.3e}".format(np.linalg.norm(dx_reduced) / x_norm))
+        print("||dx||/||x|| = {:10.3e}".format(jnp.linalg.norm(dx_reduced) / x_norm))
     if verbose > 1:
         timer.disp("Total perturbation")
 
     return eq_new
 
 
 def optimal_perturb(  # noqa: C901 - FIXME: break this up into simpler pieces
@@ -433,16 +458,16 @@
         warnings.warn(
             colored(
                 "Computing perturbations with finite differences can be "
                 + "highly inaccurate. Consider using JAX for exact derivatives.",
                 "yellow",
             )
         )
-    if np.isscalar(tr_ratio):
-        tr_ratio = tr_ratio * np.ones(order)
+    if jnp.isscalar(tr_ratio):
+        tr_ratio = tr_ratio * jnp.ones(order)
     elif len(tr_ratio) < order:
         raise ValueError(
             "Got only {} tr_ratios for order {} perturbations.".format(
                 len(tr_ratio), order
             )
         )
 
@@ -450,92 +475,98 @@
         objective_f.build(eq, verbose=verbose)
     if not objective_g.built:
         objective_g.build(eq, verbose=verbose)
 
     deltas = {}
     if type(dR) is bool or dR is None:
         if dR is True:
-            deltas["R_lmn"] = np.ones((objective_f.dimensions["R_lmn"],), dtype=bool)
-    elif np.any(dR):
+            deltas["R_lmn"] = jnp.ones((objective_f.dimensions["R_lmn"],), dtype=bool)
+    elif jnp.any(dR):
         deltas["R_lmn"] = dR
     if type(dZ) is bool or dZ is None:
         if dZ is True:
-            deltas["Z_lmn"] = np.ones((objective_f.dimensions["Z_lmn"],), dtype=bool)
-    elif np.any(dZ):
+            deltas["Z_lmn"] = jnp.ones((objective_f.dimensions["Z_lmn"],), dtype=bool)
+    elif jnp.any(dZ):
         deltas["Z_lmn"] = dZ
     if type(dL) is bool or dL is None:
         if dL is True:
-            deltas["L_lmn"] = np.ones((objective_f.dimensions["L_lmn"],), dtype=bool)
-    elif np.any(dL):
+            deltas["L_lmn"] = jnp.ones((objective_f.dimensions["L_lmn"],), dtype=bool)
+    elif jnp.any(dL):
         deltas["L_lmn"] = dL
     if type(dp) is bool or dp is None:
         if dp is True:
-            deltas["p_l"] = np.ones((objective_f.dimensions["p_l"],), dtype=bool)
-    elif np.any(dp):
+            deltas["p_l"] = jnp.ones((objective_f.dimensions["p_l"],), dtype=bool)
+    elif jnp.any(dp):
         deltas["p_l"] = dp
     if type(di) is bool or di is None:
         if di is True:
-            deltas["i_l"] = np.ones((objective_f.dimensions["i_l"],), dtype=bool)
-    elif np.any(di):
+            deltas["i_l"] = jnp.ones((objective_f.dimensions["i_l"],), dtype=bool)
+    elif jnp.any(di):
         deltas["i_l"] = di
     if type(dPsi) is bool or dPsi is None:
         if dPsi is True:
-            deltas["Psi"] = np.ones((objective_f.dimensions["Psi"],), dtype=bool)
+            deltas["Psi"] = jnp.ones((objective_f.dimensions["Psi"],), dtype=bool)
     if type(dRb) is bool or dRb is None:
         if dRb is True:
-            deltas["Rb_lmn"] = np.ones((objective_f.dimensions["Rb_lmn"],), dtype=bool)
-    elif np.any(dRb):
+            deltas["Rb_lmn"] = jnp.ones((objective_f.dimensions["Rb_lmn"],), dtype=bool)
+    elif jnp.any(dRb):
         deltas["Rb_lmn"] = dRb
     if type(dZb) is bool or dZb is None:
         if dZb is True:
-            deltas["Zb_lmn"] = np.ones((objective_f.dimensions["Zb_lmn"],), dtype=bool)
-    elif np.any(dZb):
+            deltas["Zb_lmn"] = jnp.ones((objective_f.dimensions["Zb_lmn"],), dtype=bool)
+    elif jnp.any(dZb):
         deltas["Zb_lmn"] = dZb
 
     if not len(deltas):
         raise ValueError("At least one input must be a free variable for optimization.")
 
     if verbose > 0:
         print("Perturbing {}".format(", ".join(deltas.keys())))
 
     timer = Timer()
     timer.start("Total perturbation")
 
     # parameter vector
-    c = np.array([])
-    c_idx = np.array([], dtype=bool)
+    c = jnp.array([])
+    c_idx = jnp.array([], dtype=bool)
     for key, value in deltas.items():
-        c_idx = np.append(c_idx, np.where(value)[0] + c.size)
-        c = np.concatenate((c, getattr(eq, key)))
+        c_idx = jnp.append(c_idx, jnp.where(value)[0] + c.size)
+        c = jnp.concatenate((c, getattr(eq, key)))
 
     # optimization subspace matrix
     if subspace is None:
-        subspace = np.eye(c.size)[:, c_idx]
+        subspace = jnp.eye(c.size)[:, c_idx]
     dim_c, dim_opt = subspace.shape
 
     if dim_c != c.size:
         raise ValueError(
             "Invalid dimension: opt_subspace must have {} rows.".format(c.size)
         )
     if verbose > 0:
         print("Number of parameters: {}".format(dim_opt))
         print("Number of objectives: {}".format(objective_g.dim_f))
 
     # FIXME: generalize to other constraints
     constraints = get_fixed_boundary_constraints(
         iota=eq.iota is not None, kinetic=eq.electron_temperature is not None
     )
-    for constraint in constraints:
-        if not constraint.built:
-            constraint.build(eq, verbose=verbose)
+    constraints = maybe_add_self_consistency(constraints)
+    con_args = []
+    for con in constraints:
+        con_args += con.args
+        if not con.built:
+            con.build(eq, verbose=verbose)
+    con_args += objective_f.args + objective_g.args
+    objective_f.set_args(*con_args)
+    objective_g.set_args(*con_args)
+
     (
         xp,
-        A,
-        Ainv,
-        b,
+        _,
+        _,
         Z,
         unfixed_idx,
         project,
         recover,
     ) = factorize_linear_constraints(constraints, objective_f.args)
 
     # state vector
@@ -547,36 +578,48 @@
     # perturbation vectors
     dc1 = 0
     dc2 = 0
     dx1_reduced = 0
     dx2_reduced = 0
 
     # dx/dx_reduced
-    dxdx_reduced = np.eye(objective_f.dim_x)[:, unfixed_idx] @ Z
+    dxdx_reduced = jnp.eye(objective_f.dim_x)[:, unfixed_idx] @ Z
 
     # dx/dc
-    dxdc = np.zeros((objective_f.dim_x, 0))
+    dxdc = jnp.zeros((objective_f.dim_x, 0))
     if len(
         [
             arg
             for arg in ("R_lmn", "Z_lmn", "L_lmn", "p_l", "i_l", "Psi")
             if arg in deltas.keys()
         ]
     ):
-        x_idx = np.concatenate(
+        x_idx = jnp.concatenate(
             [objective_f.x_idx[arg] for arg in arg_order if arg in deltas.keys()]
         )
-        x_idx.sort(kind="mergesort")
-        dxdc = np.eye(objective_f.dim_x)[:, x_idx]
+        x_idx = jnp.sort(x_idx)
+        dxdc = jnp.eye(objective_f.dim_x)[:, x_idx]
     if "Rb_lmn" in deltas.keys():
-        dxdRb = np.eye(objective_f.dim_x)[:, objective_f.x_idx["R_lmn"]] @ Ainv["R_lmn"]
-        dxdc = np.hstack((dxdc, dxdRb))
+        con = get_instance(constraints, BoundaryRSelfConsistency)
+        A = con.derivatives["jac"]["R_lmn"](
+            *[jnp.zeros(con.dimensions[arg]) for arg in con.args]
+        )
+        A = (con.normalization * (A.T / con.weight)).T
+        Ainv = jnp.linalg.pinv(A)
+        dxdRb = jnp.eye(objective_f.dim_x)[:, objective_f.x_idx["R_lmn"]] @ Ainv
+        dxdc = jnp.hstack((dxdc, dxdRb))
     if "Zb_lmn" in deltas.keys():
-        dxdZb = np.eye(objective_f.dim_x)[:, objective_f.x_idx["Z_lmn"]] @ Ainv["Z_lmn"]
-        dxdc = np.hstack((dxdc, dxdZb))
+        con = get_instance(constraints, BoundaryZSelfConsistency)
+        A = con.derivatives["jac"]["Z_lmn"](
+            *[jnp.zeros(con.dimensions[arg]) for arg in con.args]
+        )
+        A = (con.normalization * (A.T / con.weight)).T
+        Ainv = jnp.linalg.pinv(A)
+        dxdZb = jnp.eye(objective_f.dim_x)[:, objective_f.x_idx["Z_lmn"]] @ Ainv
+        dxdc = jnp.hstack((dxdc, dxdZb))
 
     # 1st order
     if order > 0:
 
         f = objective_f.compute(xf)
         g = objective_g.compute(xg)
 
@@ -609,42 +652,42 @@
         # some scaling to improve conditioning and rescale trust region
         wf, _ = compute_jac_scale(Fx_reduced)
         wg, _ = compute_jac_scale(Gx_reduced)
         wx = wf + wg
         Fxh = Fx_reduced * wx
         Gxh = Gx_reduced * wx
         if cutoff is None:
-            cutoff = np.finfo(Fx_reduced.dtype).eps * np.max(Fx_reduced.shape)
-        uf, sf, vtf = np.linalg.svd(Fxh, full_matrices=False)
+            cutoff = jnp.finfo(Fx_reduced.dtype).eps * max(Fx_reduced.shape)
+        uf, sf, vtf = jnp.linalg.svd(Fxh, full_matrices=False)
         sf += sf[-1]  # add a tiny bit of regularization
-        sfi = np.where(sf < cutoff * sf[0], 0, 1 / sf)
-        Fxh_inv = vtf.T @ (sfi[..., np.newaxis] * uf.T)
+        sfi = jnp.where(sf < cutoff * sf[0], 0, 1 / sf)
+        Fxh_inv = vtf.T @ (sfi[..., jnp.newaxis] * uf.T)
 
         GxFx = Gxh @ Fxh_inv
         LHS = GxFx @ Fc - Gc
         RHS_1g = g - GxFx @ f
 
         # scaling for c
         # approx dc/dx at const f
-        dcdx_f = np.linalg.lstsq(Fc, Fx_reduced, rcond=None)[0]
+        dcdx_f = jnp.linalg.lstsq(Fc, Fx_reduced, rcond=None)[0]
         wc, _ = compute_jac_scale(dcdx_f.T)
         LHSh = LHS * wc
         # restrict to optimization subspace
         LHS_opt = LHSh @ subspace
 
         if verbose > 0:
             print("Factoring LHS")
         timer.start("LHS factorization")
-        ug, sg, vtg = np.linalg.svd(LHS_opt, full_matrices=False)
+        ug, sg, vtg = jnp.linalg.svd(LHS_opt, full_matrices=False)
         timer.stop("LHS factorization")
         if verbose > 1:
             timer.disp("LHS factorization")
 
-        c_norm = np.linalg.norm(dcdx_f @ x_reduced)
-        x_norm = np.linalg.norm(wx * x_reduced)
+        c_norm = jnp.linalg.norm(dcdx_f @ x_reduced)
+        x_norm = jnp.linalg.norm(wx * x_reduced)
 
         dc1h_opt, bound_hit, _ = trust_region_step_exact_svd(
             -RHS_1g,
             ug,
             sg,
             vtg.T,
             tr_ratio[0] * c_norm,
@@ -667,19 +710,19 @@
             rtol=0.01,
             max_iter=10,
         )
         dx1_reduced = dx1h_reduced * wx
     # 2nd order
     if order > 1:
 
-        idx = np.array([], dtype=int)
+        idx = jnp.array([], dtype=int)
         for arg in objective_f.args:
             if arg not in objective_g.args:
-                idx = np.concatenate((idx, objective_f.x_idx[arg]))
-        dxf_dxg = np.delete(np.eye(objective_f.dim_x), idx, 1)
+                idx = jnp.concatenate((idx, objective_f.x_idx[arg]))
+        dxf_dxg = jnp.delete(jnp.eye(objective_f.dim_x), idx, 1)
 
         # 2nd partial derivatives of f objective wrt both x and c
         if verbose > 0:
             print("Computing d^2f")
         timer.start("d^2f computation")
         tangents_f = dxdx_reduced @ dx1_reduced + dxdc @ dc1
         RHS_2f = -0.5 * objective_f.jvp((tangents_f, tangents_f), xf)
@@ -698,30 +741,30 @@
             timer.disp("d^2g computation")
 
         dc2h_opt, _, _ = trust_region_step_exact_svd(
             -RHS_2g,
             ug,
             sg,
             vtg.T,
-            tr_ratio[1] * np.linalg.norm(dc1h_opt),
+            tr_ratio[1] * jnp.linalg.norm(dc1h_opt),
             initial_alpha=None,
             rtol=0.01,
             max_iter=10,
         )
 
         dc2h = dc2h_opt @ subspace.T
         dc2 = dc2h * wc
         RHS_2f += -Fc @ dc2
 
         dx2h_reduced, _, _ = trust_region_step_exact_svd(
             -RHS_2f,
             uf,
             sf,
             vtf.T,
-            tr_ratio[1] * np.linalg.norm(dx1h_reduced),
+            tr_ratio[1] * jnp.linalg.norm(dx1h_reduced),
             initial_alpha=None,
             rtol=0.01,
             max_iter=10,
         )
         dx2_reduced = dx2h_reduced * wx
     if order > 2:
         raise ValueError(
@@ -739,38 +782,40 @@
     # update perturbation attributes
     idx0 = 0
     for key, value in deltas.items():
         setattr(eq_new, key, getattr(eq_new, key) + dc[idx0 : idx0 + len(value)])
         idx0 += len(value)
     for constraint in constraints:
         constraint.update_target(eq_new)
-    xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+    xp, _, _, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints, objective_f.args
     )
 
     # update other attributes
     dx_reduced = dx1_reduced + dx2_reduced
     x_new = recover(x_reduced + dx_reduced)
     args = objective_f.unpack_state(x_new)
     for key, value in args.items():
         if key not in deltas:
             value = put(  # parameter values below threshold are set to 0
-                value, np.where(np.abs(value) < 10 * np.finfo(value.dtype).eps)[0], 0
+                value, jnp.where(jnp.abs(value) < 10 * jnp.finfo(value.dtype).eps)[0], 0
             )
             # don't set nonexistent profile (values are empty ndarrays)
             if value.size:
                 setattr(eq_new, key, value)
 
     predicted_reduction = -evaluate_quadratic_form_jac(LHS, -RHS_1g.T @ LHS, dc)
 
     timer.stop("Total perturbation")
     if verbose > 0:
-        print("||dc||/||c|| = {:10.3e}".format(np.linalg.norm(dc) / np.linalg.norm(c)))
+        print(
+            "||dc||/||c|| = {:10.3e}".format(jnp.linalg.norm(dc) / jnp.linalg.norm(c))
+        )
         print(
             "||dx||/||x|| = {:10.3e}".format(
-                np.linalg.norm(dx_reduced) / np.linalg.norm(x_reduced)
+                jnp.linalg.norm(dx_reduced) / jnp.linalg.norm(x_reduced)
             )
         )
     if verbose > 1:
         timer.disp("Total perturbation")
 
-    return eq_new, predicted_reduction, dc_opt, dc, np.linalg.norm(c), bound_hit
+    return eq_new, predicted_reduction, dc_opt, dc, jnp.linalg.norm(c), bound_hit
```

### Comparing `desc-opt-0.8.1/desc/plotting.py` & `desc-opt-0.8.2/desc/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -596,25 +596,17 @@
         return ValueError(colored("Grid must be 2D", "red"))
 
     data, label = _compute(eq, name, grid, kwargs.pop("component", None))
     fig, ax = _format_ax(ax, figsize=kwargs.pop("figsize", None))
     divider = make_axes_locatable(ax)
 
     if norm_F:
-        assert name == "|F|", "Can only normalize |F|."
-        if (
-            np.max(abs(eq.p_l)) <= np.finfo(eq.p_l.dtype).eps
-        ):  # normalize vacuum force by B pressure gradient
-            norm_name = "|grad(|B|^2)|/2mu0"
-            norm_data, _ = _compute(eq, norm_name, grid)
-        else:  # normalize force balance with pressure by gradient of pressure
-            norm_name = "<|grad(p)|>_vol"
-            # we can use the regular grid here because eq.compute will automatically
-            # use the correct quad grid for volume avg
-            norm_data, _ = _compute(eq, norm_name, grid, reshape=False)
+        # normalize force by B pressure gradient
+        norm_name = kwargs.pop("norm_name", "<|grad(|B|^2)|/2mu0>_vol")
+        norm_data, _ = _compute(eq, norm_name, grid, reshape=False)
         data = data / np.nanmean(np.abs(norm_data))  # normalize
 
     # reshape data to 2D
     if 0 in plot_axes:
         if 1 in plot_axes:  # rho & theta
             data = data[:, :, 0]
         else:  # rho & zeta
@@ -1016,25 +1008,17 @@
             r"$\langle " + label[0][1:] + r" \rangle_{\theta}~" + "~".join(label[1:])
         )
         values = surface_averages(grid, q=values)
         plot_data_ylabel_key = f"<{name}>_fsa"
     values = compress(grid, values)
 
     if norm_F:
-        assert name == "|F|", "Can only normalize |F|."
-        if (
-            np.max(abs(eq.p_l)) <= np.finfo(eq.p_l.dtype).eps
-        ):  # normalize vacuum force by B pressure gradient
-            norm_name = "|grad(|B|^2)|/2mu0"
-            norm_data, _ = _compute(eq, norm_name, grid)
-        else:  # normalize force balance with pressure by gradient of pressure
-            norm_name = "<|grad(p)|>_vol"
-            # we can use the regular grid here because eq.compute will automatically
-            # use the correct quad grid for volume avg
-            norm_data, _ = _compute(eq, norm_name, grid, reshape=False)
+        # normalize force by B pressure gradient
+        norm_name = kwargs.pop("norm_name", "<|grad(|B|^2)|/2mu0>_vol")
+        norm_data, _ = _compute(eq, norm_name, grid, reshape=False)
         values = values / np.nanmean(np.abs(norm_data))  # normalize
     if log:
         values = np.abs(values)  # ensure data is positive for log plot
         ax.semilogy(
             rho, values, label=kwargs.pop("label", None), color=linecolor, ls=ls, lw=lw
         )
     else:
@@ -1162,25 +1146,17 @@
         zeta = np.unique(grid.nodes[:, 2])
         nzeta = zeta.size
     rows = np.floor(np.sqrt(nzeta)).astype(int)
     cols = np.ceil(nzeta / rows).astype(int)
 
     data, label = _compute(eq, name, grid, kwargs.pop("component", None))
     if norm_F:
-        assert name == "|F|", "Can only normalize |F|."
-        if (
-            np.max(abs(eq.p_l)) <= np.finfo(eq.p_l.dtype).eps
-        ):  # normalize vacuum force by B pressure gradient
-            norm_name = "|grad(|B|^2)|/2mu0"
-            norm_data, _ = _compute(eq, norm_name, grid)
-        else:  # normalize force balance with pressure by gradient of pressure
-            norm_name = "<|grad(p)|>_vol"
-            # we can use the regular grid here because eq.compute will automatically
-            # use the correct quad grid for volume avg
-            norm_data, _ = _compute(eq, norm_name, grid, reshape=False)
+        # normalize force by B pressure gradient
+        norm_name = kwargs.pop("norm_name", "<|grad(|B|^2)|/2mu0>_vol")
+        norm_data, _ = _compute(eq, norm_name, grid, reshape=False)
         data = data / np.nanmean(np.abs(norm_data))  # normalize
 
     figw = 5 * cols
     figh = 5 * rows
     fig, ax = _format_ax(
         ax,
         rows=rows,
@@ -1406,15 +1382,15 @@
         "rho": np.linspace(0, 1, NR),
         "NFP": nfp,
         "theta": theta,
         "zeta": zeta,
     }
     if plot_theta:
         # Note: theta* (also known as vartheta) is the poloidal straight field-line
-        # anlge in PEST-like flux coordinates
+        # angle in PEST-like flux coordinates
         t_grid = _get_grid(**grid_kwargs)
         v_grid = Grid(eq.compute_theta_coords(t_grid.nodes))
     rows = np.floor(np.sqrt(nzeta)).astype(int)
     cols = np.ceil(nzeta / rows).astype(int)
 
     # rho contours
     with warnings.catch_warnings():
```

### Comparing `desc-opt-0.8.1/desc/profiles.py` & `desc-opt-0.8.2/desc/profiles.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/transform.py` & `desc-opt-0.8.2/desc/transform.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc/utils.py` & `desc-opt-0.8.2/desc/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,7 +465,12 @@
     """
     for a, b in zip(shp1[::-1], shp2[::-1]):
         if a == 1 or b == 1 or a == b:
             pass
         else:
             return False
     return True
+
+
+def get_instance(things, cls):
+    """Get thing from a collection of things that is the instance of a given class."""
+    return [t for t in things if isinstance(t, cls)][0]
```

### Comparing `desc-opt-0.8.1/desc/vmec.py` & `desc-opt-0.8.2/desc/vmec.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 from scipy.constants import mu_0
 
 from desc.basis import DoubleFourierSeries
 from desc.compat import ensure_positive_jacobian
 from desc.compute.utils import compress, surface_averages
 from desc.equilibrium import Equilibrium
 from desc.grid import Grid, LinearGrid
-from desc.objectives import FixBoundaryR, FixBoundaryZ, ObjectiveFunction
+from desc.objectives import (
+    BoundaryRSelfConsistency,
+    BoundaryZSelfConsistency,
+    FixBoundaryR,
+    FixBoundaryZ,
+    ObjectiveFunction,
+)
 from desc.objectives.utils import factorize_linear_constraints
 from desc.profiles import PowerSeriesProfile, SplineProfile
 from desc.transform import Transform
 from desc.utils import Timer
 from desc.vmec_utils import (
     fourier_to_zernike,
     ptolemy_identity_fwd,
@@ -138,19 +144,21 @@
         m, n, L_mn = ptolemy_identity_fwd(xm, xn, s=lmns, c=lmnc)
         eq.L_lmn = fourier_to_zernike(m, n, L_mn, eq.L_basis)
 
         eq = ensure_positive_jacobian(eq)
 
         # apply boundary conditions
         constraints = (
-            FixBoundaryR(fixed_boundary=True),
-            FixBoundaryZ(fixed_boundary=True),
+            FixBoundaryR(),
+            FixBoundaryZ(),
+            BoundaryRSelfConsistency(),
+            BoundaryZSelfConsistency(),
         )
         objective = ObjectiveFunction(constraints, eq=eq, verbose=0)
-        _, _, _, _, _, _, project, recover = factorize_linear_constraints(
+        _, _, _, _, _, project, recover = factorize_linear_constraints(
             constraints, objective.args
         )
         args = objective.unpack_state(recover(project(objective.x(eq))))
         for key, value in args.items():
             setattr(eq, key, value)
 
         return eq
```

### Comparing `desc-opt-0.8.1/desc/vmec_utils.py` & `desc-opt-0.8.2/desc/vmec_utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/desc_opt.egg-info/PKG-INFO` & `desc-opt-0.8.2/desc_opt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: desc-opt
-Version: 0.8.1
+Version: 0.8.2
 Summary: Computes, analyzes and optimizes 3D MHD equilibria for stellarators and tokamaks
 Home-page: https://github.com/PlasmaControl/DESC/
 Author: Daniel Dudt, Rory Conlin, Dario Panici, Egemen Kolemen
 Author-email: PlasmaControl@princeton.edu
 License: MIT
 Project-URL: Issues Tracker, https://github.com/PlasmaControl/DESC/issues
 Project-URL: Contributing, https://github.com/PlasmaControl/DESC/blob/master/CONTRIBUTING.rst
@@ -28,26 +28,24 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/PlasmaControl/DESC/master/docs/_static/images/logo_med_clear.png
 
 .. inclusion-marker-do-not-remove
 
-##############################
-Stellarator Equilibrium Solver
-##############################
+################################
+Stellarator Optimization Package
+################################
 |License| |DOI| |Issues| |Pypi|
 
 |Docs| |UnitTests| |RegressionTests| |Codecov|
 
-DESC computes 3D MHD equilibria by solving the force balance equations.
-It can also be used for perturbation analysis and sensitivity studies to see how the equilibria change as input parameters are varied.
+DESC solves for and optimizes 3D MHD equilibria using pseudo-spectral numerical methods and automatic differentiation.
 
-The theoretical approach and numerical methods used by DESC are presented in these papers [1]_ [2]_ [3]_ [4]_
-and documented at Theory_.
+The theoretical approach and implementation details used by DESC are presented in these papers [1]_ [2]_ [3]_ [4]_ and documented at Theory_.
 Please cite our work if you use DESC!
 
 .. [1] Dudt, D. & Kolemen, E. (2020). DESC: A Stellarator Equilibrium Solver. [`Physics of Plasmas <https://aip.scitation.org/doi/full/10.1063/5.0020743>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/master/docs/Dudt_Kolemen_PoP_2020.pdf>`__]
 .. [2] Panici, D. et al (2022). The DESC Stellarator Code Suite Part I: Quick and accurate equilibria computations. [`arxiv <https://arxiv.org/abs/2203.17173>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/panici2022/panici2022equilibria.pdf>`__]
 .. [3] Conlin, R. et al. (2022). The DESC Stellarator Code Suite Part II: Perturbation and continuation methods. [`arxiv <https://arxiv.org/abs/2203.15927>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/conlin2022/conlin2022perturbations.pdf>`__]
 .. [4] Dudt, D. et al. (2022). The DESC Stellarator Code Suite Part III: Quasi-symmetry optimization. [`arxiv <https://arxiv.org/abs/2204.00078>`__]    [`pdf <https://github.com/PlasmaControl/DESC/blob/c669f5f28bf32042c76597c254d85c92f62f078a/publications/dudt2022/dudt2022optimization.pdf>`__]
 .. _Theory: https://desc-docs.readthedocs.io/en/latest/theory_general.html
```

### Comparing `desc-opt-0.8.1/desc_opt.egg-info/SOURCES.txt` & `desc-opt-0.8.2/desc_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/setup.cfg` & `desc-opt-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/setup.py` & `desc-opt-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_backend.py` & `desc-opt-0.8.2/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_basis.py` & `desc-opt-0.8.2/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_bootstrap.py` & `desc-opt-0.8.2/tests/test_bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1611,13 +1611,14 @@
         ion_temperature=1,
     )
     # ion temperature too low
     with pytest.warns(UserWarning):
         obj.build(eq)
 
     # make sure default grid has the right nodes
-    assert obj.grid.num_theta == 13
-    assert obj.grid.num_zeta == 13
-    assert obj.grid.num_rho == 5
+    assert obj._transforms["grid"].num_theta == 13
+    assert obj._transforms["grid"].num_zeta == 13
+    assert obj._transforms["grid"].num_rho == 5
     np.testing.assert_allclose(
-        obj.grid.nodes[obj.grid.unique_rho_idx, 0], np.array([0.2, 0.4, 0.6, 0.8, 1.0])
+        obj._transforms["grid"].nodes[obj._transforms["grid"].unique_rho_idx, 0],
+        np.array([0.2, 0.4, 0.6, 0.8, 1.0]),
     )
```

### Comparing `desc-opt-0.8.1/tests/test_coils.py` & `desc-opt-0.8.2/tests/test_coils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_compute_funs.py` & `desc-opt-0.8.2/tests/test_compute_funs.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     rho = np.linspace(1 / 128, 1, 128)
     grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, sym=eq.sym, rho=rho)
     data = eq.compute(["S(r)", "R0"], grid=grid)
     S = 4 * data["R0"] * np.pi**2 * rho
     np.testing.assert_allclose(S, compress(grid, data["S(r)"]))
 
 
-# TODO: remove or combine with above
 @pytest.mark.unit
 def test_surface_areas_2():
     """Alternate test that the flux surface areas match known analytic formulas."""
     eq = Equilibrium()
 
     grid_r = LinearGrid(rho=1, theta=10, zeta=10)
     grid_t = LinearGrid(rho=10, theta=1, zeta=10)
@@ -868,14 +867,75 @@
         data["B_rz"].reshape((num_zeta, num_rho, 3))[2:-2, 3:-2, :],
         B_rz[2:-2, 3:-2, :],
         rtol=rtol,
         atol=atol * np.nanmean(np.abs(data["B_rz"])),
     )
 
 
+@pytest.mark.unit
+def test_metric_derivatives(DummyStellarator):
+    """Compare analytic formula for metric derivatives with finite differences."""
+    eq = Equilibrium.load(
+        load_from=str(DummyStellarator["output_path"]), file_format="hdf5"
+    )
+
+    metric_components = ["g^rr", "g^rt", "g^rz", "g^tt", "g^tz", "g^zz"]
+
+    # rho derivatives
+    grid = LinearGrid(rho=np.linspace(0.5, 0.7, 100))
+    drho = np.diff(grid.nodes[:, 0]).mean()
+    data = eq.compute(
+        metric_components + [foo + "_r" for foo in metric_components], grid=grid
+    )
+    for thing in metric_components:
+        # some of these are so close to zero FD doesn't really work...
+        scale = np.linalg.norm(data[thing]) / data[thing].size
+        if scale < 1e-16:
+            continue
+        dthing_fd = np.convolve(data[thing], FD_COEF_1_4, "same") / drho
+        dthing_ex = data[thing + "_r"]
+        np.testing.assert_allclose(
+            dthing_fd[3:-3], dthing_ex[3:-3], err_msg=thing, rtol=1e-3, atol=1e-3
+        )
+
+    # theta derivatives
+    grid = LinearGrid(theta=np.linspace(0, np.pi / 4, 100))
+    dtheta = np.diff(grid.nodes[:, 1]).mean()
+    data = eq.compute(
+        metric_components + [foo + "_t" for foo in metric_components], grid=grid
+    )
+    for thing in metric_components:
+        # some of these are so close to zero FD doesn't really work...
+        scale = np.linalg.norm(data[thing]) / data[thing].size
+        if scale < 1e-16:
+            continue
+        dthing_fd = np.convolve(data[thing], FD_COEF_1_4, "same") / dtheta
+        dthing_ex = data[thing + "_t"]
+        np.testing.assert_allclose(
+            dthing_fd[3:-3], dthing_ex[3:-3], err_msg=thing, rtol=1e-3, atol=1e-3
+        )
+
+    # zeta derivatives
+    grid = LinearGrid(zeta=np.linspace(0, np.pi / 4, 100), NFP=3)
+    dzeta = np.diff(grid.nodes[:, 2]).mean()
+    data = eq.compute(
+        metric_components + [foo + "_z" for foo in metric_components], grid=grid
+    )
+    for thing in metric_components:
+        # some of these are so close to zero FD doesn't really work...
+        scale = np.linalg.norm(data[thing]) / data[thing].size
+        if scale < 1e-16:
+            continue
+        dthing_fd = np.convolve(data[thing], FD_COEF_1_4, "same") / dzeta
+        dthing_ex = data[thing + "_z"]
+        np.testing.assert_allclose(
+            dthing_fd[3:-3], dthing_ex[3:-3], err_msg=thing, rtol=1e-3, atol=1e-3
+        )
+
+
 @pytest.mark.slow
 @pytest.mark.unit
 def test_magnetic_pressure_gradient(DummyStellarator):
     """Test that the components of grad(|B|^2)) match with numerical gradients."""
     eq = Equilibrium.load(
         load_from=str(DummyStellarator["output_path"]), file_format="hdf5"
     )
```

### Comparing `desc-opt-0.8.1/tests/test_compute_utils.py` & `desc-opt-0.8.2/tests/test_compute_utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_configuration.py` & `desc-opt-0.8.2/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_constrain_current.py` & `desc-opt-0.8.2/tests/test_constrain_current.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_curves.py` & `desc-opt-0.8.2/tests/test_curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,19 +113,19 @@
 
         c.name = "my curve"
         assert "my" in c.name
         assert c.name in str(c)
         assert "FourierRZCurve" in str(c)
         assert c.sym
 
-        with pytest.warns(UserWarning):
-            c.NFP = 3
+        c.NFP = 3
         assert c.NFP == 3
         assert c.R_basis.NFP == 3
         assert c.Z_basis.NFP == 3
+        assert c.grid.NFP == 3
 
     @pytest.mark.unit
     def test_asserts(self):
         """Test error checking when creating FourierRZCurve."""
         with pytest.raises(ValueError):
             c = FourierRZCurve(R_n=[])
         c = FourierRZCurve()
```

### Comparing `desc-opt-0.8.1/tests/test_derivatives.py` & `desc-opt-0.8.2/tests/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_equilibrium.py` & `desc-opt-0.8.2/tests/test_equilibrium.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Tests for Equilibrium class."""
 
 import os
 import pickle
+import warnings
 
 import numpy as np
 import pytest
 from netCDF4 import Dataset
 
+import desc.examples
 from desc.__main__ import main
 from desc.equilibrium import EquilibriaFamily, Equilibrium
 from desc.grid import Grid, LinearGrid
 from desc.io import InputReader
+from desc.objectives import get_equilibrium_objective
 
 from .utils import area_difference, compute_coords
 
 
 @pytest.mark.unit
 @pytest.mark.solve
 def test_compute_geometry(DSHAPE_current):
@@ -226,7 +229,18 @@
     eq = Equilibrium()
     ir = InputReader(["./tests/inputs/DSHAPE"])
     eqf = EquilibriaFamily(eq, *ir.inputs)
     assert len(eqf) == 4
 
     with pytest.raises(TypeError):
         _ = EquilibriaFamily(4, 5, 6)
+
+
+@pytest.mark.unit
+def test_change_NFP():
+    """Test that changing the eq NFP correctly changes everything."""
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        eq = desc.examples.get("HELIOTRON")
+        eq.change_resolution(NFP=4)
+        obj = get_equilibrium_objective()
+        obj.build(eq)
```

### Comparing `desc-opt-0.8.1/tests/test_examples.py` & `desc-opt-0.8.2/tests/test_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     FixCurrent,
     FixIota,
     FixPressure,
     FixPsi,
     ForceBalance,
     HelicalForceBalance,
     ObjectiveFunction,
+    QuasisymmetryBoozer,
     QuasisymmetryTwoTerm,
     RadialForceBalance,
     get_fixed_boundary_constraints,
 )
 from desc.objectives.utils import get_NAE_constraints
 from desc.optimize import Optimizer
 from desc.plotting import plot_boozer_surface
@@ -287,18 +288,17 @@
     eq1 = load(".//tests//inputs//precise_QH_step1.h5")
     eq1a = run_qh_step(0, eq0)
     rho_err, theta_err = area_difference_desc(eq1, eq1a, Nr=1, Nt=1)
     # only need crude tolerances here to make sure the boundaries are
     # similar, the main test is ensuring its not pathological and has good qs
     assert rho_err.mean() < 1
 
-    grid = LinearGrid(M=eq1a.M_grid, N=eq1a.N_grid, NFP=eq1a.NFP, sym=False, rho=1.0)
-    data = eq1a.compute(["|B|_mn", "B modes"], grid, M_booz=eq1a.M, N_booz=eq1a.N)
-    idx = np.where(np.abs(data["B modes"][:, 1] / data["B modes"][:, 2]) != 1)[0]
-    B_asym = np.sort(np.abs(data["|B|_mn"][idx]))[:-1]
+    obj = QuasisymmetryBoozer(helicity=(1, eq1a.NFP))
+    obj.build(eq1a)
+    B_asym = obj.compute(*obj.xs(eq1a))
     np.testing.assert_array_less(B_asym, 1e-1)
 
 
 @pytest.mark.regression
 @pytest.mark.solve
 def test_qh_optimization2():
     """Tests precise QH optimization, step 2."""
@@ -306,18 +306,17 @@
     eq2 = load(".//tests//inputs//precise_QH_step2.h5")
     eq2a = run_qh_step(1, eq1)
     rho_err, theta_err = area_difference_desc(eq2, eq2a, Nr=1, Nt=1)
     # only need crude tolerances here to make sure the boundaries are
     # similar, the main test is ensuring its not pathological and has good qs
     assert rho_err.mean() < 1
 
-    grid = LinearGrid(M=eq2a.M_grid, N=eq2a.N_grid, NFP=eq2a.NFP, sym=False, rho=1.0)
-    data = eq2a.compute(["|B|_mn", "B modes"], grid, M_booz=eq2a.M, N_booz=eq2a.N)
-    idx = np.where(np.abs(data["B modes"][:, 1] / data["B modes"][:, 2]) != 1)[0]
-    B_asym = np.sort(np.abs(data["|B|_mn"][idx]))[:-1]
+    obj = QuasisymmetryBoozer(helicity=(1, eq2a.NFP))
+    obj.build(eq2a)
+    B_asym = obj.compute(*obj.xs(eq2a))
     np.testing.assert_array_less(B_asym, 1e-2)
 
 
 @pytest.mark.regression
 @pytest.mark.solve
 @pytest.mark.mpl_image_compare(remove_text=True, tolerance=15)
 def test_qh_optimization3():
@@ -326,19 +325,19 @@
     eq3 = load(".//tests//inputs//precise_QH_step3.h5")
     eq3a = run_qh_step(2, eq2)
     rho_err, theta_err = area_difference_desc(eq3, eq3a, Nr=1, Nt=1)
     # only need crude tolerances here to make sure the boundaries are
     # similar, the main test is ensuring its not pathological and has good qs
     assert rho_err.mean() < 1
 
-    grid = LinearGrid(M=eq3a.M_grid, N=eq3a.N_grid, NFP=eq3a.NFP, sym=False, rho=1.0)
-    data = eq3a.compute(["|B|_mn", "B modes"], grid=grid, M_booz=eq3a.M, N_booz=eq3a.N)
-    idx = np.where(np.abs(data["B modes"][:, 1] / data["B modes"][:, 2]) != 1)[0]
-    B_asym = np.sort(np.abs(data["|B|_mn"][idx]))[:-1]
-    np.testing.assert_array_less(B_asym, 2.5e-3)
+    obj = QuasisymmetryBoozer(helicity=(1, eq3a.NFP))
+    obj.build(eq3a)
+    B_asym = obj.compute(*obj.xs(eq3a))
+    np.testing.assert_array_less(B_asym, 1e-3)
+
     fig, ax = plot_boozer_surface(eq3a)
     return fig
 
 
 @pytest.mark.regression
 @pytest.mark.solve
 def test_ATF_results(tmpdir_factory):
@@ -552,60 +551,167 @@
     np.testing.assert_allclose(rho_err[:, 0:-4], 0, atol=1e-2)
     np.testing.assert_allclose(theta_err[:, 0:-6], 0, atol=1e-3)
 
     # Make sure iota of solved equilibrium is same near axis as QSC
     grid = LinearGrid(L=10, M=20, N=20, sym=True, axis=False)
     iota = compress(grid, eq.compute("iota", grid=grid)["iota"], "rho")
 
-    np.testing.assert_allclose(iota[1], qsc.iota, atol=1e-5)
+    np.testing.assert_allclose(iota[0], qsc.iota, atol=1e-5)
     np.testing.assert_allclose(iota[1:10], qsc.iota, atol=1e-3)
 
+    # check lambda to match near axis
+    grid_2d_05 = LinearGrid(rho=np.array(1e-6), M=50, N=50, NFP=eq.NFP, endpoint=True)
+
+    # Evaluate lambda near the axis
+    data_nae = eq.compute("lambda", grid=grid_2d_05)
+    lam_nae = data_nae["lambda"]
+
+    # Reshape to form grids on theta and phi
+    zeta = (
+        grid_2d_05.nodes[:, 2]
+        .reshape(
+            (grid_2d_05.num_theta, grid_2d_05.num_rho, grid_2d_05.num_zeta), order="F"
+        )
+        .squeeze()
+    )
+
+    lam_nae = lam_nae.reshape(
+        (grid_2d_05.num_theta, grid_2d_05.num_rho, grid_2d_05.num_zeta), order="F"
+    )
+
+    phi = np.squeeze(zeta[0, :])
+    lam_nae = np.squeeze(lam_nae[:, 0, :])
+
+    lam_av_nae = np.mean(lam_nae, axis=0)
+    np.testing.assert_allclose(lam_av_nae, -qsc.iota * qsc.nu_spline(phi), atol=2e-5)
+
+    # check |B| on axis
+
+    grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, rho=np.array(1e-6))
+    # Evaluate B modes near the axis
+    data_nae = eq.compute(["|B|_mn", "B modes"], grid=grid)
+    modes = data_nae["B modes"]
+    B_mn_nae = data_nae["|B|_mn"]
+    # Evaluate B on an angular grid
+    theta = np.linspace(0, 2 * np.pi, 150)
+    phi = np.linspace(0, 2 * np.pi, qsc.nphi)
+    th, ph = np.meshgrid(theta, phi)
+    B_nae = np.zeros((qsc.nphi, 150))
+
+    for i, (l, m, n) in enumerate(modes):
+        if m >= 0 and n >= 0:
+            B_nae += B_mn_nae[i] * np.cos(m * th) * np.cos(n * ph)
+        elif m >= 0 and n < 0:
+            B_nae += -B_mn_nae[i] * np.cos(m * th) * np.sin(n * ph)
+        elif m < 0 and n >= 0:
+            B_nae += -B_mn_nae[i] * np.sin(m * th) * np.cos(n * ph)
+        elif m < 0 and n < 0:
+            B_nae += B_mn_nae[i] * np.sin(m * th) * np.sin(n * ph)
+    # Eliminate the poloidal angle to focus on the toroidal behaviour
+    B_av_nae = np.mean(B_nae, axis=1)
+    np.testing.assert_allclose(B_av_nae, np.ones(np.size(phi)) * qsc.B0, atol=1e-4)
+
 
 @pytest.mark.regression
 @pytest.mark.solve
 @pytest.mark.slow
 def test_NAE_QIC_solve():
     """Test O(rho) NAE QIC constraints solve."""
     # get Qic example
-    qsc = Qic.from_paper("r2 section 5.2", nphi=99)
+    qsc = Qic.from_paper("QI NFP2 r2", nphi=301, order="r1")
+    qsc.lasym = False  # don't need to consider stell asym for order 1 constraints
     ntheta = 75
     r = 0.01
-    N = 9
-    eq = Equilibrium.from_near_axis(qsc, r=r, L=6, M=6, N=N, ntheta=ntheta)
+    N = 11
+    eq = Equilibrium.from_near_axis(qsc, r=r, L=7, M=7, N=N, ntheta=ntheta)
 
     orig_Rax_val = eq.axis.R_n
     orig_Zax_val = eq.axis.Z_n
 
     eq_fit = eq.copy()
 
     # this has all the constraints we need,
     #  iota=False specifies we want to fix current instead of iota
     cs = get_NAE_constraints(eq, qsc, iota=False, order=1)
 
     objectives = ForceBalance()
     obj = ObjectiveFunction(objectives)
 
-    eq.solve(verbose=3, ftol=1e-2, objective=obj, maxiter=50, xtol=1e-6, constraints=cs)
+    eq.solve(
+        verbose=3, ftol=1e-2, objective=obj, maxiter=100, xtol=1e-6, constraints=cs
+    )
 
     # Make sure axis is same
     np.testing.assert_almost_equal(orig_Rax_val, eq.axis.R_n)
     np.testing.assert_almost_equal(orig_Zax_val, eq.axis.Z_n)
 
-    # Make sure surfaces of solved equilibrium are similar near axis as QSC
+    # Make sure surfaces of solved equilibrium are similar near axis as QIC
     rho_err, theta_err = area_difference_desc(eq, eq_fit)
 
-    np.testing.assert_allclose(rho_err[:, 0:-4], 0, atol=1e-2)
-    np.testing.assert_allclose(theta_err[:, 0:-6], 0, atol=1e-3)
+    np.testing.assert_allclose(rho_err[:, 0:-8], 0, atol=5e-3)
+    np.testing.assert_allclose(theta_err[:, 0:-5], 0, atol=2e-2)
 
-    # Make sure iota of solved equilibrium is same near axis as QSC
+    # Make sure iota of solved equilibrium is same near axis as QIC
     grid = LinearGrid(L=10, M=20, N=20, sym=True, axis=False)
     iota = compress(grid, eq.compute("iota", grid=grid)["iota"], "rho")
 
-    np.testing.assert_allclose(iota[1], qsc.iota, atol=2e-5)
-    np.testing.assert_allclose(iota[1:10], qsc.iota, atol=1e-3)
+    np.testing.assert_allclose(iota[1], qsc.iota, atol=1e-5)
+    np.testing.assert_allclose(iota[1:10], qsc.iota, atol=5e-4)
+
+    # check lambda to match near axis
+    grid_2d_05 = LinearGrid(rho=np.array(1e-6), M=50, N=50, NFP=eq.NFP, endpoint=True)
+
+    # Evaluate lambda near the axis
+    data_nae = eq.compute("lambda", grid=grid_2d_05)
+    lam_nae = data_nae["lambda"]
+
+    # Reshape to form grids on theta and phi
+    zeta = (
+        grid_2d_05.nodes[:, 2]
+        .reshape(
+            (grid_2d_05.num_theta, grid_2d_05.num_rho, grid_2d_05.num_zeta), order="F"
+        )
+        .squeeze()
+    )
+
+    lam_nae = lam_nae.reshape(
+        (grid_2d_05.num_theta, grid_2d_05.num_rho, grid_2d_05.num_zeta), order="F"
+    )
+
+    phi = np.squeeze(zeta[0, :])
+    lam_nae = np.squeeze(lam_nae[:, 0, :])
+
+    lam_av_nae = np.mean(lam_nae, axis=0)
+    np.testing.assert_allclose(lam_av_nae, -qsc.iota * qsc.nu_spline(phi), atol=4e-5)
+
+    # check |B| on axis
+
+    grid = LinearGrid(M=eq.M_grid, N=eq.N_grid, NFP=eq.NFP, rho=np.array(1e-6))
+    # Evaluate B modes near the axis
+    data_nae = eq.compute(["|B|_mn", "B modes"], grid=grid)
+    modes = data_nae["B modes"]
+    B_mn_nae = data_nae["|B|_mn"]
+    # Evaluate B on an angular grid
+    theta = np.linspace(0, 2 * np.pi, 150)
+    phi = np.linspace(0, 2 * np.pi, qsc.nphi)
+    th, ph = np.meshgrid(theta, phi)
+    B_nae = np.zeros((qsc.nphi, 150))
+
+    for i, (l, m, n) in enumerate(modes):
+        if m >= 0 and n >= 0:
+            B_nae += B_mn_nae[i] * np.cos(m * th) * np.cos(n * ph)
+        elif m >= 0 and n < 0:
+            B_nae += -B_mn_nae[i] * np.cos(m * th) * np.sin(n * ph)
+        elif m < 0 and n >= 0:
+            B_nae += -B_mn_nae[i] * np.sin(m * th) * np.cos(n * ph)
+        elif m < 0 and n < 0:
+            B_nae += B_mn_nae[i] * np.sin(m * th) * np.sin(n * ph)
+    # Eliminate the poloidal angle to focus on the toroidal behaviour
+    B_av_nae = np.mean(B_nae, axis=1)
+    np.testing.assert_allclose(B_av_nae, np.ones(np.size(phi)) * qsc.B0, atol=2e-2)
 
 
 class TestGetExample:
     """Tests for desc.examples.get."""
 
     @pytest.mark.unit
     def test_missing_example(self):
```

### Comparing `desc-opt-0.8.1/tests/test_geometry.py` & `desc-opt-0.8.2/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_grid.py` & `desc-opt-0.8.2/tests/test_grid.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         grid = Grid(nodes)
         weights = grid.weights
 
         w = 4 * np.pi**2 / (grid.num_nodes - 1)
         weights_ref = np.array([w, w, w / 2, w / 2, w, w])
 
         np.testing.assert_allclose(weights, weights_ref)
-        np.testing.assert_allclose(np.sum(grid.weights), (2 * np.pi) ** 2)
+        np.testing.assert_allclose(grid.weights.sum(), (2 * np.pi) ** 2)
 
     @pytest.mark.unit
     def test_linear_grid(self):
         """Test node placement in a LinearGrid."""
         L, M, N, NFP, axis, endpoint = 8, 5, 3, 2, True, False
         g = LinearGrid(L, M, N, NFP, sym=False, axis=axis, endpoint=endpoint)
 
@@ -62,43 +62,48 @@
                     g.num_rho * g.num_theta,
                 ),
             ]
         ).T
 
         np.testing.assert_allclose(g.nodes, nodes)
         np.testing.assert_allclose(g.weights.sum(), (2 * np.pi) ** 2)
-        # spacing.prod == weights for linear grids
-        # this is not true for concentric or any grid with duplicates
+        # spacing.prod != weights for grid with duplicates
         if not endpoint:
             np.testing.assert_allclose(g.spacing.prod(axis=1), g.weights)
 
     @pytest.mark.unit
-    def test_linear_grid_spacing(self):
-        """Test linear grid spacing is consistent."""
+    def test_linear_grid_spacing_consistency(self):
+        """Test consistency between alternate construction methods."""
 
         def test(sym, endpoint, axis, ntheta_is_odd):
             nrho = 1
-            # more edge cases are caught when ntheta is odd when endpoint=True
-            # and ntheta is even when endpoint is False
             ntheta = 6 + ntheta_is_odd
             nzeta = 7
             NFP = 3
-            theta = np.linspace(0, 2 * np.pi, ntheta, endpoint=endpoint)
-            if sym:
-                # When users supply nodes and set symmetry to true, they need
-                # to ensure their nodes are placed symmetrically.
-                # Here we change the array to match the effect done in grid.py,
-                # so the nodes are actually symmetric.
+            # We need to construct the theta coordinates to match
+            # whatever is done in grid.py for construction via theta=integer input.
+            # First round up ntheta + endpoint to next even integer.
+            theta = np.linspace(
+                0,
+                2 * np.pi,
+                (ntheta + endpoint + 1) // 2 * 2 - endpoint
+                if (sym and ntheta > 1)
+                else ntheta,
+                endpoint=endpoint,
+            )
+            if sym and ntheta > 1:
+                # Second, change the array to match the effect done in grid.py,
+                # which sets dtheta to a constant. This requires shifting nodes
+                # off the axis.
                 theta += theta[1] / 2
-                if endpoint:
-                    # We have to manually delete last node because the addition
-                    # above pushed it to the (2pi, pi) range which = (0, pi)
-                    # range, meaning it wouldn't have been deleted by
-                    # enforce_symmetry which only removes nodes from (pi, 2pi).
-                    theta = theta[:-1]
+                # Third, manually delete last node because the addition
+                # above pushed it to the (2pi, pi) range which = (0, pi)
+                # range, meaning it wouldn't have been deleted by
+                # enforce_symmetry which only removes nodes from (pi, 2pi).
+                theta = theta[: theta.size - endpoint]
             lg_1 = LinearGrid(
                 rho=nrho,
                 theta=ntheta,
                 zeta=nzeta,
                 NFP=NFP,
                 sym=sym,
                 axis=axis,
@@ -111,14 +116,15 @@
                 NFP=NFP,
                 sym=sym,
                 axis=axis,
                 endpoint=endpoint,
             )
             np.testing.assert_allclose(lg_1.nodes, lg_2.nodes)
             np.testing.assert_allclose(lg_1.spacing, lg_2.spacing)
+            np.testing.assert_allclose(lg_1.weights, lg_2.weights)
 
         # ntheta is odd
         test(sym=False, endpoint=False, axis=False, ntheta_is_odd=True)
         test(sym=False, endpoint=False, axis=True, ntheta_is_odd=True)
         test(sym=False, endpoint=True, axis=False, ntheta_is_odd=True)
         test(sym=False, endpoint=True, axis=True, ntheta_is_odd=True)
         test(sym=True, endpoint=False, axis=False, ntheta_is_odd=True)
@@ -132,14 +138,36 @@
         test(sym=False, endpoint=True, axis=True, ntheta_is_odd=False)
         test(sym=True, endpoint=False, axis=False, ntheta_is_odd=False)
         test(sym=True, endpoint=False, axis=True, ntheta_is_odd=False)
         test(sym=True, endpoint=True, axis=False, ntheta_is_odd=False)
         test(sym=True, endpoint=True, axis=True, ntheta_is_odd=False)
 
     @pytest.mark.unit
+    def test_linear_grid_symmetric_nodes_consistency(self):
+        """Test that specifying theta nodes from [0, pi] is sufficient."""
+        # uniform spacing
+        theta = np.linspace(0, 2 * np.pi, 10)
+        lg_1 = LinearGrid(L=5, theta=theta, N=5, sym=True)
+        lg_2 = LinearGrid(L=5, theta=theta[theta <= np.pi], N=5, sym=True)
+        np.testing.assert_allclose(lg_1.nodes, lg_2.nodes)
+        np.testing.assert_allclose(lg_1.spacing, lg_2.spacing)
+        np.testing.assert_allclose(lg_1.weights, lg_2.weights)
+
+        # non-uniform spacing
+        pts = np.linspace(0, 1, 10)
+        rho = np.asarray([r**3 for r in pts])
+        theta = 2 * np.pi * np.asarray([t**1.85 for t in pts])
+        zeta = 2 * np.pi * np.asarray([z**4 for z in pts])
+        lg_1 = LinearGrid(rho=rho, theta=theta, zeta=zeta, sym=True)
+        lg_2 = LinearGrid(rho=rho, theta=theta[theta <= np.pi], zeta=zeta, sym=True)
+        np.testing.assert_allclose(lg_1.nodes, lg_2.nodes)
+        np.testing.assert_allclose(lg_1.spacing, lg_2.spacing)
+        np.testing.assert_allclose(lg_1.weights, lg_2.weights)
+
+    @pytest.mark.unit
     def test_linear_grid_spacing_two_nodes(self):
         """Test that 2 node grids assign equal spacing to nodes."""
         node_count = 2
         NFP = 7  # any integer > 1 is good candidate for test
 
         def test(endpoint):
             lg = LinearGrid(
@@ -174,125 +202,246 @@
             rho=np.linspace(1, 0, num=1)[::-1],
             theta=np.linspace(0, 2 * np.pi, num=3, endpoint=endpoint),
             zeta=np.linspace(0, 2 * np.pi, num=1, endpoint=endpoint),
             sym=sym,
             endpoint=endpoint,
         )
         np.testing.assert_allclose(lg_2.spacing, spacing)
+        np.testing.assert_allclose(lg_2.weights, spacing.prod(axis=1))
 
     @pytest.mark.unit
-    def test_duplicate_node_spacing(self):
-        """Test surface spacing on all types of grids with endpoint=True."""
+    def test_node_spacing_non_sym(self):
+        """Test surface spacing on grids with sym=False."""
+        self._test_node_spacing_non_sym(False, 8, 13, 3)
+        self._test_node_spacing_non_sym(True, 8, 13, 3)
+
+    @staticmethod
+    def _test_node_spacing_non_sym(
+        endpoint, unique_theta_count, unique_zeta_count, NFP
+    ):
+        """Test surface spacing on grids with sym=False."""
         nrho = 1
-        ntheta = 8  # unique theta count
-        nzeta = 13  # unique zeta count
-        NFP = 3
-        axis = True
-        endpoint = True
+        sym = False
 
         def test(grid):
-            is_theta_dupe = (endpoint and (ntheta > 0) and not grid.sym) & (
+            if not endpoint:
+                # if no duplicates
+                np.testing.assert_allclose(grid.weights, grid.spacing.prod(axis=1))
+            is_theta_dupe = (endpoint and unique_theta_count > 0 and not sym) & (
                 grid.nodes[:, 1] % (2 * np.pi) == 0
             )
-            is_zeta_dupe = (endpoint and nzeta > 0) & (
+            is_zeta_dupe = (endpoint and unique_zeta_count > 0) & (
                 grid.nodes[:, 2] % (2 * np.pi / NFP) == 0
             )
 
-            def test_surface(label, actual_ds, desired_ds):
+            def test_surface(surface_label, actual_ds, desired_ds):
                 for index, ds in enumerate(actual_ds):
                     if is_theta_dupe[index] and is_zeta_dupe[index]:
                         # the grid has 4 of these nodes
-                        np.testing.assert_allclose(ds, desired_ds / 4, err_msg=label)
+                        np.testing.assert_allclose(
+                            ds, desired_ds / 4, err_msg=surface_label
+                        )
                     elif is_theta_dupe[index] or is_zeta_dupe[index]:
                         # the grid has 2 of these nodes
-                        np.testing.assert_allclose(ds, desired_ds / 2, err_msg=label)
+                        np.testing.assert_allclose(
+                            ds, desired_ds / 2, err_msg=surface_label
+                        )
                     else:
                         # unique node
-                        np.testing.assert_allclose(ds, desired_ds, err_msg=label)
+                        np.testing.assert_allclose(
+                            ds, desired_ds, err_msg=surface_label
+                        )
 
-            if grid.sym:
-                dtheta_scale = max(ntheta, 1) / grid.num_theta
-            else:
-                dtheta_scale = 1
             test_surface(
                 "rho",
                 grid.spacing[:, 1:].prod(axis=1),
-                (2 * np.pi / max(ntheta, 1))
-                * (2 * np.pi / max(nzeta, 1))
-                * dtheta_scale,
+                (2 * np.pi / max(unique_theta_count, 1))
+                * (2 * np.pi / max(unique_zeta_count, 1)),
             )
             test_surface(
                 "theta",
                 grid.spacing[:, [0, 2]].prod(axis=1),
-                (1 / nrho) * (2 * np.pi / max(nzeta, 1)),
+                (1 / nrho) * (2 * np.pi / max(unique_zeta_count, 1)),
             )
             test_surface(
                 "zeta",
                 grid.spacing[:, :2].prod(axis=1),
-                (1 / nrho) * (2 * np.pi / max(ntheta, 1)) * dtheta_scale,
+                (1 / nrho) * (2 * np.pi / max(unique_theta_count, 1)),
             )
 
         lg_1 = LinearGrid(
             rho=nrho,
-            theta=ntheta + endpoint,
-            zeta=nzeta + endpoint,
+            theta=unique_theta_count + endpoint,
+            zeta=unique_zeta_count + endpoint,
             NFP=NFP,
-            sym=False,
-            axis=axis,
+            sym=sym,
             endpoint=endpoint,
         )
-        lg_1_sym = LinearGrid(
-            rho=nrho,
-            theta=ntheta + endpoint,
-            zeta=nzeta + endpoint,
-            NFP=NFP,
-            sym=True,
-            axis=axis,
-            endpoint=endpoint,
+        rho = np.linspace(1, 0, nrho)[::-1]
+        theta = np.linspace(
+            0, 2 * np.pi, unique_theta_count + endpoint, endpoint=endpoint
         )
-        lg_2 = LinearGrid(
-            rho=np.linspace(1, 0, nrho, endpoint=axis)[::-1],
-            theta=np.linspace(0, 2 * np.pi, ntheta + endpoint, endpoint=endpoint),
-            zeta=np.linspace(0, 2 * np.pi / NFP, nzeta + endpoint, endpoint=endpoint),
-            NFP=NFP,
-            sym=False,
-            axis=axis,
-            endpoint=endpoint,
+        zeta = np.linspace(
+            0, 2 * np.pi / NFP, unique_zeta_count + endpoint, endpoint=endpoint
         )
-        lg_2_sym = LinearGrid(
-            rho=np.linspace(1, 0, nrho, endpoint=axis)[::-1],
-            theta=np.linspace(0, 2 * np.pi, ntheta + endpoint, endpoint=endpoint),
-            zeta=np.linspace(0, 2 * np.pi / NFP, nzeta + endpoint, endpoint=endpoint),
-            NFP=NFP,
-            sym=True,
-            axis=axis,
-            endpoint=endpoint,
+        lg_2 = LinearGrid(
+            rho=rho, theta=theta, zeta=zeta, NFP=NFP, sym=sym, endpoint=endpoint
         )
         lg_3 = LinearGrid(
-            rho=np.linspace(1, 0, nrho, endpoint=axis)[::-1],
-            theta=np.linspace(0, 2 * np.pi, ntheta + endpoint, endpoint=endpoint),
-            zeta=np.linspace(0, 2 * np.pi / NFP, nzeta + endpoint, endpoint=endpoint),
+            rho=rho,
+            theta=theta,
+            zeta=zeta,
             NFP=NFP,
-            sym=False,
-            axis=axis,
+            sym=sym,
             endpoint=not endpoint,  # incorrect marker should have no effect
         )
         assert lg_3.endpoint == endpoint
         test(lg_1)
-        test(lg_1_sym)
         # The test below might fail for theta and zeta surfaces only if nrho > 1.
         # This is unrelated to how duplicate node spacing is handled.
         # The cause is because grid construction does not always
         # compute drho as constant (even when the rho nodes are linearly spaced),
         # and this test assumes drho to be a constant for grids without duplicates.
         test(lg_2)
-        test(lg_2_sym)
         test(lg_3)
 
     @pytest.mark.unit
+    def test_symmetry_spacing_basic(self):
+        """Test symmetry effect on spacing in a basic case."""
+        nrho = 2
+        ntheta = 3
+        nzeta = 2
+        lg = LinearGrid(rho=nrho, theta=ntheta, zeta=nzeta, sym=False)
+        lg_sym = LinearGrid(rho=nrho, theta=ntheta, zeta=nzeta, sym=True)
+        np.testing.assert_allclose(
+            lg.spacing,
+            np.tile(
+                [1 / nrho, 2 * np.pi / ntheta, 2 * np.pi / nzeta],
+                (nrho * ntheta * nzeta, 1),
+            ),
+        )
+        np.testing.assert_allclose(lg.weights, lg.spacing.prod(axis=1))
+        np.testing.assert_allclose(
+            lg_sym.spacing,
+            np.tile(
+                [1 / nrho, 2 * np.pi / (ntheta - 1), 2 * np.pi / nzeta],
+                (nrho * (ntheta - 1) * nzeta, 1),
+            ),
+        )
+        np.testing.assert_allclose(lg_sym.weights, lg_sym.spacing.prod(axis=1))
+
+    @pytest.mark.unit
+    def test_node_spacing_sym(self):
+        """Test surface spacing on grids with sym=True."""
+        # It's useful to test with ntheta even and odd.
+        # These tests should pass for any combination of parameters.
+        self._test_node_spacing_sym(False, 8, 13, 3)
+        self._test_node_spacing_sym(False, 7, 13, 3)
+        self._test_node_spacing_sym(True, 8, 13, 3)
+        self._test_node_spacing_sym(True, 7, 13, 3)
+
+    @staticmethod
+    def _test_node_spacing_sym(endpoint, ntheta, unique_zeta_count, NFP):
+        """Test surface spacing on grids with sym=True."""
+        nrho = 1
+        sym = True
+
+        # unique_theta_and_reflection count is twice
+        # the number of nodes at unique theta coordinates (0, pi)
+        # on a given theta curve.
+        def test(grid, unique_theta_and_reflection_count):
+            is_zeta_dupe = (endpoint and unique_zeta_count > 0) & (
+                grid.nodes[:, 2] % (2 * np.pi / NFP) == 0
+            )
+
+            def test_surface(label, actual_ds, desired_ds):
+                for index, ds in enumerate(actual_ds):
+                    if label != "theta" and sym and grid.nodes[index, 1] % np.pi != 0:
+                        # these nodes should have double weight to account for
+                        # reflection across symmetry line
+                        if is_zeta_dupe[index]:
+                            # the grid has 2 of these nodes,
+                            # so each should have half weight
+                            np.testing.assert_allclose(
+                                ds, (desired_ds / 2) * 2, err_msg=label
+                            )
+                        else:
+                            np.testing.assert_allclose(
+                                ds, desired_ds * 2, err_msg=label
+                            )
+                    elif is_zeta_dupe[index]:
+                        # the grid has 2 of these nodes,
+                        # so each should have half weight
+                        np.testing.assert_allclose(ds, desired_ds / 2, err_msg=label)
+                    else:
+                        # unique node
+                        np.testing.assert_allclose(ds, desired_ds, err_msg=label)
+
+            test_surface(
+                "rho",
+                grid.spacing[:, 1:].prod(axis=1),
+                (2 * np.pi / max(unique_theta_and_reflection_count, 1))
+                * (2 * np.pi / max(unique_zeta_count, 1)),
+            )
+            test_surface(
+                "theta",
+                grid.spacing[:, [0, 2]].prod(axis=1),
+                (1 / nrho) * (2 * np.pi / max(unique_zeta_count, 1)),
+            )
+            test_surface(
+                "zeta",
+                grid.spacing[:, :2].prod(axis=1),
+                (1 / nrho) * (2 * np.pi / max(unique_theta_and_reflection_count, 1)),
+            )
+
+        lg_1_sym = LinearGrid(
+            rho=nrho,
+            theta=ntheta,
+            zeta=unique_zeta_count + endpoint,
+            NFP=NFP,
+            sym=sym,
+            endpoint=endpoint,
+        )
+        # Recall that LinearGrid created with integers forces ntheta + endpoint
+        # to be even and shifts nodes counterclockwise. The result is that
+        # unique_theta_and_reflection_count is ntheta rounded up (down) to the
+        # closest even integer when endpoint is false (true).
+        test(
+            lg_1_sym, unique_theta_and_reflection_count=(ntheta - endpoint + 1) // 2 * 2
+        )
+
+        rho = np.linspace(1, 0, nrho)[::-1]
+        theta = np.linspace(0, 2 * np.pi, ntheta, endpoint=endpoint)
+        zeta = np.linspace(
+            0, 2 * np.pi / NFP, unique_zeta_count + endpoint, endpoint=endpoint
+        )
+        lg_2_sym = LinearGrid(
+            rho=rho, theta=theta, zeta=zeta, NFP=NFP, sym=sym, endpoint=endpoint
+        )
+        lg_3_sym = LinearGrid(
+            rho=rho,
+            theta=theta,
+            zeta=zeta,
+            NFP=NFP,
+            sym=sym,
+            endpoint=not endpoint,  # incorrect marker should have no effect
+        )
+        # endpoints were deleted
+        assert not lg_1_sym.endpoint
+        assert not lg_2_sym.endpoint
+        assert not lg_3_sym.endpoint
+        # The test below might fail for theta and zeta surfaces only if nrho > 1.
+        # This is unrelated to how duplicate node spacing is handled.
+        # The cause is because grid construction does not always
+        # compute drho as constant (even when the rho nodes are linearly spaced),
+        # and this test assumes drho to be a constant for grids without duplicates.
+        test(lg_2_sym, unique_theta_and_reflection_count=ntheta - endpoint)
+        test(lg_3_sym, unique_theta_and_reflection_count=ntheta - endpoint)
+
+    @pytest.mark.unit
     def test_concentric_grid(self):
         """Test node placement in ConcentricGrid."""
         M = 2
         N = 0
         NFP = 1
 
         grid_ansi = ConcentricGrid(
@@ -357,15 +506,14 @@
                 np.array(
                     [0, 2 * np.pi / 5, 4 * np.pi / 5, 6 * np.pi / 5, 8 * np.pi / 5] * 3
                 ),
                 np.zeros(15),
             ]
         ).T
 
-        # spacing.prod == weights for quad grids (not true for concentric)
         np.testing.assert_allclose(grid_quad.spacing.prod(axis=1), grid_quad.weights)
         np.testing.assert_allclose(grid_quad.nodes, quadrature_nodes)
 
     @pytest.mark.unit
     def test_concentric_grid_high_res(self):
         """Test that we can create high resolution grids without crashing.
 
@@ -430,39 +578,16 @@
         cg = ConcentricGrid(2, 3, 4)
         cg.change_resolution(3, 4, 5)
         assert cg.L == 3
         assert cg.M == 4
         assert cg.N == 5
 
     @pytest.mark.unit
-    def test_symmetry_spacing_basic(self):
-        """Test symmetry effect on spacing in a basic case."""
-        nrho = 2
-        ntheta = 3
-        nzeta = 2
-        lg = LinearGrid(rho=nrho, theta=ntheta, zeta=nzeta, sym=False)
-        lg_sym = LinearGrid(rho=nrho, theta=ntheta, zeta=nzeta, sym=True)
-        np.testing.assert_allclose(
-            lg.spacing,
-            np.tile(
-                [1 / nrho, 2 * np.pi / ntheta, 2 * np.pi / nzeta],
-                (nrho * ntheta * nzeta, 1),
-            ),
-        )
-        np.testing.assert_allclose(
-            lg_sym.spacing,
-            np.tile(
-                [1 / nrho, 2 * np.pi / (ntheta - 1), 2 * np.pi / nzeta],
-                (nrho * (ntheta - 1) * nzeta, 1),
-            ),
-        )
-
-    @pytest.mark.unit
-    def test_enforce_symmetry(self):
-        """Test that enforce_symmetry spaces theta nodes correctly.
+    def test_enforce_symmetry_sum(self):
+        """Test that enforce_symmetry sums dtheta to 2pi.
 
         Relies on correctness of surface_integrals.
         """
 
         def test(grid):
             # check if theta nodes cover the circumference of the theta curve
             dtheta_sums = surface_integrals(grid, q=1 / grid.spacing[:, 2])
@@ -472,86 +597,255 @@
         # this grid has 2 surfaces near axis lacking theta > pi nodes.
         # These edge cases should be handled correctly.
         # Otherwise, a dimension mismatch or broadcast error should be raised.
         test(ConcentricGrid(L=20, M=3, N=2, sym=True))
         test(LinearGrid(L=20, M=3, N=2, sym=True))
 
     @pytest.mark.unit
-    def test_symmetry_1(self):
-        """Test surface averages of a smooth function."""
+    def test_enforce_symmetry(self):
+        """Test correctness of enforce_symmetry() for uniformly spaced nodes.
+
+        Unlike enforce_symmetry(), the algorithm used in LinearGrid for
+        symmetry also works if the nodes are not uniformly spaced. This test
+        compares the two methods when the grid is uniformly spaced in theta,
+        as a means to ensure enforce_symmetry() is correct.
+        """
+        ntheta = 6
+        theta = np.linspace(0, 2 * np.pi, ntheta, endpoint=False)
+        lg_1 = LinearGrid(L=5, theta=theta, N=4, NFP=4, sym=True)
+        lg_2 = LinearGrid(L=5, theta=theta, N=4, NFP=4, sym=False)
+        # precondition for the following tests to work
+        np.testing.assert_allclose(lg_2.spacing[:, 1], 2 * np.pi / ntheta)
+
+        lg_2._sym = True
+        lg_2._enforce_symmetry()
+        np.testing.assert_allclose(lg_1.nodes, lg_2.nodes)
+        np.testing.assert_allclose(lg_1.spacing, lg_2.spacing)
+        lg_2._scale_weights()
+        np.testing.assert_allclose(lg_1.spacing, lg_2.spacing)
+        np.testing.assert_allclose(lg_1.weights, lg_2.weights)
+
+    @pytest.mark.unit
+    def test_symmetry_surface_average_1(self):
+        """Test surface average of a symmetric function."""
 
-        def test(grid, err_msg):
+        def test(grid):
+            r = grid.nodes[:, 0]
             t = grid.nodes[:, 1]
             z = grid.nodes[:, 2] * grid.NFP
-            true_avg = 5
+            true_surface_avg = 5
+            function_of_rho = 1 / (r + 0.35)
             f = (
-                true_avg
+                true_surface_avg
                 + np.cos(t)
                 - 0.5 * np.cos(z)
-                + 3 * np.cos(t) * np.cos(z)
+                + 3 * np.cos(t) * np.cos(z) ** 2
                 - 2 * np.sin(z) * np.sin(t)
+            ) * function_of_rho
+            np.testing.assert_allclose(
+                surface_averages(grid, f),
+                true_surface_avg * function_of_rho,
+                rtol=1e-15,
+                err_msg=type(grid),
             )
-            numerical_avg = surface_averages(grid, f)
-            np.testing.assert_allclose(numerical_avg, true_avg, err_msg=err_msg)
 
-        L, M, N, NFP, sym = 6, 6, 3, 5, True
-        test(LinearGrid(L, M, N, NFP, sym), "LinearGrid")
-        test(QuadratureGrid(L, M, N, NFP), "QuadratureGrid")
-        test(ConcentricGrid(L, M, N, NFP, sym), "ConcentricGrid")
-
-        L, M, N, NFP, sym = 3, 6, 3, 3, True
-        test(LinearGrid(L, M, N, NFP, sym), "LinearGrid")
-        test(QuadratureGrid(L, M, N, NFP), "QuadratureGrid")
-        test(ConcentricGrid(L, M, N, NFP, sym), "ConcentricGrid")
-
-        L, M, N, NFP, sym = 5, 5, 3, 5, False
-        test(LinearGrid(L, M, N, NFP, sym), "LinearGrid")
-        test(QuadratureGrid(L, M, N, NFP), "QuadratureGrid")
-        test(ConcentricGrid(L, M, N, NFP, sym), "ConcentricGrid")
-
-        L, M, N, NFP, sym = 3, 7, 3, 3, False
-        test(LinearGrid(L, M, N, NFP, sym), "LinearGrid")
-        test(QuadratureGrid(L, M, N, NFP), "QuadratureGrid")
-        test(ConcentricGrid(L, M, N, NFP, sym), "ConcentricGrid")
+        # these tests should be run on relatively low resolution grids,
+        # or at least low enough so that the asymmetric spacing test fails
+        L = [3, 3, 5, 3]
+        M = [3, 6, 5, 7]
+        N = [2, 2, 2, 2]
+        NFP = [5, 3, 5, 3]
+        sym = np.asarray([True, True, False, False])
+        # to test code not tested on grids made with M=.
+        even_number = 4
+        n_theta = even_number - sym
+
+        # asymmetric spacing
+        with pytest.raises(AssertionError):
+            theta = 2 * np.pi * np.asarray([t**2 for t in np.linspace(0, 1, max(M))])
+            test(LinearGrid(L=max(L), theta=theta, N=max(N), sym=False))
+
+        for i in range(len(L)):
+            test(LinearGrid(L=L[i], M=M[i], N=N[i], NFP=NFP[i], sym=sym[i]))
+            test(LinearGrid(L=L[i], theta=n_theta[i], N=N[i], NFP=NFP[i], sym=sym[i]))
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, 2 * np.pi, n_theta[i]),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, 2 * np.pi, n_theta[i] + 1),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
+            test(QuadratureGrid(L=L[i], M=M[i], N=N[i], NFP=NFP[i]))
+            test(ConcentricGrid(L=L[i], M=M[i], N=N[i], NFP=NFP[i], sym=sym[i]))
+            # nonuniform spacing when sym is False, but spacing is still symmetric
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, np.pi, n_theta[i]),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, np.pi, n_theta[i] + 1),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
 
     @pytest.mark.unit
-    def test_symmetry_2(self):
+    def test_symmetry_surface_average_2(self):
         """Tests that surface averages are correct using specified basis."""
 
-        def test(grid, basis, err_msg, true_avg=1):
+        def test(grid, basis, true_avg=1):
             transform = Transform(grid, basis)
 
             # random data with specified average on each surface
             coeffs = np.random.rand(basis.num_modes)
             coeffs[np.where((basis.modes[:, 1:] == [0, 0]).all(axis=1))[0]] = 0
             coeffs[np.where((basis.modes == [0, 0, 0]).all(axis=1))[0]] = true_avg
 
             # compute average for each surface in grid
             values = transform.transform(coeffs)
             numerical_avg = compress(grid, surface_averages(grid, values))
             if isinstance(grid, ConcentricGrid):
                 # values closest to axis are never accurate enough
                 numerical_avg = numerical_avg[1:]
-            np.testing.assert_allclose(numerical_avg, true_avg, err_msg=err_msg)
+            np.testing.assert_allclose(
+                numerical_avg,
+                true_avg,
+                err_msg=str(type(grid)) + " " + str(grid.sym),
+            )
 
         M = 10
         M_grid = 23
         test(
             QuadratureGrid(L=M_grid, M=M_grid, N=0),
             FourierZernikeBasis(L=M, M=M, N=0),
-            "QuadratureGrid",
         )
         test(
             LinearGrid(L=M_grid, M=M_grid, N=0, sym=True),
             FourierZernikeBasis(L=M, M=M, N=0, sym="cos"),
-            "LinearGrid with symmetry",
         )
         test(
             ConcentricGrid(L=M_grid, M=M_grid, N=0),
             FourierZernikeBasis(L=M, M=M, N=0),
-            "ConcentricGrid without symmetry",
         )
         test(
             ConcentricGrid(L=M_grid, M=M_grid, N=0, sym=True),
             FourierZernikeBasis(L=M, M=M, N=0, sym="cos"),
-            "ConcentricGrid with symmetry",
         )
+
+    @pytest.mark.unit
+    def test_symmetry_volume_integral(self):
+        """Test volume integral of a symmetric function."""
+        # Currently, midpoint rule is false for LinearGrid made with L=number.
+        def test(grid, midpoint_rule=False):
+            r = grid.nodes[:, 0]
+            t = grid.nodes[:, 1]
+            z = grid.nodes[:, 2] * grid.NFP
+            true_surface_avg = 5
+            function_of_rho = 1 / (r + 0.35)
+            f = (
+                true_surface_avg
+                + np.cos(t)
+                - 0.5 * np.cos(z)
+                + 3 * np.cos(t) * np.cos(z) ** 2
+                - 2 * np.sin(z) * np.sin(t)
+            ) * function_of_rho
+
+            if midpoint_rule:
+                r_unique = r[grid.unique_rho_idx]
+                dr = np.empty_like(r_unique)
+                dr[0] = (r_unique[0] + r_unique[1]) / 2
+                dr[1:-1] = (r_unique[2:] - r_unique[:-2]) / 2
+                dr[-1] = 1 - (r_unique[-2] + r_unique[-1]) / 2
+            else:
+                dr = 1 / grid.num_rho
+            expected_integral = np.sum(dr * compress(grid, function_of_rho))
+            true_integral = np.log(1.35 / 0.35)
+            midpoint_rule_error_bound = np.max(dr) ** 2 / 24 * (2 / 0.35**3)
+            right_riemann_error_bound = dr * (1 / 0.35 - 1 / 1.35)
+            np.testing.assert_allclose(
+                expected_integral,
+                true_integral,
+                rtol=0,
+                atol=midpoint_rule_error_bound / 4
+                if midpoint_rule
+                else right_riemann_error_bound / 3,
+                err_msg=type(grid),
+            )
+            np.testing.assert_allclose(
+                np.sum(grid.weights * f) / (4 * np.pi**2 * true_surface_avg),
+                expected_integral,
+                rtol=1e-15,
+                err_msg=type(grid),
+            )
+
+        L = [3, 3, 5, 3]
+        M = [3, 6, 5, 7]
+        N = [2, 2, 2, 2]
+        NFP = [5, 3, 5, 3]
+        sym = np.asarray([True, True, False, False])
+        # to test code not tested on grids made with M=.
+        even_number = 4
+        n_theta = even_number - sym
+
+        for i in range(len(L)):
+            test(LinearGrid(L=L[i], M=M[i], N=N[i], NFP=NFP[i], sym=sym[i]))
+            test(LinearGrid(L=L[i], theta=n_theta[i], N=N[i], NFP=NFP[i], sym=sym[i]))
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, 2 * np.pi, n_theta[i], endpoint=False),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, 2 * np.pi, n_theta[i] + 1, endpoint=False),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
+            test(
+                ConcentricGrid(L=L[i], M=M[i], N=N[i], NFP=NFP[i], sym=sym[i]),
+                midpoint_rule=True,
+            )
+            # nonuniform spacing when sym is False, but spacing is still symmetric
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, np.pi, n_theta[i]),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
+            test(
+                LinearGrid(
+                    L=L[i],
+                    theta=np.linspace(0, np.pi, n_theta[i] + 1),
+                    N=N[i],
+                    NFP=NFP[i],
+                    sym=sym[i],
+                )
+            )
```

### Comparing `desc-opt-0.8.1/tests/test_input_output.py` & `desc-opt-0.8.2/tests/test_input_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,18 +45,17 @@
     with open(correct_file_path) as f:
         lines_correct = f.readlines()
     with open(path) as f:
         lines_direct = f.readlines()
     with open(path_converted_file) as f:
         lines_converted = f.readlines()
     # skip first 3 lines as they have date and pwd info
-    for line1, line2 in zip(lines_correct[3:], lines_converted[3:]):
+    for line1, line2 in zip(lines_correct[3:], lines_converted[4:]):
         assert line1.strip() == line2.strip()
-    # skip first 4 here as the directly written file lacks a header
-    for line1, line2 in zip(lines_correct[4:], lines_direct):
+    for line1, line2 in zip(lines_correct[3:], lines_direct):
         assert line1.strip() == line2.strip()
 
 
 @pytest.mark.unit
 def test_write_desc_input_Nones(tmpdir_factory):
     """Test converting writing DESC input file when an input tol is None."""
     # tests how None is handled as a passed-in input to the input writer
@@ -84,15 +83,15 @@
     path = tmpdir.join("desc_with_None")
     ir.write_desc_input(path, ir.inputs)
     ir2 = InputReader(cl_args=[str(path)])
     correct_ftols = [1e-2, 1e-3, 1e-3]
     for i, inp in enumerate(ir2.inputs):
         assert inp["ftol"] == correct_ftols[i]
 
-    # now check that the written line is the
+    # now check that the written line is
     # the correct "ftol = 1e-2, 1e-3"
     # and that gtol is NOT written anywhere,
     # since only None was passed in for that input
     no_gtol = True
     with open(path) as f:
         lines = f.readlines()
     for line in lines:
@@ -166,15 +165,15 @@
         assert ir.args.verbose == 1, "verbose is not default 1"
         assert ir.args.numpy is False, "numpy is not default False"
         assert (
             os.environ["DESC_BACKEND"] == "jax"
         ), "numpy environment variable incorrect with default argument"
         assert ir.args.version is False, "version is not default False"
         assert (
-            len(ir.inputs[0]) == 28
+            len(ir.inputs[0]) == 27
         ), "number of inputs does not match number expected in MIN_INPUT"
         # test equality of arguments
 
     @pytest.mark.unit
     def test_np_environ(self):
         """Test setting numpy backend via environment variable."""
         argv = self.argv2 + ["--numpy"]
```

### Comparing `desc-opt-0.8.1/tests/test_interpolate.py` & `desc-opt-0.8.2/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_linear_objectives.py` & `desc-opt-0.8.2/tests/test_linear_objectives.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Tests for linear constraints and objectives."""
-import jax.numpy as jnp
 import numpy as np
 import pytest
 import scipy.linalg
 
 import desc.examples
 from desc.compute import arg_order
 from desc.equilibrium import Equilibrium
 from desc.geometry import FourierRZToroidalSurface
 from desc.grid import LinearGrid
 from desc.objectives import (
     AspectRatio,
+    BoundaryRSelfConsistency,
+    BoundaryZSelfConsistency,
     FixAtomicNumber,
     FixAxisR,
     FixAxisZ,
     FixBoundaryR,
     FixBoundaryZ,
     FixCurrent,
     FixElectronDensity,
@@ -106,15 +107,15 @@
     np.testing.assert_allclose(surf.Z_lmn, surf5.Z_lmn, atol=1e-12)
 
 
 @pytest.mark.unit
 def test_constrain_bdry_with_only_one_mode():
     """Test Fixing boundary with a surface with only one mode in its basis."""
     eq = Equilibrium()
-    FixZ = FixBoundaryZ(fixed_boundary=True)
+    FixZ = BoundaryZSelfConsistency()
     try:
         FixZ.build(eq)
     except Exception:
         pytest.fail(
             "Error encountered when attempting to constrain surface with"
             + " only one mode in its basis"
         )
@@ -130,28 +131,18 @@
         eqi.solve(constraints=FixCurrent())
     # nonexistent rotational transform can't be constrained
     with pytest.raises(RuntimeError):
         eqc.solve(constraints=FixIota())
     # toroidal current and rotational transform can't be constrained simultaneously
     with pytest.raises(ValueError):
         eqi.solve(constraints=(FixCurrent(), FixIota()))
-    with pytest.raises(ValueError):
+    with pytest.raises(AssertionError):
         eqi.solve(constraints=(FixPressure(target=2), FixPressure(target=1)))
-    # cannot use two constraints on the same R mode
-    with pytest.raises(RuntimeError):
-        fixmode1 = FixModeR(modes=np.array([1, 1, 0]))
-        fixmode2 = FixModeR(modes=np.array([[0, 0, 0], [1, 1, 0]]))
-        eqc.solve(constraints=(fixmode1, fixmode2))
-    # cannot use two constraints on the same Z mode
-    with pytest.raises(RuntimeError):
-        fixmode1 = FixModeZ(modes=np.array([1, -1, 0]))
-        fixmode2 = FixModeZ(modes=np.array([1, -1, 0]))
-        eqc.solve(constraints=(fixmode1, fixmode2))
     # cannot use two incompatible constraints
-    with pytest.raises(ValueError):
+    with pytest.raises(AssertionError):
         con1 = FixCurrent(target=eqc.c_l)
         con2 = FixCurrent(target=eqc.c_l + 1)
         eqc.solve(constraints=(con1, con2))
 
 
 @pytest.mark.regression
 @pytest.mark.solve
@@ -174,16 +165,16 @@
     orig_Z_val = eq.Z_lmn[eq.Z_basis.get_idx(L=L, M=-M, N=0)]
 
     constraints = (
         FixLambdaGauge(),
         FixPressure(),
         FixIota(),
         FixPsi(),
-        FixBoundaryR(fixed_boundary=True),
-        FixBoundaryZ(fixed_boundary=True),
+        FixBoundaryR(),
+        FixBoundaryZ(),
         fixR,
         fixZ,
     )
 
     eq.solve(
         verbose=3,
         ftol=1e-2,
@@ -228,16 +219,16 @@
     )
 
     constraints = (
         FixLambdaGauge(),
         FixPressure(),
         FixIota(),
         FixPsi(),
-        FixBoundaryR(fixed_boundary=True),
-        FixBoundaryZ(fixed_boundary=True),
+        FixBoundaryR(),
+        FixBoundaryZ(),
         fixR,
         fixZ,
     )
 
     eq.solve(
         verbose=3,
         ftol=1e-2,
@@ -302,80 +293,56 @@
     for con in constraints:
         con.build(eq, verbose=0)
     constraints[3].bounds = (0, 1)  # bounds on FixPsi
 
     from desc.objectives.utils import factorize_linear_constraints
 
     with pytest.raises(ValueError):
-        xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+        xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
             constraints, arg_order
         )
 
 
 @pytest.mark.unit
 def test_build_init():
     """Ensure that passing an equilibrium to init builds the objective correctly.
 
     Related to gh issue #378
     """
     eq = Equilibrium(M=3, N=1)
 
     # initialize the constraints without building
-    fbR1 = FixBoundaryR(fixed_boundary=False)
-    fbZ1 = FixBoundaryZ(fixed_boundary=False)
-    fbR2 = FixBoundaryR(fixed_boundary=True)
-    fbZ2 = FixBoundaryZ(fixed_boundary=True)
-    for obj in (fbR1, fbR2, fbZ1, fbZ2):
+    fbR1 = FixBoundaryR()
+    fbZ1 = FixBoundaryZ()
+    for obj in (fbR1, fbZ1):
         obj.build(eq)
 
     arg = fbR1.args[0]
     A = fbR1.derivatives["jac"][arg](np.zeros(fbR1.dimensions[arg]))
     assert np.max(np.abs(A)) == 1
     assert A.shape == (eq.surface.R_basis.num_modes, eq.surface.R_basis.num_modes)
 
-    arg = fbR2.args[0]
-    A = fbR2.derivatives["jac"][arg](np.zeros(fbR2.dimensions[arg]))
-    assert np.max(np.abs(A)) == 1
-    assert A.shape == (eq.surface.R_basis.num_modes, eq.R_basis.num_modes)
-
     arg = fbZ1.args[0]
     A = fbZ1.derivatives["jac"][arg](np.zeros(fbZ1.dimensions[arg]))
     assert np.max(np.abs(A)) == 1
     assert A.shape == (eq.surface.Z_basis.num_modes, eq.surface.Z_basis.num_modes)
 
-    arg = fbZ2.args[0]
-    A = fbZ2.derivatives["jac"][arg](np.zeros(fbZ2.dimensions[arg]))
-    assert np.max(np.abs(A)) == 1
-    assert A.shape == (eq.surface.Z_basis.num_modes, eq.Z_basis.num_modes)
-
-    fbR1 = FixBoundaryR(fixed_boundary=False, eq=eq)
-    fbZ1 = FixBoundaryZ(fixed_boundary=False, eq=eq)
-    fbR2 = FixBoundaryR(fixed_boundary=True, eq=eq)
-    fbZ2 = FixBoundaryZ(fixed_boundary=True, eq=eq)
+    fbR1 = FixBoundaryR(eq=eq)
+    fbZ1 = FixBoundaryZ(eq=eq)
 
     arg = fbR1.args[0]
     A = fbR1.derivatives["jac"][arg](np.zeros(fbR1.dimensions[arg]))
     assert np.max(np.abs(A)) == 1
     assert A.shape == (eq.surface.R_basis.num_modes, eq.surface.R_basis.num_modes)
 
-    arg = fbR2.args[0]
-    A = fbR2.derivatives["jac"][arg](np.zeros(fbR2.dimensions[arg]))
-    assert np.max(np.abs(A)) == 1
-    assert A.shape == (eq.surface.R_basis.num_modes, eq.R_basis.num_modes)
-
     arg = fbZ1.args[0]
     A = fbZ1.derivatives["jac"][arg](np.zeros(fbZ1.dimensions[arg]))
     assert np.max(np.abs(A)) == 1
     assert A.shape == (eq.surface.Z_basis.num_modes, eq.surface.Z_basis.num_modes)
 
-    arg = fbZ2.args[0]
-    A = fbZ2.derivatives["jac"][arg](np.zeros(fbZ2.dimensions[arg]))
-    assert np.max(np.abs(A)) == 1
-    assert A.shape == (eq.surface.Z_basis.num_modes, eq.Z_basis.num_modes)
-
 
 @pytest.mark.unit
 def test_kinetic_constraints():
     """Make sure errors are raised when trying to constrain nonexistent profiles."""
     eqp = Equilibrium(L=3, M=3, N=3, pressure=np.array([1, 0, -1]))
     eqk = Equilibrium(
         L=3,
@@ -425,43 +392,39 @@
             ],
         )
     )
     Z_modes = eq.surface.Z_basis.modes[
         np.max(np.abs(eq.surface.Z_basis.modes), 1) > n + 1, :
     ]
     constraints = (
-        FixBoundaryR(modes=R_modes, fixed_boundary=True, normalize=False),
-        FixBoundaryZ(modes=Z_modes, fixed_boundary=True, normalize=False),
+        FixBoundaryR(modes=R_modes, normalize=False),
+        FixBoundaryZ(modes=Z_modes, normalize=False),
+        BoundaryRSelfConsistency(),
+        BoundaryZSelfConsistency(),
     )
     for con in constraints:
         con.build(eq, verbose=0)
     objective.build(eq)
+    objective.set_args("Rb_lmn", "Zb_lmn")
     from desc.objectives.utils import factorize_linear_constraints
 
-    xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+    xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints,
         objective.args,
     )
 
-    from scipy.linalg import block_diag
-
-    from desc.compute import arg_order
-
-    A_full = block_diag(*[A[arg] for arg in arg_order if arg in A.keys()])
-    b_full = jnp.concatenate([b[arg] for arg in arg_order if arg in b.keys()])
-
     x1 = objective.x(eq)
     x2 = recover(project(x1))
 
     atol = 2e-15
     assert np.isclose(np.max(np.abs(x1 - x2)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ xp - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x1 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x2 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ Z)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ xp[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x1[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x2[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ Z)), 0, atol=atol)
 
 
 @pytest.mark.unit
 def test_correct_indexing_passed_modes_and_passed_target():
     """Test Indexing when passing in specified modes, related to gh issue #380."""
     n = 1
 
@@ -495,47 +458,39 @@
         np.max(np.abs(eq.surface.Z_basis.modes), 1) > n + 1, :
     ]
     idxs = []
     for mode in Z_modes:
         idxs.append(eq.surface.Z_basis.get_idx(*mode))
     target_Z = eq.surface.Z_lmn[idxs]
     constraints = (
-        FixBoundaryR(
-            modes=R_modes, fixed_boundary=True, normalize=False, target=target_R
-        ),
-        FixBoundaryZ(
-            modes=Z_modes, fixed_boundary=True, normalize=False, target=target_Z
-        ),
+        FixBoundaryR(modes=R_modes, normalize=False, target=target_R),
+        FixBoundaryZ(modes=Z_modes, normalize=False, target=target_Z),
+        BoundaryRSelfConsistency(),
+        BoundaryZSelfConsistency(),
     )
     for con in constraints:
         con.build(eq, verbose=0)
     objective.build(eq)
+    objective.set_args("Rb_lmn", "Zb_lmn")
     from desc.objectives.utils import factorize_linear_constraints
 
-    xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+    xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints,
         objective.args,
     )
 
-    from scipy.linalg import block_diag
-
-    from desc.compute import arg_order
-
-    A_full = block_diag(*[A[arg] for arg in arg_order if arg in A.keys()])
-    b_full = jnp.concatenate([b[arg] for arg in arg_order if arg in b.keys()])
-
     x1 = objective.x(eq)
     x2 = recover(project(x1))
 
     atol = 2e-15
     assert np.isclose(np.max(np.abs(x1 - x2)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ xp - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x1 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x2 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ Z)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ xp[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x1[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x2[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ Z)), 0, atol=atol)
 
 
 @pytest.mark.unit
 def test_correct_indexing_passed_modes_axis():
     """Test Indexing when passing in specified axis modes, related to gh issue #380."""
     n = 1
 
@@ -576,35 +531,28 @@
         FixSumModesZ(modes=np.array([[3, 3, -3], [4, 4, -4]]), normalize=False),
     )
     for con in constraints:
         con.build(eq, verbose=0)
     objective.build(eq)
     from desc.objectives.utils import factorize_linear_constraints
 
-    xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+    xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints,
         objective.args,
     )
 
-    from scipy.linalg import block_diag
-
-    from desc.compute import arg_order
-
-    A_full = block_diag(*[A[arg] for arg in arg_order if arg in A.keys()])
-    b_full = jnp.concatenate([b[arg] for arg in arg_order if arg in b.keys()])
-
     x1 = objective.x(eq)
     x2 = recover(project(x1))
 
     atol = 2e-15
     assert np.isclose(np.max(np.abs(x1 - x2)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ xp - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x1 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x2 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ Z)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ xp[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x1[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x2[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ Z)), 0, atol=atol)
 
 
 @pytest.mark.unit
 def test_correct_indexing_passed_modes_and_passed_target_axis():
     """Test Indexing when passing in specified axis modes, related to gh issue #380."""
     n = 1
 
@@ -685,66 +633,59 @@
         ),
     )
     for con in constraints:
         con.build(eq, verbose=0)
     objective.build(eq)
     from desc.objectives.utils import factorize_linear_constraints
 
-    xp, A, Ainv, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
+    xp, A, b, Z, unfixed_idx, project, recover = factorize_linear_constraints(
         constraints,
         objective.args,
     )
 
-    from scipy.linalg import block_diag
-
-    from desc.compute import arg_order
-
-    A_full = block_diag(*[A[arg] for arg in arg_order if arg in A.keys()])
-    b_full = jnp.concatenate([b[arg] for arg in arg_order if arg in b.keys()])
-
     x1 = objective.x(eq)
     x2 = recover(project(x1))
 
     atol = 2e-15
     assert np.isclose(np.max(np.abs(x1 - x2)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ xp - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x1 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ x2 - b_full)), 0, atol=atol)
-    assert np.isclose(np.max(np.abs(A_full @ Z)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ xp[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x1[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ x2[unfixed_idx] - b)), 0, atol=atol)
+    assert np.isclose(np.max(np.abs(A @ Z)), 0, atol=atol)
 
 
 @pytest.mark.unit
 def test_FixBoundary_with_single_weight():
     """Test Fixing boundary with only a single, passed weight."""
     eq = Equilibrium()
     w = 1.1
-    FixZ = FixBoundaryZ(modes=np.array([[0, -1, 0]]), fixed_boundary=True, weight=w)
+    FixZ = FixBoundaryZ(modes=np.array([[0, -1, 0]]), weight=w)
     FixZ.build(eq)
     np.testing.assert_array_equal(FixZ.weight.size, 1)
     np.testing.assert_array_equal(FixZ.weight, w)
-    FixR = FixBoundaryR(modes=np.array([[0, 1, 0]]), fixed_boundary=True, weight=w)
+    FixR = FixBoundaryR(modes=np.array([[0, 1, 0]]), weight=w)
     FixR.build(eq)
     np.testing.assert_array_equal(FixR.weight.size, 1)
     np.testing.assert_array_equal(FixR.weight, w)
 
 
 @pytest.mark.unit
 def test_FixBoundary_passed_target_no_passed_modes_error():
     """Test Fixing boundary with no passed-in modes."""
     eq = Equilibrium()
-    FixZ = FixBoundaryZ(modes=True, fixed_boundary=True, target=np.array([[0]]))
+    FixZ = FixBoundaryZ(modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
         FixZ.build(eq)
-    FixZ = FixBoundaryZ(modes=False, fixed_boundary=False, target=np.array([[0]]))
+    FixZ = FixBoundaryZ(modes=False, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
         FixZ.build(eq)
-    FixR = FixBoundaryR(modes=True, fixed_boundary=False, target=np.array([[0]]))
+    FixR = FixBoundaryR(modes=True, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
         FixR.build(eq)
-    FixR = FixBoundaryR(modes=False, fixed_boundary=True, target=np.array([[0]]))
+    FixR = FixBoundaryR(modes=False, target=np.array([[0]]))
     with pytest.raises(RuntimeError):
         FixR.build(eq)
 
 
 @pytest.mark.unit
 def test_FixAxis_passed_target_no_passed_modes_error():
     """Test Fixing Axis with no passed-in modes."""
```

### Comparing `desc-opt-0.8.1/tests/test_magnetic_fields.py` & `desc-opt-0.8.2/tests/test_magnetic_fields.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_objective_funs.py` & `desc-opt-0.8.2/tests/test_objective_funs.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 from desc.examples import get
 from desc.geometry import FourierRZToroidalSurface
 from desc.grid import LinearGrid
 from desc.objectives import (
     AspectRatio,
     Elongation,
     Energy,
+    ForceBalance,
     GenericObjective,
+    Isodynamicity,
     MagneticWell,
     MeanCurvature,
     MercierStability,
     ObjectiveFunction,
     PlasmaVesselDistance,
     PrincipalCurvature,
     QuasisymmetryBoozer,
@@ -53,15 +55,16 @@
                 "L_lmn": eq.L_lmn,
                 "i_l": eq.i_l,
                 "c_l": eq.c_l,
                 "Psi": eq.Psi,
             }
             np.testing.assert_allclose(
                 obj.compute(**kwargs),
-                eq.compute(f, grid=obj.grid)[f] * obj.grid.weights,
+                eq.compute(f, grid=obj._transforms["grid"])[f]
+                * obj._transforms["grid"].weights,
             )
 
         test("sqrt(g)", Equilibrium())
         test("current", Equilibrium(iota=PowerSeriesProfile(0)))
         test("iota", Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
@@ -227,14 +230,26 @@
             ft = obj.compute(*obj.xs(eq))
             np.testing.assert_allclose(ft, 0)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
+    def test_isodynamicity(self):
+        """Test calculation of isodynamicity metric."""
+
+        def test(eq):
+            obj = Isodynamicity(eq=eq)
+            iso = obj.compute(*obj.xs(eq))
+            np.testing.assert_allclose(iso, 0, atol=1e-14)
+
+        test(Equilibrium(iota=PowerSeriesProfile(0)))
+        test(Equilibrium(current=PowerSeriesProfile(0)))
+
+    @pytest.mark.unit
     def test_qs_boozer_grids(self):
         """Test grid compatability with QS objectives."""
         eq = get("QAS")
 
         # symmetric grid
         grid = LinearGrid(M=eq.M, N=eq.N, NFP=eq.NFP, sym=True)
         with pytest.raises(AssertionError):
@@ -248,28 +263,28 @@
     @pytest.mark.unit
     def test_mercier_stability(self):
         """Test calculation of mercier stability criteria."""
 
         def test(eq):
             obj = MercierStability(eq=eq)
             DMerc = obj.compute(*obj.xs(eq))
-            np.testing.assert_equal(len(DMerc), obj.grid.num_rho)
+            np.testing.assert_equal(len(DMerc), obj._transforms["grid"].num_rho)
             np.testing.assert_allclose(DMerc, 0)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
     @pytest.mark.unit
     def test_magnetic_well(self):
         """Test calculation of magnetic well stability criteria."""
 
         def test(eq):
             obj = MagneticWell(eq=eq)
             magnetic_well = obj.compute(*obj.xs(eq))
-            np.testing.assert_equal(len(magnetic_well), obj.grid.num_rho)
+            np.testing.assert_equal(len(magnetic_well), obj._transforms["grid"].num_rho)
             np.testing.assert_allclose(magnetic_well, 0, atol=1e-15)
 
         test(Equilibrium(iota=PowerSeriesProfile(0)))
         test(Equilibrium(current=PowerSeriesProfile(0)))
 
 
 @pytest.mark.unit
@@ -392,20 +407,24 @@
     iota = PowerSeriesProfile([1, 0, -0.3])
     current = PowerSeriesProfile([4, 0, 1, 0, -1])
     eqi = Equilibrium(L=5, N=3, M=3, iota=iota)
     eqc = Equilibrium(L=3, N=3, M=3, current=current)
     obji = RotationalTransform(target=iota)
     obji.build(eqc)
     np.testing.assert_allclose(
-        obji.target, iota(obji.grid.nodes[obji.grid.unique_rho_idx])
+        obji.target,
+        iota(obji._transforms["grid"].nodes[obji._transforms["grid"].unique_rho_idx]),
     )
     objc = ToroidalCurrent(target=current)
     objc.build(eqi)
     np.testing.assert_allclose(
-        objc.target, current(objc.grid.nodes[objc.grid.unique_rho_idx])
+        objc.target,
+        current(
+            objc._transforms["grid"].nodes[objc._transforms["grid"].unique_rho_idx]
+        ),
     )
 
 
 @pytest.mark.unit
 def test_plasma_vessel_distance():
     """Test calculation of min distance from plasma to vessel."""
     R0 = 10.0
@@ -530,7 +549,31 @@
 
     iota = eq.compute("iota", grid=grid)["iota"]
     obj = RotationalTransform(eq=eq, grid=grid)
     test(obj, iota)
     curr = eq.compute("current", grid=grid)["current"]
     obj = ToroidalCurrent(eq=eq, grid=grid)
     test(obj, curr, normalize=True)
+
+
+@pytest.mark.unit
+def test_rebuild():
+    """Test that the objective is rebuilt correctly when needed."""
+    eq = Equilibrium(L=3, M=3)
+    f_obj = ForceBalance()
+    obj = ObjectiveFunction(f_obj)
+    eq.solve(maxiter=2, objective=obj)
+
+    # this would fail before v0.8.2 when trying to get objective.x
+    eq.change_resolution(L=5, M=5)
+    obj.build(eq)
+    eq.solve(maxiter=2, objective=obj)
+
+    eq = Equilibrium(L=3, M=3)
+    f_obj = ForceBalance()
+    obj = ObjectiveFunction(f_obj)
+    eq.solve(maxiter=2, objective=obj)
+    eq.change_resolution(L=5, M=5)
+    # this would fail at objective.compile
+    obj = ObjectiveFunction(f_obj)
+    obj.build(eq)
+    eq.solve(maxiter=2, objective=obj)
```

### Comparing `desc-opt-0.8.1/tests/test_optimizer.py` & `desc-opt-0.8.2/tests/test_optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -271,14 +271,15 @@
         name = "Dummy"
         _print_value_fmt = "Dummy: {:.3e}"
         _units = "(Foo)"
 
         def build(self, eq, *args, **kwargs):
 
             # objective = just shift x by a lil bit
+            self._args = ["R_lmn", "Z_lmn", "L_lmn", "p_l", "i_l", "c_l", "Psi"]
             self._x0 = (
                 np.concatenate(
                     [
                         eq.R_lmn,
                         eq.Z_lmn,
                         eq.L_lmn,
                         eq.p_l,
@@ -291,18 +292,17 @@
             )
             self._dim_f = self._x0.size
             self._check_dimensions()
             self._set_dimensions(eq)
             self._set_derivatives()
             self._built = True
 
-        def compute(self, R_lmn, Z_lmn, L_lmn, p_l, i_l, c_l, Psi):
-            x = jnp.concatenate(
-                [R_lmn, Z_lmn, L_lmn, p_l, i_l, c_l, jnp.atleast_1d(Psi)]
-            )
+        def compute(self, *args, **kwargs):
+            params = self._parse_args(*args, **kwargs)
+            x = jnp.concatenate([jnp.atleast_1d(params[arg]) for arg in self.args])
             return x - self._x0
 
     np.random.seed(0)
     objective = ObjectiveFunction(DummyObjective(), use_jit=False)
     # make gradient super noisy so it stalls
     objective.jac = lambda x: objective._jac(x) + 1e2 * (
         np.random.random((objective._dim_f, x.size)) - 0.5
@@ -358,16 +358,16 @@
 
 @pytest.mark.unit
 @pytest.mark.slow
 def test_maxiter_1_and_0_solve():
     """Test that solves with maxiter 1 and 0 terminate correctly."""
     # correctly meaning they terminate, instead of looping infinitely
     constraints = (
-        FixBoundaryR(fixed_boundary=True),
-        FixBoundaryZ(fixed_boundary=True),
+        FixBoundaryR(),
+        FixBoundaryZ(),
         FixPressure(),
         FixIota(),
         FixPsi(),
     )
     objectives = ForceBalance()
     obj = ObjectiveFunction(objectives)
     eq = desc.examples.get("SOLOVEV")
@@ -384,16 +384,16 @@
 
 
 @pytest.mark.unit
 @pytest.mark.slow
 def test_scipy_fail_message():
     """Test that scipy fail message does not cause an error (see PR #434)."""
     constraints = (
-        FixBoundaryR(fixed_boundary=True),
-        FixBoundaryZ(fixed_boundary=True),
+        FixBoundaryR(),
+        FixBoundaryZ(),
         FixPressure(),
         FixCurrent(),
         FixPsi(),
     )
     objectives = ForceBalance()
     obj = ObjectiveFunction(objectives)
     eq = Equilibrium()
@@ -431,32 +431,32 @@
 
 
 @pytest.mark.unit
 def test_wrappers():
     """Tests for using wrapped objectives."""
     eq = desc.examples.get("SOLOVEV")
     con = (
-        FixBoundaryR(fixed_boundary=True),
-        FixBoundaryZ(fixed_boundary=True),
+        FixBoundaryR(),
+        FixBoundaryZ(),
         FixIota(),
         FixPressure(),
         FixPsi(),
     )
     con_nl = (ForceBalance(),)
     obj = ForceBalance()
     with pytest.raises(AssertionError):
         _ = LinearConstraintProjection(obj, con)
     with pytest.raises(ValueError):
         _ = LinearConstraintProjection(ObjectiveFunction(obj), con + con_nl)
     ob = LinearConstraintProjection(ObjectiveFunction(obj), con, eq=eq)
     assert ob.built
 
     con = (
-        FixBoundaryR(fixed_boundary=True),
-        FixBoundaryZ(fixed_boundary=True),
+        FixBoundaryR(),
+        FixBoundaryZ(),
         FixIota(),
         FixPressure(),
         FixPsi(),
     )
     con_nl = (ForceBalance(),)
     obj = ForceBalance()
     with pytest.raises(AssertionError):
@@ -477,16 +477,16 @@
     """Just tests that the optimizers run without error, eg tests for the wrappers."""
     eq = desc.examples.get("SOLOVEV")
     fobj = ObjectiveFunction(ForceBalance())
     eobj = ObjectiveFunction(Energy())
     fobj.build(eq)
     eobj.build(eq)
     constraints = (
-        FixBoundaryR(fixed_boundary=True),
-        FixBoundaryZ(fixed_boundary=True),
+        FixBoundaryR(),
+        FixBoundaryZ(),
         FixIota(),
         FixPressure(),
         FixPsi(),
     )
 
     for opt in optimizers:
         print("TESTING ", opt)
```

### Comparing `desc-opt-0.8.1/tests/test_perturbations.py` & `desc-opt-0.8.2/tests/test_perturbations.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_plotting.py` & `desc-opt-0.8.2/tests/test_plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Regression tests for plotting functions, by comparing to saved baseline images."""
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pytest
+from scipy.interpolate import interp1d
 
 from desc.basis import (
     DoubleFourierSeries,
     FourierSeries,
     FourierZernikeBasis,
     PowerSeries,
 )
 from desc.coils import CoilSet, FourierXYZCoil
 from desc.equilibrium import EquilibriaFamily, Equilibrium
 from desc.examples import get
-from desc.grid import ConcentricGrid, LinearGrid, QuadratureGrid
+from desc.grid import ConcentricGrid, Grid, LinearGrid, QuadratureGrid
 from desc.plotting import (
     _find_idx,
     plot_1d,
     plot_2d,
     plot_3d,
     plot_basis,
     plot_boozer_modes,
@@ -279,15 +281,15 @@
 
 @pytest.mark.unit
 @pytest.mark.solve
 @pytest.mark.mpl_image_compare(remove_text=True, tolerance=tol_1d)
 def test_fsa_F_normalized(DSHAPE_current):
     """Test plotting flux surface average normalized force error on log scale."""
     eq = EquilibriaFamily.load(load_from=str(DSHAPE_current["desc_h5_path"]))[-1]
-    fig, ax = plot_fsa(eq, "|F|", log=True, norm_F=True)
+    fig, ax = plot_fsa(eq, "|F|", log=True, norm_F=True, norm_name="<|grad(p)|>_vol")
     ax.set_ylim([1e-5, 1e-2])
     return fig
 
 
 @pytest.mark.unit
 @pytest.mark.solve
 @pytest.mark.mpl_image_compare(remove_text=True, tolerance=tol_2d)
@@ -759,7 +761,51 @@
             return [coilset]
 
     coil_list = flatten_coils(coils2)
     for string in ["X", "Y", "Z"]:
         assert string in data.keys()
         assert len(data[string]) == len(coil_list)
     return fig
+
+
+@pytest.mark.unit
+@pytest.mark.mpl_image_compare(remove_text=True, tolerance=tol_1d)
+def test_plot_b_mag():
+    """Test plot of |B| on longer field lines for gyrokinetic simulations."""
+    psi = 0.5
+    npol = 2
+    nzgrid = 128
+    alpha = 0
+    # compute and fit iota profile
+    eq = get("W7-X")
+    data = eq.compute("iota")
+    fi = interp1d(data["rho"], data["iota"])
+
+    # get flux tube coordinate system
+    rho = np.sqrt(psi)
+    iota = fi(rho)
+    zeta = np.linspace(
+        -np.pi * npol / np.abs(iota), np.pi * npol / np.abs(iota), 2 * nzgrid + 1
+    )
+    thetas = alpha * np.ones_like(zeta) + iota * zeta
+
+    rhoa = rho * np.ones_like(zeta)
+    c = np.vstack([rhoa, thetas, zeta]).T
+    coords = eq.compute_theta_coords(c)
+    grid = Grid(coords)
+
+    # compute |B| normalized in the usual flux tube way
+    psib = np.abs(eq.compute("psi")["psi"][-1])
+    Lref = eq.compute("a")["a"]
+    Bref = 2 * psib / Lref**2
+    bmag = eq.compute("|B|", grid=grid)["|B|"] / Bref
+    fig, ax = plt.subplots()
+    ax.plot(bmag)
+    return fig
+
+
+@pytest.mark.unit
+@pytest.mark.mpl_image_compare(remove_text=True, tolerance=tol_2d)
+def test_plot_surfaces_HELIOTRON():
+    """Test plot surfaces of equilibrium for correctness of vartheta lines."""
+    fig, ax = plot_surfaces(get("HELIOTRON"))
+    return fig
```

### Comparing `desc-opt-0.8.1/tests/test_profiles.py` & `desc-opt-0.8.2/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_stability_funs.py` & `desc-opt-0.8.2/tests/test_stability_funs.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_surfaces.py` & `desc-opt-0.8.2/tests/test_surfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,19 +74,19 @@
             c.Z_lmn = s.Z_lmn
 
         c.name = "my curve"
         assert "my" in c.name
         assert c.name in str(c)
         assert "FourierRZToroidalSurface" in str(c)
 
-        with pytest.warns(UserWarning):
-            c.NFP = 3
+        c.NFP = 3
         assert c.NFP == 3
         assert c.R_basis.NFP == 3
         assert c.Z_basis.NFP == 3
+        assert c.grid.NFP == 3
 
     @pytest.mark.unit
     def test_from_input_file(self):
         """Test reading a surface from a vmec or desc input file."""
         vmec_path = ".//tests//inputs//input.DSHAPE"
         desc_path = ".//tests//inputs//DSHAPE"
         with pytest.warns(UserWarning):
```

### Comparing `desc-opt-0.8.1/tests/test_transform.py` & `desc-opt-0.8.2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_utils.py` & `desc-opt-0.8.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `desc-opt-0.8.1/tests/test_vmec.py` & `desc-opt-0.8.2/tests/test_vmec.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,36 +336,36 @@
         vmec.variables["Rmajor_p"][:], desc.variables["Rmajor_p"][:]
     )
     np.testing.assert_allclose(
         vmec.variables["Aminor_p"][:], desc.variables["Aminor_p"][:]
     )
     np.testing.assert_allclose(vmec.variables["aspect"][:], desc.variables["aspect"][:])
     np.testing.assert_allclose(
-        vmec.variables["volume_p"][:], desc.variables["volume_p"][:]
+        vmec.variables["volume_p"][:], desc.variables["volume_p"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
-        vmec.variables["volavgB"][:], desc.variables["volavgB"][:]
+        vmec.variables["volavgB"][:], desc.variables["volavgB"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
-        vmec.variables["betatotal"][:], desc.variables["betatotal"][:], rtol=1e-6
+        vmec.variables["betatotal"][:], desc.variables["betatotal"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
-        vmec.variables["betapol"][:], desc.variables["betapol"][:], rtol=1e-6
+        vmec.variables["betapol"][:], desc.variables["betapol"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
-        vmec.variables["betator"][:], desc.variables["betator"][:], rtol=1e-6
+        vmec.variables["betator"][:], desc.variables["betator"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
-        vmec.variables["ctor"][:], desc.variables["ctor"][:], rtol=1e-6
+        vmec.variables["ctor"][:], desc.variables["ctor"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
-        vmec.variables["rbtor"][:], desc.variables["rbtor"][:], rtol=1e-6
+        vmec.variables["rbtor"][:], desc.variables["rbtor"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
-        vmec.variables["rbtor0"][:], desc.variables["rbtor0"][:], rtol=1e-6
+        vmec.variables["rbtor0"][:], desc.variables["rbtor0"][:], rtol=1e-5
     )
     np.testing.assert_allclose(
         vmec.variables["b0"][:], desc.variables["b0"][:], rtol=5e-5
     )
     np.testing.assert_allclose(
         np.abs(vmec.variables["bdotb"][20:100]),
         np.abs(desc.variables["bdotb"][20:100]),
@@ -380,20 +380,20 @@
         np.abs(vmec.variables["bvco"][20:100]),
         np.abs(desc.variables["bvco"][20:100]),
         rtol=3e-2,
     )
     np.testing.assert_allclose(
         np.abs(vmec.variables["jdotb"][20:100]),
         np.abs(desc.variables["jdotb"][20:100]),
-        rtol=1e-6,
+        rtol=1e-5,
     )
     np.testing.assert_allclose(
         np.abs(vmec.variables["jcuru"][20:100]),
         np.abs(desc.variables["jcuru"][20:100]),
-        rtol=1e-5,
+        rtol=1e-2,
     )
     np.testing.assert_allclose(
         np.abs(vmec.variables["jcurv"][20:100]),
         np.abs(desc.variables["jcurv"][20:100]),
         rtol=3e-2,
     )
     np.testing.assert_allclose(
@@ -674,15 +674,15 @@
         desc.variables["xm_nyq"][:],
         desc.variables["xn_nyq"][:],
         theta=theta_desc,
         phi=grid.nodes[:, 2],
         s=grid.nodes[:, 0],
         sym=False,
     )
-    np.testing.assert_allclose(bsubs_vmec, bsubs_desc, rtol=1e-2, atol=1e-3)
+    np.testing.assert_allclose(bsubs_vmec, bsubs_desc, rtol=1e-2, atol=2e-3)
 
     # J^theta
     curru_vmec = VMECIO.vmec_interpolate(
         vmec.variables["currumnc"][:],
         np.zeros_like(vmec.variables["currumnc"][:]),
         vmec.variables["xm_nyq"][:],
         vmec.variables["xn_nyq"][:],
```

### Comparing `desc-opt-0.8.1/versioneer.py` & `desc-opt-0.8.2/versioneer.py`

 * *Files identical despite different names*

